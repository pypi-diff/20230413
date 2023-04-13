# Comparing `tmp/python_ms_core-0.0.8-py3-none-any.whl.zip` & `tmp/python_ms_core-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,52 @@
-Zip file size: 15134 bytes, number of entries: 26
--rw-r--r--  2.0 unx     5076 b- defN 23-Feb-23 06:17 python_ms_core/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/logger/__init__.py
--rw-r--r--  2.0 unx     1631 b- defN 23-Feb-23 06:17 python_ms_core/core/logger/local_logger.py
--rw-r--r--  2.0 unx     1616 b- defN 23-Feb-23 06:17 python_ms_core/core/logger/logger.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/logger/abstracts/__init__.py
--rw-r--r--  2.0 unx      542 b- defN 23-Feb-23 06:17 python_ms_core/core/logger/abstracts/logger_abstract.py
--rw-r--r--  2.0 unx     6065 b- defN 23-Feb-23 06:17 python_ms_core/core/resource_errors/__init__.py
--rw-r--r--  2.0 unx      989 b- defN 23-Feb-23 06:17 python_ms_core/core/resource_errors/errors.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/abstract/__init__.py
--rw-r--r--  2.0 unx      476 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/abstract/file_entity.py
--rw-r--r--  2.0 unx      312 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/abstract/storage_client.py
--rw-r--r--  2.0 unx      292 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/abstract/storage_container.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/models/__init__.py
--rw-r--r--  2.0 unx      226 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/models/config.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/providers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/providers/azure/__init__.py
--rw-r--r--  2.0 unx      898 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/providers/azure/azure_file_entity.py
--rw-r--r--  2.0 unx     1886 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/providers/azure/azure_storage_client.py
--rw-r--r--  2.0 unx      993 b- defN 23-Feb-23 06:17 python_ms_core/core/storage/providers/azure/azure_storage_container.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Feb-23 06:17 python_ms_core-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     9963 b- defN 23-Feb-23 06:17 python_ms_core-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-23 06:17 python_ms_core-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-23 06:17 python_ms_core-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2598 b- defN 23-Feb-23 06:17 python_ms_core-0.0.8.dist-info/RECORD
-26 files, 34743 bytes uncompressed, 10724 bytes compressed:  69.1%
+Zip file size: 24843 bytes, number of entries: 50
+-rw-r--r--  2.0 unx     5076 b- defN 23-Feb-23 07:13 python_ms_core/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/abstracts/__init__.py
+-rw-r--r--  2.0 unx      281 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/abstracts/authorizer_abstract.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/models/__init__.py
+-rw-r--r--  2.0 unx     1526 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/models/permission_request.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/provider/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/provider/hosted/__init__.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/provider/hosted/hosted_authorizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/provider/simulated/__init__.py
+-rw-r--r--  2.0 unx      434 b- defN 23-Feb-23 07:13 python_ms_core/core/auth/provider/simulated/simulated_authorizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/config/__init__.py
+-rw-r--r--  2.0 unx     3384 b- defN 23-Feb-23 07:13 python_ms_core/core/config/config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/logger/__init__.py
+-rw-r--r--  2.0 unx     1631 b- defN 23-Feb-23 07:13 python_ms_core/core/logger/local_logger.py
+-rw-r--r--  2.0 unx     1616 b- defN 23-Feb-23 07:13 python_ms_core/core/logger/logger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/logger/abstracts/__init__.py
+-rw-r--r--  2.0 unx      542 b- defN 23-Feb-23 07:13 python_ms_core/core/logger/abstracts/logger_abstract.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/__init__.py
+-rw-r--r--  2.0 unx     1004 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/local_queue.py
+-rw-r--r--  2.0 unx      994 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/queue.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/abstracts/__init__.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/abstracts/queue_abstract.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/config/__init__.py
+-rw-r--r--  2.0 unx      555 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/config/queue_config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/models/__init__.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-Feb-23 07:13 python_ms_core/core/queue/models/queue_message.py
+-rw-r--r--  2.0 unx     6065 b- defN 23-Feb-23 07:13 python_ms_core/core/resource_errors/__init__.py
+-rw-r--r--  2.0 unx      989 b- defN 23-Feb-23 07:13 python_ms_core/core/resource_errors/errors.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/abstract/__init__.py
+-rw-r--r--  2.0 unx      476 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/abstract/file_entity.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/abstract/storage_client.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/abstract/storage_container.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/models/__init__.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/models/config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/providers/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/providers/azure/__init__.py
+-rw-r--r--  2.0 unx      898 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/providers/azure/azure_file_entity.py
+-rw-r--r--  2.0 unx     1886 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/providers/azure/azure_storage_client.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Feb-23 07:13 python_ms_core/core/storage/providers/azure/azure_storage_container.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-23 07:13 python_ms_core/core/topic/__init__.py
+-rw-r--r--  2.0 unx     2400 b- defN 23-Feb-23 07:13 python_ms_core/core/topic/local_topic.py
+-rw-r--r--  2.0 unx     2002 b- defN 23-Feb-23 07:13 python_ms_core/core/topic/topic.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Feb-23 07:13 python_ms_core-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9963 b- defN 23-Feb-23 07:13 python_ms_core-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-23 07:13 python_ms_core-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Feb-23 07:13 python_ms_core-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5020 b- defN 23-Feb-23 07:13 python_ms_core-0.0.9.dist-info/RECORD
+50 files, 53359 bytes uncompressed, 16417 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,13 +1,49 @@
 Filename: python_ms_core/__init__.py
 Comment: 
 
 Filename: python_ms_core/core/__init__.py
 Comment: 
 
