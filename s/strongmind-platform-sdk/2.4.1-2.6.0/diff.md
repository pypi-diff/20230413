# Comparing `tmp/strongmind-platform-sdk-2.4.1.tar.gz` & `tmp/strongmind-platform-sdk-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strongmind-platform-sdk-2.4.1.tar", last modified: Mon Apr 10 22:44:15 2023, max compression
+gzip compressed data, was "strongmind-platform-sdk-2.6.0.tar", last modified: Thu Apr 13 21:08:09 2023, max compression
```

## Comparing `strongmind-platform-sdk-2.4.1.tar` & `strongmind-platform-sdk-2.6.0.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/clients/user_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/helpers/link_header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/cloud_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.478132 strongmind-platform-sdk-2.4.1/platform_sdk/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/shared/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/platform_sdk/shared/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.482132 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 22:44:15.000000 strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.482132 strongmind-platform-sdk-2.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:44:15.486132 strongmind-platform-sdk-2.4.1/test/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/event_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_academic_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_course.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_guidref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_lineitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_org_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/oneroster_user_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/factories/user_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_events_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_exception_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_identity_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_link_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_ods_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_oneroster_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_oneroster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_slack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-10 22:43:06.000000 strongmind-platform-sdk-2.4.1/test/test_user_creation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.063936 strongmind-platform-sdk-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 21:08:09.063936 strongmind-platform-sdk-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.051936 strongmind-platform-sdk-2.6.0/platform_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.051936 strongmind-platform-sdk-2.6.0/platform_sdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/mapper_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/clients/user_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.051936 strongmind-platform-sdk-2.6.0/platform_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/helpers/exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/helpers/link_header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.051936 strongmind-platform-sdk-2.6.0/platform_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/models/cloud_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/models/link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/models/partner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.055936 strongmind-platform-sdk-2.6.0/platform_sdk/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/shared/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/shared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/platform_sdk/shared/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:08:09.063936 strongmind-platform-sdk-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.055936 strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 21:08:08.000000 strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-13 21:08:08.000000 strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:08:08.000000 strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 21:08:08.000000 strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:08:08.000000 strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.059936 strongmind-platform-sdk-2.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:08:09.059936 strongmind-platform-sdk-2.6.0/test/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/event_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_academic_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_guidref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 21:06:43.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_org_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/factories/oneroster_user_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/factories/partner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/factories/response_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/factories/standalone_partner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/factories/user_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_events_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_exception_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33101 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_identity_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_link_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_ods_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_oneroster_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_oneroster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_slack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-13 21:06:44.000000 strongmind-platform-sdk-2.6.0/test/test_user_creation_client.py
```

### Comparing `strongmind-platform-sdk-2.4.1/PKG-INFO` & `strongmind-platform-sdk-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.4.1
+Version: 2.6.0
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.4.1/README.md` & `strongmind-platform-sdk-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/clients/events_client.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/clients/events_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/clients/identity_client.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/clients/identity_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import datetime
 
 import requests
 from cryptography.hazmat.backends import default_backend
-from cryptography.x509 import load_pem_x509_certificate, load_der_x509_certificate
+from cryptography.x509 import load_der_x509_certificate
 from requests import HTTPError
 from requests.auth import HTTPBasicAuth
 
 from platform_sdk.helpers.exception_logger import raise_for_status_with_dependency_name
 from platform_sdk.shared.constants import IDENTITY_SERVER
```

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/clients/ods_client.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/clients/ods_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 
 import requests
-from platform_sdk.helpers.exception_logger import raise_for_status_with_dependency_name
 
+from platform_sdk.helpers.exception_logger import raise_for_status_with_dependency_name
 from platform_sdk.shared.constants import ONEROSTER_DATA_STORE
 from platform_sdk.shared.utilities import get_plural_oneroster_type
 
 
 class OneRosterDataStoreClient:
     def __init__(self, base_url: str, key: str):
         self.base_url = base_url
```

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_authentication.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/clients/oneroster_authentication.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/clients/oneroster_client.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/clients/oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/clients/slack.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/clients/slack.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/clients/user_creation.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/clients/user_creation.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/helpers/exception_logger.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/helpers/exception_logger.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/helpers/link_header.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/helpers/link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/platform_sdk/models/user.py` & `strongmind-platform-sdk-2.6.0/platform_sdk/models/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from datetime import datetime, date
+from datetime import date
 from enum import Enum
