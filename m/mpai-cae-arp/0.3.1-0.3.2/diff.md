# Comparing `tmp/mpai_cae_arp-0.3.1.tar.gz` & `tmp/mpai_cae_arp-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpai_cae_arp-0.3.1.tar", max compression
+gzip compressed data, was "mpai_cae_arp-0.3.2.tar", max compression
```

## Comparing `mpai_cae_arp-0.3.1.tar` & `mpai_cae_arp-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-04-03 21:35:54.975907 mpai_cae_arp-0.3.1/LICENSE
--rw-r--r--   0        0        0      491 2023-04-03 21:22:02.773309 mpai_cae_arp-0.3.1/README.md
--rw-r--r--   0        0        0      276 2023-04-04 08:31:02.533352 mpai_cae_arp-0.3.1/mpai_cae_arp/__init__.py
--rw-r--r--   0        0        0      176 2023-04-04 07:37:21.160932 mpai_cae_arp-0.3.1/mpai_cae_arp/audio/__init__.py
--rw-r--r--   0        0        0    17904 2023-04-06 15:03:52.274016 mpai_cae_arp-0.3.1/mpai_cae_arp/audio/_audio.py
--rw-r--r--   0        0        0     2516 2023-04-04 07:38:52.008419 mpai_cae_arp-0.3.1/mpai_cae_arp/audio/_noise.py
--rw-r--r--   0        0        0      219 2023-04-03 21:48:20.943719 mpai_cae_arp-0.3.1/mpai_cae_arp/audio/standards.py
--rw-r--r--   0        0        0     4211 2023-04-04 07:22:07.372604 mpai_cae_arp-0.3.1/mpai_cae_arp/audio/utils.py
--rw-r--r--   0        0        0     2055 2023-04-10 18:12:57.428996 mpai_cae_arp-0.3.1/mpai_cae_arp/files.py
--rw-r--r--   0        0        0     1304 2023-04-06 14:57:19.804922 mpai_cae_arp-0.3.1/mpai_cae_arp/io.py
--rw-r--r--   0        0        0     1470 2023-04-11 18:41:39.855128 mpai_cae_arp-0.3.1/mpai_cae_arp/network/arp.proto
--rw-r--r--   0        0        0     3320 2023-04-11 18:46:42.741189 mpai_cae_arp-0.3.1/mpai_cae_arp/network/arp_pb2.py
--rw-r--r--   0        0        0    18550 2023-04-11 18:46:53.137122 mpai_cae_arp-0.3.1/mpai_cae_arp/network/arp_pb2_grpc.py
--rw-r--r--   0        0        0     3100 2023-04-03 21:32:30.045143 mpai_cae_arp-0.3.1/mpai_cae_arp/time.py
--rw-r--r--   0        0        0        0 2023-04-03 21:25:06.272009 mpai_cae_arp-0.3.1/mpai_cae_arp/types/__init__.py
--rw-r--r--   0        0        0     7311 2023-04-13 11:52:35.097562 mpai_cae_arp-0.3.1/mpai_cae_arp/types/irregularity.py
--rw-r--r--   0        0        0     1668 2023-04-03 21:48:21.015718 mpai_cae_arp-0.3.1/mpai_cae_arp/types/schema.py
--rw-r--r--   0        0        0     1240 2023-04-13 12:58:51.700310 mpai_cae_arp-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.1/setup.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-03 21:35:54.975907 mpai_cae_arp-0.3.2/LICENSE
+-rw-r--r--   0        0        0      491 2023-04-03 21:22:02.773309 mpai_cae_arp-0.3.2/README.md
+-rw-r--r--   0        0        0      276 2023-04-04 08:31:02.533352 mpai_cae_arp-0.3.2/mpai_cae_arp/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-04 07:37:21.160932 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/__init__.py
+-rw-r--r--   0        0        0    17904 2023-04-06 15:03:52.274016 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_audio.py
+-rw-r--r--   0        0        0     2516 2023-04-04 07:38:52.008419 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_noise.py
+-rw-r--r--   0        0        0      219 2023-04-03 21:48:20.943719 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/standards.py
+-rw-r--r--   0        0        0     4211 2023-04-04 07:22:07.372604 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/utils.py
+-rw-r--r--   0        0        0     2055 2023-04-10 18:12:57.428996 mpai_cae_arp-0.3.2/mpai_cae_arp/files.py
+-rw-r--r--   0        0        0     1304 2023-04-06 14:57:19.804922 mpai_cae_arp-0.3.2/mpai_cae_arp/io.py
+-rw-r--r--   0        0        0     2246 2023-04-13 16:30:33.142293 mpai_cae_arp-0.3.2/mpai_cae_arp/network/arp_pb2.py
+-rw-r--r--   0        0        0     3679 2023-04-13 16:31:08.282079 mpai_cae_arp-0.3.2/mpai_cae_arp/network/arp_pb2_grpc.py
+-rw-r--r--   0        0        0     3100 2023-04-03 21:32:30.045143 mpai_cae_arp-0.3.2/mpai_cae_arp/time.py
+-rw-r--r--   0        0        0        0 2023-04-03 21:25:06.272009 mpai_cae_arp-0.3.2/mpai_cae_arp/types/__init__.py
+-rw-r--r--   0        0        0     7311 2023-04-13 11:52:35.097562 mpai_cae_arp-0.3.2/mpai_cae_arp/types/irregularity.py
+-rw-r--r--   0        0        0     1668 2023-04-03 21:48:21.015718 mpai_cae_arp-0.3.2/mpai_cae_arp/types/schema.py
+-rw-r--r--   0        0        0     1240 2023-04-13 16:33:06.769367 mpai_cae_arp-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.2/setup.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.2/PKG-INFO
```

### Comparing `mpai_cae_arp-0.3.1/LICENSE` & `mpai_cae_arp-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/audio/_audio.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_audio.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/audio/_noise.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_noise.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/audio/utils.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/audio/utils.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/files.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/files.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/io.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/io.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/network/arp_pb2.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/network/arp_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,37 +9,29 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tarp.proto\x12\x03\x61rp\"+\n\x0bInfoRequest\x12\x12\n\x05\x66ield\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_field\"&\n\x07\x43ontact\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\"$\n\x07License\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\"y\n\x04Info\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1d\n\x07\x63ontact\x18\x04 \x01(\x0b\x32\x0c.arp.Contact\x12\x1d\n\x07license\x18\x05 \x01(\x0b\x32\x0c.arp.License\"=\n\x12\x43omputationRequest\x12\x13\n\x0bworking_dir\x18\x01 \x01(\t\x12\x12\n\nfiles_name\x18\x02 \x01(\t\"5\n\x11\x43omputationResult\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0f\n\x07message\x18\x02 \x01(\t2|\n\rAudioAnalyser\x12+\n\ngetAimInfo\x12\x10.arp.InfoRequest\x1a\t.arp.Info\"\x00\x12>\n\x07\x61nalyse\x12\x17.arp.ComputationRequest\x1a\x16.arp.ComputationResult\"\x00\x30\x01\x32|\n\rVideoAnalyser\x12+\n\ngetAimInfo\x12\x10.arp.InfoRequest\x1a\t.arp.Info\"\x00\x12>\n\x07\x61nalyse\x12\x17.arp.ComputationRequest\x1a\x16.arp.ComputationResult\"\x00\x30\x01\x32\x8a\x01\n\x1aTapeIrregularityClassifier\x12+\n\ngetAimInfo\x12\x10.arp.InfoRequest\x1a\t.arp.Info\"\x00\x12?\n\x08\x63lassify\x12\x17.arp.ComputationRequest\x1a\x16.arp.ComputationResult\"\x00\x30\x01\x32\x83\x01\n\x14TapeAudioRestoration\x12+\n\ngetAimInfo\x12\x10.arp.InfoRequest\x1a\t.arp.Info\"\x00\x12>\n\x07restore\x12\x17.arp.ComputationRequest\x1a\x16.arp.ComputationResult\"\x00\x30\x01\x32w\n\x08Packager\x12+\n\ngetAimInfo\x12\x10.arp.InfoRequest\x1a\t.arp.Info\"\x00\x12>\n\x07package\x12\x17.arp.ComputationRequest\x1a\x16.arp.ComputationResult\"\x00\x30\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tarp.proto\x12\x03\x61rp\"+\n\x0bInfoRequest\x12\x12\n\x05\x66ield\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_field\"S\n\nJobRequest\x12\x13\n\x0bworking_dir\x18\x01 \x01(\t\x12\x12\n\nfiles_name\x18\x02 \x01(\t\x12\x12\n\x05index\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_index\".\n\x0bJobResponse\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\"&\n\x07\x43ontact\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\"$\n\x07License\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\"\x81\x01\n\x0cInfoResponse\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1d\n\x07\x63ontact\x18\x04 \x01(\x0b\x32\x0c.arp.Contact\x12\x1d\n\x07license\x18\x05 \x01(\x0b\x32\x0c.arp.License2f\n\x03\x41IM\x12\x30\n\x07getInfo\x12\x10.arp.InfoRequest\x1a\x11.arp.InfoResponse\"\x00\x12-\n\x04work\x12\x0f.arp.JobRequest\x1a\x10.arp.JobResponse\"\x00\x30\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arp_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _INFOREQUEST._serialized_start=18
   _INFOREQUEST._serialized_end=61
