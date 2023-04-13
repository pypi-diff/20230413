# Comparing `tmp/zcatalyst_sdk-0.0.2rc1.tar.gz` & `tmp/zcatalyst_sdk-0.0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcatalyst_sdk-0.0.2rc1.tar", last modified: Fri Mar 17 12:45:35 2023, max compression
+gzip compressed data, was "zcatalyst_sdk-0.0.2rc2.tar", last modified: Thu Apr 13 07:54:35 2023, max compression
```

## Comparing `zcatalyst_sdk-0.0.2rc1.tar` & `zcatalyst_sdk-0.0.2rc2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      639 2023-03-07 13:18:06.000000 zcatalyst_sdk-0.0.2rc1/LICENSE
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       98 2023-03-07 13:18:06.000000 zcatalyst_sdk-0.0.2rc1/MANIFEST.in
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/PKG-INFO
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1441 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/README.md
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       38 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/setup.cfg
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1129 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/setup.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.095033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6151 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       57 2023-03-16 09:58:21.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/__version__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3488 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/_constants.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7393 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/_http_client.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      519 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/_thread_util.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7851 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/authentication.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/cache/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1675 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/cache/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3589 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/cache/_segment.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6050 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/catalyst_app.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2183 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/circuit.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/connection/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2397 2023-03-14 21:48:12.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/connection/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4064 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/connection/_connector.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)    11824 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/credentials.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3313 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/cron.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/datastore/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1599 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/datastore/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3191 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/datastore/_bulk_job.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     5574 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/datastore/_table.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2496 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/email.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3387 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/exceptions.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/filestore/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2001 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/filestore/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4478 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/filestore/_folder.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      405 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/filestore/_helper.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1140 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/functions.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/push_notification/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      794 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/push_notification/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1280 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/push_notification/_mobile_notification.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1035 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/push_notification/_web_notificaton.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1203 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/search.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/types/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7235 2023-03-17 09:47:13.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/types/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2999 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/types/zia.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     8462 2023-03-16 09:56:29.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/validator.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1073 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/zcql.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/zia/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7843 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/zia/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      583 2023-03-14 19:43:07.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/zia/_helper.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-03-17 12:45:35.099033 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-03-17 12:45:35.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1277 2023-03-17 12:45:35.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)        1 2023-03-17 12:45:35.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       17 2023-03-17 12:45:35.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/requires.txt
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       14 2023-03-17 12:45:35.000000 zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      639 2023-03-07 13:18:06.000000 zcatalyst_sdk-0.0.2rc2/LICENSE
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       98 2023-03-30 10:55:22.000000 zcatalyst_sdk-0.0.2rc2/MANIFEST.in
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/PKG-INFO
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1441 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/README.md
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       16 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/requirements.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       38 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/setup.cfg
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1129 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/setup.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6151 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       57 2023-04-13 07:52:53.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/__version__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3525 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_constants.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7485 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_http_client.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      519 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_thread_util.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7851 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/authentication.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1675 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3589 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/_segment.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6190 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/catalyst_app.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2183 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/circuit.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2397 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4064 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/_connector.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)    11824 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/credentials.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3313 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cron.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1599 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3092 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_bulk_job.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     5552 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_table.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2611 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/email.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3539 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/exceptions.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2001 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4544 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/_folder.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1140 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/functions.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      794 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1280 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_mobile_notification.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1035 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_web_notificaton.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1203 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/search.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4027 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/smart_browz.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7235 2023-03-29 09:36:20.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1630 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/smart_browz.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2999 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/zia.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     8879 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/validator.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1073 2023-04-10 07:00:22.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zcql.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     8247 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zia.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1285 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)        1 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       17 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/requires.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       14 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/top_level.txt
```

### Comparing `zcatalyst_sdk-0.0.2rc1/LICENSE` & `zcatalyst_sdk-0.0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/PKG-INFO` & `zcatalyst_sdk-0.0.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcatalyst_sdk
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: Zoho Catalyst SDK for Python
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcatalyst_sdk Version: 0.0.2rc1 Summary: Zoho
+Metadata-Version: 2.1 Name: zcatalyst_sdk Version: 0.0.2rc2 Summary: Zoho
 Catalyst SDK for Python Home-page: https://catalyst.zoho.com/ Author: Catalyst
 by Zoho Author-email: support@zohocatalyst.com License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Requires-Python: >= 3.9