-from typing import Optional, Any, Dict
+from typing import Optional, Dict
 
 from pydantic import BaseModel, Field
 
 
 class RoleEnum(str, Enum):
     administrator = 'administrator'
     aide = 'aide'
```

### Comparing `strongmind-platform-sdk-2.4.1/setup.py` & `strongmind-platform-sdk-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='strongmind-platform-sdk',
-    version='2.4.1',
+    version='2.6.0',
     packages=find_packages(),
     url='https://github.com/StrongMind/platform-python-sdk',
     license='',
     author='Team Platform',
     author_email='platform@strongmind.com',
     description='Common utilities, models, and clients used with StrongMind Platform APIs',
     long_description=long_description,
```

### Comparing `strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/PKG-INFO` & `strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind-platform-sdk
-Version: 2.4.1
+Version: 2.6.0
 Summary: Common utilities, models, and clients used with StrongMind Platform APIs
 Home-page: https://github.com/StrongMind/platform-python-sdk
 Author: Team Platform
 Author-email: platform@strongmind.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `strongmind-platform-sdk-2.4.1/strongmind_platform_sdk.egg-info/SOURCES.txt` & `strongmind-platform-sdk-2.6.0/strongmind_platform_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 README.md
 setup.py
 platform_sdk/__init__.py
 platform_sdk/clients/__init__.py
 platform_sdk/clients/events_client.py
 platform_sdk/clients/identity_client.py
+platform_sdk/clients/mapper_client.py
 platform_sdk/clients/ods_client.py
 platform_sdk/clients/oneroster_authentication.py
 platform_sdk/clients/oneroster_client.py
 platform_sdk/clients/slack.py
 platform_sdk/clients/user_creation.py
 platform_sdk/helpers/__init__.py
 platform_sdk/helpers/exception_logger.py
 platform_sdk/helpers/link_header.py
 platform_sdk/models/__init__.py
 platform_sdk/models/cloud_event.py
 platform_sdk/models/link_header.py
+platform_sdk/models/partner.py
 platform_sdk/models/user.py
 platform_sdk/shared/__init__.py
 platform_sdk/shared/constants.py
+platform_sdk/shared/exceptions.py
 platform_sdk/shared/utilities.py
 strongmind_platform_sdk.egg-info/PKG-INFO
 strongmind_platform_sdk.egg-info/SOURCES.txt
 strongmind_platform_sdk.egg-info/dependency_links.txt
 strongmind_platform_sdk.egg-info/requires.txt
 strongmind_platform_sdk.egg-info/top_level.txt
 test/__init__.py
@@ -42,8 +45,11 @@
 test/factories/oneroster_enrollment.py
 test/factories/oneroster_guidref.py
 test/factories/oneroster_lineitem.py
 test/factories/oneroster_org_factory.py
 test/factories/oneroster_result.py
 test/factories/oneroster_user.py
 test/factories/oneroster_user_id.py
+test/factories/partner.py
+test/factories/response_factory.py
+test/factories/standalone_partner.py
 test/factories/user_factories.py
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/event_factories.py` & `strongmind-platform-sdk-2.6.0/test/factories/event_factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 
 from factory import Dict, Faker, LazyAttribute, SelfAttribute, Factory
+
 from platform_sdk.models.cloud_event import CloudEvent
 
 
 class PowerSchoolEventFactory(Factory):
     class Meta:
         model = CloudEvent
         exclude = 'powerschool_domain', 'recordid', 'api_name'
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_academic_session.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_academic_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from factory import Factory, List, Faker, SubFactory, LazyAttribute
 from oneroster_client.models import SingleAcademicSessionType, AcademicSessionType
+
 from test.factories.oneroster_guidref import OneRosterGuidRefFactory
 
 
 class OneRosterAcademicSessionFactory(Factory):
     class Meta:
         model = AcademicSessionType
         exclude = ('base_url')
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_class.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from factory import Dict, List, Faker, LazyAttribute, Factory, SubFactory
+from factory import List, Faker, LazyAttribute, Factory, SubFactory
 from oneroster_client import SingleClassType
-
-from oneroster_client.models import ClassType, GUIDRefType
+from oneroster_client.models import ClassType
 
 from test.factories.oneroster_guidref import OneRosterGuidRefFactory
 
 
 class OneRosterClassFactory(Factory):
     class Meta:
         model = ClassType
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_course.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_course.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from factory import List, Faker, LazyAttribute, Factory, SubFactory
 from oneroster_client import SingleCourseType
-
 from oneroster_client.models import CourseType
 
 from test.factories.oneroster_guidref import OneRosterGuidRefFactory
 
 
 class OneRosterCourseFactory(Factory):
     class Meta:
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_enrollment.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_enrollment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from factory import Dict, Faker, LazyAttribute, Factory, SubFactory, List
-from oneroster_client import SingleEnrollmentType, EnrollmentsType, GUIDRefType
-
+from factory import Faker, LazyAttribute, Factory, SubFactory, List
+from oneroster_client import SingleEnrollmentType, EnrollmentsType
 from oneroster_client.models import EnrollmentType
 
 from test.factories.oneroster_guidref import OneRosterGuidRefFactory
 
 
 class OneRosterEnrollmentFactory(Factory):
     class Meta:
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_guidref.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_guidref.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_lineitem.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_lineitem.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,10 +54,12 @@
     class Meta:
         model = LineItemsType
         exclude = "class_uuid"
 
     class_uuid = Faker("uuid4")
 
     line_items = List([
-        SubFactory(OneRosterLineItemFactory, _class__sourced_id=class_uuid, category__sourced_id=GUID_ONEROSTER_CURRENT_GRADE_CATEGORY_ID),
-        SubFactory(OneRosterLineItemFactory, _class__sourced_id=class_uuid, category__sourced_id=GUID_ONEROSTER_FINAL_GRADE_CATEGORY_ID)
+        SubFactory(OneRosterLineItemFactory, _class__sourced_id=class_uuid,
+                   category__sourced_id=GUID_ONEROSTER_CURRENT_GRADE_CATEGORY_ID),
+        SubFactory(OneRosterLineItemFactory, _class__sourced_id=class_uuid,
+                   category__sourced_id=GUID_ONEROSTER_FINAL_GRADE_CATEGORY_ID)
     ])
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_org_factory.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_org_factory.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_result.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_result.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/oneroster_user.py` & `strongmind-platform-sdk-2.6.0/test/factories/oneroster_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from factory import Factory, Faker, LazyAttribute, SubFactory, List
 from oneroster_client import UsersType
-from oneroster_client.models.user_type import UserType
 from oneroster_client.models.single_user_type import SingleUserType
-from factory import Factory, Faker, LazyAttribute, SubFactory, List, Dict
+from oneroster_client.models.user_type import UserType
 
 from test.factories.oneroster_guidref import OneRosterGuidRefFactory
 from test.factories.oneroster_user_id import OneRosterUserIdFactory
 
 
 class OneRosterUserFactory(Factory):
     class Meta:
@@ -46,22 +46,24 @@
     phone = Faker("msisdn")
     agents = List([
         SubFactory(OneRosterGuidRefFactory),
         SubFactory(OneRosterGuidRefFactory)
     ])
     orgs = List([
         SubFactory(OneRosterGuidRefFactory,
-                   href=LazyAttribute(lambda o: f'{o.factory_parent.factory_parent.base_url}orgs/{o.factory_parent.factory_parent.org_sourced_id}'),
+                   href=LazyAttribute(lambda
+                                          o: f'{o.factory_parent.factory_parent.base_url}orgs/{o.factory_parent.factory_parent.org_sourced_id}'),
                    sourced_id=Faker('uuid4'),
                    type='org'
                    )
     ])
     grades = List([Faker('word',
-                   ext_word_list=['IT', 'PR', 'PK', 'TK', 'KG', '01', '02', '03', '04', '05', '06', '07', '08', '09',
-                                  '10', '11', '12', '13', 'PS', 'UG', 'Other'])])
+                         ext_word_list=['IT', 'PR', 'PK', 'TK', 'KG', '01', '02', '03', '04', '05', '06', '07', '08',
+                                        '09',
+                                        '10', '11', '12', '13', 'PS', 'UG', 'Other'])])
     password = None
 
 
 class OneRosterSingleUserFactory(Factory):
     class Meta:
         model = SingleUserType
```