+Filename: python_ms_core/core/auth/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/auth/abstracts/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/auth/abstracts/authorizer_abstract.py
+Comment: 
+
+Filename: python_ms_core/core/auth/models/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/auth/models/permission_request.py
+Comment: 
+
+Filename: python_ms_core/core/auth/provider/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/auth/provider/hosted/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/auth/provider/hosted/hosted_authorizer.py
+Comment: 
+
+Filename: python_ms_core/core/auth/provider/simulated/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/auth/provider/simulated/simulated_authorizer.py
+Comment: 
+
+Filename: python_ms_core/core/config/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/config/config.py
+Comment: 
+
 Filename: python_ms_core/core/logger/__init__.py
 Comment: 
 
 Filename: python_ms_core/core/logger/local_logger.py
 Comment: 
 
 Filename: python_ms_core/core/logger/logger.py
@@ -15,14 +51,41 @@
 
 Filename: python_ms_core/core/logger/abstracts/__init__.py
 Comment: 
 
 Filename: python_ms_core/core/logger/abstracts/logger_abstract.py
 Comment: 
 
+Filename: python_ms_core/core/queue/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/queue/local_queue.py
+Comment: 
+
+Filename: python_ms_core/core/queue/queue.py
+Comment: 
+
+Filename: python_ms_core/core/queue/abstracts/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/queue/abstracts/queue_abstract.py
+Comment: 
+
+Filename: python_ms_core/core/queue/config/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/queue/config/queue_config.py
+Comment: 
+
+Filename: python_ms_core/core/queue/models/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/queue/models/queue_message.py
+Comment: 
+
 Filename: python_ms_core/core/resource_errors/__init__.py
 Comment: 
 
 Filename: python_ms_core/core/resource_errors/errors.py
 Comment: 
 
 Filename: python_ms_core/core/storage/__init__.py
@@ -57,23 +120,32 @@
 
 Filename: python_ms_core/core/storage/providers/azure/azure_storage_client.py
 Comment: 
 
 Filename: python_ms_core/core/storage/providers/azure/azure_storage_container.py
 Comment: 
 
-Filename: python_ms_core-0.0.8.dist-info/LICENSE
+Filename: python_ms_core/core/topic/__init__.py
+Comment: 
+
+Filename: python_ms_core/core/topic/local_topic.py
+Comment: 
+
+Filename: python_ms_core/core/topic/topic.py
+Comment: 
+
+Filename: python_ms_core-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: python_ms_core-0.0.8.dist-info/METADATA
+Filename: python_ms_core-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: python_ms_core-0.0.8.dist-info/WHEEL
+Filename: python_ms_core-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: python_ms_core-0.0.8.dist-info/top_level.txt
+Filename: python_ms_core-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: python_ms_core-0.0.8.dist-info/RECORD
+Filename: python_ms_core-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_ms_core-0.0.8.dist-info/LICENSE` & `python_ms_core-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_ms_core-0.0.8.dist-info/METADATA` & `python_ms_core-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ms-core
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Boilerplate with cloud interaction
 Home-page: https://github.com/TaskarCenterAtUW/TDEI-Python-ms-core
 Author: Sujata Misra
 Author-email: sujatam@gaussiansolutions.com
 Project-URL: Documentation, https://github.com/TaskarCenterAtUW/TDEI-Python-ms-core/blob/main/README.md
 Project-URL: GitHub, https://github.com/TaskarCenterAtUW/TDEI-Python-ms-core
 Project-URL: Changelog, https://github.com/TaskarCenterAtUW/TDEI-Python-ms-core/blob/develop/CHANGELOG.md
```

## Comparing `python_ms_core-0.0.8.dist-info/RECORD` & `python_ms_core-0.0.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,50 @@
 python_ms_core/__init__.py,sha256=VpwiWglaqAKtk2sDe5WXPLa5-H1S5I85hqM5x9oP9W8,5076
 python_ms_core/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/auth/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/auth/abstracts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/auth/abstracts/authorizer_abstract.py,sha256=B5eKyfm9t20L5nZPqQl383ADHsb_rxq9dSwV2Oi74iE,281
