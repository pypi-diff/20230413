# Comparing `tmp/mypy-boto3-chime-sdk-voice-1.26.77.tar.gz` & `tmp/mypy-boto3-chime-sdk-voice-1.26.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-voice-1.26.77.tar` & `mypy-boto3-chime-sdk-voice-1.26.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.518112 mypy-boto3-chime-sdk-voice-1.26.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-02-22 20:34:22.518112 mypy-boto3-chime-sdk-voice-1.26.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.510112 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59061 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58978 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55734 2023-02-22 20:33:49.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55695 2023-02-22 20:33:48.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.518112 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-02-22 20:34:22.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-22 20:34:22.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-22 20:34:22.000000 mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.518112 mypy-boto3-chime-sdk-voice-1.26.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-22 20:33:47.000000 mypy-boto3-chime-sdk-voice-1.26.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-voice-1.26.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23460 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-voice-1.26.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71962 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71860 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-03-23 19:32:06.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69305 2023-03-23 19:32:06.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23460 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-voice-1.26.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/setup.py
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/LICENSE` & `mypy-boto3-chime-sdk-voice-1.26.98/LICENSE`

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

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.26.98/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.26.77
-Summary: Type annotations for boto3.ChimeSDKVoice 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKVoice 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,14 +309,15 @@
 ```python
 from mypy_boto3_chime_sdk_voice.literals import (
     AlexaSkillStatusType,
     CallingNameStatusType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
+    LanguageCodeType,
     ListSipMediaApplicationsPaginatorName,
     ListSipRulesPaginatorName,
     NotificationTargetType,
     NumberSelectionBehaviorType,
     OrderedPhoneNumberStatusType,
     OriginationRouteProtocolType,
     PhoneNumberAssociationNameType,
@@ -352,101 +353,127 @@
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
     ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
+    CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
     SipMediaApplicationCallTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
+    TagTypeDef,
+    CreateVoiceProfileRequestRequestTypeDef,
+    VoiceProfileTypeDef,
     CredentialTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
     DeleteVoiceConnectorOriginationRequestRequestTypeDef,
     DeleteVoiceConnectorProxyRequestRequestTypeDef,
     DeleteVoiceConnectorRequestRequestTypeDef,
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
+    DeleteVoiceProfileDomainRequestRequestTypeDef,
+    DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
+    GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     LoggingConfigurationTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
+    GetVoiceProfileDomainRequestRequestTypeDef,
+    GetVoiceProfileRequestRequestTypeDef,
+    GetVoiceToneAnalysisTaskRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
+    ListVoiceProfileDomainsRequestRequestTypeDef,
+    VoiceProfileDomainSummaryTypeDef,
+    ListVoiceProfilesRequestRequestTypeDef,
+    VoiceProfileSummaryTypeDef,
+    MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SpeakerSearchResultTypeDef,
+    StartSpeakerSearchTaskRequestRequestTypeDef,
+    StartVoiceToneAnalysisTaskRequestRequestTypeDef,
+    StopSpeakerSearchTaskRequestRequestTypeDef,
+    StopVoiceToneAnalysisTaskRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
+    UpdateVoiceProfileDomainRequestRequestTypeDef,
+    UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
+    VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
@@ -456,14 +483,21 @@
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
+    VoiceProfileDomainTypeDef,
+    CreateVoiceProfileDomainRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateVoiceProfileResponseTypeDef,
+    GetVoiceProfileResponseTypeDef,
+    UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
@@ -478,31 +512,39 @@
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListVoiceProfileDomainsResponseTypeDef,
+    ListVoiceProfilesResponseTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    SpeakerSearchDetailsTypeDef,
     StreamingConfigurationTypeDef,
+    GetVoiceToneAnalysisTaskResponseTypeDef,
+    StartVoiceToneAnalysisTaskResponseTypeDef,
     CreateSipMediaApplicationResponseTypeDef,
     GetSipMediaApplicationResponseTypeDef,
     ListSipMediaApplicationsResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     CreateSipRuleResponseTypeDef,
     GetSipRuleResponseTypeDef,
     ListSipRulesResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
@@ -512,59 +554,62 @@
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
+    SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    GetSpeakerSearchTaskResponseTypeDef,
+    StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/README.md` & `mypy-boto3-chime-sdk-voice-1.26.98/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,14 +277,15 @@
 ```python
 from mypy_boto3_chime_sdk_voice.literals import (
     AlexaSkillStatusType,
     CallingNameStatusType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
+    LanguageCodeType,
     ListSipMediaApplicationsPaginatorName,
     ListSipRulesPaginatorName,
     NotificationTargetType,
     NumberSelectionBehaviorType,
     OrderedPhoneNumberStatusType,
     OriginationRouteProtocolType,
     PhoneNumberAssociationNameType,
@@ -320,101 +321,127 @@
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
     ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
+    CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
     SipMediaApplicationCallTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
+    TagTypeDef,
+    CreateVoiceProfileRequestRequestTypeDef,
+    VoiceProfileTypeDef,
     CredentialTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
     DeleteVoiceConnectorOriginationRequestRequestTypeDef,
     DeleteVoiceConnectorProxyRequestRequestTypeDef,
     DeleteVoiceConnectorRequestRequestTypeDef,
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
+    DeleteVoiceProfileDomainRequestRequestTypeDef,
+    DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
+    GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     LoggingConfigurationTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
+    GetVoiceProfileDomainRequestRequestTypeDef,
+    GetVoiceProfileRequestRequestTypeDef,
+    GetVoiceToneAnalysisTaskRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
+    ListVoiceProfileDomainsRequestRequestTypeDef,
+    VoiceProfileDomainSummaryTypeDef,
+    ListVoiceProfilesRequestRequestTypeDef,
+    VoiceProfileSummaryTypeDef,
+    MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SpeakerSearchResultTypeDef,
+    StartSpeakerSearchTaskRequestRequestTypeDef,
+    StartVoiceToneAnalysisTaskRequestRequestTypeDef,
+    StopSpeakerSearchTaskRequestRequestTypeDef,
+    StopVoiceToneAnalysisTaskRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
+    UpdateVoiceProfileDomainRequestRequestTypeDef,
+    UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
+    VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
@@ -424,14 +451,21 @@
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
+    VoiceProfileDomainTypeDef,
+    CreateVoiceProfileDomainRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateVoiceProfileResponseTypeDef,
+    GetVoiceProfileResponseTypeDef,
+    UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
@@ -446,31 +480,39 @@
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListVoiceProfileDomainsResponseTypeDef,
+    ListVoiceProfilesResponseTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    SpeakerSearchDetailsTypeDef,
     StreamingConfigurationTypeDef,
+    GetVoiceToneAnalysisTaskResponseTypeDef,
+    StartVoiceToneAnalysisTaskResponseTypeDef,
     CreateSipMediaApplicationResponseTypeDef,
     GetSipMediaApplicationResponseTypeDef,
     ListSipMediaApplicationsResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     CreateSipRuleResponseTypeDef,
     GetSipRuleResponseTypeDef,
     ListSipRulesResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
@@ -480,59 +522,62 @@
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
+    SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    GetSpeakerSearchTaskResponseTypeDef,
+    StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/__init__.py` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/__init__.pyi` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/__main__.py` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKVoice 1.26.77\nVersion:         1.26.77\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.ChimeSDKVoice 1.26.98\nVersion:         1.26.98\nBuilder"
+        " version: 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.77")
+    print("1.26.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/client.py` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     CreatePhoneNumberOrderResponseTypeDef,
     CreateProxySessionResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationResponseTypeDef,
     CreateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     CreateVoiceConnectorResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    CreateVoiceProfileResponseTypeDef,
     CredentialTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetGlobalSettingsResponseTypeDef,
@@ -53,59 +55,72 @@
     GetPhoneNumberResponseTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionResponseTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetSipMediaApplicationResponseTypeDef,
     GetSipRuleResponseTypeDef,
+    GetSpeakerSearchTaskResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileResponseTypeDef,
+    GetVoiceToneAnalysisTaskResponseTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     ListSipMediaApplicationsResponseTypeDef,
     ListSipRulesResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    ListVoiceProfileDomainsResponseTypeDef,
+    ListVoiceProfilesResponseTypeDef,
     LoggingConfigurationTypeDef,
     OriginationTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
+    StartSpeakerSearchTaskResponseTypeDef,
+    StartVoiceToneAnalysisTaskResponseTypeDef,
     StreamingConfigurationTypeDef,
+    TagTypeDef,
     TerminationTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileResponseTypeDef,
     ValidateE911AddressResponseTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -126,20 +141,22 @@
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
+    GoneException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottledClientException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
+    UnprocessableEntityException: Type[BotocoreClientError]
 
 
 class ChimeSDKVoiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/)
     """
@@ -313,14 +330,42 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/CreateVoiceConnectorGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector_group)
         """
 