-  _CONTACT._serialized_start=63
-  _CONTACT._serialized_end=101
-  _LICENSE._serialized_start=103
-  _LICENSE._serialized_end=139
-  _INFO._serialized_start=141
-  _INFO._serialized_end=262
-  _COMPUTATIONREQUEST._serialized_start=264
-  _COMPUTATIONREQUEST._serialized_end=325
-  _COMPUTATIONRESULT._serialized_start=327
-  _COMPUTATIONRESULT._serialized_end=380
-  _AUDIOANALYSER._serialized_start=382
-  _AUDIOANALYSER._serialized_end=506
-  _VIDEOANALYSER._serialized_start=508
-  _VIDEOANALYSER._serialized_end=632
-  _TAPEIRREGULARITYCLASSIFIER._serialized_start=635
-  _TAPEIRREGULARITYCLASSIFIER._serialized_end=773
-  _TAPEAUDIORESTORATION._serialized_start=776
-  _TAPEAUDIORESTORATION._serialized_end=907
-  _PACKAGER._serialized_start=909
-  _PACKAGER._serialized_end=1028
+  _JOBREQUEST._serialized_start=63
+  _JOBREQUEST._serialized_end=146
+  _JOBRESPONSE._serialized_start=148
+  _JOBRESPONSE._serialized_end=194
+  _CONTACT._serialized_start=196
+  _CONTACT._serialized_end=234
+  _LICENSE._serialized_start=236
+  _LICENSE._serialized_end=272
+  _INFORESPONSE._serialized_start=275
+  _INFORESPONSE._serialized_end=404
+  _AIM._serialized_start=406
+  _AIM._serialized_end=508
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/time.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/time.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/types/irregularity.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/types/irregularity.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/mpai_cae_arp/types/schema.py` & `mpai_cae_arp-0.3.2/mpai_cae_arp/types/schema.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.1/pyproject.toml` & `mpai_cae_arp-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpai-cae-arp"
-version = "0.3.1"
+version = "0.3.2"
 description = "The MPAI CAE-ARP software API"
 authors = ["Matteo Spanio <dev2@audioinnova.com>"]
 readme = "README.md"
 packages = [{include = "mpai_cae_arp"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `mpai_cae_arp-0.3.1/setup.py` & `mpai_cae_arp-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'llvmlite>=0.39.1,<0.40.0',
  'numpy==1.23.3',
  'pydantic>=1.10.7,<2.0.0',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'mpai-cae-arp',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'The MPAI CAE-ARP software API',
     'long_description': '# MPAI CAE-ARP API\n\n[![LICENSE](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://img.shields.io/badge/license-GPLv3-blue.svg)\n\n## Description\n\nThis package provides a set of tools for common task in MPAI CAE-ARP standard. It is usend in the official implementation of the standard and can be used as well to develop your own.\n\n## License\n\nThis software is licensed under the GPLv3 license. See the [official site](http://www.gnu.org/licenses/gpl-3.0.html) for more information.\n',
     'author': 'Matteo Spanio',
     'author_email': 'dev2@audioinnova.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mpai_cae_arp-0.3.1/PKG-INFO` & `mpai_cae_arp-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpai-cae-arp
-Version: 0.3.1
+Version: 0.3.2
 Summary: The MPAI CAE-ARP software API
 Author: Matteo Spanio
 Author-email: dev2@audioinnova.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