```

### Comparing `zcatalyst_sdk-0.0.2rc1/README.md` & `zcatalyst_sdk-0.0.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/setup.py` & `zcatalyst_sdk-0.0.2rc2/setup.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/_constants.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 # URL constants
 PROJECT_URL = "project"
 PROJECT_KEY_NAME = "PROJECT_ID"
 FILE_SEPERATOR = "/"
 IS_LOCAL = env_override("X_ZOHO_CATALYST_IS_LOCAL", "False")
 CSRF_TOKEN_COOKIE = "ZD_CSRF_TOKEN"
 APP_DOMAIN = env_override("X_ZOHO_CATALYST_CONSOLE_URL", "https://console.catalyst.localzoho.com")
-APP_BAAS = "/baas"
 APP_VERSION_V1 = "/v1"
-APP_BASE_URL = APP_DOMAIN + APP_BAAS + APP_VERSION_V1
 ACCOUNTS_URL = env_override("X_ZOHO_CATALYST_ACCOUNTS_URL", "https://accounts.localzoho.com")
 
 # Header Constants
 CONTENT_TYPE = "Content-Type"
 CLIENT_HEADER = "PROJECT_ID"
 COOKIE_HEADER = "Cookie"
 CSRF_HEADER = "X-ZCSRF-TOKEN"
@@ -111,14 +109,15 @@
     ZIA = "Zia"
     CRON = "Cron"
     DATA_STORE = "DataStore"
     FUNCTION = "Function"
     AUTHENTICATION = "Authentication"
     CIRCUIT = "Circuit"
     PUSH_NOTIFICATION = "PushNotification"
+    SMART_BROWZ = "SmartBrowz"
 
 
 class CredentialType:
     token = 'token'
     ticket = 'ticket'
 
 
@@ -134,7 +133,12 @@
     admin_cred_type = 'X-ZC-Admin-Cred-Type'
     user_cred_type = 'X-ZC-User-Cred-Type'
     admin_token = 'X-ZC-Admin-Cred-Token'
     user_token = 'X-ZC-User-Cred-Token'
     cookie = 'x-zc-cookie'
     zcsrf = 'X-ZCSRF-TOKEN'
     user = 'X-ZC-User-Type'
+
+
+class CatalystService:
+    SERVERLESS = 'baas'
+    BROWSER360 = 'browser360'
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/_http_client.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import os
 from typing import Dict
 import requests
 from requests import Response
 from urllib3.util import retry
 from .exceptions import CatalystAPIError
 from .credentials import (
     AccessTokenCredential,
     RefreshTokenCredential,
     TicketCredential,
     CatalystCredential
 )
 from ._constants import (
     APP_DOMAIN,
-    APP_BAAS,
     APP_VERSION_V1,
     USER_AGENT,
     SDK_VERSION,
     AUTHORIZATION,
     TICKET_PREFIX,
     OAUTH_PREFIX,
     COOKIE_HEADER,
@@ -26,15 +26,16 @@
     ENVIRONMENT_KEY_NAME,
     ENVIRONMENT,
     PROJECT_SECRET_KEY,
     USER_KEY_NAME,
     PROJECT_DOMAIN,
     AcceptHeader,
     CredentialUser,
-    ProjectHeader
+    ProjectHeader,
+    CatalystService
 )
 
 USERAGENT_HEADER = {USER_AGENT: "zc-python-sdk/" + SDK_VERSION}
 
 # Default timeout for connect and read operation in seconds
 DEFAULT_TIMEOUT = (60, 30)
 
@@ -132,15 +133,15 @@
 
     def request(
         self,
         method: str,
         url: str = None,
         path: str = None,
         user=CredentialUser.ADMIN,
-        catalyst=None,
+        catalyst_service=None,
         **kwargs
     ):
         if 'timeout' not in kwargs:
             kwargs['timeout'] = self._timeout
 
         if 'headers' not in kwargs:
             kwargs['headers'] = {}
@@ -168,22 +169,22 @@
             if IS_LOCAL == 'true':
                 if user == CredentialUser.ADMIN:
                     self._base_url = \
                         'https://' + APP_DOMAIN.replace('https://', '').replace('http://', '')
                 elif user == CredentialUser.USER:
                     self._base_url = 'https://' + self._app.config.get(PROJECT_DOMAIN)
 
-            if catalyst:
+            if catalyst_service:
                 project_id = self._app.config.get('project_id')
-                path = APP_BAAS + APP_VERSION_V1 + f'/project/{project_id}' + (path or '')
+                path = catalyst_service + APP_VERSION_V1 + f'/project/{project_id}' + (path or '')
                 headers[AcceptHeader.KEY] = AcceptHeader.VALUE
 
         self._base_url = self._base_url or APP_DOMAIN
 