+    def create_voice_profile(
+        self, *, SpeakerSearchTaskId: str
+    ) -> CreateVoiceProfileResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/CreateVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile)
+        """
+
+    def create_voice_profile_domain(
+        self,
+        *,
+        Name: str,
+        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
+        Description: str = ...,
+        ClientRequestToken: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateVoiceProfileDomainResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/CreateVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile_domain)
+        """
+
     def delete_phone_number(self, *, PhoneNumberId: str) -> EmptyResponseMetadataTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/DeletePhoneNumber).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_phone_number)
@@ -439,14 +484,34 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/DeleteVoiceConnectorTerminationCredentials).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_termination_credentials)
         """
 
+    def delete_voice_profile(self, *, VoiceProfileId: str) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/DeleteVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile)
+        """
+
+    def delete_voice_profile_domain(
+        self, *, VoiceProfileDomainId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/DeleteVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile_domain)
+        """
+
     def disassociate_phone_numbers_from_voice_connector(
         self, *, VoiceConnectorId: str, E164PhoneNumbers: Sequence[str]
     ) -> DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/DisassociatePhoneNumbersFromVoiceConnector).
 
@@ -566,14 +631,25 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/GetSipRule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_rule)
         """
 
+    def get_speaker_search_task(
+        self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
+    ) -> GetSpeakerSearchTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetSpeakerSearchTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_speaker_search_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_speaker_search_task)
+        """
+
     def get_voice_connector(self, *, VoiceConnectorId: str) -> GetVoiceConnectorResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/GetVoiceConnector).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector)
@@ -663,14 +739,45 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/GetVoiceConnectorTerminationHealth).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_termination_health)
         """
 
+    def get_voice_profile(self, *, VoiceProfileId: str) -> GetVoiceProfileResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile)
+        """
+
+    def get_voice_profile_domain(
+        self, *, VoiceProfileDomainId: str
+    ) -> GetVoiceProfileDomainResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile_domain)
+        """
+
+    def get_voice_tone_analysis_task(
+        self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str, IsCaller: bool
+    ) -> GetVoiceToneAnalysisTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetVoiceToneAnalysisTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_tone_analysis_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_tone_analysis_task)
+        """
+
     def list_available_voice_connector_regions(
         self,
     ) -> ListAvailableVoiceConnectorRegionsResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListAvailableVoiceConnectorRegions).
 
@@ -752,14 +859,23 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListSupportedPhoneNumberCountries).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_supported_phone_number_countries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_supported_phone_number_countries)
         """
 
+    def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/ListTagsForResource).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_tags_for_resource)
+        """
+
     def list_voice_connector_groups(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceConnectorGroupsResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListVoiceConnectorGroups).
 
@@ -785,14 +901,36 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListVoiceConnectors).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connectors)
         """
 
+    def list_voice_profile_domains(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListVoiceProfileDomainsResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/ListVoiceProfileDomains).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profile_domains)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profile_domains)
+        """
+
+    def list_voice_profiles(
+        self, *, VoiceProfileDomainId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListVoiceProfilesResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/ListVoiceProfiles).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
+        """
+
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
         SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
@@ -928,14 +1066,90 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/SearchAvailablePhoneNumbers).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#search_available_phone_numbers)
         """
 
+    def start_speaker_search_task(
+        self,
+        *,
+        VoiceConnectorId: str,
+        TransactionId: str,
+        VoiceProfileDomainId: str,
+        ClientRequestToken: str = ...
+    ) -> StartSpeakerSearchTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StartSpeakerSearchTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_speaker_search_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_speaker_search_task)
+        """
+
+    def start_voice_tone_analysis_task(
+        self,
+        *,
+        VoiceConnectorId: str,
+        TransactionId: str,
+        LanguageCode: Literal["en-US"],
+        ClientRequestToken: str = ...
+    ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StartVoiceToneAnalysisTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_voice_tone_analysis_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_voice_tone_analysis_task)
+        """
+
+    def stop_speaker_search_task(
+        self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StopSpeakerSearchTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_speaker_search_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_speaker_search_task)
+        """
+
+    def stop_voice_tone_analysis_task(
+        self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StopVoiceToneAnalysisTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_voice_tone_analysis_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_voice_tone_analysis_task)
+        """
+
+    def tag_resource(
+        self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/TagResource).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#tag_resource)
+        """
+
+    def untag_resource(
+        self, *, ResourceARN: str, TagKeys: Sequence[str]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/UntagResource).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#untag_resource)
+        """
+
     def update_global_settings(
         self, *, VoiceConnector: VoiceConnectorSettingsTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/UpdateGlobalSettings).
 
@@ -1047,14 +1261,36 @@
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/UpdateVoiceConnectorGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector_group)
         """
 
