# Comparing `tmp/icotest-voice-1.0.33.tar.gz` & `tmp/icotest-voice-1.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icotest-voice-1.0.33.tar", last modified: Tue Apr 11 16:58:42 2023, max compression
+gzip compressed data, was "icotest-voice-1.0.34.tar", last modified: Thu Apr 13 12:31:01 2023, max compression
```

## Comparing `icotest-voice-1.0.33.tar` & `icotest-voice-1.0.34.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.33/LICENSE
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.33/MANIFEST.in
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8426 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6838 2023-04-11 16:53:31.000000 icotest-voice-1.0.33/README.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.429165 icotest-voice-1.0.33/docs/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      832 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Controller.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/ControllersApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Device.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    37038 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/DevicesApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/HostConfig.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineObject.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineObject1.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineResponse200.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineResponse200Files.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Message.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Request.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/RequestsApi.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/__init__.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice/api/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   102070 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/requests_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api_client.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/configuration.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/exceptions.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice/models/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10413 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14073 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/rest.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice.egg-info/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8426 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/SOURCES.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/dependency_links.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/requires.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/top_level.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-04-11 16:48:26.000000 icotest-voice-1.0.33/pyproject.toml
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/setup.cfg
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/test/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1831 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_requests_api.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.34/LICENSE
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.34/MANIFEST.in
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8427 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6839 2023-04-13 12:26:43.000000 icotest-voice-1.0.34/README.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.724501 icotest-voice-1.0.34/docs/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      832 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Controller.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/ControllersApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Device.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    37038 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/DevicesApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/HostConfig.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineObject.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineObject1.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineResponse200.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/InlineResponse200Files.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Message.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/Request.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/docs/RequestsApi.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/__init__.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice/api/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   102070 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api/requests_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/api_client.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/configuration.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/exceptions.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice/models/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10413 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14628 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/models/request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/icotest_voice/rest.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.728501 icotest-voice-1.0.34/icotest_voice.egg-info/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8427 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/requires.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-04-13 12:31:01.000000 icotest-voice-1.0.34/icotest_voice.egg-info/top_level.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-04-13 12:28:49.000000 icotest-voice-1.0.34/pyproject.toml
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/setup.cfg
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-13 12:31:01.732501 icotest-voice-1.0.34/test/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1830 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-04-13 12:22:04.000000 icotest-voice-1.0.34/test/test_requests_api.py
```

### Comparing `icotest-voice-1.0.33/LICENSE` & `icotest-voice-1.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/PKG-INFO` & `icotest-voice-1.0.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.33
+Version: 1.0.34
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.33
-- Package version: 1.0.33
+- API version: 1.0.34
+- Package version: 1.0.34
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -64,15 +64,16 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c'  # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
+
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 ```
```

### Comparing `icotest-voice-1.0.33/README.md` & `icotest-voice-1.0.34/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.33
-- Package version: 1.0.33
+- API version: 1.0.34
+- Package version: 1.0.34
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -43,15 +43,16 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c'  # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
+
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 ```
```

### Comparing `icotest-voice-1.0.33/docs/Controller.md` & `icotest-voice-1.0.34/docs/Controller.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/docs/ControllersApi.md` & `icotest-voice-1.0.34/docs/ControllersApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/docs/Device.md` & `icotest-voice-1.0.34/docs/Device.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/docs/DevicesApi.md` & `icotest-voice-1.0.34/docs/DevicesApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/docs/Request.md` & `icotest-voice-1.0.34/docs/Request.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/docs/RequestsApi.md` & `icotest-voice-1.0.34/docs/RequestsApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/icotest_voice/__init__.py` & `icotest-voice-1.0.34/icotest_voice/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.33"
+__version__ = "1.0.34"
 
 # import apis into sdk package
 from icotest_voice.api.controllers_api import ControllersApi
 from icotest_voice.api.devices_api import DevicesApi
 from icotest_voice.api.requests_api import RequestsApi
 
 # import ApiClient