-        url = url or (self._base_url + path)
+        url = url or (os.path.join(self._base_url, path))
         resp = self._session.request(method, url, **kwargs)
 
         return DefaultHttpResponse(resp)
 
     def close(self):
         self._session.close()
         self._session = None
@@ -198,20 +199,20 @@
 
     def request(
         self,
         method: str,
         url: str = None,
         path: str = None,
         user=CredentialUser.USER,
-        catalyst=True,
+        catalyst_service=CatalystService.SERVERLESS,
         **kwargs
     ):
         self._app.credential._switch_user(user)  # pylint: disable=protected-access
         self._authenticate_request(kwargs)
-        return super().request(method, url, path, user, catalyst, **kwargs)
+        return super().request(method, url, path, user, catalyst_service, **kwargs)
 
     def _authenticate_request(self, kwargs):
 
         # if 'headers' not in kwargs:
         #     kwargs['headers'] = {}
         # headers = kwargs['headers']
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/_thread_util.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_thread_util.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/authentication.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/authentication.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/cache/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/cache/_segment.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/_segment.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/catalyst_app.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/catalyst_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .search import Search
 from .functions import Functions
 from .authentication import Authentication
 from .push_notification import PushNotification
 from .zia import Zia
 from .circuit import Circuit
 from .connection import Connection
+from .smart_browz import SmartBrowz
 
 CATALYST_OPTIONS_ENV_KEY = 'CATALYST_OPTIONS'
 CONFIG_MANDATORIES = {
     APIConstants.PROJECT_ID: (int, str),
     APIConstants.PROJECT_KEY: (int, str),
     APIConstants.PROJECT_DOMAIN: (str,)
 }
@@ -173,12 +174,15 @@
 
     def circuit(self) -> Circuit:
         return self._ensure_service('circuit', Circuit)
 
     def connection(self, properties: Union[str, Dict[str, Dict[str, str]]]) -> Connection:
         return self._ensure_service('connection', Connection, override=True, properties=properties)
 
+    def smart_browz(self) -> SmartBrowz:
+        return self._ensure_service('SmartBrowz', SmartBrowz)
+
     def _ensure_service(self, service_name: str, initializer, **kwargs):
         with self._lock:
             if service_name not in self._services or kwargs.get('override'):
                 self._services[service_name] = initializer(self, **kwargs)
             return self._services[service_name]
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/circuit.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/circuit.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/connection/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/connection/_connector.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/_connector.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/credentials.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/credentials.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/cron.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cron.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/datastore/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/datastore/_bulk_job.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_bulk_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC
 from typing import Union