+    def update_voice_profile(
+        self, *, VoiceProfileId: str, SpeakerSearchTaskId: str
+    ) -> UpdateVoiceProfileResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/UpdateVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile)
+        """
+
+    def update_voice_profile_domain(
+        self, *, VoiceProfileDomainId: str, Name: str = ..., Description: str = ...
+    ) -> UpdateVoiceProfileDomainResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/UpdateVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile_domain)
+        """
+
     def validate_e911_address(
         self,
         *,
         AwsAccountId: str,
         StreetNumber: str,
         StreetInfo: str,
         City: str,
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/client.pyi` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     CreatePhoneNumberOrderResponseTypeDef,
     CreateProxySessionResponseTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationResponseTypeDef,
     CreateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     CreateVoiceConnectorResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    CreateVoiceProfileResponseTypeDef,
     CredentialTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetGlobalSettingsResponseTypeDef,
@@ -53,59 +55,72 @@
     GetPhoneNumberResponseTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionResponseTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     GetSipMediaApplicationLoggingConfigurationResponseTypeDef,
     GetSipMediaApplicationResponseTypeDef,
     GetSipRuleResponseTypeDef,
+    GetSpeakerSearchTaskResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileResponseTypeDef,
+    GetVoiceToneAnalysisTaskResponseTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     ListSipMediaApplicationsResponseTypeDef,
     ListSipRulesResponseTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    ListVoiceProfileDomainsResponseTypeDef,
+    ListVoiceProfilesResponseTypeDef,
     LoggingConfigurationTypeDef,
     OriginationTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
+    StartSpeakerSearchTaskResponseTypeDef,
+    StartVoiceToneAnalysisTaskResponseTypeDef,
     StreamingConfigurationTypeDef,
+    TagTypeDef,
     TerminationTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileResponseTypeDef,
     ValidateE911AddressResponseTypeDef,
     VoiceConnectorItemTypeDef,
     VoiceConnectorSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -123,20 +138,22 @@
 
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
+    GoneException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottledClientException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
+    UnprocessableEntityException: Type[BotocoreClientError]
 
 class ChimeSDKVoiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/)
     """
 
@@ -295,14 +312,40 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/CreateVoiceConnectorGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector_group)
         """
+    def create_voice_profile(
+        self, *, SpeakerSearchTaskId: str
+    ) -> CreateVoiceProfileResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/CreateVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile)
+        """
+    def create_voice_profile_domain(
+        self,
+        *,
+        Name: str,
+        ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
+        Description: str = ...,
+        ClientRequestToken: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateVoiceProfileDomainResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/CreateVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile_domain)
+        """
     def delete_phone_number(self, *, PhoneNumberId: str) -> EmptyResponseMetadataTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/DeletePhoneNumber).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_phone_number)
@@ -409,14 +452,32 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/DeleteVoiceConnectorTerminationCredentials).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_termination_credentials)
         """
+    def delete_voice_profile(self, *, VoiceProfileId: str) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/DeleteVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile)
+        """
+    def delete_voice_profile_domain(
+        self, *, VoiceProfileDomainId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/DeleteVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile_domain)
+        """
     def disassociate_phone_numbers_from_voice_connector(
         self, *, VoiceConnectorId: str, E164PhoneNumbers: Sequence[str]
     ) -> DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/DisassociatePhoneNumbersFromVoiceConnector).
 
@@ -524,14 +585,24 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/GetSipRule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_rule)
         """
+    def get_speaker_search_task(
+        self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
+    ) -> GetSpeakerSearchTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetSpeakerSearchTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_speaker_search_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_speaker_search_task)
+        """
     def get_voice_connector(self, *, VoiceConnectorId: str) -> GetVoiceConnectorResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/GetVoiceConnector).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector)
@@ -612,14 +683,42 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/GetVoiceConnectorTerminationHealth).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_termination_health)
         """
+    def get_voice_profile(self, *, VoiceProfileId: str) -> GetVoiceProfileResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile)
+        """
+    def get_voice_profile_domain(
+        self, *, VoiceProfileDomainId: str
+    ) -> GetVoiceProfileDomainResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile_domain)
+        """
+    def get_voice_tone_analysis_task(
+        self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str, IsCaller: bool
+    ) -> GetVoiceToneAnalysisTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/GetVoiceToneAnalysisTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_tone_analysis_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_tone_analysis_task)
+        """
     def list_available_voice_connector_regions(
         self,
     ) -> ListAvailableVoiceConnectorRegionsResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListAvailableVoiceConnectorRegions).
 
@@ -694,14 +793,22 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListSupportedPhoneNumberCountries).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_supported_phone_number_countries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_supported_phone_number_countries)
         """
+    def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/ListTagsForResource).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_tags_for_resource)
+        """
     def list_voice_connector_groups(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceConnectorGroupsResponseTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListVoiceConnectorGroups).
 
@@ -724,14 +831,34 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/ListVoiceConnectors).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connectors)
         """
+    def list_voice_profile_domains(
+        self, *, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListVoiceProfileDomainsResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/ListVoiceProfileDomains).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profile_domains)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profile_domains)
+        """
+    def list_voice_profiles(
+        self, *, VoiceProfileDomainId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListVoiceProfilesResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/ListVoiceProfiles).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profiles)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
+        """
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
         SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
@@ -856,14 +983,84 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/SearchAvailablePhoneNumbers).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#search_available_phone_numbers)
         """
+    def start_speaker_search_task(
+        self,
+        *,
+        VoiceConnectorId: str,
+        TransactionId: str,
+        VoiceProfileDomainId: str,
+        ClientRequestToken: str = ...
+    ) -> StartSpeakerSearchTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StartSpeakerSearchTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_speaker_search_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_speaker_search_task)
+        """
+    def start_voice_tone_analysis_task(
+        self,
+        *,
+        VoiceConnectorId: str,
+        TransactionId: str,
+        LanguageCode: Literal["en-US"],
+        ClientRequestToken: str = ...
+    ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StartVoiceToneAnalysisTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_voice_tone_analysis_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_voice_tone_analysis_task)
+        """
+    def stop_speaker_search_task(
+        self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StopSpeakerSearchTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_speaker_search_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_speaker_search_task)
+        """
+    def stop_voice_tone_analysis_task(
+        self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/StopVoiceToneAnalysisTask).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_voice_tone_analysis_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_voice_tone_analysis_task)
+        """
+    def tag_resource(
+        self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/TagResource).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#tag_resource)
+        """
+    def untag_resource(
+        self, *, ResourceARN: str, TagKeys: Sequence[str]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/UntagResource).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#untag_resource)
+        """
     def update_global_settings(
         self, *, VoiceConnector: VoiceConnectorSettingsTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/UpdateGlobalSettings).
 
@@ -966,14 +1163,34 @@
         """
         See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
         sdk-voice-2022-08-03/UpdateVoiceConnectorGroup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector_group)
         """
+    def update_voice_profile(
+        self, *, VoiceProfileId: str, SpeakerSearchTaskId: str
+    ) -> UpdateVoiceProfileResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/UpdateVoiceProfile).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile)
+        """
+    def update_voice_profile_domain(
+        self, *, VoiceProfileDomainId: str, Name: str = ..., Description: str = ...
+    ) -> UpdateVoiceProfileDomainResponseTypeDef:
+        """
+        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
+        sdk-voice-2022-08-03/UpdateVoiceProfileDomain).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile_domain)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile_domain)
+        """
     def validate_e911_address(
         self,
         *,
         AwsAccountId: str,
         StreetNumber: str,
         StreetInfo: str,
         City: str,
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/literals.py` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = (
     "AlexaSkillStatusType",
     "CallingNameStatusType",
     "CapabilityType",
     "ErrorCodeType",
     "GeoMatchLevelType",
+    "LanguageCodeType",
     "ListSipMediaApplicationsPaginatorName",
     "ListSipRulesPaginatorName",
     "NotificationTargetType",
     "NumberSelectionBehaviorType",
     "OrderedPhoneNumberStatusType",
     "OriginationRouteProtocolType",
     "PhoneNumberAssociationNameType",
@@ -66,14 +67,15 @@
     "Throttled",
     "Throttling",
     "Unauthorized",
     "Unprocessable",
     "VoiceConnectorGroupAssociationsExist",
 ]
 GeoMatchLevelType = Literal["AreaCode", "Country"]
+LanguageCodeType = Literal["en-US"]
 ListSipMediaApplicationsPaginatorName = Literal["list_sip_media_applications"]
 ListSipRulesPaginatorName = Literal["list_sip_rules"]
 NotificationTargetType = Literal["EventBridge", "SNS", "SQS"]
 NumberSelectionBehaviorType = Literal["AvoidSticky", "PreferSticky"]
 OrderedPhoneNumberStatusType = Literal["Acquired", "Failed", "Processing"]
 OriginationRouteProtocolType = Literal["TCP", "UDP"]
 PhoneNumberAssociationNameType = Literal["SipRuleId", "VoiceConnectorGroupId", "VoiceConnectorId"]
@@ -265,14 +267,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -283,14 +286,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/literals.pyi` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 __all__ = (
     "AlexaSkillStatusType",
     "CallingNameStatusType",
     "CapabilityType",
     "ErrorCodeType",
     "GeoMatchLevelType",
+    "LanguageCodeType",
     "ListSipMediaApplicationsPaginatorName",
     "ListSipRulesPaginatorName",
     "NotificationTargetType",
     "NumberSelectionBehaviorType",
     "OrderedPhoneNumberStatusType",
     "OriginationRouteProtocolType",
     "PhoneNumberAssociationNameType",
@@ -64,14 +65,15 @@
     "Throttled",
     "Throttling",
     "Unauthorized",
     "Unprocessable",
     "VoiceConnectorGroupAssociationsExist",
 ]
 GeoMatchLevelType = Literal["AreaCode", "Country"]
+LanguageCodeType = Literal["en-US"]
 ListSipMediaApplicationsPaginatorName = Literal["list_sip_media_applications"]
 ListSipRulesPaginatorName = Literal["list_sip_rules"]
 NotificationTargetType = Literal["EventBridge", "SNS", "SQS"]
 NumberSelectionBehaviorType = Literal["AvoidSticky", "PreferSticky"]
 OrderedPhoneNumberStatusType = Literal["Acquired", "Failed", "Processing"]
 OriginationRouteProtocolType = Literal["TCP", "UDP"]
 PhoneNumberAssociationNameType = Literal["SipRuleId", "VoiceConnectorGroupId", "VoiceConnectorId"]
@@ -263,14 +265,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -281,14 +284,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/paginator.py` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/paginator.pyi` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/type_defs.py` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,114 +33,144 @@
     PhoneNumberTypeType,
     ProxySessionStatusType,
     SipRuleTriggerTypeType,
     VoiceConnectorAwsRegionType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddressTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
+    "CallDetailsTypeDef",
     "CandidateAddressTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
     "SipMediaApplicationCallTypeDef",
     "SipMediaApplicationEndpointTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
+    "ServerSideEncryptionConfigurationTypeDef",
+    "TagTypeDef",
+    "CreateVoiceProfileRequestRequestTypeDef",
+    "VoiceProfileTypeDef",
     "CredentialTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
     "DeleteSipRuleRequestRequestTypeDef",
     "DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorGroupRequestRequestTypeDef",
     "DeleteVoiceConnectorOriginationRequestRequestTypeDef",
     "DeleteVoiceConnectorProxyRequestRequestTypeDef",
     "DeleteVoiceConnectorRequestRequestTypeDef",
     "DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
+    "DeleteVoiceProfileDomainRequestRequestTypeDef",
+    "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
+    "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "LoggingConfigurationTypeDef",
     "GetVoiceConnectorOriginationRequestRequestTypeDef",
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationTypeDef",
+    "GetVoiceProfileDomainRequestRequestTypeDef",
+    "GetVoiceProfileRequestRequestTypeDef",
+    "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
+    "ListVoiceProfileDomainsRequestRequestTypeDef",
+    "VoiceProfileDomainSummaryTypeDef",
+    "ListVoiceProfilesRequestRequestTypeDef",
+    "VoiceProfileSummaryTypeDef",
+    "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
+    "SpeakerSearchResultTypeDef",
+    "StartSpeakerSearchTaskRequestRequestTypeDef",
+    "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
+    "StopSpeakerSearchTaskRequestRequestTypeDef",
+    "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
+    "UpdateVoiceProfileDomainRequestRequestTypeDef",
+    "UpdateVoiceProfileRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetPhoneNumberSettingsResponseTypeDef",
     "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
+    "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
     "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
@@ -150,14 +180,21 @@
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
+    "VoiceProfileDomainTypeDef",
+    "CreateVoiceProfileDomainRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateVoiceProfileResponseTypeDef",
+    "GetVoiceProfileResponseTypeDef",
+    "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
@@ -172,31 +209,39 @@
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
+    "ListVoiceProfileDomainsResponseTypeDef",
+    "ListVoiceProfilesResponseTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "SpeakerSearchDetailsTypeDef",
     "StreamingConfigurationTypeDef",
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
     "CreateSipMediaApplicationResponseTypeDef",
     "GetSipMediaApplicationResponseTypeDef",
     "ListSipMediaApplicationsResponseTypeDef",
     "UpdateSipMediaApplicationResponseTypeDef",
     "CreateSipRuleResponseTypeDef",
     "GetSipRuleResponseTypeDef",
     "ListSipRulesResponseTypeDef",
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
+    "CreateVoiceProfileDomainResponseTypeDef",
+    "GetVoiceProfileDomainResponseTypeDef",
+    "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
@@ -206,17 +251,20 @@
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
+    "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "GetSpeakerSearchTaskResponseTypeDef",
+    "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "streetName": str,
         "streetSuffix": str,
@@ -324,14 +372,24 @@
 
 class UpdatePhoneNumberRequestItemTypeDef(
     _RequiredUpdatePhoneNumberRequestItemTypeDef, _OptionalUpdatePhoneNumberRequestItemTypeDef
 ):
     pass
 
 
+CallDetailsTypeDef = TypedDict(
+    "CallDetailsTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "TransactionId": str,
+        "IsCaller": bool,
+    },
+    total=False,
+)
+
 CandidateAddressTypeDef = TypedDict(
     "CandidateAddressTypeDef",
     {
         "streetInfo": str,
         "streetNumber": str,
         "city": str,
         "state": str,
@@ -451,14 +509,49 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "VoiceConnectorArn": str,
     },
     total=False,
 )
 
+ServerSideEncryptionConfigurationTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+)
+
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+CreateVoiceProfileRequestRequestTypeDef = TypedDict(
+    "CreateVoiceProfileRequestRequestTypeDef",
+    {
+        "SpeakerSearchTaskId": str,
+    },
+)
+
+VoiceProfileTypeDef = TypedDict(
+    "VoiceProfileTypeDef",
+    {
+        "VoiceProfileId": str,
+        "VoiceProfileArn": str,
+        "VoiceProfileDomainId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ExpirationTimestamp": datetime,
+    },
+    total=False,
+)
+
 CredentialTypeDef = TypedDict(
     "CredentialTypeDef",
     {
         "Username": str,
         "Password": str,
     },
     total=False,
@@ -569,14 +662,28 @@
 DeleteVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
+DeleteVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "DeleteVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+
+DeleteVoiceProfileRequestRequestTypeDef = TypedDict(
+    "DeleteVoiceProfileRequestRequestTypeDef",
+    {
+        "VoiceProfileId": str,
+    },
+)
+
 DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorGroupId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -659,14 +766,22 @@
 GetSipRuleRequestRequestTypeDef = TypedDict(
     "GetSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
     },
 )
 
+GetSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "GetSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "SpeakerSearchTaskId": str,
+    },
+)
+
 GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