+python_ms_core/core/auth/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/auth/models/permission_request.py,sha256=AmOx25QYsHtK3NSKm1fdLBfEfq-0QSHPwEGYNYQoXVA,1526
+python_ms_core/core/auth/provider/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/auth/provider/hosted/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/auth/provider/hosted/hosted_authorizer.py,sha256=zHVK2f33Yg3qm0C0AcCOWUhPMUfUbqFi0WgyfiuOQKE,927
+python_ms_core/core/auth/provider/simulated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/auth/provider/simulated/simulated_authorizer.py,sha256=S43RW-pPSh29wCvBiRoWtR-jnLbFbgckd-4p5_hmcsI,434
+python_ms_core/core/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/config/config.py,sha256=qpRj5dEkFuWAA1jm_B_PIpOZKaBiTeTMpjRcGrGOwyQ,3384
 python_ms_core/core/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_ms_core/core/logger/local_logger.py,sha256=CkkD05dl0-sqg1fTB39wEWcPqzECTIPp9khDsj-A3FE,1631
 python_ms_core/core/logger/logger.py,sha256=Zq4xU946ZS2u6v44tTxNHrU11KEu2Pj8DPo8k5w1RXo,1616
 python_ms_core/core/logger/abstracts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_ms_core/core/logger/abstracts/logger_abstract.py,sha256=pV1wQpbRX0kILK0-b0_Hq2itYPAYesSRj9dtjsng3o0,542
+python_ms_core/core/queue/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/queue/local_queue.py,sha256=RnHLI8zshuB0bocWJaRGtwFsZCBwHKcsdaeT8GzzhqA,1004
+python_ms_core/core/queue/queue.py,sha256=cVyLPEgQvV_xL8uFC-jFRJlgQBU5o465v5qYh2ebzWk,994
+python_ms_core/core/queue/abstracts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/queue/abstracts/queue_abstract.py,sha256=GTGlmJF5kTM6KnCMka3XU3uzAt-Z-vHUWY5uUnFXTvs,328
+python_ms_core/core/queue/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/queue/config/queue_config.py,sha256=iOQt20QRkYuMUV3OUZ4eNIepYNfi2jJNg3PHE2pg2LM,555
+python_ms_core/core/queue/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/queue/models/queue_message.py,sha256=rid-3h5SfWjgVv6Mu0mcgKFPcfTSHPIc5hmSqCXrGz0,2359
 python_ms_core/core/resource_errors/__init__.py,sha256=rQCXY5EquaWKBAQthLK-xZcLa5nR7mQTfVY7OAYjt8E,6065
 python_ms_core/core/resource_errors/errors.py,sha256=Arv6AwJcCEa1oxZo8TYzLiODIB8rH0E6w71WbbuViOs,989
 python_ms_core/core/storage/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_ms_core/core/storage/abstract/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_ms_core/core/storage/abstract/file_entity.py,sha256=uWPpoda11EM8Dc491dHUiIdDjV6usW9UpC31bGHmwzo,476
 python_ms_core/core/storage/abstract/storage_client.py,sha256=Ec6KVVPYjovVZXmqbW7kV_6u3YACTBBdtSMwe_0xaN8,312
 python_ms_core/core/storage/abstract/storage_container.py,sha256=vEbJmhdigjYraCToCnxDH6S_L4rWFAOrU_MZuTzQ4z8,292
 python_ms_core/core/storage/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_ms_core/core/storage/models/config.py,sha256=ST4hTB7rJ5MEVgC6ENiLfPOV26uekKfikF12vtmZANs,226
 python_ms_core/core/storage/providers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_ms_core/core/storage/providers/azure/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 python_ms_core/core/storage/providers/azure/azure_file_entity.py,sha256=uC2KX89xjB2HBRVxtR1efmt9JpEFCOaZm0yur3sN4KA,898
 python_ms_core/core/storage/providers/azure/azure_storage_client.py,sha256=SvdAw_02w1GuvaqrhYXtukkg1BTl5XF21u6DixZp12Q,1886
 python_ms_core/core/storage/providers/azure/azure_storage_container.py,sha256=sQrssFuGsq9W1Tdr9tJ-8rMbPDwgSYJgyVkEG70jNjM,993
-python_ms_core-0.0.8.dist-info/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
-python_ms_core-0.0.8.dist-info/METADATA,sha256=vTsR4iXSr0CMtMS7jw9EApuTzuTIcMms2d18-RR_wMs,9963
-python_ms_core-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-python_ms_core-0.0.8.dist-info/top_level.txt,sha256=aFL1VFT6l18B5KDtuULgCN-Y_rhbtoc5_bD95gjkRo8,15
-python_ms_core-0.0.8.dist-info/RECORD,,
+python_ms_core/core/topic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+python_ms_core/core/topic/local_topic.py,sha256=vQpGvksI_KZmzqg-WwSlubc1R4BwNn-lRafNa2g4ahE,2400
+python_ms_core/core/topic/topic.py,sha256=X8zuQRcOm3CsRPqlNlLBhyIqycKcLflz_gCOa-q0Lgc,2002
+python_ms_core-0.0.9.dist-info/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
+python_ms_core-0.0.9.dist-info/METADATA,sha256=Z8L2fra5dIB63_GYlLZE2wsKIVaU4S4qZwIE47HSGls,9963
+python_ms_core-0.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+python_ms_core-0.0.9.dist-info/top_level.txt,sha256=aFL1VFT6l18B5KDtuULgCN-Y_rhbtoc5_bD95gjkRo8,15
+python_ms_core-0.0.9.dist-info/RECORD,,
```

