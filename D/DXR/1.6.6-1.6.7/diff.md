# Comparing `tmp/DXR-1.6.6.tar.gz` & `tmp/DXR-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.6.6.tar", last modified: Thu Apr  6 00:37:28 2023, max compression
+gzip compressed data, was "DXR-1.6.7.tar", last modified: Thu Apr 13 01:30:49 2023, max compression
```

## Comparing `DXR-1.6.6.tar` & `DXR-1.6.7.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.955577 DXR-1.6.6/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.888887 DXR-1.6.6/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-06 00:37:28.000000 DXR-1.6.6/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1291 2023-04-06 00:37:28.000000 DXR-1.6.6/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-06 00:37:28.000000 DXR-1.6.6/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-06 00:37:28.000000 DXR-1.6.6/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-06 00:37:28.000000 DXR-1.6.6/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.890597 DXR-1.6.6/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.6.6/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.6.6/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.6.6/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.893814 DXR-1.6.6/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.6.6/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.898882 DXR-1.6.6/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.6.6/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.6.6/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2724 2023-02-24 03:25:36.000000 DXR-1.6.6/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.6.6/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.6.6/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.911434 DXR-1.6.6/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.6.6/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.6.6/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.6.6/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.6.6/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.6.6/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.6.6/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.6.6/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.6.6/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.920006 DXR-1.6.6/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.6.6/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    26816 2023-03-13 07:09:40.000000 DXR-1.6.6/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.6.6/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.6.6/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.6.6/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.924057 DXR-1.6.6/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.930446 DXR-1.6.6/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13719 2023-03-21 15:42:01.000000 DXR-1.6.6/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.6.6/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.934295 DXR-1.6.6/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.6.6/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.938434 DXR-1.6.6/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.950187 DXR-1.6.6/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.952230 DXR-1.6.6/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.6.6/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.6.6/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:37:28.954399 DXR-1.6.6/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.6.6/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.6/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-06 00:37:28.954939 DXR-1.6.6/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.6.6/README.md
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-06 00:37:28.955953 DXR-1.6.6/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-06 00:37:21.000000 DXR-1.6.6/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.376507 DXR-1.6.7/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.330310 DXR-1.6.7/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1291 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-13 01:30:49.000000 DXR-1.6.7/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.331985 DXR-1.6.7/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.6.7/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.6.7/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.6.7/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.333937 DXR-1.6.7/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.6.7/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.337215 DXR-1.6.7/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2724 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.6.7/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.6.7/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.343263 DXR-1.6.7/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.6.7/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.6.7/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.6.7/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.6.7/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.6.7/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.346635 DXR-1.6.7/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.6.7/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28811 2023-04-13 01:29:11.000000 DXR-1.6.7/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.6.7/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.6.7/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.6.7/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.348302 DXR-1.6.7/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.353774 DXR-1.6.7/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13811 2023-04-13 01:29:11.000000 DXR-1.6.7/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.6.7/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.357704 DXR-1.6.7/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.6.7/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.361499 DXR-1.6.7/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.370169 DXR-1.6.7/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.373849 DXR-1.6.7/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.6.7/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.6.7/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-13 01:30:49.375128 DXR-1.6.7/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.6.7/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.7/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-13 01:30:49.375797 DXR-1.6.7/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.6.7/README.md
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-13 01:30:49.376739 DXR-1.6.7/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-13 01:30:43.000000 DXR-1.6.7/setup.py
```

### Comparing `DXR-1.6.6/DXR.egg-info/SOURCES.txt` & `DXR-1.6.7/DXR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_Chat/ChatGPT.py` & `DXR-1.6.7/Dxr_Chat/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_Chat/utils.py` & `DXR-1.6.7/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_bytes/Dxr_bytes.py` & `DXR-1.6.7/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_file/dxr_file.py` & `DXR-1.6.7/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_file/dxr_request.py` & `DXR-1.6.7/Dxr_file/dxr_request.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_file/dxr_request_ros.py` & `DXR-1.6.7/Dxr_file/dxr_request_ros.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_file/dxr_ssh.py` & `DXR-1.6.7/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/Datas_pb2.py` & `DXR-1.6.7/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.6.7/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/audios_pb2.py` & `DXR-1.6.7/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.6.7/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.6.7/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.6.7/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.6.7/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_isapi/api.py` & `DXR-1.6.7/Dxr_isapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             self.ptz_absoluteEx_url = '%s/ISAPI/PTZCtrl/channels/1/absoluteEx' % self._base
             self.onepushfocus_url = '%s/ISAPI/PTZCtrl/channels/1/onepushfoucs/start' % self._base
             self.absoluteStatus_url = '%s/ISAPI/PTZCtrl/channels/1/status' % self._base
             self.imageFocus_url = '%s/ISAPI/Image/channels/1/focusConfiguration' % self._base
             self.ptz_capabilities_url = '%s/ISAPI/PTZCtrl/capabilities' % self._base
             self.ptz_autopan_url = '%s/ISAPI/PTZCtrl/channels/1/autopan' % self._base
             self.streamParam_url = '%s/ISAPI/Thermal/channels/2/streamParam' % self._base