### Comparing `strongmind-platform-sdk-2.4.1/test/factories/user_factories.py` & `strongmind-platform-sdk-2.6.0/test/factories/user_factories.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/test_events_client.py` & `strongmind-platform-sdk-2.6.0/test/test_events_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 from expects import expect, equal
 from faker import Faker
 from freezegun import freeze_time
 from mockito import when, mock, unstub, verifyStubbedInvocationsAreUsed
 from pydantic.json import pydantic_encoder
 from requests import HTTPError
 
-from test.factories.event_factories import PowerSchoolEventFactory
-
 from platform_sdk.clients.events_client import EventPlatformClient
 from platform_sdk.clients.identity_client import IdentityServerClient
+from test.factories.event_factories import PowerSchoolEventFactory
 from test.helpers.test_helpers import create_http_error
 
 fake = Faker()
 
 
 class TestEventPipelineClient(unittest.TestCase):
     def setUp(self) -> None:
```

### Comparing `strongmind-platform-sdk-2.4.1/test/test_exception_logger.py` & `strongmind-platform-sdk-2.6.0/test/test_exception_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import unittest
-from logging import Logger
 
 import requests
 from expects import expect, equal
 from faker import Faker
 from mockito import mock, when, verify, arg_that
 from requests import HTTPError, Response
 