```

### Comparing `icotest-voice-1.0.33/icotest_voice/api/controllers_api.py` & `icotest-voice-1.0.34/icotest_voice/api/controllers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/icotest_voice/api/devices_api.py` & `icotest-voice-1.0.34/icotest_voice/api/devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/icotest_voice/api/requests_api.py` & `icotest-voice-1.0.34/icotest_voice/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/icotest_voice/api_client.py` & `icotest-voice-1.0.34/icotest_voice/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.33/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.34/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `icotest-voice-1.0.33/icotest_voice/configuration.py` & `icotest-voice-1.0.34/icotest_voice/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -251,16 +251,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.33\n"\
-               "SDK Package Version: 1.0.33".\
+               "Version of the API: 1.0.34\n"\
+               "SDK Package Version: 1.0.34".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `icotest-voice-1.0.33/icotest_voice/exceptions.py` & `icotest-voice-1.0.34/icotest_voice/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/__init__.py` & `icotest-voice-1.0.34/icotest_voice/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/controller.py` & `icotest-voice-1.0.34/icotest_voice/models/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/device.py` & `icotest-voice-1.0.34/icotest_voice/models/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -333,14 +333,20 @@
         """Sets the callback_port of this Device.
 
         The call back port number  # noqa: E501
 
         :param callback_port: The callback_port of this Device.  # noqa: E501
         :type: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                callback_port is not None and callback_port > 65535):  # noqa: E501
+            raise ValueError("Invalid value for `callback_port`, must be a value less than or equal to `65535`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                callback_port is not None and callback_port < 1):  # noqa: E501
+            raise ValueError("Invalid value for `callback_port`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._callback_port = callback_port
 
     @property
     def management_status(self):
         """Gets the management_status of this Device.  # noqa: E501
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/host_config.py` & `icotest-voice-1.0.34/icotest_voice/models/host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/inline_object.py` & `icotest-voice-1.0.34/icotest_voice/models/inline_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/inline_object1.py` & `icotest-voice-1.0.34/icotest_voice/models/inline_object1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/inline_response200.py` & `icotest-voice-1.0.34/icotest_voice/models/inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/inline_response200_files.py` & `icotest-voice-1.0.34/icotest_voice/models/inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/message.py` & `icotest-voice-1.0.34/icotest_voice/models/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/models/request.py` & `icotest-voice-1.0.34/icotest_voice/models/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.33/icotest_voice/rest.py` & `icotest-voice-1.0.34/icotest_voice/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/icotest_voice.egg-info/PKG-INFO` & `icotest-voice-1.0.34/icotest_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.33
+Version: 1.0.34
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.33
-- Package version: 1.0.33
+- API version: 1.0.34
+- Package version: 1.0.34
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -64,15 +64,16 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c'  # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
+
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 ```
```

### Comparing `icotest-voice-1.0.33/icotest_voice.egg-info/SOURCES.txt` & `icotest-voice-1.0.34/icotest_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.33/pyproject.toml` & `icotest-voice-1.0.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icotest-voice"
-version = "1.0.33"
+version = "1.0.34"
 description = "Icotest Voice API"
 readme = "README.md"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Icotest Voice"]
 authors = [
     { name = "Shaun Hirst", email =  "shaun.hirst@3adesign.co.uk" },
     { name = "Ivo Shipkaliev", email = "ivo@3adesign.co.uk" }
 ]
```

### Comparing `icotest-voice-1.0.33/test/test_controller.py` & `icotest-voice-1.0.34/test/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_controllers_api.py` & `icotest-voice-1.0.34/test/test_controllers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_device.py` & `icotest-voice-1.0.34/test/test_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -41,15 +41,15 @@
                 serial_no = 'serial-123456', 
                 device_type = 'handset', 
                 url = '/dev/ttyACM1', 
                 created = '2021-06-24T14:15:22Z', 
                 updated = '2021-06-24T14:15:22Z', 
                 controller_id = '10cda64a-0dce-4663-8b47-6ec1867f9568', 
                 device_status = icotest_voice.models.device_status.device_status(), 
-                callback_port = 56, 
+                callback_port = 1, 
                 management_status = True, 
                 last_contact = '2019-08-24T14:15:22Z'
             )
         else :
             return Device(
         )
```

### Comparing `icotest-voice-1.0.33/test/test_devices_api.py` & `icotest-voice-1.0.34/test/test_devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_host_config.py` & `icotest-voice-1.0.34/test/test_host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_inline_object.py` & `icotest-voice-1.0.34/test/test_inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_inline_object1.py` & `icotest-voice-1.0.34/test/test_inline_object1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_inline_response200.py` & `icotest-voice-1.0.34/test/test_inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_inline_response200_files.py` & `icotest-voice-1.0.34/test/test_inline_response200_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_message.py` & `icotest-voice-1.0.34/test/test_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_request.py` & `icotest-voice-1.0.34/test/test_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.33/test/test_requests_api.py` & `icotest-voice-1.0.34/test/test_requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.33
+    The version of the OpenAPI document: 1.0.34
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