-from urllib3.response import HTTPResponse
 from ..exceptions import CatalystDatastoreError
 from ..types import (
     Component,
     ICatalystBulkJob,
     ICatalystBulkCallback,
     ICatalystBulkReadQuery,
     ICatalystBulkWriteInput
@@ -32,23 +31,23 @@
         resp = self._requester.request(
             method=RequestMethod.GET,
             path=f'/bulk/{self._operation}/{job_id}',
             user=CredentialUser.ADMIN
         )
         return resp.response_json.get('data')
 
-    def get_result(self, job_id: Union[str, int]) -> HTTPResponse:
+    def get_result(self, job_id: Union[str, int]):
         validator.is_non_empty_string_or_number(job_id, 'job_id', CatalystDatastoreError)
         resp = self._requester.request(
             method=RequestMethod.GET,
             path=f'/bulk/{self._operation}/{job_id}/download',
             user=CredentialUser.ADMIN,
             stream=True
         )
-        return resp._response.raw  # pylint: disable=protected-access
+        return resp.response
 
 
 class BulkRead(BulkJob):
     def __init__(self, table_instance):
         super().__init__(table_instance, 'read')
 
     def create_job(
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/datastore/_table.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             params=req_params,
             user=CredentialUser.USER
         )
 
         resp_json = resp.response_json
         return resp_json
 
-    def get_iterable_rows(self) -> List[ICatalystRow]:
+    def get_iterable_rows(self):
         next_token: str = None
         while True:
             rows_output = self.get_paged_rows(next_token)
             for row in rows_output.get('data'):
                 yield row
             next_token = rows_output.get('next_token')
             if next_token is None:
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/email.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
                     if key == 'attachments':
                         for attachment in mail_obj[key]:
                             Email._is_valid_attachment(attachment)
                             data.append((key, attachment))
                     else:
                         listed_keys: list = mail_obj[key]
                         data.append((key, (None, ','.join(listed_keys))))
+                elif data_type is bool:
+                    data.append((key, (None, str(mail_obj[key]).lower())))
                 else:
                     data.append((key, (None, mail_obj[key])))
         return data
 
     @staticmethod
     def _is_valid_attachment(attachment):
         if not isinstance(attachment, BufferedReader):
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/exceptions.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,7 +114,12 @@
     def __init__(self, code, message, value=None):
         CatalystError.__init__(self, code, message, value)
 
 
 class CatalystZiaError(CatalystError):
     def __init__(self, code, message, value=None):
         CatalystError.__init__(self, code, message, value)
+
+
+class BrowserLogicError(CatalystError):
+    def __init__(self, code, message, value=None):
+        CatalystError.__init__(self, code, message, value)
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/filestore/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/filestore/_folder.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/_folder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 from io import BufferedReader
-from typing import Dict, Union
-from urllib3.response import HTTPResponse
-from ..types import ParsableComponent
+from typing import Dict, Optional, Union
 from ..exceptions import CatalystFilestoreError
 from .._http_client import AuthorizedHttpClient
 from .. import validator
 from .._constants import (
     RequestMethod,
     CredentialUser,
     Components
 )
-from ._helper import (
-    ICatalystFileDetails,
-    ICatalystFolderDetails
+from ..types import (
+    ParsableComponent,
+    ICatalystFile,
+    ICatalystFolder,
+    ICatalystGResponse,
+    ICatalystProject,
+    ICatalystSysUser
 )
 
 
+class ICatalystFolderDetails(ICatalystFolder):
+    created_time: Optional[str]
+    created_by: Optional[ICatalystSysUser]
+    project_details: Optional[ICatalystProject]
+
+
+class ICatalystFileDetails(ICatalystFile, ICatalystGResponse):
+    pass
+
+
 class Folder(ParsableComponent):
     def __init__(self, filestore_instance, folder_details: Dict):
         validator.is_non_empty_dict(folder_details, 'folder_details', CatalystFilestoreError)
         self._requester: AuthorizedHttpClient = filestore_instance._requester
         self._folder_details = folder_details
         self._id = folder_details.get('id')
 
@@ -92,30 +104,26 @@
             },
             user=CredentialUser.USER
         )
         resp_json = resp.response_json
         return resp_json.get('data')
 
     def download_file(self, file_id: Union[int, str]):
-        resp = self._hit_download_req(file_id)
+        resp = self.get_file_stream(file_id)
         return resp.content
 
-    def get_file_stream(self, file_id: Union[int, str]) -> HTTPResponse:
-        resp = self._hit_download_req(file_id)
-        return resp.raw
-
-    def _hit_download_req(self, file_id: Union[int, str]):
+    def get_file_stream(self, file_id: Union[int, str]):
         validator.is_non_empty_string_or_number(file_id, 'file_id', CatalystFilestoreError)
         resp = self._requester.request(
             method=RequestMethod.GET,
             path=f'/folder/{self._id}/file/{file_id}/download',
             user=CredentialUser.USER,
             stream=True
         )