+            self.auxcontrol_url = '%s/ISAPI/PTZCtrl/channels/1/auxcontrols/1' % self._base
 
         else:
             self.motion_url = '%s/MotionDetection/1' % self._base
             self.deviceinfo_url = '%s/System/deviceInfo' % self._base
             self.ptzctrl_url = '%s/PTZCtrl/capabilities' % self._base
             self.ptzpreset_url = '%s/PTZCtrl/channels/1/presets' % self._base
             self.pic_url = '%s/System/Video/channels/1/picture' % self._base
@@ -744,7 +745,60 @@
                 return
 
             if enabled_element[0].text.strip() == 'OK':
                 pass
 
         except AttributeError as attrib_err:
             return
+    
+    # 打开雨刷
+    def enable_wiper(self,status = 'on', element_to_query=None):
+        """ Enable Wiper """
+        data_xml = '<?xml version: "1.0" encoding="UTF-8"?><PTZAux><id>1</id><type>WIPER</type><status>'+ status +'</status></PTZAux>'
+        response = requests.put(
+            self.auxcontrol_url,
+            auth=self._auth_fn(self._username, self._password),
+            data=data_xml,
+            )
+        if response.status_code != 200:
+            return None
+
+        if element_to_query is None:
+            return response.text
+        try:
+            tree = tree_no_ns_from_string(response.text)
+
+            element_to_query = './/%s%s' % (
+                self._xml_namespace, element_to_query)
+            result = tree.findall(element_to_query)
+            if len(result) > 0:
+                return result[0].text.strip()
+        except AttributeError as attib_err:
+            return None
+        return None
+    
+    # 补光灯控制
+    def enable_light(self,status = 'on', element_to_query=None):
+        """ Enable Light """
+        data_xml = '<?xml version: "1.0" encoding="UTF-8"?><PTZAux><id>1</id><type>LIGHT</type><status>'+ status +'</status></PTZAux>'
+        response = requests.put(
+            self.auxcontrol_url,
+            auth=self._auth_fn(self._username, self._password),
+            data=data_xml,
+            )
+        if response.status_code != 200:
+            return None
+
+        if element_to_query is None:
+            return response.text
+        try:
+            tree = tree_no_ns_from_string(response.text)
+
+            element_to_query = './/%s%s' % (
+                self._xml_namespace, element_to_query)
+            result = tree.findall(element_to_query)
+            if len(result) > 0:
+                return result[0].text.strip()
+        except AttributeError as attib_err:
+            return None
+        return None
+
```

### Comparing `DXR-1.6.6/Dxr_isapi/error.py` & `DXR-1.6.7/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_isapi/ir_client.py` & `DXR-1.6.7/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_log/log.py` & `DXR-1.6.7/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.6.7/Dxr_mqtt/dxr_mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,16 @@
             if isinstance(topic, str):
                 await_topic = topic
             else:
                 await_topic = topic.topic
         if await_topic is None:
             return None
         await_topic = await_topic.replace('pc', 'client')
+        if await_topic in callback_dit:
+            callback_dit[await_topic]['msg'] = None
         cond = get_cond(await_topic)
         if cond is None:
             return None
         if timeout is None:
             cond.wait()
         else:
             cond.wait(timeout)
```

### Comparing `DXR-1.6.6/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.6.7/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_mqtt/msg.py` & `DXR-1.6.7/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_serial/Dxr_serial.py` & `DXR-1.6.7/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_utils/dxr_ftp.py` & `DXR-1.6.7/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_utils/dxr_utils.py` & `DXR-1.6.7/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/Datas_pb2.py` & `DXR-1.6.7/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.6.7/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/HCNetSDK.py` & `DXR-1.6.7/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/PlayCtrl.py` & `DXR-1.6.7/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/test_main.py` & `DXR-1.6.7/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/video.py` & `DXR-1.6.7/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/video_hk.py` & `DXR-1.6.7/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_video/video_server.py` & `DXR-1.6.7/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_voice/dxr_tts.py` & `DXR-1.6.7/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/Dxr_yaml/Dxr_yaml.py` & `DXR-1.6.7/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/README.md` & `DXR-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.6.6/setup.py` & `DXR-1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.6.6',
+    version='1.6.7',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```