@@ -763,14 +878,37 @@
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
     total=False,
 )
 
+GetVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "GetVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+
+GetVoiceProfileRequestRequestTypeDef = TypedDict(
+    "GetVoiceProfileRequestRequestTypeDef",
+    {
+        "VoiceProfileId": str,
+    },
+)
+
+GetVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "VoiceToneAnalysisTaskId": str,
+        "IsCaller": bool,
+    },
+)
+
 ListPhoneNumberOrdersRequestRequestTypeDef = TypedDict(
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -853,14 +991,21 @@
     {
         "CountryCode": str,
         "SupportedPhoneNumberTypes": List[PhoneNumberTypeType],
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+
 ListVoiceConnectorGroupsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -878,14 +1023,80 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListVoiceProfileDomainsRequestRequestTypeDef = TypedDict(
+    "ListVoiceProfileDomainsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+VoiceProfileDomainSummaryTypeDef = TypedDict(
+    "VoiceProfileDomainSummaryTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+_RequiredListVoiceProfilesRequestRequestTypeDef = TypedDict(
+    "_RequiredListVoiceProfilesRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+_OptionalListVoiceProfilesRequestRequestTypeDef = TypedDict(
+    "_OptionalListVoiceProfilesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListVoiceProfilesRequestRequestTypeDef(
+    _RequiredListVoiceProfilesRequestRequestTypeDef, _OptionalListVoiceProfilesRequestRequestTypeDef
+):
+    pass
+
+
+VoiceProfileSummaryTypeDef = TypedDict(
+    "VoiceProfileSummaryTypeDef",
+    {
+        "VoiceProfileId": str,
+        "VoiceProfileArn": str,
+        "VoiceProfileDomainId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ExpirationTimestamp": datetime,
+    },
+    total=False,
+)
+
+MediaInsightsConfigurationTypeDef = TypedDict(
+    "MediaInsightsConfigurationTypeDef",
+    {
+        "Disabled": bool,
+        "ConfigurationArn": str,
+    },
+    total=False,
+)
+
 OrderedPhoneNumberTypeDef = TypedDict(
     "OrderedPhoneNumberTypeDef",
     {
         "E164PhoneNumber": str,
         "Status": OrderedPhoneNumberStatusType,
     },
     total=False,
@@ -978,22 +1189,103 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+SpeakerSearchResultTypeDef = TypedDict(
+    "SpeakerSearchResultTypeDef",
+    {
+        "ConfidenceScore": float,
+        "VoiceProfileId": str,
+    },
+    total=False,
+)
+
+_RequiredStartSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "TransactionId": str,
+        "VoiceProfileDomainId": str,
+    },
+)
+_OptionalStartSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class StartSpeakerSearchTaskRequestRequestTypeDef(
+    _RequiredStartSpeakerSearchTaskRequestRequestTypeDef,
+    _OptionalStartSpeakerSearchTaskRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "TransactionId": str,
+        "LanguageCode": Literal["en-US"],
+    },
+)
+_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class StartVoiceToneAnalysisTaskRequestRequestTypeDef(
+    _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef,
+    _OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef,
+):
+    pass
+
+
+StopSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "StopSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "SpeakerSearchTaskId": str,
+    },
+)
+
+StopVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "VoiceToneAnalysisTaskId": str,
+    },
+)
+
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
     total=False,
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -1057,14 +1349,45 @@
     {
         "VoiceConnectorId": str,
         "Name": str,
         "RequireEncryption": bool,
     },
 )
 