@@ -13,15 +12,15 @@
 from test.helpers.test_helpers import create_http_error
 
 fake = Faker()
 
 
 class TestExceptionLogger(unittest.TestCase):
     def setUp(self) -> None:
-        self.logger = mock(Logger)
+        self.logger = mock()
         when(self.logger).exception(...)
         self.request_body = json.dumps({fake.word(): fake.sentence()})
         self.request_headers = {fake.word(): fake.sentence()}
         self.url = fake.url()
         self.dependency_name = fake.word()
         self.status_code = fake.random_int()
         self.response_text = fake.sentence()
```

### Comparing `strongmind-platform-sdk-2.4.1/test/test_identity_client.py` & `strongmind-platform-sdk-2.6.0/test/test_identity_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         mock_response = mock({'text': response_text})
         when(self.id_server_client)._headers().thenReturn(headers)
         when(requests).patch(url, headers=headers, json=data).thenReturn(mock_response)
         with self.assertRaises(IdentityClientError) as assert_error:
             self.id_server_client.update_account(identity_id, username=data['username'])
         expect(str(assert_error.exception)).to(equal(response_text))
 
-
     @freeze_time("2020-07-31")
     def test_identity_client_issues_new_token_when_none_exists(self):
         """When there is no token, we should get a new one so that we can have access"""
         expected_token = fake.word()
         response = mock({'status_code': 200, 'json': lambda: {"access_token": expected_token, "expires_in": 3600}})
         self.mock_token_retrieval(response)
         token = self.id_server_client.get_token()
```

### Comparing `strongmind-platform-sdk-2.4.1/test/test_link_header.py` & `strongmind-platform-sdk-2.6.0/test/test_link_header.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/test_ods_client.py` & `strongmind-platform-sdk-2.6.0/test/test_ods_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/test_oneroster_authentication.py` & `strongmind-platform-sdk-2.6.0/test/test_oneroster_authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import unittest
 
-import mockito.invocation
 import requests
-import urllib3
-from faker import Faker
 from expects import *
-from mockito import mock, when, patch, unstub, captor
+from faker import Faker
+from mockito import mock, when, unstub, captor
 from oneroster_client import ApiClient
-from oneroster_client.rest import RESTResponse
 from requests import Response
 from requests.structures import CaseInsensitiveDict
 
 from platform_sdk.clients.identity_client import IdentityServerClient
 from platform_sdk.clients.oneroster_authentication import get_authenticated_oneroster_client_with_identity_server, \
     AuthenticatedConfig
 
@@ -30,15 +27,15 @@
         self.mock_response = mock(Response)
         self.mock_response.status_code = 200
         self.mock_response.headers = CaseInsensitiveDict({})
         when(self.mock_response).raise_for_status()
 
         self.header_captor = captor()
 
-        when(requests).request(any, any, params=any, json=any, headers=self.header_captor, timeout=any)\
+        when(requests).request(any, any, params=any, json=any, headers=self.header_captor, timeout=any) \
             .thenReturn(self.mock_response)
 
     def test_gets_authenticated_client(self):
         # Arrange
         when(self.id_server_client).get_token().thenReturn(self.token)
         base_url = f"https://{fake.domain_word()}"
```

### Comparing `strongmind-platform-sdk-2.4.1/test/test_oneroster_client.py` & `strongmind-platform-sdk-2.6.0/test/test_oneroster_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/test_slack_client.py` & `strongmind-platform-sdk-2.6.0/test/test_slack_client.py`

 * *Files identical despite different names*

### Comparing `strongmind-platform-sdk-2.4.1/test/test_user_creation_client.py` & `strongmind-platform-sdk-2.6.0/test/test_user_creation_client.py`

 * *Files identical despite different names*