-        return resp._response  # pylint: disable=protected-access
+        return resp.response
 
     @staticmethod
     def _validate_file_details(name, file):
         if not isinstance(file, BufferedReader):
             raise CatalystFilestoreError(
                 'INVALID_FILE_DETAILS',
                 'Code must be an instance of BufferReader and cannot be empty'
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/functions.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/functions.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/push_notification/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/push_notification/_mobile_notification.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_mobile_notification.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/push_notification/_web_notificaton.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_web_notificaton.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/search.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/search.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/types/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/types/zia.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/zia.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/validator.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,7 +361,24 @@
                 raise exception(
                     'Invalid-Argument',
                     f"Value for the key '{key}' cannot be None or undefined in {attr_name} dict",
                     obj
                 )
             return False
     return True
+
+
+def is_valid_url(url):
+    """
+    validates the given value is a valid url
+
+    Args:
+        email: The value to validate.
+
+    Returns:
+        bool: Whether the value is a valid url or not.
+    """
+    regex = """^https?:\\/\\/(?:www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}
+            \\.[a-zA-Z0-9()]{1,6}\\b(?:[-a-zA-Z0-9()@:%_\\+.~#?&\\/=]*)$"""
+    if re.match(regex, url):
+        return True
+    return False
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/zcql.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zcql.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk/zia/__init__.py` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zia.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 from io import BufferedReader
-from typing import Any, Dict, List, Optional, Union
-from .. import validator
-from ..types import Component
-from .._http_client import AuthorizedHttpClient
-from ..exceptions import CatalystZiaError
-from .._constants import Components, RequestMethod, CredentialUser
-from ..types.zia import (
+from typing import Any, Dict, List, Optional, TypedDict, Union
+from . import validator
+from .types import Component
+from ._http_client import AuthorizedHttpClient
+from .exceptions import CatalystZiaError
+from ._constants import Components, RequestMethod, CredentialUser
+from .types.zia import (
     ICatalystZiaKeywordExtraction,
     ICatalystZiaBarcode,
     ICatalystZiaFace,
     ICatalystZiaFaceComparison,
     ICatalystZiaModeration,
     ICatalystZiaOCR,
     ICatalystZiaObject,
     ICatalystZiaSentimentAnalysis
 )
-from ._helper import (
-    ICatalystOCROptions,
-    ICatalystImageModerationOpts,
-    ICatalystBarCodeOptions,
-    ICatalystFaceAnalysisOptions
-)
+
+ICatalystOCROptions = TypedDict('ICatalystOCROptions', {
+    'language': Optional[str],
+    'model_type': Optional[str]
+}, total=False)
+
+ICatalystBarCodeOptions = TypedDict('ICatalystBarCodeOptions', {
+    'format': Optional[str]
+})
+
+ICatalystImageModerationOpts = TypedDict('ICatalystImageModerationOpt', {
+    'mode': Optional[str]
+})
+
+ICatalystFaceAnalysisOptions = TypedDict('ICatalystFaceAnalysisOptions', {
+    'mode': Optional[str],
+    'emotion': Optional[bool],
+    'age': Optional[bool],
+    'gender': Optional[bool]
+}, total=False)
+
 
 
 class Zia(Component):
     def __init__(self, app):
         self._app = app
         self._requester = AuthorizedHttpClient(app)
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/PKG-INFO` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcatalyst-sdk
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: Zoho Catalyst SDK for Python
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcatalyst-sdk Version: 0.0.2rc1 Summary: Zoho
+Metadata-Version: 2.1 Name: zcatalyst-sdk Version: 0.0.2rc2 Summary: Zoho
 Catalyst SDK for Python Home-page: https://catalyst.zoho.com/ Author: Catalyst
 by Zoho Author-email: support@zohocatalyst.com License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Requires-Python: >= 3.9
```

### Comparing `zcatalyst_sdk-0.0.2rc1/zcatalyst_sdk.egg-info/SOURCES.txt` & `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 zcatalyst_sdk/__init__.py
 zcatalyst_sdk/__version__.py
 zcatalyst_sdk/_constants.py
 zcatalyst_sdk/_http_client.py
 zcatalyst_sdk/_thread_util.py
 zcatalyst_sdk/authentication.py
@@ -12,31 +13,31 @@
 zcatalyst_sdk/circuit.py
 zcatalyst_sdk/credentials.py
 zcatalyst_sdk/cron.py
 zcatalyst_sdk/email.py
 zcatalyst_sdk/exceptions.py
 zcatalyst_sdk/functions.py
 zcatalyst_sdk/search.py
+zcatalyst_sdk/smart_browz.py
 zcatalyst_sdk/validator.py
 zcatalyst_sdk/zcql.py
+zcatalyst_sdk/zia.py
 zcatalyst_sdk.egg-info/PKG-INFO
 zcatalyst_sdk.egg-info/SOURCES.txt
 zcatalyst_sdk.egg-info/dependency_links.txt
 zcatalyst_sdk.egg-info/requires.txt
 zcatalyst_sdk.egg-info/top_level.txt
 zcatalyst_sdk/cache/__init__.py
 zcatalyst_sdk/cache/_segment.py
 zcatalyst_sdk/connection/__init__.py
 zcatalyst_sdk/connection/_connector.py
 zcatalyst_sdk/datastore/__init__.py
 zcatalyst_sdk/datastore/_bulk_job.py
 zcatalyst_sdk/datastore/_table.py
 zcatalyst_sdk/filestore/__init__.py
 zcatalyst_sdk/filestore/_folder.py
-zcatalyst_sdk/filestore/_helper.py
 zcatalyst_sdk/push_notification/__init__.py
 zcatalyst_sdk/push_notification/_mobile_notification.py
 zcatalyst_sdk/push_notification/_web_notificaton.py
 zcatalyst_sdk/types/__init__.py
-zcatalyst_sdk/types/zia.py
-zcatalyst_sdk/zia/__init__.py
-zcatalyst_sdk/zia/_helper.py
+zcatalyst_sdk/types/smart_browz.py
+zcatalyst_sdk/types/zia.py
```