+_RequiredUpdateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+_OptionalUpdateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateVoiceProfileDomainRequestRequestTypeDef(
+    _RequiredUpdateVoiceProfileDomainRequestRequestTypeDef,
+    _OptionalUpdateVoiceProfileDomainRequestRequestTypeDef,
+):
+    pass
+
+
+UpdateVoiceProfileRequestRequestTypeDef = TypedDict(
+    "UpdateVoiceProfileRequestRequestTypeDef",
+    {
+        "VoiceProfileId": str,
+        "SpeakerSearchTaskId": str,
+    },
+)
+
 ValidateE911AddressRequestRequestTypeDef = TypedDict(
     "ValidateE911AddressRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "StreetNumber": str,
         "StreetInfo": str,
         "City": str,
@@ -1166,14 +1489,28 @@
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
+VoiceToneAnalysisTaskTypeDef = TypedDict(
+    "VoiceToneAnalysisTaskTypeDef",
+    {
+        "VoiceToneAnalysisTaskId": str,
+        "VoiceToneAnalysisTaskStatus": str,
+        "CallDetails": CallDetailsTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "StartedTimestamp": datetime,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
@@ -1405,14 +1742,93 @@
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+_RequiredCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+    },
+)
+_OptionalCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateVoiceProfileDomainRequestRequestTypeDef(
+    _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
+    _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
+):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateVoiceProfileResponseTypeDef = TypedDict(
+    "CreateVoiceProfileResponseTypeDef",
+    {
+        "VoiceProfile": VoiceProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceProfileResponseTypeDef = TypedDict(
+    "GetVoiceProfileResponseTypeDef",
+    {
+        "VoiceProfile": VoiceProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceProfileResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileResponseTypeDef",
+    {
+        "VoiceProfile": VoiceProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
@@ -1630,14 +2046,32 @@
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListVoiceProfileDomainsResponseTypeDef = TypedDict(
+    "ListVoiceProfileDomainsResponseTypeDef",
+    {
+        "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVoiceProfilesResponseTypeDef = TypedDict(
+    "ListVoiceProfilesResponseTypeDef",
+    {
+        "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
         "ProductType": PhoneNumberProductTypeType,
         "Status": PhoneNumberOrderStatusType,
         "OrderType": PhoneNumberOrderTypeType,
@@ -1694,36 +2128,62 @@
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
         "OrderId": str,
     },
     total=False,
 )
 
+SpeakerSearchDetailsTypeDef = TypedDict(
+    "SpeakerSearchDetailsTypeDef",
+    {
+        "Results": List[SpeakerSearchResultTypeDef],
+        "VoiceprintGenerationStatus": str,
+    },
+    total=False,
+)
+
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
         "Disabled": bool,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
 
+GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
+    {
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
+    {
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateSipMediaApplicationResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1815,14 +2275,38 @@
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "CreateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceProfileDomainResponseTypeDef = TypedDict(
+    "GetVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1954,14 +2438,29 @@
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SpeakerSearchTaskTypeDef = TypedDict(
+    "SpeakerSearchTaskTypeDef",
+    {
+        "SpeakerSearchTaskId": str,
+        "SpeakerSearchTaskStatus": str,
+        "CallDetails": CallDetailsTypeDef,
+        "SpeakerSearchDetails": SpeakerSearchDetailsTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "StartedTimestamp": datetime,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1977,7 +2476,23 @@
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+GetSpeakerSearchTaskResponseTypeDef = TypedDict(
+    "GetSpeakerSearchTaskResponseTypeDef",
+    {
+        "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSpeakerSearchTaskResponseTypeDef = TypedDict(
+    "StartSpeakerSearchTaskResponseTypeDef",
+    {
+        "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice/type_defs.pyi` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -33,113 +33,143 @@
     PhoneNumberTypeType,
     ProxySessionStatusType,
     SipRuleTriggerTypeType,
     VoiceConnectorAwsRegionType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddressTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
+    "CallDetailsTypeDef",
     "CandidateAddressTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
     "SipMediaApplicationCallTypeDef",
     "SipMediaApplicationEndpointTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
     "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
+    "ServerSideEncryptionConfigurationTypeDef",
+    "TagTypeDef",
+    "CreateVoiceProfileRequestRequestTypeDef",
+    "VoiceProfileTypeDef",
     "CredentialTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
     "DeleteSipRuleRequestRequestTypeDef",
     "DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorGroupRequestRequestTypeDef",
     "DeleteVoiceConnectorOriginationRequestRequestTypeDef",
     "DeleteVoiceConnectorProxyRequestRequestTypeDef",
     "DeleteVoiceConnectorRequestRequestTypeDef",
     "DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
+    "DeleteVoiceProfileDomainRequestRequestTypeDef",
+    "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
+    "GetSpeakerSearchTaskRequestRequestTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorGroupRequestRequestTypeDef",
     "GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "LoggingConfigurationTypeDef",
     "GetVoiceConnectorOriginationRequestRequestTypeDef",
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationTypeDef",
+    "GetVoiceProfileDomainRequestRequestTypeDef",
+    "GetVoiceProfileRequestRequestTypeDef",
+    "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
+    "ListVoiceProfileDomainsRequestRequestTypeDef",
+    "VoiceProfileDomainSummaryTypeDef",
+    "ListVoiceProfilesRequestRequestTypeDef",
+    "VoiceProfileSummaryTypeDef",
+    "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
+    "SpeakerSearchResultTypeDef",
+    "StartSpeakerSearchTaskRequestRequestTypeDef",
+    "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
+    "StopSpeakerSearchTaskRequestRequestTypeDef",
+    "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
+    "UpdateVoiceProfileDomainRequestRequestTypeDef",
+    "UpdateVoiceProfileRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetPhoneNumberSettingsResponseTypeDef",
     "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
+    "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
     "CreateSipMediaApplicationRequestRequestTypeDef",
     "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
@@ -149,14 +179,21 @@
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
+    "VoiceProfileDomainTypeDef",
+    "CreateVoiceProfileDomainRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateVoiceProfileResponseTypeDef",
+    "GetVoiceProfileResponseTypeDef",
+    "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
@@ -171,31 +208,39 @@
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
+    "ListVoiceProfileDomainsResponseTypeDef",
+    "ListVoiceProfilesResponseTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "SpeakerSearchDetailsTypeDef",
     "StreamingConfigurationTypeDef",
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
     "CreateSipMediaApplicationResponseTypeDef",
     "GetSipMediaApplicationResponseTypeDef",
     "ListSipMediaApplicationsResponseTypeDef",
     "UpdateSipMediaApplicationResponseTypeDef",
     "CreateSipRuleResponseTypeDef",
     "GetSipRuleResponseTypeDef",
     "ListSipRulesResponseTypeDef",
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
+    "CreateVoiceProfileDomainResponseTypeDef",
+    "GetVoiceProfileDomainResponseTypeDef",
+    "UpdateVoiceProfileDomainResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
@@ -205,17 +250,20 @@
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
+    "SpeakerSearchTaskTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "GetSpeakerSearchTaskResponseTypeDef",
+    "StartSpeakerSearchTaskResponseTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "streetName": str,
         "streetSuffix": str,
@@ -317,14 +365,24 @@
 )
 
 class UpdatePhoneNumberRequestItemTypeDef(
     _RequiredUpdatePhoneNumberRequestItemTypeDef, _OptionalUpdatePhoneNumberRequestItemTypeDef
 ):
     pass
 
+CallDetailsTypeDef = TypedDict(
+    "CallDetailsTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "TransactionId": str,
+        "IsCaller": bool,
+    },
+    total=False,
+)
+
 CandidateAddressTypeDef = TypedDict(
     "CandidateAddressTypeDef",
     {
         "streetInfo": str,
         "streetNumber": str,
         "city": str,
         "state": str,
@@ -440,14 +498,49 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "VoiceConnectorArn": str,
     },
     total=False,
 )
 
+ServerSideEncryptionConfigurationTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+)
+
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+CreateVoiceProfileRequestRequestTypeDef = TypedDict(
+    "CreateVoiceProfileRequestRequestTypeDef",
+    {
+        "SpeakerSearchTaskId": str,
+    },
+)
+
+VoiceProfileTypeDef = TypedDict(
+    "VoiceProfileTypeDef",
+    {
+        "VoiceProfileId": str,
+        "VoiceProfileArn": str,
+        "VoiceProfileDomainId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ExpirationTimestamp": datetime,
+    },
+    total=False,
+)
+
 CredentialTypeDef = TypedDict(
     "CredentialTypeDef",
     {
         "Username": str,
         "Password": str,
     },
     total=False,
@@ -556,14 +649,28 @@
 DeleteVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
+DeleteVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "DeleteVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+
+DeleteVoiceProfileRequestRequestTypeDef = TypedDict(
+    "DeleteVoiceProfileRequestRequestTypeDef",
+    {
+        "VoiceProfileId": str,
+    },
+)
+
 DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorGroupId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -646,14 +753,22 @@
 GetSipRuleRequestRequestTypeDef = TypedDict(
     "GetSipRuleRequestRequestTypeDef",
     {
         "SipRuleId": str,
     },
 )
 
+GetSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "GetSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "SpeakerSearchTaskId": str,
+    },
+)
+
 GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
@@ -750,14 +865,37 @@
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
     total=False,
 )
 
+GetVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "GetVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+
+GetVoiceProfileRequestRequestTypeDef = TypedDict(
+    "GetVoiceProfileRequestRequestTypeDef",
+    {
+        "VoiceProfileId": str,
+    },
+)
+
+GetVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "VoiceToneAnalysisTaskId": str,
+        "IsCaller": bool,
+    },
+)
+
 ListPhoneNumberOrdersRequestRequestTypeDef = TypedDict(
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -838,14 +976,21 @@
     {
         "CountryCode": str,
         "SupportedPhoneNumberTypes": List[PhoneNumberTypeType],
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+
 ListVoiceConnectorGroupsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -863,14 +1008,78 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListVoiceProfileDomainsRequestRequestTypeDef = TypedDict(
+    "ListVoiceProfileDomainsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+VoiceProfileDomainSummaryTypeDef = TypedDict(
+    "VoiceProfileDomainSummaryTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+_RequiredListVoiceProfilesRequestRequestTypeDef = TypedDict(
+    "_RequiredListVoiceProfilesRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+_OptionalListVoiceProfilesRequestRequestTypeDef = TypedDict(
+    "_OptionalListVoiceProfilesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListVoiceProfilesRequestRequestTypeDef(
+    _RequiredListVoiceProfilesRequestRequestTypeDef, _OptionalListVoiceProfilesRequestRequestTypeDef
+):
+    pass
+
+VoiceProfileSummaryTypeDef = TypedDict(
+    "VoiceProfileSummaryTypeDef",
+    {
+        "VoiceProfileId": str,
+        "VoiceProfileArn": str,
+        "VoiceProfileDomainId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ExpirationTimestamp": datetime,
+    },
+    total=False,
+)
+
+MediaInsightsConfigurationTypeDef = TypedDict(
+    "MediaInsightsConfigurationTypeDef",
+    {
+        "Disabled": bool,
+        "ConfigurationArn": str,
+    },
+    total=False,
+)
+
 OrderedPhoneNumberTypeDef = TypedDict(
     "OrderedPhoneNumberTypeDef",
     {
         "E164PhoneNumber": str,
         "Status": OrderedPhoneNumberStatusType,
     },
     total=False,
@@ -961,22 +1170,99 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+SpeakerSearchResultTypeDef = TypedDict(
+    "SpeakerSearchResultTypeDef",
+    {
+        "ConfidenceScore": float,
+        "VoiceProfileId": str,
+    },
+    total=False,
+)
+
+_RequiredStartSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "TransactionId": str,
+        "VoiceProfileDomainId": str,
+    },
+)
+_OptionalStartSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class StartSpeakerSearchTaskRequestRequestTypeDef(
+    _RequiredStartSpeakerSearchTaskRequestRequestTypeDef,
+    _OptionalStartSpeakerSearchTaskRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "TransactionId": str,
+        "LanguageCode": Literal["en-US"],
+    },
+)
+_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class StartVoiceToneAnalysisTaskRequestRequestTypeDef(
+    _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef,
+    _OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef,
+):
+    pass
+
+StopSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
+    "StopSpeakerSearchTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "SpeakerSearchTaskId": str,
+    },
+)
+
+StopVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
+    "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "VoiceToneAnalysisTaskId": str,
+    },
+)
+
 StreamingNotificationTargetTypeDef = TypedDict(
     "StreamingNotificationTargetTypeDef",
     {
         "NotificationTarget": NotificationTargetType,
     },
     total=False,
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
+    },
+)
+
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -1036,14 +1322,43 @@
     {
         "VoiceConnectorId": str,
         "Name": str,
         "RequireEncryption": bool,
     },
 )
 
+_RequiredUpdateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+    },
+)
+_OptionalUpdateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateVoiceProfileDomainRequestRequestTypeDef(
+    _RequiredUpdateVoiceProfileDomainRequestRequestTypeDef,
+    _OptionalUpdateVoiceProfileDomainRequestRequestTypeDef,
+):
+    pass
+
+UpdateVoiceProfileRequestRequestTypeDef = TypedDict(
+    "UpdateVoiceProfileRequestRequestTypeDef",
+    {
+        "VoiceProfileId": str,
+        "SpeakerSearchTaskId": str,
+    },
+)
+
 ValidateE911AddressRequestRequestTypeDef = TypedDict(
     "ValidateE911AddressRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "StreetNumber": str,
         "StreetInfo": str,
         "City": str,
@@ -1145,14 +1460,28 @@
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
+VoiceToneAnalysisTaskTypeDef = TypedDict(
+    "VoiceToneAnalysisTaskTypeDef",
+    {
+        "VoiceToneAnalysisTaskId": str,
+        "VoiceToneAnalysisTaskStatus": str,
+        "CallDetails": CallDetailsTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "StartedTimestamp": datetime,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
@@ -1374,14 +1703,91 @@
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
+    {
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
+_RequiredCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+    },
+)
+_OptionalCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVoiceProfileDomainRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateVoiceProfileDomainRequestRequestTypeDef(
+    _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
+    _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
+):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateVoiceProfileResponseTypeDef = TypedDict(
+    "CreateVoiceProfileResponseTypeDef",
+    {
+        "VoiceProfile": VoiceProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceProfileResponseTypeDef = TypedDict(
+    "GetVoiceProfileResponseTypeDef",
+    {
+        "VoiceProfile": VoiceProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceProfileResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileResponseTypeDef",
+    {
+        "VoiceProfile": VoiceProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
@@ -1593,14 +1999,32 @@
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListVoiceProfileDomainsResponseTypeDef = TypedDict(
+    "ListVoiceProfileDomainsResponseTypeDef",
+    {
+        "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVoiceProfilesResponseTypeDef = TypedDict(
+    "ListVoiceProfilesResponseTypeDef",
+    {
+        "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
         "ProductType": PhoneNumberProductTypeType,
         "Status": PhoneNumberOrderStatusType,
         "OrderType": PhoneNumberOrderTypeType,
@@ -1657,34 +2081,60 @@
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
         "OrderId": str,
     },
     total=False,
 )
 
+SpeakerSearchDetailsTypeDef = TypedDict(
+    "SpeakerSearchDetailsTypeDef",
+    {
+        "Results": List[SpeakerSearchResultTypeDef],
+        "VoiceprintGenerationStatus": str,
+    },
+    total=False,
+)
+
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
         "Disabled": bool,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
+GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "GetVoiceToneAnalysisTaskResponseTypeDef",
+    {
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
+    "StartVoiceToneAnalysisTaskResponseTypeDef",
+    {
+        "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateSipMediaApplicationResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1776,14 +2226,38 @@
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "CreateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVoiceProfileDomainResponseTypeDef = TypedDict(
+    "GetVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
+    "UpdateVoiceProfileDomainResponseTypeDef",
+    {
+        "VoiceProfileDomain": VoiceProfileDomainTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1915,14 +2389,29 @@
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SpeakerSearchTaskTypeDef = TypedDict(
+    "SpeakerSearchTaskTypeDef",
+    {
+        "SpeakerSearchTaskId": str,
+        "SpeakerSearchTaskStatus": str,
+        "CallDetails": CallDetailsTypeDef,
+        "SpeakerSearchDetails": SpeakerSearchDetailsTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "StartedTimestamp": datetime,
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1938,7 +2427,23 @@
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+GetSpeakerSearchTaskResponseTypeDef = TypedDict(
+    "GetSpeakerSearchTaskResponseTypeDef",
+    {
+        "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSpeakerSearchTaskResponseTypeDef = TypedDict(
+    "StartSpeakerSearchTaskResponseTypeDef",
+    {
+        "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.26.77
-Summary: Type annotations for boto3.ChimeSDKVoice 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKVoice 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,14 +309,15 @@
 ```python
 from mypy_boto3_chime_sdk_voice.literals import (
     AlexaSkillStatusType,
     CallingNameStatusType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
+    LanguageCodeType,
     ListSipMediaApplicationsPaginatorName,
     ListSipRulesPaginatorName,
     NotificationTargetType,
     NumberSelectionBehaviorType,
     OrderedPhoneNumberStatusType,
     OriginationRouteProtocolType,
     PhoneNumberAssociationNameType,
@@ -352,101 +353,127 @@
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
     ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
+    CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
     SipMediaApplicationCallTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
     CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
+    TagTypeDef,
+    CreateVoiceProfileRequestRequestTypeDef,
+    VoiceProfileTypeDef,
     CredentialTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
     DeleteSipRuleRequestRequestTypeDef,
     DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorGroupRequestRequestTypeDef,
     DeleteVoiceConnectorOriginationRequestRequestTypeDef,
     DeleteVoiceConnectorProxyRequestRequestTypeDef,
     DeleteVoiceConnectorRequestRequestTypeDef,
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
+    DeleteVoiceProfileDomainRequestRequestTypeDef,
+    DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
+    GetSpeakerSearchTaskRequestRequestTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorGroupRequestRequestTypeDef,
     GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     LoggingConfigurationTypeDef,
     GetVoiceConnectorOriginationRequestRequestTypeDef,
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
+    GetVoiceProfileDomainRequestRequestTypeDef,
+    GetVoiceProfileRequestRequestTypeDef,
+    GetVoiceToneAnalysisTaskRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
+    ListVoiceProfileDomainsRequestRequestTypeDef,
+    VoiceProfileDomainSummaryTypeDef,
+    ListVoiceProfilesRequestRequestTypeDef,
+    VoiceProfileSummaryTypeDef,
+    MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SpeakerSearchResultTypeDef,
+    StartSpeakerSearchTaskRequestRequestTypeDef,
+    StartVoiceToneAnalysisTaskRequestRequestTypeDef,
+    StopSpeakerSearchTaskRequestRequestTypeDef,
+    StopVoiceToneAnalysisTaskRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
+    UpdateVoiceProfileDomainRequestRequestTypeDef,
+    UpdateVoiceProfileRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetPhoneNumberSettingsResponseTypeDef,
     ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
+    VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
     CreateSipMediaApplicationRequestRequestTypeDef,
     SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
@@ -456,14 +483,21 @@
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
+    VoiceProfileDomainTypeDef,
+    CreateVoiceProfileDomainRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateVoiceProfileResponseTypeDef,
+    GetVoiceProfileResponseTypeDef,
+    UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef,
@@ -478,31 +512,39 @@
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
+    ListVoiceProfileDomainsResponseTypeDef,
+    ListVoiceProfilesResponseTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    SpeakerSearchDetailsTypeDef,
     StreamingConfigurationTypeDef,
+    GetVoiceToneAnalysisTaskResponseTypeDef,
+    StartVoiceToneAnalysisTaskResponseTypeDef,
     CreateSipMediaApplicationResponseTypeDef,
     GetSipMediaApplicationResponseTypeDef,
     ListSipMediaApplicationsResponseTypeDef,
     UpdateSipMediaApplicationResponseTypeDef,
     CreateSipRuleResponseTypeDef,
     GetSipRuleResponseTypeDef,
     ListSipRulesResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
+    CreateVoiceProfileDomainResponseTypeDef,
+    GetVoiceProfileDomainResponseTypeDef,
+    UpdateVoiceProfileDomainResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
@@ -512,59 +554,62 @@
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
+    SpeakerSearchTaskTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
     PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    GetSpeakerSearchTaskResponseTypeDef,
+    StartSpeakerSearchTaskResponseTypeDef,
 )
 
 
 def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.77/setup.py` & `mypy-boto3-chime-sdk-voice-1.26.98/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-chime-sdk-voice.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-voice",
-    version="1.26.77",
+    version="1.26.98",
     packages=["mypy_boto3_chime_sdk_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKVoice 1.26.77 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.ChimeSDKVoice 1.26.98 service generated with mypy-boto3-builder"
+        " 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/",
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

