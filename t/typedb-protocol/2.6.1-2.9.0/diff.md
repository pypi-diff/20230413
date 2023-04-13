# Comparing `tmp/typedb-protocol-2.6.1.tar.gz` & `tmp/typedb-protocol-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/typedb-protocol-2.6.1.tar", last modified: Fri Jan 14 16:51:18 2022, max compression
+gzip compressed data, was "dist/typedb-protocol-2.9.0.tar", last modified: Fri May 20 12:57:07 2022, max compression
```

## Comparing `typedb-protocol-2.6.1.tar` & `typedb-protocol-2.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/
--rw-r--r--   0 grabl     (1000) grabl     (1000)       67 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/setup.cfg
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    10616 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/options_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/options_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/query_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/answer_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    57456 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/query_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    46940 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/transaction_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)   284527 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/concept_pb2.py
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/__init__.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    39434 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/logic_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    24882 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/answer_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/logic_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/transaction_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/concept_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    13401 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/session_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/common/session_pb2_grpc.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)     5938 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_server_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    22643 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_user_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    13405 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_database_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)     6110 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_service_pb2.py
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/__init__.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_server_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_database_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_user_pb2_grpc.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)     9050 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_service_pb2_grpc.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/core/
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)     5804 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/core/core_service_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)     8738 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/core/core_service_pb2_grpc.py
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/core/__init__.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)    18755 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/core/core_database_pb2.py
--r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/core/core_database_pb2_grpc.py
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol.egg-info/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol.egg-info/not-zip-safe
--rw-r--r--   0 grabl     (1000) grabl     (1000)       16 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol.egg-info/top_level.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)     2579 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol.egg-info/PKG-INFO
--rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)     1485 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/typedb_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)     2579 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/PKG-INFO
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1465 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/README.md
--rw-r--r--   0 grabl     (1000) grabl     (1000)     1904 2022-01-14 16:51:18.000000 typedb-protocol-2.6.1/setup.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     2416 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/PKG-INFO
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1465 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/README.md
+-rw-r--r--   0 grabl     (1000) grabl     (1000)       67 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/setup.cfg
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     1904 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/setup.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/typedb_protocol/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/__init__.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    13405 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_database_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_database_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)     5938 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_server_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_server_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)     6110 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_service_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)     9050 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_service_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    22643 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_user_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_user_pb2_grpc.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/typedb_protocol/common/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/__init__.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    24882 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/answer_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/answer_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)   338216 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/concept_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/concept_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    39434 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/logic_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/logic_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    10616 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/options_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/options_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    57456 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/query_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/query_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    13401 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/session_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/session_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    46940 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/transaction_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/common/transaction_pb2_grpc.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/typedb_protocol/core/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/core/__init__.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    25818 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/core/core_database_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)       83 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/core/core_database_pb2_grpc.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)     6775 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/core/core_service_pb2.py
+-r-xr-xr-x   0 grabl     (1000) grabl     (1000)    10594 2022-05-20 12:57:05.000000 typedb-protocol-2.9.0/typedb_protocol/core/core_service_pb2_grpc.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/typedb_protocol.egg-info/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     2416 2022-05-20 12:57:06.000000 typedb-protocol-2.9.0/typedb_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     1485 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/typedb_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-05-20 12:57:06.000000 typedb-protocol-2.9.0/typedb_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-05-20 12:57:06.000000 typedb-protocol-2.9.0/typedb_protocol.egg-info/not-zip-safe
+-rw-r--r--   0 grabl     (1000) grabl     (1000)       16 2022-05-20 12:57:07.000000 typedb-protocol-2.9.0/typedb_protocol.egg-info/top_level.txt
```

### Comparing `typedb-protocol-2.6.1/typedb_protocol/common/options_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/common/options_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/common/query_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/common/query_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/common/transaction_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/common/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/common/concept_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/common/concept_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='common/concept.proto',
   package='typedb.protocol',
   syntax='proto3',
   serialized_options=_b('\n\033com.vaticle.typedb.protocolB\014ConceptProto'),
-  serialized_pb=_b('\n\x14\x63ommon/concept.proto\x12\x0ftypedb.protocol\"\x84\r\n\x0e\x43onceptManager\x1a\xfc\x03\n\x03Req\x12_\n\x12get_thing_type_req\x18\x01 \x01(\x0b\x32\x30.typedb.protocol.ConceptManager.GetThingType.ReqH\x00R\x0fgetThingTypeReq\x12R\n\rget_thing_req\x18\x02 \x01(\x0b\x32,.typedb.protocol.ConceptManager.GetThing.ReqH\x00R\x0bgetThingReq\x12\x62\n\x13put_entity_type_req\x18\x03 \x01(\x0b\x32\x31.typedb.protocol.ConceptManager.PutEntityType.ReqH\x00R\x10putEntityTypeReq\x12k\n\x16put_attribute_type_req\x18\x04 \x01(\x0b\x32\x34.typedb.protocol.ConceptManager.PutAttributeType.ReqH\x00R\x13putAttributeTypeReq\x12h\n\x15put_relation_type_req\x18\x05 \x01(\x0b\x32\x33.typedb.protocol.ConceptManager.PutRelationType.ReqH\x00R\x12putRelationTypeReqB\x05\n\x03req\x1a\xfc\x03\n\x03Res\x12_\n\x12get_thing_type_res\x18\x01 \x01(\x0b\x32\x30.typedb.protocol.ConceptManager.GetThingType.ResH\x00R\x0fgetThingTypeRes\x12R\n\rget_thing_res\x18\x02 \x01(\x0b\x32,.typedb.protocol.ConceptManager.GetThing.ResH\x00R\x0bgetThingRes\x12\x62\n\x13put_entity_type_res\x18\x03 \x01(\x0b\x32\x31.typedb.protocol.ConceptManager.PutEntityType.ResH\x00R\x10putEntityTypeRes\x12k\n\x16put_attribute_type_res\x18\x04 \x01(\x0b\x32\x34.typedb.protocol.ConceptManager.PutAttributeType.ResH\x00R\x13putAttributeTypeRes\x12h\n\x15put_relation_type_res\x18\x05 \x01(\x0b\x32\x33.typedb.protocol.ConceptManager.PutRelationType.ResH\x00R\x12putRelationTypeResB\x05\n\x03res\x1aq\n\x0cGetThingType\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x44\n\x03Res\x12\x36\n\nthing_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\tthingTypeB\x05\n\x03res\x1a\x61\n\x08GetThing\x1a\x17\n\x03Req\x12\x10\n\x03iid\x18\x01 \x01(\x0cR\x03iid\x1a<\n\x03Res\x12.\n\x05thing\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingH\x00R\x05thingB\x05\n\x03res\x1ak\n\rPutEntityType\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a=\n\x03Res\x12\x36\n\x0b\x65ntity_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\nentityType\x1a\xbd\x01\n\x10PutAttributeType\x1a\x64\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12G\n\nvalue_type\x18\x02 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeR\tvalueType\x1a\x43\n\x03Res\x12<\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\rattributeType\x1aq\n\x0fPutRelationType\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x41\n\x03Res\x12:\n\rrelation_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x0crelationType\"q\n\x07\x43oncept\x12.\n\x05thing\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingH\x00R\x05thing\x12+\n\x04type\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x04typeB\t\n\x07\x63oncept\"\x96\x1b\n\x05Thing\x12\x10\n\x03iid\x18\x01 \x01(\x0cR\x03iid\x12)\n\x04type\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x04type\x12\x36\n\x05value\x18\x03 \x01(\x0b\x32 .typedb.protocol.Attribute.ValueR\x05value\x12\x1a\n\x08inferred\x18\x04 \x01(\x08R\x08inferred\x1a\x80\n\n\x03Req\x12\x10\n\x03iid\x18\x01 \x01(\x0cR\x03iid\x12M\n\x10thing_delete_req\x18\x64 \x01(\x0b\x32!.typedb.protocol.Thing.Delete.ReqH\x00R\x0ethingDeleteReq\x12Q\n\x12thing_get_type_req\x18\x65 \x01(\x0b\x32\".typedb.protocol.Thing.GetType.ReqH\x00R\x0fthingGetTypeReq\x12N\n\x11thing_get_has_req\x18\x66 \x01(\x0b\x32!.typedb.protocol.Thing.GetHas.ReqH\x00R\x0ethingGetHasReq\x12N\n\x11thing_set_has_req\x18g \x01(\x0b\x32!.typedb.protocol.Thing.SetHas.ReqH\x00R\x0ethingSetHasReq\x12T\n\x13thing_unset_has_req\x18h \x01(\x0b\x32#.typedb.protocol.Thing.UnsetHas.ReqH\x00R\x10thingUnsetHasReq\x12`\n\x17thing_get_relations_req\x18i \x01(\x0b\x32\'.typedb.protocol.Thing.GetRelations.ReqH\x00R\x14thingGetRelationsReq\x12Z\n\x15thing_get_playing_req\x18j \x01(\x0b\x32%.typedb.protocol.Thing.GetPlaying.ReqH\x00R\x12thingGetPlayingReq\x12\x61\n\x17relation_add_player_req\x18\xc8\x01 \x01(\x0b\x32\'.typedb.protocol.Relation.AddPlayer.ReqH\x00R\x14relationAddPlayerReq\x12j\n\x1arelation_remove_player_req\x18\xc9\x01 \x01(\x0b\x32*.typedb.protocol.Relation.RemovePlayer.ReqH\x00R\x17relationRemovePlayerReq\x12\x64\n\x18relation_get_players_req\x18\xca\x01 \x01(\x0b\x32(.typedb.protocol.Relation.GetPlayers.ReqH\x00R\x15relationGetPlayersReq\x12\x85\x01\n%relation_get_players_by_role_type_req\x18\xcb\x01 \x01(\x0b\x32\x32.typedb.protocol.Relation.GetPlayersByRoleType.ReqH\x00R\x1frelationGetPlayersByRoleTypeReq\x12g\n\x19relation_get_relating_req\x18\xcc\x01 \x01(\x0b\x32).typedb.protocol.Relation.GetRelating.ReqH\x00R\x16relationGetRelatingReq\x12\x64\n\x18\x61ttribute_get_owners_req\x18\xac\x02 \x01(\x0b\x32(.typedb.protocol.Attribute.GetOwners.ReqH\x00R\x15\x61ttributeGetOwnersReqB\x05\n\x03req\x1a\xa3\x04\n\x03Res\x12M\n\x10thing_delete_res\x18\x64 \x01(\x0b\x32!.typedb.protocol.Thing.Delete.ResH\x00R\x0ethingDeleteRes\x12Q\n\x12thing_get_type_res\x18\x65 \x01(\x0b\x32\".typedb.protocol.Thing.GetType.ResH\x00R\x0fthingGetTypeRes\x12N\n\x11thing_set_has_res\x18\x66 \x01(\x0b\x32!.typedb.protocol.Thing.SetHas.ResH\x00R\x0ethingSetHasRes\x12T\n\x13thing_unset_has_res\x18g \x01(\x0b\x32#.typedb.protocol.Thing.UnsetHas.ResH\x00R\x10thingUnsetHasRes\x12\x61\n\x17relation_add_player_res\x18\xc8\x01 \x01(\x0b\x32\'.typedb.protocol.Relation.AddPlayer.ResH\x00R\x14relationAddPlayerRes\x12j\n\x1arelation_remove_player_res\x18\xc9\x01 \x01(\x0b\x32*.typedb.protocol.Relation.RemovePlayer.ResH\x00R\x17relationRemovePlayerResB\x05\n\x03res\x1a\xb6\x06\n\x07ResPart\x12[\n\x16thing_get_has_res_part\x18\x64 \x01(\x0b\x32%.typedb.protocol.Thing.GetHas.ResPartH\x00R\x12thingGetHasResPart\x12m\n\x1cthing_get_relations_res_part\x18\x65 \x01(\x0b\x32+.typedb.protocol.Thing.GetRelations.ResPartH\x00R\x18thingGetRelationsResPart\x12g\n\x1athing_get_playing_res_part\x18\x66 \x01(\x0b\x32).typedb.protocol.Thing.GetPlaying.ResPartH\x00R\x16thingGetPlayingResPart\x12q\n\x1drelation_get_players_res_part\x18\xc8\x01 \x01(\x0b\x32,.typedb.protocol.Relation.GetPlayers.ResPartH\x00R\x19relationGetPlayersResPart\x12\x92\x01\n*relation_get_players_by_role_type_res_part\x18\xc9\x01 \x01(\x0b\x32\x36.typedb.protocol.Relation.GetPlayersByRoleType.ResPartH\x00R#relationGetPlayersByRoleTypeResPart\x12t\n\x1erelation_get_relating_res_part\x18\xca\x01 \x01(\x0b\x32-.typedb.protocol.Relation.GetRelating.ResPartH\x00R\x1arelationGetRelatingResPart\x12q\n\x1d\x61ttribute_get_owners_res_part\x18\xac\x02 \x01(\x0b\x32,.typedb.protocol.Attribute.GetOwners.ResPartH\x00R\x19\x61ttributeGetOwnersResPartB\x05\n\x03res\x1a\x16\n\x06\x44\x65lete\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1aM\n\x07GetType\x1a\x05\n\x03Req\x1a;\n\x03Res\x12\x34\n\nthing_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\tthingType\x1aL\n\x06SetHas\x1a;\n\x03Req\x12\x34\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\tattribute\x1a\x05\n\x03Res\x1aN\n\x08UnsetHas\x1a;\n\x03Req\x12\x34\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\tattribute\x1a\x05\n\x03Res\x1a\xaf\x01\n\x06GetHas\x1a\x62\n\x03Req\x12>\n\x0f\x61ttribute_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x0e\x61ttributeTypes\x12\x1b\n\tkeys_only\x18\x02 \x01(\x08R\x08keysOnly\x1a\x41\n\x07ResPart\x12\x36\n\nattributes\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\nattributes\x1aT\n\nGetPlaying\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a\x8c\x01\n\x0cGetRelations\x1a;\n\x03Req\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a?\n\x07ResPart\x12\x34\n\trelations\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\trelations\"\x8a\x06\n\x08Relation\x1a}\n\tAddPlayer\x1ai\n\x03Req\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x12.\n\x06player\x18\x02 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06player\x1a\x05\n\x03Res\x1a\x80\x01\n\x0cRemovePlayer\x1ai\n\x03Req\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x12.\n\x06player\x18\x02 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06player\x1a\x05\n\x03Res\x1a\x84\x01\n\nGetPlayers\x1a;\n\x03Req\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\x1a\x9d\x02\n\x14GetPlayersByRoleType\x1ax\n\x12RoleTypeWithPlayer\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x12.\n\x06player\x18\x02 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06player\x1a\x05\n\x03Req\x1a\x83\x01\n\x07ResPart\x12x\n\x17role_types_with_players\x18\x01 \x03(\x0b\x32\x41.typedb.protocol.Relation.GetPlayersByRoleType.RoleTypeWithPlayerR\x14roleTypesWithPlayers\x1aU\n\x0bGetRelating\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\"\xb5\x02\n\tAttribute\x1a\x95\x01\n\x05Value\x12\x18\n\x06string\x18\x01 \x01(\tH\x00R\x06string\x12\x1a\n\x07\x62oolean\x18\x02 \x01(\x08H\x00R\x07\x62oolean\x12\x14\n\x04long\x18\x03 \x01(\x03H\x00R\x04long\x12\x18\n\x06\x64ouble\x18\x04 \x01(\x01H\x00R\x06\x64ouble\x12\x1d\n\tdate_time\x18\x05 \x01(\x03H\x00R\x08\x64\x61teTimeB\x07\n\x05value\x1a\x8f\x01\n\tGetOwners\x1aG\n\x03Req\x12\x36\n\nthing_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\tthingTypeB\x08\n\x06\x66ilter\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\"\xe0\x36\n\x04Type\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12\x14\n\x05scope\x18\x02 \x01(\tR\x05scope\x12:\n\x08\x65ncoding\x18\x03 \x01(\x0e\x32\x1e.typedb.protocol.Type.EncodingR\x08\x65ncoding\x12G\n\nvalue_type\x18\x04 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeR\tvalueType\x12\x12\n\x04root\x18\x05 \x01(\x08R\x04root\x1a\x8b\x18\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12\x14\n\x05scope\x18\x02 \x01(\tR\x05scope\x12J\n\x0ftype_delete_req\x18\x64 \x01(\x0b\x32 .typedb.protocol.Type.Delete.ReqH\x00R\rtypeDeleteReq\x12Q\n\x12type_set_label_req\x18\x65 \x01(\x0b\x32\".typedb.protocol.Type.SetLabel.ReqH\x00R\x0ftypeSetLabelReq\x12W\n\x14type_is_abstract_req\x18\x66 \x01(\x0b\x32$.typedb.protocol.Type.IsAbstract.ReqH\x00R\x11typeIsAbstractReq\x12]\n\x16type_get_supertype_req\x18g \x01(\x0b\x32&.typedb.protocol.Type.GetSupertype.ReqH\x00R\x13typeGetSupertypeReq\x12]\n\x16type_set_supertype_req\x18h \x01(\x0b\x32&.typedb.protocol.Type.SetSupertype.ReqH\x00R\x13typeSetSupertypeReq\x12`\n\x17type_get_supertypes_req\x18i \x01(\x0b\x32\'.typedb.protocol.Type.GetSupertypes.ReqH\x00R\x14typeGetSupertypesReq\x12Z\n\x15type_get_subtypes_req\x18j \x01(\x0b\x32%.typedb.protocol.Type.GetSubtypes.ReqH\x00R\x12typeGetSubtypesReq\x12x\n role_type_get_relation_types_req\x18\xc8\x01 \x01(\x0b\x32..typedb.protocol.RoleType.GetRelationTypes.ReqH\x00R\x1broleTypeGetRelationTypesReq\x12\x65\n\x19role_type_get_players_req\x18\xc9\x01 \x01(\x0b\x32(.typedb.protocol.RoleType.GetPlayers.ReqH\x00R\x15roleTypeGetPlayersReq\x12n\n\x1cthing_type_get_instances_req\x18\xac\x02 \x01(\x0b\x32+.typedb.protocol.ThingType.GetInstances.ReqH\x00R\x18thingTypeGetInstancesReq\x12k\n\x1bthing_type_set_abstract_req\x18\xad\x02 \x01(\x0b\x32*.typedb.protocol.ThingType.SetAbstract.ReqH\x00R\x17thingTypeSetAbstractReq\x12q\n\x1dthing_type_unset_abstract_req\x18\xae\x02 \x01(\x0b\x32,.typedb.protocol.ThingType.UnsetAbstract.ReqH\x00R\x19thingTypeUnsetAbstractReq\x12_\n\x17thing_type_get_owns_req\x18\xaf\x02 \x01(\x0b\x32&.typedb.protocol.ThingType.GetOwns.ReqH\x00R\x13thingTypeGetOwnsReq\x12_\n\x17thing_type_set_owns_req\x18\xb0\x02 \x01(\x0b\x32&.typedb.protocol.ThingType.SetOwns.ReqH\x00R\x13thingTypeSetOwnsReq\x12\x65\n\x19thing_type_unset_owns_req\x18\xb1\x02 \x01(\x0b\x32(.typedb.protocol.ThingType.UnsetOwns.ReqH\x00R\x15thingTypeUnsetOwnsReq\x12\x62\n\x18thing_type_get_plays_req\x18\xb2\x02 \x01(\x0b\x32\'.typedb.protocol.ThingType.GetPlays.ReqH\x00R\x14thingTypeGetPlaysReq\x12\x62\n\x18thing_type_set_plays_req\x18\xb3\x02 \x01(\x0b\x32\'.typedb.protocol.ThingType.SetPlays.ReqH\x00R\x14thingTypeSetPlaysReq\x12h\n\x1athing_type_unset_plays_req\x18\xb4\x02 \x01(\x0b\x32).typedb.protocol.ThingType.UnsetPlays.ReqH\x00R\x16thingTypeUnsetPlaysReq\x12^\n\x16\x65ntity_type_create_req\x18\x90\x03 \x01(\x0b\x32&.typedb.protocol.EntityType.Create.ReqH\x00R\x13\x65ntityTypeCreateReq\x12\x64\n\x18relation_type_create_req\x18\xf4\x03 \x01(\x0b\x32(.typedb.protocol.RelationType.Create.ReqH\x00R\x15relationTypeCreateReq\x12\x98\x01\n,relation_type_get_relates_for_role_label_req\x18\xf5\x03 \x01(\x0b\x32\x38.typedb.protocol.RelationType.GetRelatesForRoleLabel.ReqH\x00R%relationTypeGetRelatesForRoleLabelReq\x12q\n\x1drelation_type_get_relates_req\x18\xf6\x03 \x01(\x0b\x32,.typedb.protocol.RelationType.GetRelates.ReqH\x00R\x19relationTypeGetRelatesReq\x12q\n\x1drelation_type_set_relates_req\x18\xf7\x03 \x01(\x0b\x32,.typedb.protocol.RelationType.SetRelates.ReqH\x00R\x19relationTypeSetRelatesReq\x12w\n\x1frelation_type_unset_relates_req\x18\xf8\x03 \x01(\x0b\x32..typedb.protocol.RelationType.UnsetRelates.ReqH\x00R\x1brelationTypeUnsetRelatesReq\x12^\n\x16\x61ttribute_type_put_req\x18\xd8\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Put.ReqH\x00R\x13\x61ttributeTypePutReq\x12^\n\x16\x61ttribute_type_get_req\x18\xd9\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Get.ReqH\x00R\x13\x61ttributeTypeGetReq\x12n\n\x1c\x61ttribute_type_get_regex_req\x18\xda\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.GetRegex.ReqH\x00R\x18\x61ttributeTypeGetRegexReq\x12n\n\x1c\x61ttribute_type_set_regex_req\x18\xdb\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.SetRegex.ReqH\x00R\x18\x61ttributeTypeSetRegexReq\x12q\n\x1d\x61ttribute_type_get_owners_req\x18\xdc\x04 \x01(\x0b\x32,.typedb.protocol.AttributeType.GetOwners.ReqH\x00R\x19\x61ttributeTypeGetOwnersReqB\x05\n\x03req\x1a\xa5\x10\n\x03Res\x12J\n\x0ftype_delete_res\x18\x64 \x01(\x0b\x32 .typedb.protocol.Type.Delete.ResH\x00R\rtypeDeleteRes\x12Q\n\x12type_set_label_res\x18\x65 \x01(\x0b\x32\".typedb.protocol.Type.SetLabel.ResH\x00R\x0ftypeSetLabelRes\x12W\n\x14type_is_abstract_res\x18\x66 \x01(\x0b\x32$.typedb.protocol.Type.IsAbstract.ResH\x00R\x11typeIsAbstractRes\x12]\n\x16type_get_supertype_res\x18g \x01(\x0b\x32&.typedb.protocol.Type.GetSupertype.ResH\x00R\x13typeGetSupertypeRes\x12]\n\x16type_set_supertype_res\x18h \x01(\x0b\x32&.typedb.protocol.Type.SetSupertype.ResH\x00R\x13typeSetSupertypeRes\x12k\n\x1bthing_type_set_abstract_res\x18\xac\x02 \x01(\x0b\x32*.typedb.protocol.ThingType.SetAbstract.ResH\x00R\x17thingTypeSetAbstractRes\x12q\n\x1dthing_type_unset_abstract_res\x18\xad\x02 \x01(\x0b\x32,.typedb.protocol.ThingType.UnsetAbstract.ResH\x00R\x19thingTypeUnsetAbstractRes\x12_\n\x17thing_type_set_owns_res\x18\xae\x02 \x01(\x0b\x32&.typedb.protocol.ThingType.SetOwns.ResH\x00R\x13thingTypeSetOwnsRes\x12\x65\n\x19thing_type_unset_owns_res\x18\xaf\x02 \x01(\x0b\x32(.typedb.protocol.ThingType.UnsetOwns.ResH\x00R\x15thingTypeUnsetOwnsRes\x12\x62\n\x18thing_type_set_plays_res\x18\xb0\x02 \x01(\x0b\x32\'.typedb.protocol.ThingType.SetPlays.ResH\x00R\x14thingTypeSetPlaysRes\x12h\n\x1athing_type_unset_plays_res\x18\xb1\x02 \x01(\x0b\x32).typedb.protocol.ThingType.UnsetPlays.ResH\x00R\x16thingTypeUnsetPlaysRes\x12^\n\x16\x65ntity_type_create_res\x18\x90\x03 \x01(\x0b\x32&.typedb.protocol.EntityType.Create.ResH\x00R\x13\x65ntityTypeCreateRes\x12\x64\n\x18relation_type_create_res\x18\xf4\x03 \x01(\x0b\x32(.typedb.protocol.RelationType.Create.ResH\x00R\x15relationTypeCreateRes\x12\x98\x01\n,relation_type_get_relates_for_role_label_res\x18\xf5\x03 \x01(\x0b\x32\x38.typedb.protocol.RelationType.GetRelatesForRoleLabel.ResH\x00R%relationTypeGetRelatesForRoleLabelRes\x12q\n\x1drelation_type_set_relates_res\x18\xf6\x03 \x01(\x0b\x32,.typedb.protocol.RelationType.SetRelates.ResH\x00R\x19relationTypeSetRelatesRes\x12w\n\x1frelation_type_unset_relates_res\x18\xf7\x03 \x01(\x0b\x32..typedb.protocol.RelationType.UnsetRelates.ResH\x00R\x1brelationTypeUnsetRelatesRes\x12^\n\x16\x61ttribute_type_put_res\x18\xd8\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Put.ResH\x00R\x13\x61ttributeTypePutRes\x12^\n\x16\x61ttribute_type_get_res\x18\xd9\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Get.ResH\x00R\x13\x61ttributeTypeGetRes\x12n\n\x1c\x61ttribute_type_get_regex_res\x18\xda\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.GetRegex.ResH\x00R\x18\x61ttributeTypeGetRegexRes\x12n\n\x1c\x61ttribute_type_set_regex_res\x18\xdb\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.SetRegex.ResH\x00R\x18\x61ttributeTypeSetRegexResB\x05\n\x03res\x1a\xc0\x08\n\x07ResPart\x12m\n\x1ctype_get_supertypes_res_part\x18\x64 \x01(\x0b\x32+.typedb.protocol.Type.GetSupertypes.ResPartH\x00R\x18typeGetSupertypesResPart\x12g\n\x1atype_get_subtypes_res_part\x18\x65 \x01(\x0b\x32).typedb.protocol.Type.GetSubtypes.ResPartH\x00R\x16typeGetSubtypesResPart\x12\x85\x01\n%role_type_get_relation_types_res_part\x18\xc8\x01 \x01(\x0b\x32\x32.typedb.protocol.RoleType.GetRelationTypes.ResPartH\x00R\x1froleTypeGetRelationTypesResPart\x12r\n\x1erole_type_get_players_res_part\x18\xc9\x01 \x01(\x0b\x32,.typedb.protocol.RoleType.GetPlayers.ResPartH\x00R\x19roleTypeGetPlayersResPart\x12{\n!thing_type_get_instances_res_part\x18\xac\x02 \x01(\x0b\x32/.typedb.protocol.ThingType.GetInstances.ResPartH\x00R\x1cthingTypeGetInstancesResPart\x12l\n\x1cthing_type_get_owns_res_part\x18\xad\x02 \x01(\x0b\x32*.typedb.protocol.ThingType.GetOwns.ResPartH\x00R\x17thingTypeGetOwnsResPart\x12o\n\x1dthing_type_get_plays_res_part\x18\xae\x02 \x01(\x0b\x32+.typedb.protocol.ThingType.GetPlays.ResPartH\x00R\x18thingTypeGetPlaysResPart\x12~\n\"relation_type_get_relates_res_part\x18\xf4\x03 \x01(\x0b\x32\x30.typedb.protocol.RelationType.GetRelates.ResPartH\x00R\x1drelationTypeGetRelatesResPart\x12~\n\"attribute_type_get_owners_res_part\x18\xd8\x04 \x01(\x0b\x32\x30.typedb.protocol.AttributeType.GetOwners.ResPartH\x00R\x1d\x61ttributeTypeGetOwnersResPartB\x05\n\x03res\x1a\x16\n\x06\x44\x65lete\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1a.\n\x08SetLabel\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x05\n\x03Res\x1a\x36\n\nIsAbstract\x1a\x05\n\x03Req\x1a!\n\x03Res\x12\x1a\n\x08\x61\x62stract\x18\x01 \x01(\x08R\x08\x61\x62stract\x1aP\n\x0cGetSupertype\x1a\x05\n\x03Req\x1a\x39\n\x03Res\x12+\n\x04type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x04typeB\x05\n\x03res\x1aG\n\x0cSetSupertype\x1a\x30\n\x03Req\x12)\n\x04type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x04type\x1a\x05\n\x03Res\x1aN\n\rGetSupertypes\x1a\x05\n\x03Req\x1a\x36\n\x07ResPart\x12+\n\x05types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05types\x1aL\n\x0bGetSubtypes\x1a\x05\n\x03Req\x1a\x36\n\x07ResPart\x12+\n\x05types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05types\"a\n\x08\x45ncoding\x12\x0e\n\nTHING_TYPE\x10\x00\x12\x0f\n\x0b\x45NTITY_TYPE\x10\x01\x12\x11\n\rRELATION_TYPE\x10\x02\x12\x12\n\x0e\x41TTRIBUTE_TYPE\x10\x03\x12\r\n\tROLE_TYPE\x10\x04\"\xc6\x01\n\x08RoleType\x1a\x62\n\x10GetRelationTypes\x1a\x05\n\x03Req\x1aG\n\x07ResPart\x12<\n\x0erelation_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\rrelationTypes\x1aV\n\nGetPlayers\x1a\x05\n\x03Req\x1a\x41\n\x07ResPart\x12\x36\n\x0bthing_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\nthingTypes\"\xab\x07\n\tThingType\x1a\x1b\n\x0bSetAbstract\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1a\x1d\n\rUnsetAbstract\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1aP\n\x0cGetInstances\x1a\x05\n\x03Req\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\x1a\xcd\x01\n\x07GetOwns\x1aw\n\x03Req\x12I\n\nvalue_type\x18\x01 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeH\x00R\tvalueType\x12\x1b\n\tkeys_only\x18\x03 \x01(\x08R\x08keysOnlyB\x08\n\x06\x66ilter\x1aI\n\x07ResPart\x12>\n\x0f\x61ttribute_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x0e\x61ttributeTypes\x1aI\n\x08GetPlays\x1a\x05\n\x03Req\x1a\x36\n\x07ResPart\x12+\n\x05roles\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05roles\x1a\xbd\x01\n\x07SetOwns\x1a\xaa\x01\n\x03Req\x12<\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\rattributeType\x12@\n\x0foverridden_type\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x0eoverriddenType\x12\x15\n\x06is_key\x18\x03 \x01(\x08R\x05isKeyB\x0c\n\noverridden\x1a\x05\n\x03Res\x1a\x94\x01\n\x08SetPlays\x1a\x80\x01\n\x03Req\x12)\n\x04role\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x04role\x12@\n\x0foverridden_role\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x0eoverriddenRoleB\x0c\n\noverridden\x1a\x05\n\x03Res\x1aW\n\tUnsetOwns\x1a\x43\n\x03Req\x12<\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\rattributeType\x1a\x05\n\x03Res\x1a\x45\n\nUnsetPlays\x1a\x30\n\x03Req\x12)\n\x04role\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x04role\x1a\x05\n\x03Res\"T\n\nEntityType\x1a\x46\n\x06\x43reate\x1a\x05\n\x03Req\x1a\x35\n\x03Res\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06\x65ntity\"\xc4\x03\n\x0cRelationType\x1aJ\n\x06\x43reate\x1a\x05\n\x03Req\x1a\x39\n\x03Res\x12\x32\n\x08relation\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x08relation\x1aK\n\nGetRelates\x1a\x05\n\x03Req\x1a\x36\n\x07ResPart\x12+\n\x05roles\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05roles\x1az\n\x16GetRelatesForRoleLabel\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x43\n\x03Res\x12\x34\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x08roleTypeB\x06\n\x04role\x1ak\n\nSetRelates\x1aV\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12+\n\x10overridden_label\x18\x02 \x01(\tH\x00R\x0foverriddenLabelB\x0c\n\noverridden\x1a\x05\n\x03Res\x1a\x32\n\x0cUnsetRelates\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x05\n\x03Res\"\x85\x07\n\rAttributeType\x1a\x81\x01\n\x03Put\x1a=\n\x03Req\x12\x36\n\x05value\x18\x01 \x01(\x0b\x32 .typedb.protocol.Attribute.ValueR\x05value\x1a;\n\x03Res\x12\x34\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\tattribute\x1a\x8a\x01\n\x03Get\x1a=\n\x03Req\x12\x36\n\x05value\x18\x01 \x01(\x0b\x32 .typedb.protocol.Attribute.ValueR\x05value\x1a\x44\n\x03Res\x12\x36\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingH\x00R\tattributeB\x05\n\x03res\x1ag\n\tGetOwners\x1a \n\x03Req\x12\x19\n\x08only_key\x18\x01 \x01(\x08R\x07onlyKey\x1a\x38\n\x07ResPart\x12-\n\x06owners\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x06owners\x1a.\n\x08GetRegex\x1a\x05\n\x03Req\x1a\x1b\n\x03Res\x12\x14\n\x05regex\x18\x01 \x01(\tR\x05regex\x1a.\n\x08SetRegex\x1a\x1b\n\x03Req\x12\x14\n\x05regex\x18\x01 \x01(\tR\x05regex\x1a\x05\n\x03Res\x1a\x9e\x01\n\x0bGetSubtypes\x1aW\n\x03Req\x12I\n\nvalue_type\x18\x01 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeH\x00R\tvalueTypeB\x05\n\x03req\x1a\x36\n\x07ResPart\x12+\n\x05types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05types\x1a\xa2\x01\n\x0cGetInstances\x1aW\n\x03Req\x12I\n\nvalue_type\x18\x01 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeH\x00R\tvalueTypeB\x05\n\x03req\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\"T\n\tValueType\x12\n\n\x06OBJECT\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\x08\n\x04LONG\x10\x02\x12\n\n\x06\x44OUBLE\x10\x03\x12\n\n\x06STRING\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05\x42+\n\x1b\x63om.vaticle.typedb.protocolB\x0c\x43onceptProtob\x06proto3')
+  serialized_pb=_b('\n\x14\x63ommon/concept.proto\x12\x0ftypedb.protocol\"\x84\r\n\x0e\x43onceptManager\x1a\xfc\x03\n\x03Req\x12_\n\x12get_thing_type_req\x18\x01 \x01(\x0b\x32\x30.typedb.protocol.ConceptManager.GetThingType.ReqH\x00R\x0fgetThingTypeReq\x12R\n\rget_thing_req\x18\x02 \x01(\x0b\x32,.typedb.protocol.ConceptManager.GetThing.ReqH\x00R\x0bgetThingReq\x12\x62\n\x13put_entity_type_req\x18\x03 \x01(\x0b\x32\x31.typedb.protocol.ConceptManager.PutEntityType.ReqH\x00R\x10putEntityTypeReq\x12k\n\x16put_attribute_type_req\x18\x04 \x01(\x0b\x32\x34.typedb.protocol.ConceptManager.PutAttributeType.ReqH\x00R\x13putAttributeTypeReq\x12h\n\x15put_relation_type_req\x18\x05 \x01(\x0b\x32\x33.typedb.protocol.ConceptManager.PutRelationType.ReqH\x00R\x12putRelationTypeReqB\x05\n\x03req\x1a\xfc\x03\n\x03Res\x12_\n\x12get_thing_type_res\x18\x01 \x01(\x0b\x32\x30.typedb.protocol.ConceptManager.GetThingType.ResH\x00R\x0fgetThingTypeRes\x12R\n\rget_thing_res\x18\x02 \x01(\x0b\x32,.typedb.protocol.ConceptManager.GetThing.ResH\x00R\x0bgetThingRes\x12\x62\n\x13put_entity_type_res\x18\x03 \x01(\x0b\x32\x31.typedb.protocol.ConceptManager.PutEntityType.ResH\x00R\x10putEntityTypeRes\x12k\n\x16put_attribute_type_res\x18\x04 \x01(\x0b\x32\x34.typedb.protocol.ConceptManager.PutAttributeType.ResH\x00R\x13putAttributeTypeRes\x12h\n\x15put_relation_type_res\x18\x05 \x01(\x0b\x32\x33.typedb.protocol.ConceptManager.PutRelationType.ResH\x00R\x12putRelationTypeResB\x05\n\x03res\x1aq\n\x0cGetThingType\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x44\n\x03Res\x12\x36\n\nthing_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\tthingTypeB\x05\n\x03res\x1a\x61\n\x08GetThing\x1a\x17\n\x03Req\x12\x10\n\x03iid\x18\x01 \x01(\x0cR\x03iid\x1a<\n\x03Res\x12.\n\x05thing\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingH\x00R\x05thingB\x05\n\x03res\x1ak\n\rPutEntityType\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a=\n\x03Res\x12\x36\n\x0b\x65ntity_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\nentityType\x1a\xbd\x01\n\x10PutAttributeType\x1a\x64\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12G\n\nvalue_type\x18\x02 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeR\tvalueType\x1a\x43\n\x03Res\x12<\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\rattributeType\x1aq\n\x0fPutRelationType\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x41\n\x03Res\x12:\n\rrelation_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x0crelationType\"q\n\x07\x43oncept\x12.\n\x05thing\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingH\x00R\x05thing\x12+\n\x04type\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x04typeB\t\n\x07\x63oncept\"\x96\x1b\n\x05Thing\x12\x10\n\x03iid\x18\x01 \x01(\x0cR\x03iid\x12)\n\x04type\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x04type\x12\x36\n\x05value\x18\x03 \x01(\x0b\x32 .typedb.protocol.Attribute.ValueR\x05value\x12\x1a\n\x08inferred\x18\x04 \x01(\x08R\x08inferred\x1a\x80\n\n\x03Req\x12\x10\n\x03iid\x18\x01 \x01(\x0cR\x03iid\x12M\n\x10thing_delete_req\x18\x64 \x01(\x0b\x32!.typedb.protocol.Thing.Delete.ReqH\x00R\x0ethingDeleteReq\x12Q\n\x12thing_get_type_req\x18\x65 \x01(\x0b\x32\".typedb.protocol.Thing.GetType.ReqH\x00R\x0fthingGetTypeReq\x12N\n\x11thing_get_has_req\x18\x66 \x01(\x0b\x32!.typedb.protocol.Thing.GetHas.ReqH\x00R\x0ethingGetHasReq\x12N\n\x11thing_set_has_req\x18g \x01(\x0b\x32!.typedb.protocol.Thing.SetHas.ReqH\x00R\x0ethingSetHasReq\x12T\n\x13thing_unset_has_req\x18h \x01(\x0b\x32#.typedb.protocol.Thing.UnsetHas.ReqH\x00R\x10thingUnsetHasReq\x12`\n\x17thing_get_relations_req\x18i \x01(\x0b\x32\'.typedb.protocol.Thing.GetRelations.ReqH\x00R\x14thingGetRelationsReq\x12Z\n\x15thing_get_playing_req\x18j \x01(\x0b\x32%.typedb.protocol.Thing.GetPlaying.ReqH\x00R\x12thingGetPlayingReq\x12\x61\n\x17relation_add_player_req\x18\xc8\x01 \x01(\x0b\x32\'.typedb.protocol.Relation.AddPlayer.ReqH\x00R\x14relationAddPlayerReq\x12j\n\x1arelation_remove_player_req\x18\xc9\x01 \x01(\x0b\x32*.typedb.protocol.Relation.RemovePlayer.ReqH\x00R\x17relationRemovePlayerReq\x12\x64\n\x18relation_get_players_req\x18\xca\x01 \x01(\x0b\x32(.typedb.protocol.Relation.GetPlayers.ReqH\x00R\x15relationGetPlayersReq\x12\x85\x01\n%relation_get_players_by_role_type_req\x18\xcb\x01 \x01(\x0b\x32\x32.typedb.protocol.Relation.GetPlayersByRoleType.ReqH\x00R\x1frelationGetPlayersByRoleTypeReq\x12g\n\x19relation_get_relating_req\x18\xcc\x01 \x01(\x0b\x32).typedb.protocol.Relation.GetRelating.ReqH\x00R\x16relationGetRelatingReq\x12\x64\n\x18\x61ttribute_get_owners_req\x18\xac\x02 \x01(\x0b\x32(.typedb.protocol.Attribute.GetOwners.ReqH\x00R\x15\x61ttributeGetOwnersReqB\x05\n\x03req\x1a\xa3\x04\n\x03Res\x12M\n\x10thing_delete_res\x18\x64 \x01(\x0b\x32!.typedb.protocol.Thing.Delete.ResH\x00R\x0ethingDeleteRes\x12Q\n\x12thing_get_type_res\x18\x65 \x01(\x0b\x32\".typedb.protocol.Thing.GetType.ResH\x00R\x0fthingGetTypeRes\x12N\n\x11thing_set_has_res\x18\x66 \x01(\x0b\x32!.typedb.protocol.Thing.SetHas.ResH\x00R\x0ethingSetHasRes\x12T\n\x13thing_unset_has_res\x18g \x01(\x0b\x32#.typedb.protocol.Thing.UnsetHas.ResH\x00R\x10thingUnsetHasRes\x12\x61\n\x17relation_add_player_res\x18\xc8\x01 \x01(\x0b\x32\'.typedb.protocol.Relation.AddPlayer.ResH\x00R\x14relationAddPlayerRes\x12j\n\x1arelation_remove_player_res\x18\xc9\x01 \x01(\x0b\x32*.typedb.protocol.Relation.RemovePlayer.ResH\x00R\x17relationRemovePlayerResB\x05\n\x03res\x1a\xb6\x06\n\x07ResPart\x12[\n\x16thing_get_has_res_part\x18\x64 \x01(\x0b\x32%.typedb.protocol.Thing.GetHas.ResPartH\x00R\x12thingGetHasResPart\x12m\n\x1cthing_get_relations_res_part\x18\x65 \x01(\x0b\x32+.typedb.protocol.Thing.GetRelations.ResPartH\x00R\x18thingGetRelationsResPart\x12g\n\x1athing_get_playing_res_part\x18\x66 \x01(\x0b\x32).typedb.protocol.Thing.GetPlaying.ResPartH\x00R\x16thingGetPlayingResPart\x12q\n\x1drelation_get_players_res_part\x18\xc8\x01 \x01(\x0b\x32,.typedb.protocol.Relation.GetPlayers.ResPartH\x00R\x19relationGetPlayersResPart\x12\x92\x01\n*relation_get_players_by_role_type_res_part\x18\xc9\x01 \x01(\x0b\x32\x36.typedb.protocol.Relation.GetPlayersByRoleType.ResPartH\x00R#relationGetPlayersByRoleTypeResPart\x12t\n\x1erelation_get_relating_res_part\x18\xca\x01 \x01(\x0b\x32-.typedb.protocol.Relation.GetRelating.ResPartH\x00R\x1arelationGetRelatingResPart\x12q\n\x1d\x61ttribute_get_owners_res_part\x18\xac\x02 \x01(\x0b\x32,.typedb.protocol.Attribute.GetOwners.ResPartH\x00R\x19\x61ttributeGetOwnersResPartB\x05\n\x03res\x1a\x16\n\x06\x44\x65lete\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1aM\n\x07GetType\x1a\x05\n\x03Req\x1a;\n\x03Res\x12\x34\n\nthing_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\tthingType\x1aL\n\x06SetHas\x1a;\n\x03Req\x12\x34\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\tattribute\x1a\x05\n\x03Res\x1aN\n\x08UnsetHas\x1a;\n\x03Req\x12\x34\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\tattribute\x1a\x05\n\x03Res\x1a\xaf\x01\n\x06GetHas\x1a\x62\n\x03Req\x12>\n\x0f\x61ttribute_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x0e\x61ttributeTypes\x12\x1b\n\tkeys_only\x18\x02 \x01(\x08R\x08keysOnly\x1a\x41\n\x07ResPart\x12\x36\n\nattributes\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\nattributes\x1aT\n\nGetPlaying\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a\x8c\x01\n\x0cGetRelations\x1a;\n\x03Req\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a?\n\x07ResPart\x12\x34\n\trelations\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\trelations\"\x8a\x06\n\x08Relation\x1a}\n\tAddPlayer\x1ai\n\x03Req\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x12.\n\x06player\x18\x02 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06player\x1a\x05\n\x03Res\x1a\x80\x01\n\x0cRemovePlayer\x1ai\n\x03Req\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x12.\n\x06player\x18\x02 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06player\x1a\x05\n\x03Res\x1a\x84\x01\n\nGetPlayers\x1a;\n\x03Req\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\x1a\x9d\x02\n\x14GetPlayersByRoleType\x1ax\n\x12RoleTypeWithPlayer\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x12.\n\x06player\x18\x02 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06player\x1a\x05\n\x03Req\x1a\x83\x01\n\x07ResPart\x12x\n\x17role_types_with_players\x18\x01 \x03(\x0b\x32\x41.typedb.protocol.Relation.GetPlayersByRoleType.RoleTypeWithPlayerR\x14roleTypesWithPlayers\x1aU\n\x0bGetRelating\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\"\xb5\x02\n\tAttribute\x1a\x95\x01\n\x05Value\x12\x18\n\x06string\x18\x01 \x01(\tH\x00R\x06string\x12\x1a\n\x07\x62oolean\x18\x02 \x01(\x08H\x00R\x07\x62oolean\x12\x14\n\x04long\x18\x03 \x01(\x03H\x00R\x04long\x12\x18\n\x06\x64ouble\x18\x04 \x01(\x01H\x00R\x06\x64ouble\x12\x1d\n\tdate_time\x18\x05 \x01(\x03H\x00R\x08\x64\x61teTimeB\x07\n\x05value\x1a\x8f\x01\n\tGetOwners\x1aG\n\x03Req\x12\x36\n\nthing_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\tthingTypeB\x08\n\x06\x66ilter\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\"\xd5J\n\x04Type\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12\x14\n\x05scope\x18\x02 \x01(\tR\x05scope\x12:\n\x08\x65ncoding\x18\x03 \x01(\x0e\x32\x1e.typedb.protocol.Type.EncodingR\x08\x65ncoding\x12G\n\nvalue_type\x18\x04 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeR\tvalueType\x12\x12\n\x04root\x18\x05 \x01(\x08R\x04root\x1a\xb2!\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12\x14\n\x05scope\x18\x02 \x01(\tR\x05scope\x12J\n\x0ftype_delete_req\x18\x64 \x01(\x0b\x32 .typedb.protocol.Type.Delete.ReqH\x00R\rtypeDeleteReq\x12Q\n\x12type_set_label_req\x18\x65 \x01(\x0b\x32\".typedb.protocol.Type.SetLabel.ReqH\x00R\x0ftypeSetLabelReq\x12W\n\x14type_is_abstract_req\x18\x66 \x01(\x0b\x32$.typedb.protocol.Type.IsAbstract.ReqH\x00R\x11typeIsAbstractReq\x12]\n\x16type_get_supertype_req\x18g \x01(\x0b\x32&.typedb.protocol.Type.GetSupertype.ReqH\x00R\x13typeGetSupertypeReq\x12]\n\x16type_set_supertype_req\x18h \x01(\x0b\x32&.typedb.protocol.Type.SetSupertype.ReqH\x00R\x13typeSetSupertypeReq\x12`\n\x17type_get_supertypes_req\x18i \x01(\x0b\x32\'.typedb.protocol.Type.GetSupertypes.ReqH\x00R\x14typeGetSupertypesReq\x12Z\n\x15type_get_subtypes_req\x18j \x01(\x0b\x32%.typedb.protocol.Type.GetSubtypes.ReqH\x00R\x12typeGetSubtypesReq\x12s\n\x1etype_get_subtypes_explicit_req\x18k \x01(\x0b\x32-.typedb.protocol.Type.GetSubtypesExplicit.ReqH\x00R\x1atypeGetSubtypesExplicitReq\x12x\n role_type_get_relation_types_req\x18\xc8\x01 \x01(\x0b\x32..typedb.protocol.RoleType.GetRelationTypes.ReqH\x00R\x1broleTypeGetRelationTypesReq\x12\x65\n\x19role_type_get_players_req\x18\xc9\x01 \x01(\x0b\x32(.typedb.protocol.RoleType.GetPlayers.ReqH\x00R\x15roleTypeGetPlayersReq\x12n\n\x1cthing_type_get_instances_req\x18\xac\x02 \x01(\x0b\x32+.typedb.protocol.ThingType.GetInstances.ReqH\x00R\x18thingTypeGetInstancesReq\x12\x87\x01\n%thing_type_get_instances_explicit_req\x18\xb5\x02 \x01(\x0b\x32\x33.typedb.protocol.ThingType.GetInstancesExplicit.ReqH\x00R thingTypeGetInstancesExplicitReq\x12k\n\x1bthing_type_set_abstract_req\x18\xad\x02 \x01(\x0b\x32*.typedb.protocol.ThingType.SetAbstract.ReqH\x00R\x17thingTypeSetAbstractReq\x12q\n\x1dthing_type_unset_abstract_req\x18\xae\x02 \x01(\x0b\x32,.typedb.protocol.ThingType.UnsetAbstract.ReqH\x00R\x19thingTypeUnsetAbstractReq\x12_\n\x17thing_type_get_owns_req\x18\xaf\x02 \x01(\x0b\x32&.typedb.protocol.ThingType.GetOwns.ReqH\x00R\x13thingTypeGetOwnsReq\x12x\n thing_type_get_owns_explicit_req\x18\xb6\x02 \x01(\x0b\x32..typedb.protocol.ThingType.GetOwnsExplicit.ReqH\x00R\x1bthingTypeGetOwnsExplicitReq\x12~\n\"thing_type_get_owns_overridden_req\x18\xb7\x02 \x01(\x0b\x32\x30.typedb.protocol.ThingType.GetOwnsOverridden.ReqH\x00R\x1dthingTypeGetOwnsOverriddenReq\x12_\n\x17thing_type_set_owns_req\x18\xb0\x02 \x01(\x0b\x32&.typedb.protocol.ThingType.SetOwns.ReqH\x00R\x13thingTypeSetOwnsReq\x12\x65\n\x19thing_type_unset_owns_req\x18\xb1\x02 \x01(\x0b\x32(.typedb.protocol.ThingType.UnsetOwns.ReqH\x00R\x15thingTypeUnsetOwnsReq\x12\x62\n\x18thing_type_get_plays_req\x18\xb2\x02 \x01(\x0b\x32\'.typedb.protocol.ThingType.GetPlays.ReqH\x00R\x14thingTypeGetPlaysReq\x12{\n!thing_type_get_plays_explicit_req\x18\xb8\x02 \x01(\x0b\x32/.typedb.protocol.ThingType.GetPlaysExplicit.ReqH\x00R\x1cthingTypeGetPlaysExplicitReq\x12\x81\x01\n#thing_type_get_plays_overridden_req\x18\xb9\x02 \x01(\x0b\x32\x31.typedb.protocol.ThingType.GetPlaysOverridden.ReqH\x00R\x1ethingTypeGetPlaysOverriddenReq\x12\x62\n\x18thing_type_set_plays_req\x18\xb3\x02 \x01(\x0b\x32\'.typedb.protocol.ThingType.SetPlays.ReqH\x00R\x14thingTypeSetPlaysReq\x12h\n\x1athing_type_unset_plays_req\x18\xb4\x02 \x01(\x0b\x32).typedb.protocol.ThingType.UnsetPlays.ReqH\x00R\x16thingTypeUnsetPlaysReq\x12^\n\x16\x65ntity_type_create_req\x18\x90\x03 \x01(\x0b\x32&.typedb.protocol.EntityType.Create.ReqH\x00R\x13\x65ntityTypeCreateReq\x12\x64\n\x18relation_type_create_req\x18\xf4\x03 \x01(\x0b\x32(.typedb.protocol.RelationType.Create.ReqH\x00R\x15relationTypeCreateReq\x12q\n\x1drelation_type_get_relates_req\x18\xf6\x03 \x01(\x0b\x32,.typedb.protocol.RelationType.GetRelates.ReqH\x00R\x19relationTypeGetRelatesReq\x12\x8a\x01\n&relation_type_get_relates_explicit_req\x18\xf9\x03 \x01(\x0b\x32\x34.typedb.protocol.RelationType.GetRelatesExplicit.ReqH\x00R!relationTypeGetRelatesExplicitReq\x12\x98\x01\n,relation_type_get_relates_for_role_label_req\x18\xf5\x03 \x01(\x0b\x32\x38.typedb.protocol.RelationType.GetRelatesForRoleLabel.ReqH\x00R%relationTypeGetRelatesForRoleLabelReq\x12\x90\x01\n(relation_type_get_relates_overridden_req\x18\xfa\x03 \x01(\x0b\x32\x36.typedb.protocol.RelationType.GetRelatesOverridden.ReqH\x00R#relationTypeGetRelatesOverriddenReq\x12q\n\x1drelation_type_set_relates_req\x18\xf7\x03 \x01(\x0b\x32,.typedb.protocol.RelationType.SetRelates.ReqH\x00R\x19relationTypeSetRelatesReq\x12w\n\x1frelation_type_unset_relates_req\x18\xf8\x03 \x01(\x0b\x32..typedb.protocol.RelationType.UnsetRelates.ReqH\x00R\x1brelationTypeUnsetRelatesReq\x12^\n\x16\x61ttribute_type_put_req\x18\xd8\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Put.ReqH\x00R\x13\x61ttributeTypePutReq\x12^\n\x16\x61ttribute_type_get_req\x18\xd9\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Get.ReqH\x00R\x13\x61ttributeTypeGetReq\x12n\n\x1c\x61ttribute_type_get_regex_req\x18\xda\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.GetRegex.ReqH\x00R\x18\x61ttributeTypeGetRegexReq\x12n\n\x1c\x61ttribute_type_set_regex_req\x18\xdb\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.SetRegex.ReqH\x00R\x18\x61ttributeTypeSetRegexReq\x12q\n\x1d\x61ttribute_type_get_owners_req\x18\xdc\x04 \x01(\x0b\x32,.typedb.protocol.AttributeType.GetOwners.ReqH\x00R\x19\x61ttributeTypeGetOwnersReq\x12\x8a\x01\n&attribute_type_get_owners_explicit_req\x18\xdd\x04 \x01(\x0b\x32\x34.typedb.protocol.AttributeType.GetOwnersExplicit.ReqH\x00R!attributeTypeGetOwnersExplicitReqB\x05\n\x03req\x1a\xbc\x13\n\x03Res\x12J\n\x0ftype_delete_res\x18\x64 \x01(\x0b\x32 .typedb.protocol.Type.Delete.ResH\x00R\rtypeDeleteRes\x12Q\n\x12type_set_label_res\x18\x65 \x01(\x0b\x32\".typedb.protocol.Type.SetLabel.ResH\x00R\x0ftypeSetLabelRes\x12W\n\x14type_is_abstract_res\x18\x66 \x01(\x0b\x32$.typedb.protocol.Type.IsAbstract.ResH\x00R\x11typeIsAbstractRes\x12]\n\x16type_get_supertype_res\x18g \x01(\x0b\x32&.typedb.protocol.Type.GetSupertype.ResH\x00R\x13typeGetSupertypeRes\x12]\n\x16type_set_supertype_res\x18h \x01(\x0b\x32&.typedb.protocol.Type.SetSupertype.ResH\x00R\x13typeSetSupertypeRes\x12k\n\x1bthing_type_set_abstract_res\x18\xac\x02 \x01(\x0b\x32*.typedb.protocol.ThingType.SetAbstract.ResH\x00R\x17thingTypeSetAbstractRes\x12q\n\x1dthing_type_unset_abstract_res\x18\xad\x02 \x01(\x0b\x32,.typedb.protocol.ThingType.UnsetAbstract.ResH\x00R\x19thingTypeUnsetAbstractRes\x12~\n\"thing_type_get_owns_overridden_res\x18\xb2\x02 \x01(\x0b\x32\x30.typedb.protocol.ThingType.GetOwnsOverridden.ResH\x00R\x1dthingTypeGetOwnsOverriddenRes\x12_\n\x17thing_type_set_owns_res\x18\xae\x02 \x01(\x0b\x32&.typedb.protocol.ThingType.SetOwns.ResH\x00R\x13thingTypeSetOwnsRes\x12\x65\n\x19thing_type_unset_owns_res\x18\xaf\x02 \x01(\x0b\x32(.typedb.protocol.ThingType.UnsetOwns.ResH\x00R\x15thingTypeUnsetOwnsRes\x12\x81\x01\n#thing_type_get_plays_overridden_res\x18\xb3\x02 \x01(\x0b\x32\x31.typedb.protocol.ThingType.GetPlaysOverridden.ResH\x00R\x1ethingTypeGetPlaysOverriddenRes\x12\x62\n\x18thing_type_set_plays_res\x18\xb0\x02 \x01(\x0b\x32\'.typedb.protocol.ThingType.SetPlays.ResH\x00R\x14thingTypeSetPlaysRes\x12h\n\x1athing_type_unset_plays_res\x18\xb1\x02 \x01(\x0b\x32).typedb.protocol.ThingType.UnsetPlays.ResH\x00R\x16thingTypeUnsetPlaysRes\x12^\n\x16\x65ntity_type_create_res\x18\x90\x03 \x01(\x0b\x32&.typedb.protocol.EntityType.Create.ResH\x00R\x13\x65ntityTypeCreateRes\x12\x64\n\x18relation_type_create_res\x18\xf4\x03 \x01(\x0b\x32(.typedb.protocol.RelationType.Create.ResH\x00R\x15relationTypeCreateRes\x12\x98\x01\n,relation_type_get_relates_for_role_label_res\x18\xf5\x03 \x01(\x0b\x32\x38.typedb.protocol.RelationType.GetRelatesForRoleLabel.ResH\x00R%relationTypeGetRelatesForRoleLabelRes\x12\x90\x01\n(relation_type_get_relates_overridden_res\x18\xf8\x03 \x01(\x0b\x32\x36.typedb.protocol.RelationType.GetRelatesOverridden.ResH\x00R#relationTypeGetRelatesOverriddenRes\x12q\n\x1drelation_type_set_relates_res\x18\xf6\x03 \x01(\x0b\x32,.typedb.protocol.RelationType.SetRelates.ResH\x00R\x19relationTypeSetRelatesRes\x12w\n\x1frelation_type_unset_relates_res\x18\xf7\x03 \x01(\x0b\x32..typedb.protocol.RelationType.UnsetRelates.ResH\x00R\x1brelationTypeUnsetRelatesRes\x12^\n\x16\x61ttribute_type_put_res\x18\xd8\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Put.ResH\x00R\x13\x61ttributeTypePutRes\x12^\n\x16\x61ttribute_type_get_res\x18\xd9\x04 \x01(\x0b\x32&.typedb.protocol.AttributeType.Get.ResH\x00R\x13\x61ttributeTypeGetRes\x12n\n\x1c\x61ttribute_type_get_regex_res\x18\xda\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.GetRegex.ResH\x00R\x18\x61ttributeTypeGetRegexRes\x12n\n\x1c\x61ttribute_type_set_regex_res\x18\xdb\x04 \x01(\x0b\x32+.typedb.protocol.AttributeType.SetRegex.ResH\x00R\x18\x61ttributeTypeSetRegexResB\x05\n\x03res\x1a\xa1\x0f\n\x07ResPart\x12m\n\x1ctype_get_supertypes_res_part\x18\x64 \x01(\x0b\x32+.typedb.protocol.Type.GetSupertypes.ResPartH\x00R\x18typeGetSupertypesResPart\x12g\n\x1atype_get_subtypes_res_part\x18\x65 \x01(\x0b\x32).typedb.protocol.Type.GetSubtypes.ResPartH\x00R\x16typeGetSubtypesResPart\x12\x80\x01\n#type_get_subtypes_explicit_res_part\x18\x66 \x01(\x0b\x32\x31.typedb.protocol.Type.GetSubtypesExplicit.ResPartH\x00R\x1etypeGetSubtypesExplicitResPart\x12\x85\x01\n%role_type_get_relation_types_res_part\x18\xc8\x01 \x01(\x0b\x32\x32.typedb.protocol.RoleType.GetRelationTypes.ResPartH\x00R\x1froleTypeGetRelationTypesResPart\x12r\n\x1erole_type_get_players_res_part\x18\xc9\x01 \x01(\x0b\x32,.typedb.protocol.RoleType.GetPlayers.ResPartH\x00R\x19roleTypeGetPlayersResPart\x12{\n!thing_type_get_instances_res_part\x18\xac\x02 \x01(\x0b\x32/.typedb.protocol.ThingType.GetInstances.ResPartH\x00R\x1cthingTypeGetInstancesResPart\x12\x94\x01\n*thing_type_get_instances_explicit_res_part\x18\xaf\x02 \x01(\x0b\x32\x37.typedb.protocol.ThingType.GetInstancesExplicit.ResPartH\x00R$thingTypeGetInstancesExplicitResPart\x12l\n\x1cthing_type_get_owns_res_part\x18\xad\x02 \x01(\x0b\x32*.typedb.protocol.ThingType.GetOwns.ResPartH\x00R\x17thingTypeGetOwnsResPart\x12\x85\x01\n%thing_type_get_owns_explicit_res_part\x18\xb0\x02 \x01(\x0b\x32\x32.typedb.protocol.ThingType.GetOwnsExplicit.ResPartH\x00R\x1fthingTypeGetOwnsExplicitResPart\x12o\n\x1dthing_type_get_plays_res_part\x18\xae\x02 \x01(\x0b\x32+.typedb.protocol.ThingType.GetPlays.ResPartH\x00R\x18thingTypeGetPlaysResPart\x12\x88\x01\n&thing_type_get_plays_explicit_res_part\x18\xb1\x02 \x01(\x0b\x32\x33.typedb.protocol.ThingType.GetPlaysExplicit.ResPartH\x00R thingTypeGetPlaysExplicitResPart\x12~\n\"relation_type_get_relates_res_part\x18\xf4\x03 \x01(\x0b\x32\x30.typedb.protocol.RelationType.GetRelates.ResPartH\x00R\x1drelationTypeGetRelatesResPart\x12\x97\x01\n+relation_type_get_relates_explicit_res_part\x18\xf5\x03 \x01(\x0b\x32\x38.typedb.protocol.RelationType.GetRelatesExplicit.ResPartH\x00R%relationTypeGetRelatesExplicitResPart\x12~\n\"attribute_type_get_owners_res_part\x18\xd8\x04 \x01(\x0b\x32\x30.typedb.protocol.AttributeType.GetOwners.ResPartH\x00R\x1d\x61ttributeTypeGetOwnersResPart\x12\x97\x01\n+attribute_type_get_owners_explicit_res_part\x18\xd9\x04 \x01(\x0b\x32\x38.typedb.protocol.AttributeType.GetOwnersExplicit.ResPartH\x00R%attributeTypeGetOwnersExplicitResPartB\x05\n\x03res\x1a\x16\n\x06\x44\x65lete\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1a.\n\x08SetLabel\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x05\n\x03Res\x1a\x36\n\nIsAbstract\x1a\x05\n\x03Req\x1a!\n\x03Res\x12\x1a\n\x08\x61\x62stract\x18\x01 \x01(\x08R\x08\x61\x62stract\x1aP\n\x0cGetSupertype\x1a\x05\n\x03Req\x1a\x39\n\x03Res\x12+\n\x04type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x04typeB\x05\n\x03res\x1aG\n\x0cSetSupertype\x1a\x30\n\x03Req\x12)\n\x04type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x04type\x1a\x05\n\x03Res\x1aN\n\rGetSupertypes\x1a\x05\n\x03Req\x1a\x36\n\x07ResPart\x12+\n\x05types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05types\x1aL\n\x0bGetSubtypes\x1a\x05\n\x03Req\x1a\x36\n\x07ResPart\x12+\n\x05types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05types\x1aT\n\x13GetSubtypesExplicit\x1a\x05\n\x03Req\x1a\x36\n\x07ResPart\x12+\n\x05types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x05types\"a\n\x08\x45ncoding\x12\x0e\n\nTHING_TYPE\x10\x00\x12\x0f\n\x0b\x45NTITY_TYPE\x10\x01\x12\x11\n\rRELATION_TYPE\x10\x02\x12\x12\n\x0e\x41TTRIBUTE_TYPE\x10\x03\x12\r\n\tROLE_TYPE\x10\x04\"\xc6\x01\n\x08RoleType\x1a\x62\n\x10GetRelationTypes\x1a\x05\n\x03Req\x1aG\n\x07ResPart\x12<\n\x0erelation_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\rrelationTypes\x1aV\n\nGetPlayers\x1a\x05\n\x03Req\x1a\x41\n\x07ResPart\x12\x36\n\x0bthing_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\nthingTypes\"\x93\r\n\tThingType\x1a\x1b\n\x0bSetAbstract\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1a\x1d\n\rUnsetAbstract\x1a\x05\n\x03Req\x1a\x05\n\x03Res\x1aP\n\x0cGetInstances\x1a\x05\n\x03Req\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\x1aX\n\x14GetInstancesExplicit\x1a\x05\n\x03Req\x1a\x39\n\x07ResPart\x12.\n\x06things\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\x06things\x1a\xcd\x01\n\x07GetOwns\x1aw\n\x03Req\x12I\n\nvalue_type\x18\x01 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeH\x00R\tvalueType\x12\x1b\n\tkeys_only\x18\x03 \x01(\x08R\x08keysOnlyB\x08\n\x06\x66ilter\x1aI\n\x07ResPart\x12>\n\x0f\x61ttribute_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x0e\x61ttributeTypes\x1a\xd5\x01\n\x0fGetOwnsExplicit\x1aw\n\x03Req\x12I\n\nvalue_type\x18\x01 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeH\x00R\tvalueType\x12\x1b\n\tkeys_only\x18\x03 \x01(\x08R\x08keysOnlyB\x08\n\x06\x66ilter\x1aI\n\x07ResPart\x12>\n\x0f\x61ttribute_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x0e\x61ttributeTypes\x1a\xa6\x01\n\x11GetOwnsOverridden\x1a\x43\n\x03Req\x12<\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\rattributeType\x1aL\n\x03Res\x12>\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\rattributeTypeB\x05\n\x03res\x1a\xbd\x01\n\x07SetOwns\x1a\xaa\x01\n\x03Req\x12<\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\rattributeType\x12@\n\x0foverridden_type\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x0eoverriddenType\x12\x15\n\x06is_key\x18\x03 \x01(\x08R\x05isKeyB\x0c\n\noverridden\x1a\x05\n\x03Res\x1aW\n\tUnsetOwns\x1a\x43\n\x03Req\x12<\n\x0e\x61ttribute_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\rattributeType\x1a\x05\n\x03Res\x1aR\n\x08GetPlays\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1aZ\n\x10GetPlaysExplicit\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a\x93\x01\n\x12GetPlaysOverridden\x1a\x39\n\x03Req\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x1a\x42\n\x03Res\x12\x34\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x08roleTypeB\x05\n\x03res\x1a\x9d\x01\n\x08SetPlays\x1a\x89\x01\n\x03Req\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x12@\n\x0foverridden_type\x18\x02 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x0eoverriddenTypeB\x0c\n\noverridden\x1a\x05\n\x03Res\x1aN\n\nUnsetPlays\x1a\x39\n\x03Req\x12\x32\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeR\x08roleType\x1a\x05\n\x03Res\"T\n\nEntityType\x1a\x46\n\x06\x43reate\x1a\x05\n\x03Req\x1a\x35\n\x03Res\x12.\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x06\x65ntity\"\xa4\x05\n\x0cRelationType\x1aJ\n\x06\x43reate\x1a\x05\n\x03Req\x1a\x39\n\x03Res\x12\x32\n\x08relation\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\x08relation\x1aT\n\nGetRelates\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1a\\\n\x12GetRelatesExplicit\x1a\x05\n\x03Req\x1a?\n\x07ResPart\x12\x34\n\nrole_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\troleTypes\x1az\n\x16GetRelatesForRoleLabel\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x43\n\x03Res\x12\x34\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x08roleTypeB\x06\n\x04role\x1aw\n\x14GetRelatesOverridden\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x42\n\x03Res\x12\x34\n\trole_type\x18\x01 \x01(\x0b\x32\x15.typedb.protocol.TypeH\x00R\x08roleTypeB\x05\n\x03res\x1ak\n\nSetRelates\x1aV\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12+\n\x10overridden_label\x18\x02 \x01(\tH\x00R\x0foverriddenLabelB\x0c\n\noverridden\x1a\x05\n\x03Res\x1a\x32\n\x0cUnsetRelates\x1a\x1b\n\x03Req\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x1a\x05\n\x03Res\"\xa3\x08\n\rAttributeType\x1a\x81\x01\n\x03Put\x1a=\n\x03Req\x12\x36\n\x05value\x18\x01 \x01(\x0b\x32 .typedb.protocol.Attribute.ValueR\x05value\x1a;\n\x03Res\x12\x34\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingR\tattribute\x1a\x8a\x01\n\x03Get\x1a=\n\x03Req\x12\x36\n\x05value\x18\x01 \x01(\x0b\x32 .typedb.protocol.Attribute.ValueR\x05value\x1a\x44\n\x03Res\x12\x36\n\tattribute\x18\x01 \x01(\x0b\x32\x16.typedb.protocol.ThingH\x00R\tattributeB\x05\n\x03res\x1ap\n\tGetOwners\x1a \n\x03Req\x12\x19\n\x08only_key\x18\x01 \x01(\x08R\x07onlyKey\x1a\x41\n\x07ResPart\x12\x36\n\x0bthing_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\nthingTypes\x1ax\n\x11GetOwnersExplicit\x1a \n\x03Req\x12\x19\n\x08only_key\x18\x01 \x01(\x08R\x07onlyKey\x1a\x41\n\x07ResPart\x12\x36\n\x0bthing_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\nthingTypes\x1a.\n\x08GetRegex\x1a\x05\n\x03Req\x1a\x1b\n\x03Res\x12\x14\n\x05regex\x18\x01 \x01(\tR\x05regex\x1a.\n\x08SetRegex\x1a\x1b\n\x03Req\x12\x14\n\x05regex\x18\x01 \x01(\tR\x05regex\x1a\x05\n\x03Res\x1a\xb1\x01\n\x0bGetSubtypes\x1aW\n\x03Req\x12I\n\nvalue_type\x18\x01 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeH\x00R\tvalueTypeB\x05\n\x03req\x1aI\n\x07ResPart\x12>\n\x0f\x61ttribute_types\x18\x01 \x03(\x0b\x32\x15.typedb.protocol.TypeR\x0e\x61ttributeTypes\x1a\xaa\x01\n\x0cGetInstances\x1aW\n\x03Req\x12I\n\nvalue_type\x18\x01 \x01(\x0e\x32(.typedb.protocol.AttributeType.ValueTypeH\x00R\tvalueTypeB\x05\n\x03req\x1a\x41\n\x07ResPart\x12\x36\n\nattributes\x18\x01 \x03(\x0b\x32\x16.typedb.protocol.ThingR\nattributes\"T\n\tValueType\x12\n\n\x06OBJECT\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\x08\n\x04LONG\x10\x02\x12\n\n\x06\x44OUBLE\x10\x03\x12\n\n\x06STRING\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05\x42+\n\x1b\x63om.vaticle.typedb.protocolB\x0c\x43onceptProtob\x06proto3')
 )
 
 
 
 _TYPE_ENCODING = _descriptor.EnumDescriptor(
   name='Encoding',
   full_name='typedb.protocol.Type.Encoding',
@@ -49,16 +49,16 @@
     _descriptor.EnumValueDescriptor(
       name='ROLE_TYPE', index=4, number=4,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=13313,
-  serialized_end=13410,
+  serialized_start=15862,
+  serialized_end=15959,
 )
 _sym_db.RegisterEnumDescriptor(_TYPE_ENCODING)
 
 _ATTRIBUTETYPE_VALUETYPE = _descriptor.EnumDescriptor(
   name='ValueType',
   full_name='typedb.protocol.AttributeType.ValueType',
   filename=None,
@@ -87,16 +87,16 @@
     _descriptor.EnumValueDescriptor(
       name='DATETIME', index=5, number=5,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=15914,
-  serialized_end=15998,
+  serialized_start=19589,
+  serialized_end=19673,
 )
 _sym_db.RegisterEnumDescriptor(_ATTRIBUTETYPE_VALUETYPE)
 
 
 _CONCEPTMANAGER_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.ConceptManager.Req',
@@ -2277,167 +2277,230 @@
       name='type_get_subtypes_req', full_name='typedb.protocol.Type.Req.type_get_subtypes_req', index=8,
       number=106, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='typeGetSubtypesReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='role_type_get_relation_types_req', full_name='typedb.protocol.Type.Req.role_type_get_relation_types_req', index=9,
+      name='type_get_subtypes_explicit_req', full_name='typedb.protocol.Type.Req.type_get_subtypes_explicit_req', index=9,
+      number=107, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='typeGetSubtypesExplicitReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='role_type_get_relation_types_req', full_name='typedb.protocol.Type.Req.role_type_get_relation_types_req', index=10,
       number=200, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='roleTypeGetRelationTypesReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='role_type_get_players_req', full_name='typedb.protocol.Type.Req.role_type_get_players_req', index=10,
+      name='role_type_get_players_req', full_name='typedb.protocol.Type.Req.role_type_get_players_req', index=11,
       number=201, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='roleTypeGetPlayersReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_get_instances_req', full_name='typedb.protocol.Type.Req.thing_type_get_instances_req', index=11,
+      name='thing_type_get_instances_req', full_name='typedb.protocol.Type.Req.thing_type_get_instances_req', index=12,
       number=300, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeGetInstancesReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_set_abstract_req', full_name='typedb.protocol.Type.Req.thing_type_set_abstract_req', index=12,
+      name='thing_type_get_instances_explicit_req', full_name='typedb.protocol.Type.Req.thing_type_get_instances_explicit_req', index=13,
+      number=309, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetInstancesExplicitReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_set_abstract_req', full_name='typedb.protocol.Type.Req.thing_type_set_abstract_req', index=14,
       number=301, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeSetAbstractReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_unset_abstract_req', full_name='typedb.protocol.Type.Req.thing_type_unset_abstract_req', index=13,
+      name='thing_type_unset_abstract_req', full_name='typedb.protocol.Type.Req.thing_type_unset_abstract_req', index=15,
       number=302, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeUnsetAbstractReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_get_owns_req', full_name='typedb.protocol.Type.Req.thing_type_get_owns_req', index=14,
+      name='thing_type_get_owns_req', full_name='typedb.protocol.Type.Req.thing_type_get_owns_req', index=16,
       number=303, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeGetOwnsReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_set_owns_req', full_name='typedb.protocol.Type.Req.thing_type_set_owns_req', index=15,
+      name='thing_type_get_owns_explicit_req', full_name='typedb.protocol.Type.Req.thing_type_get_owns_explicit_req', index=17,
+      number=310, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetOwnsExplicitReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_get_owns_overridden_req', full_name='typedb.protocol.Type.Req.thing_type_get_owns_overridden_req', index=18,
+      number=311, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetOwnsOverriddenReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_set_owns_req', full_name='typedb.protocol.Type.Req.thing_type_set_owns_req', index=19,
       number=304, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeSetOwnsReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_unset_owns_req', full_name='typedb.protocol.Type.Req.thing_type_unset_owns_req', index=16,
+      name='thing_type_unset_owns_req', full_name='typedb.protocol.Type.Req.thing_type_unset_owns_req', index=20,
       number=305, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeUnsetOwnsReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_get_plays_req', full_name='typedb.protocol.Type.Req.thing_type_get_plays_req', index=17,
+      name='thing_type_get_plays_req', full_name='typedb.protocol.Type.Req.thing_type_get_plays_req', index=21,
       number=306, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeGetPlaysReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_set_plays_req', full_name='typedb.protocol.Type.Req.thing_type_set_plays_req', index=18,
+      name='thing_type_get_plays_explicit_req', full_name='typedb.protocol.Type.Req.thing_type_get_plays_explicit_req', index=22,
+      number=312, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetPlaysExplicitReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_get_plays_overridden_req', full_name='typedb.protocol.Type.Req.thing_type_get_plays_overridden_req', index=23,
+      number=313, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetPlaysOverriddenReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_set_plays_req', full_name='typedb.protocol.Type.Req.thing_type_set_plays_req', index=24,
       number=307, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeSetPlaysReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_unset_plays_req', full_name='typedb.protocol.Type.Req.thing_type_unset_plays_req', index=19,
+      name='thing_type_unset_plays_req', full_name='typedb.protocol.Type.Req.thing_type_unset_plays_req', index=25,
       number=308, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeUnsetPlaysReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='entity_type_create_req', full_name='typedb.protocol.Type.Req.entity_type_create_req', index=20,
+      name='entity_type_create_req', full_name='typedb.protocol.Type.Req.entity_type_create_req', index=26,
       number=400, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='entityTypeCreateReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_create_req', full_name='typedb.protocol.Type.Req.relation_type_create_req', index=21,
+      name='relation_type_create_req', full_name='typedb.protocol.Type.Req.relation_type_create_req', index=27,
       number=500, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeCreateReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_get_relates_for_role_label_req', full_name='typedb.protocol.Type.Req.relation_type_get_relates_for_role_label_req', index=22,
+      name='relation_type_get_relates_req', full_name='typedb.protocol.Type.Req.relation_type_get_relates_req', index=28,
+      number=502, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='relationTypeGetRelatesReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='relation_type_get_relates_explicit_req', full_name='typedb.protocol.Type.Req.relation_type_get_relates_explicit_req', index=29,
+      number=505, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='relationTypeGetRelatesExplicitReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='relation_type_get_relates_for_role_label_req', full_name='typedb.protocol.Type.Req.relation_type_get_relates_for_role_label_req', index=30,
       number=501, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeGetRelatesForRoleLabelReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_get_relates_req', full_name='typedb.protocol.Type.Req.relation_type_get_relates_req', index=23,
-      number=502, type=11, cpp_type=10, label=1,
+      name='relation_type_get_relates_overridden_req', full_name='typedb.protocol.Type.Req.relation_type_get_relates_overridden_req', index=31,
+      number=506, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='relationTypeGetRelatesReq', file=DESCRIPTOR),
+      serialized_options=None, json_name='relationTypeGetRelatesOverriddenReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_set_relates_req', full_name='typedb.protocol.Type.Req.relation_type_set_relates_req', index=24,
+      name='relation_type_set_relates_req', full_name='typedb.protocol.Type.Req.relation_type_set_relates_req', index=32,
       number=503, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeSetRelatesReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_unset_relates_req', full_name='typedb.protocol.Type.Req.relation_type_unset_relates_req', index=25,
+      name='relation_type_unset_relates_req', full_name='typedb.protocol.Type.Req.relation_type_unset_relates_req', index=33,
       number=504, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeUnsetRelatesReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_put_req', full_name='typedb.protocol.Type.Req.attribute_type_put_req', index=26,
+      name='attribute_type_put_req', full_name='typedb.protocol.Type.Req.attribute_type_put_req', index=34,
       number=600, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypePutReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_get_req', full_name='typedb.protocol.Type.Req.attribute_type_get_req', index=27,
+      name='attribute_type_get_req', full_name='typedb.protocol.Type.Req.attribute_type_get_req', index=35,
       number=601, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeGetReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_get_regex_req', full_name='typedb.protocol.Type.Req.attribute_type_get_regex_req', index=28,
+      name='attribute_type_get_regex_req', full_name='typedb.protocol.Type.Req.attribute_type_get_regex_req', index=36,
       number=602, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeGetRegexReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_set_regex_req', full_name='typedb.protocol.Type.Req.attribute_type_set_regex_req', index=29,
+      name='attribute_type_set_regex_req', full_name='typedb.protocol.Type.Req.attribute_type_set_regex_req', index=37,
       number=603, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeSetRegexReq', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_get_owners_req', full_name='typedb.protocol.Type.Req.attribute_type_get_owners_req', index=30,
+      name='attribute_type_get_owners_req', full_name='typedb.protocol.Type.Req.attribute_type_get_owners_req', index=38,
       number=604, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeGetOwnersReq', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='attribute_type_get_owners_explicit_req', full_name='typedb.protocol.Type.Req.attribute_type_get_owners_explicit_req', index=39,
+      number=605, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='attributeTypeGetOwnersExplicitReq', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -2446,15 +2509,15 @@
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='req', full_name='typedb.protocol.Type.Req.req',
       index=0, containing_type=None, fields=[]),
   ],
   serialized_start=6608,
-  serialized_end=9691,
+  serialized_end=10882,
 )
 
 _TYPE_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.Type.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -2506,99 +2569,120 @@
       name='thing_type_unset_abstract_res', full_name='typedb.protocol.Type.Res.thing_type_unset_abstract_res', index=6,
       number=301, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeUnsetAbstractRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_set_owns_res', full_name='typedb.protocol.Type.Res.thing_type_set_owns_res', index=7,
+      name='thing_type_get_owns_overridden_res', full_name='typedb.protocol.Type.Res.thing_type_get_owns_overridden_res', index=7,
+      number=306, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetOwnsOverriddenRes', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_set_owns_res', full_name='typedb.protocol.Type.Res.thing_type_set_owns_res', index=8,
       number=302, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeSetOwnsRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_unset_owns_res', full_name='typedb.protocol.Type.Res.thing_type_unset_owns_res', index=8,
+      name='thing_type_unset_owns_res', full_name='typedb.protocol.Type.Res.thing_type_unset_owns_res', index=9,
       number=303, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeUnsetOwnsRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_set_plays_res', full_name='typedb.protocol.Type.Res.thing_type_set_plays_res', index=9,
+      name='thing_type_get_plays_overridden_res', full_name='typedb.protocol.Type.Res.thing_type_get_plays_overridden_res', index=10,
+      number=307, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetPlaysOverriddenRes', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_set_plays_res', full_name='typedb.protocol.Type.Res.thing_type_set_plays_res', index=11,
       number=304, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeSetPlaysRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_unset_plays_res', full_name='typedb.protocol.Type.Res.thing_type_unset_plays_res', index=10,
+      name='thing_type_unset_plays_res', full_name='typedb.protocol.Type.Res.thing_type_unset_plays_res', index=12,
       number=305, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeUnsetPlaysRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='entity_type_create_res', full_name='typedb.protocol.Type.Res.entity_type_create_res', index=11,
+      name='entity_type_create_res', full_name='typedb.protocol.Type.Res.entity_type_create_res', index=13,
       number=400, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='entityTypeCreateRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_create_res', full_name='typedb.protocol.Type.Res.relation_type_create_res', index=12,
+      name='relation_type_create_res', full_name='typedb.protocol.Type.Res.relation_type_create_res', index=14,
       number=500, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeCreateRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_get_relates_for_role_label_res', full_name='typedb.protocol.Type.Res.relation_type_get_relates_for_role_label_res', index=13,
+      name='relation_type_get_relates_for_role_label_res', full_name='typedb.protocol.Type.Res.relation_type_get_relates_for_role_label_res', index=15,
       number=501, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeGetRelatesForRoleLabelRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_set_relates_res', full_name='typedb.protocol.Type.Res.relation_type_set_relates_res', index=14,
+      name='relation_type_get_relates_overridden_res', full_name='typedb.protocol.Type.Res.relation_type_get_relates_overridden_res', index=16,
+      number=504, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='relationTypeGetRelatesOverriddenRes', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='relation_type_set_relates_res', full_name='typedb.protocol.Type.Res.relation_type_set_relates_res', index=17,
       number=502, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeSetRelatesRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_unset_relates_res', full_name='typedb.protocol.Type.Res.relation_type_unset_relates_res', index=15,
+      name='relation_type_unset_relates_res', full_name='typedb.protocol.Type.Res.relation_type_unset_relates_res', index=18,
       number=503, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeUnsetRelatesRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_put_res', full_name='typedb.protocol.Type.Res.attribute_type_put_res', index=16,
+      name='attribute_type_put_res', full_name='typedb.protocol.Type.Res.attribute_type_put_res', index=19,
       number=600, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypePutRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_get_res', full_name='typedb.protocol.Type.Res.attribute_type_get_res', index=17,
+      name='attribute_type_get_res', full_name='typedb.protocol.Type.Res.attribute_type_get_res', index=20,
       number=601, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeGetRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_get_regex_res', full_name='typedb.protocol.Type.Res.attribute_type_get_regex_res', index=18,
+      name='attribute_type_get_regex_res', full_name='typedb.protocol.Type.Res.attribute_type_get_regex_res', index=21,
       number=602, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeGetRegexRes', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_set_regex_res', full_name='typedb.protocol.Type.Res.attribute_type_set_regex_res', index=19,
+      name='attribute_type_set_regex_res', full_name='typedb.protocol.Type.Res.attribute_type_set_regex_res', index=22,
       number=603, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeSetRegexRes', file=DESCRIPTOR),
   ],
   extensions=[
@@ -2611,16 +2695,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='res', full_name='typedb.protocol.Type.Res.res',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=9694,
-  serialized_end=11779,
+  serialized_start=10885,
+  serialized_end=13377,
 )
 
 _TYPE_RESPART = _descriptor.Descriptor(
   name='ResPart',
   full_name='typedb.protocol.Type.ResPart',
   filename=None,
   file=DESCRIPTOR,
@@ -2637,62 +2721,104 @@
       name='type_get_subtypes_res_part', full_name='typedb.protocol.Type.ResPart.type_get_subtypes_res_part', index=1,
       number=101, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='typeGetSubtypesResPart', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='role_type_get_relation_types_res_part', full_name='typedb.protocol.Type.ResPart.role_type_get_relation_types_res_part', index=2,
+      name='type_get_subtypes_explicit_res_part', full_name='typedb.protocol.Type.ResPart.type_get_subtypes_explicit_res_part', index=2,
+      number=102, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='typeGetSubtypesExplicitResPart', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='role_type_get_relation_types_res_part', full_name='typedb.protocol.Type.ResPart.role_type_get_relation_types_res_part', index=3,
       number=200, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='roleTypeGetRelationTypesResPart', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='role_type_get_players_res_part', full_name='typedb.protocol.Type.ResPart.role_type_get_players_res_part', index=3,
+      name='role_type_get_players_res_part', full_name='typedb.protocol.Type.ResPart.role_type_get_players_res_part', index=4,
       number=201, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='roleTypeGetPlayersResPart', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_get_instances_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_instances_res_part', index=4,
+      name='thing_type_get_instances_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_instances_res_part', index=5,
       number=300, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeGetInstancesResPart', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_get_owns_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_owns_res_part', index=5,
+      name='thing_type_get_instances_explicit_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_instances_explicit_res_part', index=6,
+      number=303, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetInstancesExplicitResPart', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_get_owns_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_owns_res_part', index=7,
       number=301, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeGetOwnsResPart', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='thing_type_get_plays_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_plays_res_part', index=6,
+      name='thing_type_get_owns_explicit_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_owns_explicit_res_part', index=8,
+      number=304, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetOwnsExplicitResPart', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='thing_type_get_plays_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_plays_res_part', index=9,
       number=302, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='thingTypeGetPlaysResPart', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='relation_type_get_relates_res_part', full_name='typedb.protocol.Type.ResPart.relation_type_get_relates_res_part', index=7,
+      name='thing_type_get_plays_explicit_res_part', full_name='typedb.protocol.Type.ResPart.thing_type_get_plays_explicit_res_part', index=10,
+      number=305, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypeGetPlaysExplicitResPart', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='relation_type_get_relates_res_part', full_name='typedb.protocol.Type.ResPart.relation_type_get_relates_res_part', index=11,
       number=500, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='relationTypeGetRelatesResPart', file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='attribute_type_get_owners_res_part', full_name='typedb.protocol.Type.ResPart.attribute_type_get_owners_res_part', index=8,
+      name='relation_type_get_relates_explicit_res_part', full_name='typedb.protocol.Type.ResPart.relation_type_get_relates_explicit_res_part', index=12,
+      number=501, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='relationTypeGetRelatesExplicitResPart', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='attribute_type_get_owners_res_part', full_name='typedb.protocol.Type.ResPart.attribute_type_get_owners_res_part', index=13,
       number=600, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='attributeTypeGetOwnersResPart', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='attribute_type_get_owners_explicit_res_part', full_name='typedb.protocol.Type.ResPart.attribute_type_get_owners_explicit_res_part', index=14,
+      number=601, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='attributeTypeGetOwnersExplicitResPart', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -2700,16 +2826,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='res', full_name='typedb.protocol.Type.ResPart.res',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=11782,
-  serialized_end=12870,
+  serialized_start=13380,
+  serialized_end=15333,
 )
 
 _TYPE_DELETE_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.Type.Delete.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -2845,16 +2971,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12896,
-  serialized_end=12942,
+  serialized_start=15359,
+  serialized_end=15405,
 )
 
 _TYPE_ISABSTRACT_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.Type.IsAbstract.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -2898,16 +3024,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12965,
-  serialized_end=12998,
+  serialized_start=15428,
+  serialized_end=15461,
 )
 
 _TYPE_ISABSTRACT = _descriptor.Descriptor(
   name='IsAbstract',
   full_name='typedb.protocol.Type.IsAbstract',
   filename=None,
   file=DESCRIPTOR,
@@ -2921,16 +3047,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12944,
-  serialized_end=12998,
+  serialized_start=15407,
+  serialized_end=15461,
 )
 
 _TYPE_GETSUPERTYPE_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.Type.GetSupertype.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -2977,16 +3103,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='res', full_name='typedb.protocol.Type.GetSupertype.Res.res',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=13023,
-  serialized_end=13080,
+  serialized_start=15486,
+  serialized_end=15543,
 )
 
 _TYPE_GETSUPERTYPE = _descriptor.Descriptor(
   name='GetSupertype',
   full_name='typedb.protocol.Type.GetSupertype',
   filename=None,
   file=DESCRIPTOR,
@@ -3000,16 +3126,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13000,
-  serialized_end=13080,
+  serialized_start=15463,
+  serialized_end=15543,
 )
 
 _TYPE_SETSUPERTYPE_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.Type.SetSupertype.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3030,16 +3156,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13098,
-  serialized_end=13146,
+  serialized_start=15561,
+  serialized_end=15609,
 )
 
 _TYPE_SETSUPERTYPE_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.Type.SetSupertype.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -3076,16 +3202,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13082,
-  serialized_end=13153,
+  serialized_start=15545,
+  serialized_end=15616,
 )
 
 _TYPE_GETSUPERTYPES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.Type.GetSupertypes.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3129,16 +3255,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13179,
-  serialized_end=13233,
+  serialized_start=15642,
+  serialized_end=15696,
 )
 
 _TYPE_GETSUPERTYPES = _descriptor.Descriptor(
   name='GetSupertypes',
   full_name='typedb.protocol.Type.GetSupertypes',
   filename=None,
   file=DESCRIPTOR,
@@ -3152,16 +3278,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13155,
-  serialized_end=13233,
+  serialized_start=15618,
+  serialized_end=15696,
 )
 
 _TYPE_GETSUBTYPES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.Type.GetSubtypes.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3205,16 +3331,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13179,
-  serialized_end=13233,
+  serialized_start=15642,
+  serialized_end=15696,
 )
 
 _TYPE_GETSUBTYPES = _descriptor.Descriptor(
   name='GetSubtypes',
   full_name='typedb.protocol.Type.GetSubtypes',
   filename=None,
   file=DESCRIPTOR,
@@ -3228,16 +3354,92 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13235,
-  serialized_end=13311,
+  serialized_start=15698,
+  serialized_end=15774,
+)
+
+_TYPE_GETSUBTYPESEXPLICIT_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.Type.GetSubtypesExplicit.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=61,
+  serialized_end=66,
+)
+
+_TYPE_GETSUBTYPESEXPLICIT_RESPART = _descriptor.Descriptor(
+  name='ResPart',
+  full_name='typedb.protocol.Type.GetSubtypesExplicit.ResPart',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='types', full_name='typedb.protocol.Type.GetSubtypesExplicit.ResPart.types', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='types', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=15642,
+  serialized_end=15696,
+)
+
+_TYPE_GETSUBTYPESEXPLICIT = _descriptor.Descriptor(
+  name='GetSubtypesExplicit',
+  full_name='typedb.protocol.Type.GetSubtypesExplicit',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_TYPE_GETSUBTYPESEXPLICIT_REQ, _TYPE_GETSUBTYPESEXPLICIT_RESPART, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=15776,
+  serialized_end=15860,
 )
 
 _TYPE = _descriptor.Descriptor(
   name='Type',
   full_name='typedb.protocol.Type',
   filename=None,
   file=DESCRIPTOR,
@@ -3277,26 +3479,26 @@
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='root', file=DESCRIPTOR),
   ],
   extensions=[
   ],
-  nested_types=[_TYPE_REQ, _TYPE_RES, _TYPE_RESPART, _TYPE_DELETE, _TYPE_SETLABEL, _TYPE_ISABSTRACT, _TYPE_GETSUPERTYPE, _TYPE_SETSUPERTYPE, _TYPE_GETSUPERTYPES, _TYPE_GETSUBTYPES, ],
+  nested_types=[_TYPE_REQ, _TYPE_RES, _TYPE_RESPART, _TYPE_DELETE, _TYPE_SETLABEL, _TYPE_ISABSTRACT, _TYPE_GETSUPERTYPE, _TYPE_SETSUPERTYPE, _TYPE_GETSUPERTYPES, _TYPE_GETSUBTYPES, _TYPE_GETSUBTYPESEXPLICIT, ],
   enum_types=[
     _TYPE_ENCODING,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=6402,
-  serialized_end=13410,
+  serialized_end=15959,
 )
 
 
 _ROLETYPE_GETRELATIONTYPES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.RoleType.GetRelationTypes.Req',
   filename=None,
@@ -3341,16 +3543,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13452,
-  serialized_end=13523,
+  serialized_start=16001,
+  serialized_end=16072,
 )
 
 _ROLETYPE_GETRELATIONTYPES = _descriptor.Descriptor(
   name='GetRelationTypes',
   full_name='typedb.protocol.RoleType.GetRelationTypes',
   filename=None,
   file=DESCRIPTOR,
@@ -3364,16 +3566,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13425,
-  serialized_end=13523,
+  serialized_start=15974,
+  serialized_end=16072,
 )
 
 _ROLETYPE_GETPLAYERS_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.RoleType.GetPlayers.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3417,16 +3619,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13546,
-  serialized_end=13611,
+  serialized_start=16095,
+  serialized_end=16160,
 )
 
 _ROLETYPE_GETPLAYERS = _descriptor.Descriptor(
   name='GetPlayers',
   full_name='typedb.protocol.RoleType.GetPlayers',
   filename=None,
   file=DESCRIPTOR,
@@ -3440,16 +3642,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13525,
-  serialized_end=13611,
+  serialized_start=16074,
+  serialized_end=16160,
 )
 
 _ROLETYPE = _descriptor.Descriptor(
   name='RoleType',
   full_name='typedb.protocol.RoleType',
   filename=None,
   file=DESCRIPTOR,
@@ -3463,16 +3665,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13413,
-  serialized_end=13611,
+  serialized_start=15962,
+  serialized_end=16160,
 )
 
 
 _THINGTYPE_SETABSTRACT_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.ThingType.SetAbstract.Req',
   filename=None,
@@ -3533,16 +3735,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13627,
-  serialized_end=13654,
+  serialized_start=16176,
+  serialized_end=16203,
 )
 
 _THINGTYPE_UNSETABSTRACT_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.ThingType.UnsetAbstract.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3602,16 +3804,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13656,
-  serialized_end=13685,
+  serialized_start=16205,
+  serialized_end=16234,
 )
 
 _THINGTYPE_GETINSTANCES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.ThingType.GetInstances.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3678,16 +3880,92 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13687,
-  serialized_end=13767,
+  serialized_start=16236,
+  serialized_end=16316,
+)
+
+_THINGTYPE_GETINSTANCESEXPLICIT_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.ThingType.GetInstancesExplicit.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=61,
+  serialized_end=66,
+)
+
+_THINGTYPE_GETINSTANCESEXPLICIT_RESPART = _descriptor.Descriptor(
+  name='ResPart',
+  full_name='typedb.protocol.ThingType.GetInstancesExplicit.ResPart',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='things', full_name='typedb.protocol.ThingType.GetInstancesExplicit.ResPart.things', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='things', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=5655,
+  serialized_end=5712,
+)
+
+_THINGTYPE_GETINSTANCESEXPLICIT = _descriptor.Descriptor(
+  name='GetInstancesExplicit',
+  full_name='typedb.protocol.ThingType.GetInstancesExplicit',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_THINGTYPE_GETINSTANCESEXPLICIT_REQ, _THINGTYPE_GETINSTANCESEXPLICIT_RESPART, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=16318,
+  serialized_end=16406,
 )
 
 _THINGTYPE_GETOWNS_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.ThingType.GetOwns.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3718,16 +3996,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='filter', full_name='typedb.protocol.ThingType.GetOwns.Req.filter',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=13781,
-  serialized_end=13900,
+  serialized_start=16420,
+  serialized_end=16539,
 )
 
 _THINGTYPE_GETOWNS_RESPART = _descriptor.Descriptor(
   name='ResPart',
   full_name='typedb.protocol.ThingType.GetOwns.ResPart',
   filename=None,
   file=DESCRIPTOR,
@@ -3748,16 +4026,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13902,
-  serialized_end=13975,
+  serialized_start=16541,
+  serialized_end=16614,
 )
 
 _THINGTYPE_GETOWNS = _descriptor.Descriptor(
   name='GetOwns',
   full_name='typedb.protocol.ThingType.GetOwns',
   filename=None,
   file=DESCRIPTOR,
@@ -3771,92 +4049,195 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13770,
-  serialized_end=13975,
+  serialized_start=16409,
+  serialized_end=16614,
 )
 
-_THINGTYPE_GETPLAYS_REQ = _descriptor.Descriptor(
+_THINGTYPE_GETOWNSEXPLICIT_REQ = _descriptor.Descriptor(
   name='Req',
-  full_name='typedb.protocol.ThingType.GetPlays.Req',
+  full_name='typedb.protocol.ThingType.GetOwnsExplicit.Req',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
+    _descriptor.FieldDescriptor(
+      name='value_type', full_name='typedb.protocol.ThingType.GetOwnsExplicit.Req.value_type', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='valueType', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='keys_only', full_name='typedb.protocol.ThingType.GetOwnsExplicit.Req.keys_only', index=1,
+      number=3, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='keysOnly', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
+    _descriptor.OneofDescriptor(
+      name='filter', full_name='typedb.protocol.ThingType.GetOwnsExplicit.Req.filter',
+      index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=61,
-  serialized_end=66,
+  serialized_start=16420,
+  serialized_end=16539,
 )
 
-_THINGTYPE_GETPLAYS_RESPART = _descriptor.Descriptor(
+_THINGTYPE_GETOWNSEXPLICIT_RESPART = _descriptor.Descriptor(
   name='ResPart',
-  full_name='typedb.protocol.ThingType.GetPlays.ResPart',
+  full_name='typedb.protocol.ThingType.GetOwnsExplicit.ResPart',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='roles', full_name='typedb.protocol.ThingType.GetPlays.ResPart.roles', index=0,
+      name='attribute_types', full_name='typedb.protocol.ThingType.GetOwnsExplicit.ResPart.attribute_types', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='roles', file=DESCRIPTOR),
+      serialized_options=None, json_name='attributeTypes', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13996,
-  serialized_end=14050,
+  serialized_start=16541,
+  serialized_end=16614,
 )
 
-_THINGTYPE_GETPLAYS = _descriptor.Descriptor(
-  name='GetPlays',
-  full_name='typedb.protocol.ThingType.GetPlays',
+_THINGTYPE_GETOWNSEXPLICIT = _descriptor.Descriptor(
+  name='GetOwnsExplicit',
+  full_name='typedb.protocol.ThingType.GetOwnsExplicit',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
-  nested_types=[_THINGTYPE_GETPLAYS_REQ, _THINGTYPE_GETPLAYS_RESPART, ],
+  nested_types=[_THINGTYPE_GETOWNSEXPLICIT_REQ, _THINGTYPE_GETOWNSEXPLICIT_RESPART, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=16617,
+  serialized_end=16830,
+)
+
+_THINGTYPE_GETOWNSOVERRIDDEN_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.ThingType.GetOwnsOverridden.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='attribute_type', full_name='typedb.protocol.ThingType.GetOwnsOverridden.Req.attribute_type', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='attributeType', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13977,
-  serialized_end=14050,
+  serialized_start=16854,
+  serialized_end=16921,
+)
+
+_THINGTYPE_GETOWNSOVERRIDDEN_RES = _descriptor.Descriptor(
+  name='Res',
+  full_name='typedb.protocol.ThingType.GetOwnsOverridden.Res',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='attribute_type', full_name='typedb.protocol.ThingType.GetOwnsOverridden.Res.attribute_type', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='attributeType', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='res', full_name='typedb.protocol.ThingType.GetOwnsOverridden.Res.res',
+      index=0, containing_type=None, fields=[]),
+  ],
+  serialized_start=16923,
+  serialized_end=16999,
+)
+
+_THINGTYPE_GETOWNSOVERRIDDEN = _descriptor.Descriptor(
+  name='GetOwnsOverridden',
+  full_name='typedb.protocol.ThingType.GetOwnsOverridden',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_THINGTYPE_GETOWNSOVERRIDDEN_REQ, _THINGTYPE_GETOWNSOVERRIDDEN_RES, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=16833,
+  serialized_end=16999,
 )
 
 _THINGTYPE_SETOWNS_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.ThingType.SetOwns.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -3894,16 +4275,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='overridden', full_name='typedb.protocol.ThingType.SetOwns.Req.overridden',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=14065,
-  serialized_end=14235,
+  serialized_start=17014,
+  serialized_end=17184,
 )
 
 _THINGTYPE_SETOWNS_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.ThingType.SetOwns.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -3940,137 +4321,375 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14053,
-  serialized_end=14242,
+  serialized_start=17002,
+  serialized_end=17191,
 )
 
-_THINGTYPE_SETPLAYS_REQ = _descriptor.Descriptor(
+_THINGTYPE_UNSETOWNS_REQ = _descriptor.Descriptor(
   name='Req',
-  full_name='typedb.protocol.ThingType.SetPlays.Req',
+  full_name='typedb.protocol.ThingType.UnsetOwns.Req',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='role', full_name='typedb.protocol.ThingType.SetPlays.Req.role', index=0,
+      name='attribute_type', full_name='typedb.protocol.ThingType.UnsetOwns.Req.attribute_type', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='role', file=DESCRIPTOR),
+      serialized_options=None, json_name='attributeType', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=16854,
+  serialized_end=16921,
+)
+
+_THINGTYPE_UNSETOWNS_RES = _descriptor.Descriptor(
+  name='Res',
+  full_name='typedb.protocol.ThingType.UnsetOwns.Res',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=572,
+  serialized_end=577,
+)
+
+_THINGTYPE_UNSETOWNS = _descriptor.Descriptor(
+  name='UnsetOwns',
+  full_name='typedb.protocol.ThingType.UnsetOwns',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_THINGTYPE_UNSETOWNS_REQ, _THINGTYPE_UNSETOWNS_RES, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=17193,
+  serialized_end=17280,
+)
+
+_THINGTYPE_GETPLAYS_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.ThingType.GetPlays.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=61,
+  serialized_end=66,
+)
+
+_THINGTYPE_GETPLAYS_RESPART = _descriptor.Descriptor(
+  name='ResPart',
+  full_name='typedb.protocol.ThingType.GetPlays.ResPart',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='role_types', full_name='typedb.protocol.ThingType.GetPlays.ResPart.role_types', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='roleTypes', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=5100,
+  serialized_end=5163,
+)
+
+_THINGTYPE_GETPLAYS = _descriptor.Descriptor(
+  name='GetPlays',
+  full_name='typedb.protocol.ThingType.GetPlays',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_THINGTYPE_GETPLAYS_REQ, _THINGTYPE_GETPLAYS_RESPART, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=17282,
+  serialized_end=17364,
+)
+
+_THINGTYPE_GETPLAYSEXPLICIT_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.ThingType.GetPlaysExplicit.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=61,
+  serialized_end=66,
+)
+
+_THINGTYPE_GETPLAYSEXPLICIT_RESPART = _descriptor.Descriptor(
+  name='ResPart',
+  full_name='typedb.protocol.ThingType.GetPlaysExplicit.ResPart',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='overridden_role', full_name='typedb.protocol.ThingType.SetPlays.Req.overridden_role', index=1,
-      number=2, type=11, cpp_type=10, label=1,
+      name='role_types', full_name='typedb.protocol.ThingType.GetPlaysExplicit.ResPart.role_types', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='roleTypes', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=5100,
+  serialized_end=5163,
+)
+
+_THINGTYPE_GETPLAYSEXPLICIT = _descriptor.Descriptor(
+  name='GetPlaysExplicit',
+  full_name='typedb.protocol.ThingType.GetPlaysExplicit',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_THINGTYPE_GETPLAYSEXPLICIT_REQ, _THINGTYPE_GETPLAYSEXPLICIT_RESPART, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=17366,
+  serialized_end=17456,
+)
+
+_THINGTYPE_GETPLAYSOVERRIDDEN_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.ThingType.GetPlaysOverridden.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='role_type', full_name='typedb.protocol.ThingType.GetPlaysOverridden.Req.role_type', index=0,
+      number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='overriddenRole', file=DESCRIPTOR),
+      serialized_options=None, json_name='roleType', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
-    _descriptor.OneofDescriptor(
-      name='overridden', full_name='typedb.protocol.ThingType.SetPlays.Req.overridden',
-      index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=14258,
-  serialized_end=14386,
+  serialized_start=5334,
+  serialized_end=5391,
 )
 
-_THINGTYPE_SETPLAYS_RES = _descriptor.Descriptor(
+_THINGTYPE_GETPLAYSOVERRIDDEN_RES = _descriptor.Descriptor(
   name='Res',
-  full_name='typedb.protocol.ThingType.SetPlays.Res',
+  full_name='typedb.protocol.ThingType.GetPlaysOverridden.Res',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
+    _descriptor.FieldDescriptor(
+      name='role_type', full_name='typedb.protocol.ThingType.GetPlaysOverridden.Res.role_type', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='roleType', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
+    _descriptor.OneofDescriptor(
+      name='res', full_name='typedb.protocol.ThingType.GetPlaysOverridden.Res.res',
+      index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=572,
-  serialized_end=577,
+  serialized_start=17540,
+  serialized_end=17606,
 )
 
-_THINGTYPE_SETPLAYS = _descriptor.Descriptor(
-  name='SetPlays',
-  full_name='typedb.protocol.ThingType.SetPlays',
+_THINGTYPE_GETPLAYSOVERRIDDEN = _descriptor.Descriptor(
+  name='GetPlaysOverridden',
+  full_name='typedb.protocol.ThingType.GetPlaysOverridden',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
-  nested_types=[_THINGTYPE_SETPLAYS_REQ, _THINGTYPE_SETPLAYS_RES, ],
+  nested_types=[_THINGTYPE_GETPLAYSOVERRIDDEN_REQ, _THINGTYPE_GETPLAYSOVERRIDDEN_RES, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14245,
-  serialized_end=14393,
+  serialized_start=17459,
+  serialized_end=17606,
 )
 
-_THINGTYPE_UNSETOWNS_REQ = _descriptor.Descriptor(
+_THINGTYPE_SETPLAYS_REQ = _descriptor.Descriptor(
   name='Req',
-  full_name='typedb.protocol.ThingType.UnsetOwns.Req',
+  full_name='typedb.protocol.ThingType.SetPlays.Req',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='attribute_type', full_name='typedb.protocol.ThingType.UnsetOwns.Req.attribute_type', index=0,
+      name='role_type', full_name='typedb.protocol.ThingType.SetPlays.Req.role_type', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='attributeType', file=DESCRIPTOR),
+      serialized_options=None, json_name='roleType', file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='overridden_type', full_name='typedb.protocol.ThingType.SetPlays.Req.overridden_type', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='overriddenType', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
+    _descriptor.OneofDescriptor(
+      name='overridden', full_name='typedb.protocol.ThingType.SetPlays.Req.overridden',
+      index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=14065,
-  serialized_end=14132,
+  serialized_start=17622,
+  serialized_end=17759,
 )
 
-_THINGTYPE_UNSETOWNS_RES = _descriptor.Descriptor(
+_THINGTYPE_SETPLAYS_RES = _descriptor.Descriptor(
   name='Res',
-  full_name='typedb.protocol.ThingType.UnsetOwns.Res',
+  full_name='typedb.protocol.ThingType.SetPlays.Res',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
@@ -4083,65 +4702,65 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=572,
   serialized_end=577,
 )
 
-_THINGTYPE_UNSETOWNS = _descriptor.Descriptor(
-  name='UnsetOwns',
-  full_name='typedb.protocol.ThingType.UnsetOwns',
+_THINGTYPE_SETPLAYS = _descriptor.Descriptor(
+  name='SetPlays',
+  full_name='typedb.protocol.ThingType.SetPlays',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
-  nested_types=[_THINGTYPE_UNSETOWNS_REQ, _THINGTYPE_UNSETOWNS_RES, ],
+  nested_types=[_THINGTYPE_SETPLAYS_REQ, _THINGTYPE_SETPLAYS_RES, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14395,
-  serialized_end=14482,
+  serialized_start=17609,
+  serialized_end=17766,
 )
 
 _THINGTYPE_UNSETPLAYS_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.ThingType.UnsetPlays.Req',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='role', full_name='typedb.protocol.ThingType.UnsetPlays.Req.role', index=0,
+      name='role_type', full_name='typedb.protocol.ThingType.UnsetPlays.Req.role_type', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='role', file=DESCRIPTOR),
+      serialized_options=None, json_name='roleType', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14258,
-  serialized_end=14306,
+  serialized_start=5334,
+  serialized_end=5391,
 )
 
 _THINGTYPE_UNSETPLAYS_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.ThingType.UnsetPlays.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -4178,39 +4797,39 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14484,
-  serialized_end=14553,
+  serialized_start=17768,
+  serialized_end=17846,
 )
 
 _THINGTYPE = _descriptor.Descriptor(
   name='ThingType',
   full_name='typedb.protocol.ThingType',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
-  nested_types=[_THINGTYPE_SETABSTRACT, _THINGTYPE_UNSETABSTRACT, _THINGTYPE_GETINSTANCES, _THINGTYPE_GETOWNS, _THINGTYPE_GETPLAYS, _THINGTYPE_SETOWNS, _THINGTYPE_SETPLAYS, _THINGTYPE_UNSETOWNS, _THINGTYPE_UNSETPLAYS, ],
+  nested_types=[_THINGTYPE_SETABSTRACT, _THINGTYPE_UNSETABSTRACT, _THINGTYPE_GETINSTANCES, _THINGTYPE_GETINSTANCESEXPLICIT, _THINGTYPE_GETOWNS, _THINGTYPE_GETOWNSEXPLICIT, _THINGTYPE_GETOWNSOVERRIDDEN, _THINGTYPE_SETOWNS, _THINGTYPE_UNSETOWNS, _THINGTYPE_GETPLAYS, _THINGTYPE_GETPLAYSEXPLICIT, _THINGTYPE_GETPLAYSOVERRIDDEN, _THINGTYPE_SETPLAYS, _THINGTYPE_UNSETPLAYS, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13614,
-  serialized_end=14553,
+  serialized_start=16163,
+  serialized_end=17846,
 )
 
 
 _ENTITYTYPE_CREATE_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.EntityType.Create.Req',
   filename=None,
@@ -4255,16 +4874,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14586,
-  serialized_end=14639,
+  serialized_start=17879,
+  serialized_end=17932,
 )
 
 _ENTITYTYPE_CREATE = _descriptor.Descriptor(
   name='Create',
   full_name='typedb.protocol.EntityType.Create',
   filename=None,
   file=DESCRIPTOR,
@@ -4278,16 +4897,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14569,
-  serialized_end=14639,
+  serialized_start=17862,
+  serialized_end=17932,
 )
 
 _ENTITYTYPE = _descriptor.Descriptor(
   name='EntityType',
   full_name='typedb.protocol.EntityType',
   filename=None,
   file=DESCRIPTOR,
@@ -4301,16 +4920,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14555,
-  serialized_end=14639,
+  serialized_start=17848,
+  serialized_end=17932,
 )
 
 
 _RELATIONTYPE_CREATE_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.RelationType.Create.Req',
   filename=None,
@@ -4355,16 +4974,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14675,
-  serialized_end=14732,
+  serialized_start=17968,
+  serialized_end=18025,
 )
 
 _RELATIONTYPE_CREATE = _descriptor.Descriptor(
   name='Create',
   full_name='typedb.protocol.RelationType.Create',
   filename=None,
   file=DESCRIPTOR,
@@ -4378,16 +4997,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14658,
-  serialized_end=14732,
+  serialized_start=17951,
+  serialized_end=18025,
 )
 
 _RELATIONTYPE_GETRELATES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.RelationType.GetRelates.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -4413,34 +5032,34 @@
   name='ResPart',
   full_name='typedb.protocol.RelationType.GetRelates.ResPart',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='roles', full_name='typedb.protocol.RelationType.GetRelates.ResPart.roles', index=0,
+      name='role_types', full_name='typedb.protocol.RelationType.GetRelates.ResPart.role_types', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='roles', file=DESCRIPTOR),
+      serialized_options=None, json_name='roleTypes', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13996,
-  serialized_end=14050,
+  serialized_start=5100,
+  serialized_end=5163,
 )
 
 _RELATIONTYPE_GETRELATES = _descriptor.Descriptor(
   name='GetRelates',
   full_name='typedb.protocol.RelationType.GetRelates',
   filename=None,
   file=DESCRIPTOR,
@@ -4454,16 +5073,92 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14734,
-  serialized_end=14809,
+  serialized_start=18027,
+  serialized_end=18111,
+)
+
+_RELATIONTYPE_GETRELATESEXPLICIT_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.RelationType.GetRelatesExplicit.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=61,
+  serialized_end=66,
+)
+
+_RELATIONTYPE_GETRELATESEXPLICIT_RESPART = _descriptor.Descriptor(
+  name='ResPart',
+  full_name='typedb.protocol.RelationType.GetRelatesExplicit.ResPart',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='role_types', full_name='typedb.protocol.RelationType.GetRelatesExplicit.ResPart.role_types', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='roleTypes', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=5100,
+  serialized_end=5163,
+)
+
+_RELATIONTYPE_GETRELATESEXPLICIT = _descriptor.Descriptor(
+  name='GetRelatesExplicit',
+  full_name='typedb.protocol.RelationType.GetRelatesExplicit',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_RELATIONTYPE_GETRELATESEXPLICIT_REQ, _RELATIONTYPE_GETRELATESEXPLICIT_RESPART, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=18113,
+  serialized_end=18205,
 )
 
 _RELATIONTYPE_GETRELATESFORROLELABEL_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.RelationType.GetRelatesForRoleLabel.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -4517,16 +5212,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='role', full_name='typedb.protocol.RelationType.GetRelatesForRoleLabel.Res.role',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=14866,
-  serialized_end=14933,
+  serialized_start=18262,
+  serialized_end=18329,
 )
 
 _RELATIONTYPE_GETRELATESFORROLELABEL = _descriptor.Descriptor(
   name='GetRelatesForRoleLabel',
   full_name='typedb.protocol.RelationType.GetRelatesForRoleLabel',
   filename=None,
   file=DESCRIPTOR,
@@ -4540,16 +5235,102 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14811,
-  serialized_end=14933,
+  serialized_start=18207,
+  serialized_end=18329,
+)
+
+_RELATIONTYPE_GETRELATESOVERRIDDEN_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.RelationType.GetRelatesOverridden.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='label', full_name='typedb.protocol.RelationType.GetRelatesOverridden.Req.label', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='label', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1098,
+  serialized_end=1125,
+)
+
+_RELATIONTYPE_GETRELATESOVERRIDDEN_RES = _descriptor.Descriptor(
+  name='Res',
+  full_name='typedb.protocol.RelationType.GetRelatesOverridden.Res',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='role_type', full_name='typedb.protocol.RelationType.GetRelatesOverridden.Res.role_type', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='roleType', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='res', full_name='typedb.protocol.RelationType.GetRelatesOverridden.Res.res',
+      index=0, containing_type=None, fields=[]),
+  ],
+  serialized_start=17540,
+  serialized_end=17606,
+)
+
+_RELATIONTYPE_GETRELATESOVERRIDDEN = _descriptor.Descriptor(
+  name='GetRelatesOverridden',
+  full_name='typedb.protocol.RelationType.GetRelatesOverridden',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_RELATIONTYPE_GETRELATESOVERRIDDEN_REQ, _RELATIONTYPE_GETRELATESOVERRIDDEN_RES, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=18331,
+  serialized_end=18450,
 )
 
 _RELATIONTYPE_SETRELATES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.RelationType.SetRelates.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -4580,16 +5361,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='overridden', full_name='typedb.protocol.RelationType.SetRelates.Req.overridden',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=14949,
-  serialized_end=15035,
+  serialized_start=18466,
+  serialized_end=18552,
 )
 
 _RELATIONTYPE_SETRELATES_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.RelationType.SetRelates.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -4626,16 +5407,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14935,
-  serialized_end=15042,
+  serialized_start=18452,
+  serialized_end=18559,
 )
 
 _RELATIONTYPE_UNSETRELATES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.RelationType.UnsetRelates.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -4702,39 +5483,39 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15044,
-  serialized_end=15094,
+  serialized_start=18561,
+  serialized_end=18611,
 )
 
 _RELATIONTYPE = _descriptor.Descriptor(
   name='RelationType',
   full_name='typedb.protocol.RelationType',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
-  nested_types=[_RELATIONTYPE_CREATE, _RELATIONTYPE_GETRELATES, _RELATIONTYPE_GETRELATESFORROLELABEL, _RELATIONTYPE_SETRELATES, _RELATIONTYPE_UNSETRELATES, ],
+  nested_types=[_RELATIONTYPE_CREATE, _RELATIONTYPE_GETRELATES, _RELATIONTYPE_GETRELATESEXPLICIT, _RELATIONTYPE_GETRELATESFORROLELABEL, _RELATIONTYPE_GETRELATESOVERRIDDEN, _RELATIONTYPE_SETRELATES, _RELATIONTYPE_UNSETRELATES, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14642,
-  serialized_end=15094,
+  serialized_start=17935,
+  serialized_end=18611,
 )
 
 
 _ATTRIBUTETYPE_PUT_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.AttributeType.Put.Req',
   filename=None,
@@ -4756,16 +5537,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15122,
-  serialized_end=15183,
+  serialized_start=18639,
+  serialized_end=18700,
 )
 
 _ATTRIBUTETYPE_PUT_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.AttributeType.Put.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -4786,16 +5567,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15185,
-  serialized_end=15244,
+  serialized_start=18702,
+  serialized_end=18761,
 )
 
 _ATTRIBUTETYPE_PUT = _descriptor.Descriptor(
   name='Put',
   full_name='typedb.protocol.AttributeType.Put',
   filename=None,
   file=DESCRIPTOR,
@@ -4809,16 +5590,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15115,
-  serialized_end=15244,
+  serialized_start=18632,
+  serialized_end=18761,
 )
 
 _ATTRIBUTETYPE_GET_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.AttributeType.Get.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -4839,16 +5620,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15122,
-  serialized_end=15183,
+  serialized_start=18639,
+  serialized_end=18700,
 )
 
 _ATTRIBUTETYPE_GET_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.AttributeType.Get.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -4872,16 +5653,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='res', full_name='typedb.protocol.AttributeType.Get.Res.res',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=15317,
-  serialized_end=15385,
+  serialized_start=18834,
+  serialized_end=18902,
 )
 
 _ATTRIBUTETYPE_GET = _descriptor.Descriptor(
   name='Get',
   full_name='typedb.protocol.AttributeType.Get',
   filename=None,
   file=DESCRIPTOR,
@@ -4895,16 +5676,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15247,
-  serialized_end=15385,
+  serialized_start=18764,
+  serialized_end=18902,
 )
 
 _ATTRIBUTETYPE_GETOWNERS_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.AttributeType.GetOwners.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -4925,46 +5706,46 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15400,
-  serialized_end=15432,
+  serialized_start=18917,
+  serialized_end=18949,
 )
 
 _ATTRIBUTETYPE_GETOWNERS_RESPART = _descriptor.Descriptor(
   name='ResPart',
   full_name='typedb.protocol.AttributeType.GetOwners.ResPart',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='owners', full_name='typedb.protocol.AttributeType.GetOwners.ResPart.owners', index=0,
+      name='thing_types', full_name='typedb.protocol.AttributeType.GetOwners.ResPart.thing_types', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='owners', file=DESCRIPTOR),
+      serialized_options=None, json_name='thingTypes', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15434,
-  serialized_end=15490,
+  serialized_start=16095,
+  serialized_end=16160,
 )
 
 _ATTRIBUTETYPE_GETOWNERS = _descriptor.Descriptor(
   name='GetOwners',
   full_name='typedb.protocol.AttributeType.GetOwners',
   filename=None,
   file=DESCRIPTOR,
@@ -4978,16 +5759,99 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15387,
-  serialized_end=15490,
+  serialized_start=18904,
+  serialized_end=19016,
+)
+
+_ATTRIBUTETYPE_GETOWNERSEXPLICIT_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.AttributeType.GetOwnersExplicit.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='only_key', full_name='typedb.protocol.AttributeType.GetOwnersExplicit.Req.only_key', index=0,
+      number=1, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='onlyKey', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=18917,
+  serialized_end=18949,
+)
+
+_ATTRIBUTETYPE_GETOWNERSEXPLICIT_RESPART = _descriptor.Descriptor(
+  name='ResPart',
+  full_name='typedb.protocol.AttributeType.GetOwnersExplicit.ResPart',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='thing_types', full_name='typedb.protocol.AttributeType.GetOwnersExplicit.ResPart.thing_types', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='thingTypes', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=16095,
+  serialized_end=16160,
+)
+
+_ATTRIBUTETYPE_GETOWNERSEXPLICIT = _descriptor.Descriptor(
+  name='GetOwnersExplicit',
+  full_name='typedb.protocol.AttributeType.GetOwnersExplicit',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_ATTRIBUTETYPE_GETOWNERSEXPLICIT_REQ, _ATTRIBUTETYPE_GETOWNERSEXPLICIT_RESPART, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=19018,
+  serialized_end=19138,
 )
 
 _ATTRIBUTETYPE_GETREGEX_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.AttributeType.GetRegex.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -5031,16 +5895,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15511,
-  serialized_end=15538,
+  serialized_start=19159,
+  serialized_end=19186,
 )
 
 _ATTRIBUTETYPE_GETREGEX = _descriptor.Descriptor(
   name='GetRegex',
   full_name='typedb.protocol.AttributeType.GetRegex',
   filename=None,
   file=DESCRIPTOR,
@@ -5054,16 +5918,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15492,
-  serialized_end=15538,
+  serialized_start=19140,
+  serialized_end=19186,
 )
 
 _ATTRIBUTETYPE_SETREGEX_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.AttributeType.SetRegex.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -5084,16 +5948,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15552,
-  serialized_end=15579,
+  serialized_start=19200,
+  serialized_end=19227,
 )
 
 _ATTRIBUTETYPE_SETREGEX_RES = _descriptor.Descriptor(
   name='Res',
   full_name='typedb.protocol.AttributeType.SetRegex.Res',
   filename=None,
   file=DESCRIPTOR,
@@ -5130,16 +5994,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15540,
-  serialized_end=15586,
+  serialized_start=19188,
+  serialized_end=19234,
 )
 
 _ATTRIBUTETYPE_GETSUBTYPES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.AttributeType.GetSubtypes.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -5163,46 +6027,46 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='req', full_name='typedb.protocol.AttributeType.GetSubtypes.Req.req',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=15604,
-  serialized_end=15691,
+  serialized_start=19252,
+  serialized_end=19339,
 )
 
 _ATTRIBUTETYPE_GETSUBTYPES_RESPART = _descriptor.Descriptor(
   name='ResPart',
   full_name='typedb.protocol.AttributeType.GetSubtypes.ResPart',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='types', full_name='typedb.protocol.AttributeType.GetSubtypes.ResPart.types', index=0,
+      name='attribute_types', full_name='typedb.protocol.AttributeType.GetSubtypes.ResPart.attribute_types', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='types', file=DESCRIPTOR),
+      serialized_options=None, json_name='attributeTypes', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13179,
-  serialized_end=13233,
+  serialized_start=16541,
+  serialized_end=16614,
 )
 
 _ATTRIBUTETYPE_GETSUBTYPES = _descriptor.Descriptor(
   name='GetSubtypes',
   full_name='typedb.protocol.AttributeType.GetSubtypes',
   filename=None,
   file=DESCRIPTOR,
@@ -5216,16 +6080,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15589,
-  serialized_end=15747,
+  serialized_start=19237,
+  serialized_end=19414,
 )
 
 _ATTRIBUTETYPE_GETINSTANCES_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.AttributeType.GetInstances.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -5249,46 +6113,46 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='req', full_name='typedb.protocol.AttributeType.GetInstances.Req.req',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=15604,
-  serialized_end=15691,
+  serialized_start=19252,
+  serialized_end=19339,
 )
 
 _ATTRIBUTETYPE_GETINSTANCES_RESPART = _descriptor.Descriptor(
   name='ResPart',
   full_name='typedb.protocol.AttributeType.GetInstances.ResPart',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='things', full_name='typedb.protocol.AttributeType.GetInstances.ResPart.things', index=0,
+      name='attributes', full_name='typedb.protocol.AttributeType.GetInstances.ResPart.attributes', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='things', file=DESCRIPTOR),
+      serialized_options=None, json_name='attributes', file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5655,
-  serialized_end=5712,
+  serialized_start=5012,
+  serialized_end=5077,
 )
 
 _ATTRIBUTETYPE_GETINSTANCES = _descriptor.Descriptor(
   name='GetInstances',
   full_name='typedb.protocol.AttributeType.GetInstances',
   filename=None,
   file=DESCRIPTOR,
@@ -5302,40 +6166,40 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15750,
-  serialized_end=15912,
+  serialized_start=19417,
+  serialized_end=19587,
 )
 
 _ATTRIBUTETYPE = _descriptor.Descriptor(
   name='AttributeType',
   full_name='typedb.protocol.AttributeType',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
-  nested_types=[_ATTRIBUTETYPE_PUT, _ATTRIBUTETYPE_GET, _ATTRIBUTETYPE_GETOWNERS, _ATTRIBUTETYPE_GETREGEX, _ATTRIBUTETYPE_SETREGEX, _ATTRIBUTETYPE_GETSUBTYPES, _ATTRIBUTETYPE_GETINSTANCES, ],
+  nested_types=[_ATTRIBUTETYPE_PUT, _ATTRIBUTETYPE_GET, _ATTRIBUTETYPE_GETOWNERS, _ATTRIBUTETYPE_GETOWNERSEXPLICIT, _ATTRIBUTETYPE_GETREGEX, _ATTRIBUTETYPE_SETREGEX, _ATTRIBUTETYPE_GETSUBTYPES, _ATTRIBUTETYPE_GETINSTANCES, ],
   enum_types=[
     _ATTRIBUTETYPE_VALUETYPE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=15097,
-  serialized_end=15998,
+  serialized_start=18614,
+  serialized_end=19673,
 )
 
 _CONCEPTMANAGER_REQ.fields_by_name['get_thing_type_req'].message_type = _CONCEPTMANAGER_GETTHINGTYPE_REQ
 _CONCEPTMANAGER_REQ.fields_by_name['get_thing_req'].message_type = _CONCEPTMANAGER_GETTHING_REQ
 _CONCEPTMANAGER_REQ.fields_by_name['put_entity_type_req'].message_type = _CONCEPTMANAGER_PUTENTITYTYPE_REQ
 _CONCEPTMANAGER_REQ.fields_by_name['put_attribute_type_req'].message_type = _CONCEPTMANAGER_PUTATTRIBUTETYPE_REQ
 _CONCEPTMANAGER_REQ.fields_by_name['put_relation_type_req'].message_type = _CONCEPTMANAGER_PUTRELATIONTYPE_REQ
@@ -5602,36 +6466,45 @@
 _TYPE_REQ.fields_by_name['type_delete_req'].message_type = _TYPE_DELETE_REQ
 _TYPE_REQ.fields_by_name['type_set_label_req'].message_type = _TYPE_SETLABEL_REQ
 _TYPE_REQ.fields_by_name['type_is_abstract_req'].message_type = _TYPE_ISABSTRACT_REQ
 _TYPE_REQ.fields_by_name['type_get_supertype_req'].message_type = _TYPE_GETSUPERTYPE_REQ
 _TYPE_REQ.fields_by_name['type_set_supertype_req'].message_type = _TYPE_SETSUPERTYPE_REQ
 _TYPE_REQ.fields_by_name['type_get_supertypes_req'].message_type = _TYPE_GETSUPERTYPES_REQ
 _TYPE_REQ.fields_by_name['type_get_subtypes_req'].message_type = _TYPE_GETSUBTYPES_REQ
+_TYPE_REQ.fields_by_name['type_get_subtypes_explicit_req'].message_type = _TYPE_GETSUBTYPESEXPLICIT_REQ
 _TYPE_REQ.fields_by_name['role_type_get_relation_types_req'].message_type = _ROLETYPE_GETRELATIONTYPES_REQ
 _TYPE_REQ.fields_by_name['role_type_get_players_req'].message_type = _ROLETYPE_GETPLAYERS_REQ
 _TYPE_REQ.fields_by_name['thing_type_get_instances_req'].message_type = _THINGTYPE_GETINSTANCES_REQ
+_TYPE_REQ.fields_by_name['thing_type_get_instances_explicit_req'].message_type = _THINGTYPE_GETINSTANCESEXPLICIT_REQ
 _TYPE_REQ.fields_by_name['thing_type_set_abstract_req'].message_type = _THINGTYPE_SETABSTRACT_REQ
 _TYPE_REQ.fields_by_name['thing_type_unset_abstract_req'].message_type = _THINGTYPE_UNSETABSTRACT_REQ
 _TYPE_REQ.fields_by_name['thing_type_get_owns_req'].message_type = _THINGTYPE_GETOWNS_REQ
+_TYPE_REQ.fields_by_name['thing_type_get_owns_explicit_req'].message_type = _THINGTYPE_GETOWNSEXPLICIT_REQ
+_TYPE_REQ.fields_by_name['thing_type_get_owns_overridden_req'].message_type = _THINGTYPE_GETOWNSOVERRIDDEN_REQ
 _TYPE_REQ.fields_by_name['thing_type_set_owns_req'].message_type = _THINGTYPE_SETOWNS_REQ
 _TYPE_REQ.fields_by_name['thing_type_unset_owns_req'].message_type = _THINGTYPE_UNSETOWNS_REQ
 _TYPE_REQ.fields_by_name['thing_type_get_plays_req'].message_type = _THINGTYPE_GETPLAYS_REQ
+_TYPE_REQ.fields_by_name['thing_type_get_plays_explicit_req'].message_type = _THINGTYPE_GETPLAYSEXPLICIT_REQ
+_TYPE_REQ.fields_by_name['thing_type_get_plays_overridden_req'].message_type = _THINGTYPE_GETPLAYSOVERRIDDEN_REQ
 _TYPE_REQ.fields_by_name['thing_type_set_plays_req'].message_type = _THINGTYPE_SETPLAYS_REQ
 _TYPE_REQ.fields_by_name['thing_type_unset_plays_req'].message_type = _THINGTYPE_UNSETPLAYS_REQ
 _TYPE_REQ.fields_by_name['entity_type_create_req'].message_type = _ENTITYTYPE_CREATE_REQ
 _TYPE_REQ.fields_by_name['relation_type_create_req'].message_type = _RELATIONTYPE_CREATE_REQ
-_TYPE_REQ.fields_by_name['relation_type_get_relates_for_role_label_req'].message_type = _RELATIONTYPE_GETRELATESFORROLELABEL_REQ
 _TYPE_REQ.fields_by_name['relation_type_get_relates_req'].message_type = _RELATIONTYPE_GETRELATES_REQ
+_TYPE_REQ.fields_by_name['relation_type_get_relates_explicit_req'].message_type = _RELATIONTYPE_GETRELATESEXPLICIT_REQ
+_TYPE_REQ.fields_by_name['relation_type_get_relates_for_role_label_req'].message_type = _RELATIONTYPE_GETRELATESFORROLELABEL_REQ
+_TYPE_REQ.fields_by_name['relation_type_get_relates_overridden_req'].message_type = _RELATIONTYPE_GETRELATESOVERRIDDEN_REQ
 _TYPE_REQ.fields_by_name['relation_type_set_relates_req'].message_type = _RELATIONTYPE_SETRELATES_REQ
 _TYPE_REQ.fields_by_name['relation_type_unset_relates_req'].message_type = _RELATIONTYPE_UNSETRELATES_REQ
 _TYPE_REQ.fields_by_name['attribute_type_put_req'].message_type = _ATTRIBUTETYPE_PUT_REQ
 _TYPE_REQ.fields_by_name['attribute_type_get_req'].message_type = _ATTRIBUTETYPE_GET_REQ
 _TYPE_REQ.fields_by_name['attribute_type_get_regex_req'].message_type = _ATTRIBUTETYPE_GETREGEX_REQ
 _TYPE_REQ.fields_by_name['attribute_type_set_regex_req'].message_type = _ATTRIBUTETYPE_SETREGEX_REQ
 _TYPE_REQ.fields_by_name['attribute_type_get_owners_req'].message_type = _ATTRIBUTETYPE_GETOWNERS_REQ
+_TYPE_REQ.fields_by_name['attribute_type_get_owners_explicit_req'].message_type = _ATTRIBUTETYPE_GETOWNERSEXPLICIT_REQ
 _TYPE_REQ.containing_type = _TYPE
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['type_delete_req'])
 _TYPE_REQ.fields_by_name['type_delete_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['type_set_label_req'])
 _TYPE_REQ.fields_by_name['type_set_label_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
@@ -5647,58 +6520,82 @@
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['type_get_supertypes_req'])
 _TYPE_REQ.fields_by_name['type_get_supertypes_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['type_get_subtypes_req'])
 _TYPE_REQ.fields_by_name['type_get_subtypes_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['type_get_subtypes_explicit_req'])
+_TYPE_REQ.fields_by_name['type_get_subtypes_explicit_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['role_type_get_relation_types_req'])
 _TYPE_REQ.fields_by_name['role_type_get_relation_types_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['role_type_get_players_req'])
 _TYPE_REQ.fields_by_name['role_type_get_players_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_get_instances_req'])
 _TYPE_REQ.fields_by_name['thing_type_get_instances_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['thing_type_get_instances_explicit_req'])
+_TYPE_REQ.fields_by_name['thing_type_get_instances_explicit_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_set_abstract_req'])
 _TYPE_REQ.fields_by_name['thing_type_set_abstract_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_unset_abstract_req'])
 _TYPE_REQ.fields_by_name['thing_type_unset_abstract_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_get_owns_req'])
 _TYPE_REQ.fields_by_name['thing_type_get_owns_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['thing_type_get_owns_explicit_req'])
+_TYPE_REQ.fields_by_name['thing_type_get_owns_explicit_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['thing_type_get_owns_overridden_req'])
+_TYPE_REQ.fields_by_name['thing_type_get_owns_overridden_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_set_owns_req'])
 _TYPE_REQ.fields_by_name['thing_type_set_owns_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_unset_owns_req'])
 _TYPE_REQ.fields_by_name['thing_type_unset_owns_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_get_plays_req'])
 _TYPE_REQ.fields_by_name['thing_type_get_plays_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['thing_type_get_plays_explicit_req'])
+_TYPE_REQ.fields_by_name['thing_type_get_plays_explicit_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['thing_type_get_plays_overridden_req'])
+_TYPE_REQ.fields_by_name['thing_type_get_plays_overridden_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_set_plays_req'])
 _TYPE_REQ.fields_by_name['thing_type_set_plays_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['thing_type_unset_plays_req'])
 _TYPE_REQ.fields_by_name['thing_type_unset_plays_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['entity_type_create_req'])
 _TYPE_REQ.fields_by_name['entity_type_create_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['relation_type_create_req'])
 _TYPE_REQ.fields_by_name['relation_type_create_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['relation_type_get_relates_req'])
+_TYPE_REQ.fields_by_name['relation_type_get_relates_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['relation_type_get_relates_explicit_req'])
+_TYPE_REQ.fields_by_name['relation_type_get_relates_explicit_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['relation_type_get_relates_for_role_label_req'])
 _TYPE_REQ.fields_by_name['relation_type_get_relates_for_role_label_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
-  _TYPE_REQ.fields_by_name['relation_type_get_relates_req'])
-_TYPE_REQ.fields_by_name['relation_type_get_relates_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+  _TYPE_REQ.fields_by_name['relation_type_get_relates_overridden_req'])
+_TYPE_REQ.fields_by_name['relation_type_get_relates_overridden_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['relation_type_set_relates_req'])
 _TYPE_REQ.fields_by_name['relation_type_set_relates_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['relation_type_unset_relates_req'])
 _TYPE_REQ.fields_by_name['relation_type_unset_relates_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
@@ -5712,28 +6609,34 @@
 _TYPE_REQ.fields_by_name['attribute_type_get_regex_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['attribute_type_set_regex_req'])
 _TYPE_REQ.fields_by_name['attribute_type_set_regex_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_REQ.oneofs_by_name['req'].fields.append(
   _TYPE_REQ.fields_by_name['attribute_type_get_owners_req'])
 _TYPE_REQ.fields_by_name['attribute_type_get_owners_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
+_TYPE_REQ.oneofs_by_name['req'].fields.append(
+  _TYPE_REQ.fields_by_name['attribute_type_get_owners_explicit_req'])
+_TYPE_REQ.fields_by_name['attribute_type_get_owners_explicit_req'].containing_oneof = _TYPE_REQ.oneofs_by_name['req']
 _TYPE_RES.fields_by_name['type_delete_res'].message_type = _TYPE_DELETE_RES
 _TYPE_RES.fields_by_name['type_set_label_res'].message_type = _TYPE_SETLABEL_RES
 _TYPE_RES.fields_by_name['type_is_abstract_res'].message_type = _TYPE_ISABSTRACT_RES
 _TYPE_RES.fields_by_name['type_get_supertype_res'].message_type = _TYPE_GETSUPERTYPE_RES
 _TYPE_RES.fields_by_name['type_set_supertype_res'].message_type = _TYPE_SETSUPERTYPE_RES
 _TYPE_RES.fields_by_name['thing_type_set_abstract_res'].message_type = _THINGTYPE_SETABSTRACT_RES
 _TYPE_RES.fields_by_name['thing_type_unset_abstract_res'].message_type = _THINGTYPE_UNSETABSTRACT_RES
+_TYPE_RES.fields_by_name['thing_type_get_owns_overridden_res'].message_type = _THINGTYPE_GETOWNSOVERRIDDEN_RES
 _TYPE_RES.fields_by_name['thing_type_set_owns_res'].message_type = _THINGTYPE_SETOWNS_RES
 _TYPE_RES.fields_by_name['thing_type_unset_owns_res'].message_type = _THINGTYPE_UNSETOWNS_RES
+_TYPE_RES.fields_by_name['thing_type_get_plays_overridden_res'].message_type = _THINGTYPE_GETPLAYSOVERRIDDEN_RES
 _TYPE_RES.fields_by_name['thing_type_set_plays_res'].message_type = _THINGTYPE_SETPLAYS_RES
 _TYPE_RES.fields_by_name['thing_type_unset_plays_res'].message_type = _THINGTYPE_UNSETPLAYS_RES
 _TYPE_RES.fields_by_name['entity_type_create_res'].message_type = _ENTITYTYPE_CREATE_RES
 _TYPE_RES.fields_by_name['relation_type_create_res'].message_type = _RELATIONTYPE_CREATE_RES
 _TYPE_RES.fields_by_name['relation_type_get_relates_for_role_label_res'].message_type = _RELATIONTYPE_GETRELATESFORROLELABEL_RES
+_TYPE_RES.fields_by_name['relation_type_get_relates_overridden_res'].message_type = _RELATIONTYPE_GETRELATESOVERRIDDEN_RES
 _TYPE_RES.fields_by_name['relation_type_set_relates_res'].message_type = _RELATIONTYPE_SETRELATES_RES
 _TYPE_RES.fields_by_name['relation_type_unset_relates_res'].message_type = _RELATIONTYPE_UNSETRELATES_RES
 _TYPE_RES.fields_by_name['attribute_type_put_res'].message_type = _ATTRIBUTETYPE_PUT_RES
 _TYPE_RES.fields_by_name['attribute_type_get_res'].message_type = _ATTRIBUTETYPE_GET_RES
 _TYPE_RES.fields_by_name['attribute_type_get_regex_res'].message_type = _ATTRIBUTETYPE_GETREGEX_RES
 _TYPE_RES.fields_by_name['attribute_type_set_regex_res'].message_type = _ATTRIBUTETYPE_SETREGEX_RES
 _TYPE_RES.containing_type = _TYPE
@@ -5755,20 +6658,26 @@
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['thing_type_set_abstract_res'])
 _TYPE_RES.fields_by_name['thing_type_set_abstract_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['thing_type_unset_abstract_res'])
 _TYPE_RES.fields_by_name['thing_type_unset_abstract_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
+  _TYPE_RES.fields_by_name['thing_type_get_owns_overridden_res'])
+_TYPE_RES.fields_by_name['thing_type_get_owns_overridden_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
+_TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['thing_type_set_owns_res'])
 _TYPE_RES.fields_by_name['thing_type_set_owns_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['thing_type_unset_owns_res'])
 _TYPE_RES.fields_by_name['thing_type_unset_owns_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
+  _TYPE_RES.fields_by_name['thing_type_get_plays_overridden_res'])
+_TYPE_RES.fields_by_name['thing_type_get_plays_overridden_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
+_TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['thing_type_set_plays_res'])
 _TYPE_RES.fields_by_name['thing_type_set_plays_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['thing_type_unset_plays_res'])
 _TYPE_RES.fields_by_name['thing_type_unset_plays_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['entity_type_create_res'])
@@ -5776,14 +6685,17 @@
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['relation_type_create_res'])
 _TYPE_RES.fields_by_name['relation_type_create_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['relation_type_get_relates_for_role_label_res'])
 _TYPE_RES.fields_by_name['relation_type_get_relates_for_role_label_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
+  _TYPE_RES.fields_by_name['relation_type_get_relates_overridden_res'])
+_TYPE_RES.fields_by_name['relation_type_get_relates_overridden_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
+_TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['relation_type_set_relates_res'])
 _TYPE_RES.fields_by_name['relation_type_set_relates_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['relation_type_unset_relates_res'])
 _TYPE_RES.fields_by_name['relation_type_unset_relates_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['attribute_type_put_res'])
@@ -5795,49 +6707,73 @@
   _TYPE_RES.fields_by_name['attribute_type_get_regex_res'])
 _TYPE_RES.fields_by_name['attribute_type_get_regex_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RES.oneofs_by_name['res'].fields.append(
   _TYPE_RES.fields_by_name['attribute_type_set_regex_res'])
 _TYPE_RES.fields_by_name['attribute_type_set_regex_res'].containing_oneof = _TYPE_RES.oneofs_by_name['res']
 _TYPE_RESPART.fields_by_name['type_get_supertypes_res_part'].message_type = _TYPE_GETSUPERTYPES_RESPART
 _TYPE_RESPART.fields_by_name['type_get_subtypes_res_part'].message_type = _TYPE_GETSUBTYPES_RESPART
+_TYPE_RESPART.fields_by_name['type_get_subtypes_explicit_res_part'].message_type = _TYPE_GETSUBTYPESEXPLICIT_RESPART
 _TYPE_RESPART.fields_by_name['role_type_get_relation_types_res_part'].message_type = _ROLETYPE_GETRELATIONTYPES_RESPART
 _TYPE_RESPART.fields_by_name['role_type_get_players_res_part'].message_type = _ROLETYPE_GETPLAYERS_RESPART
 _TYPE_RESPART.fields_by_name['thing_type_get_instances_res_part'].message_type = _THINGTYPE_GETINSTANCES_RESPART
+_TYPE_RESPART.fields_by_name['thing_type_get_instances_explicit_res_part'].message_type = _THINGTYPE_GETINSTANCESEXPLICIT_RESPART
 _TYPE_RESPART.fields_by_name['thing_type_get_owns_res_part'].message_type = _THINGTYPE_GETOWNS_RESPART
+_TYPE_RESPART.fields_by_name['thing_type_get_owns_explicit_res_part'].message_type = _THINGTYPE_GETOWNSEXPLICIT_RESPART
 _TYPE_RESPART.fields_by_name['thing_type_get_plays_res_part'].message_type = _THINGTYPE_GETPLAYS_RESPART
+_TYPE_RESPART.fields_by_name['thing_type_get_plays_explicit_res_part'].message_type = _THINGTYPE_GETPLAYSEXPLICIT_RESPART
 _TYPE_RESPART.fields_by_name['relation_type_get_relates_res_part'].message_type = _RELATIONTYPE_GETRELATES_RESPART
+_TYPE_RESPART.fields_by_name['relation_type_get_relates_explicit_res_part'].message_type = _RELATIONTYPE_GETRELATESEXPLICIT_RESPART
 _TYPE_RESPART.fields_by_name['attribute_type_get_owners_res_part'].message_type = _ATTRIBUTETYPE_GETOWNERS_RESPART
+_TYPE_RESPART.fields_by_name['attribute_type_get_owners_explicit_res_part'].message_type = _ATTRIBUTETYPE_GETOWNERSEXPLICIT_RESPART
 _TYPE_RESPART.containing_type = _TYPE
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['type_get_supertypes_res_part'])
 _TYPE_RESPART.fields_by_name['type_get_supertypes_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['type_get_subtypes_res_part'])
 _TYPE_RESPART.fields_by_name['type_get_subtypes_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
+  _TYPE_RESPART.fields_by_name['type_get_subtypes_explicit_res_part'])
+_TYPE_RESPART.fields_by_name['type_get_subtypes_explicit_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
+_TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['role_type_get_relation_types_res_part'])
 _TYPE_RESPART.fields_by_name['role_type_get_relation_types_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['role_type_get_players_res_part'])
 _TYPE_RESPART.fields_by_name['role_type_get_players_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['thing_type_get_instances_res_part'])
 _TYPE_RESPART.fields_by_name['thing_type_get_instances_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
+  _TYPE_RESPART.fields_by_name['thing_type_get_instances_explicit_res_part'])
+_TYPE_RESPART.fields_by_name['thing_type_get_instances_explicit_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
+_TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['thing_type_get_owns_res_part'])
 _TYPE_RESPART.fields_by_name['thing_type_get_owns_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
+  _TYPE_RESPART.fields_by_name['thing_type_get_owns_explicit_res_part'])
+_TYPE_RESPART.fields_by_name['thing_type_get_owns_explicit_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
+_TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['thing_type_get_plays_res_part'])
 _TYPE_RESPART.fields_by_name['thing_type_get_plays_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
+  _TYPE_RESPART.fields_by_name['thing_type_get_plays_explicit_res_part'])
+_TYPE_RESPART.fields_by_name['thing_type_get_plays_explicit_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
+_TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['relation_type_get_relates_res_part'])
 _TYPE_RESPART.fields_by_name['relation_type_get_relates_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_RESPART.oneofs_by_name['res'].fields.append(
+  _TYPE_RESPART.fields_by_name['relation_type_get_relates_explicit_res_part'])
+_TYPE_RESPART.fields_by_name['relation_type_get_relates_explicit_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
+_TYPE_RESPART.oneofs_by_name['res'].fields.append(
   _TYPE_RESPART.fields_by_name['attribute_type_get_owners_res_part'])
 _TYPE_RESPART.fields_by_name['attribute_type_get_owners_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
+_TYPE_RESPART.oneofs_by_name['res'].fields.append(
+  _TYPE_RESPART.fields_by_name['attribute_type_get_owners_explicit_res_part'])
+_TYPE_RESPART.fields_by_name['attribute_type_get_owners_explicit_res_part'].containing_oneof = _TYPE_RESPART.oneofs_by_name['res']
 _TYPE_DELETE_REQ.containing_type = _TYPE_DELETE
 _TYPE_DELETE_RES.containing_type = _TYPE_DELETE
 _TYPE_DELETE.containing_type = _TYPE
 _TYPE_SETLABEL_REQ.containing_type = _TYPE_SETLABEL
 _TYPE_SETLABEL_RES.containing_type = _TYPE_SETLABEL
 _TYPE_SETLABEL.containing_type = _TYPE
 _TYPE_ISABSTRACT_REQ.containing_type = _TYPE_ISABSTRACT
@@ -5858,14 +6794,18 @@
 _TYPE_GETSUPERTYPES_RESPART.fields_by_name['types'].message_type = _TYPE
 _TYPE_GETSUPERTYPES_RESPART.containing_type = _TYPE_GETSUPERTYPES
 _TYPE_GETSUPERTYPES.containing_type = _TYPE
 _TYPE_GETSUBTYPES_REQ.containing_type = _TYPE_GETSUBTYPES
 _TYPE_GETSUBTYPES_RESPART.fields_by_name['types'].message_type = _TYPE
 _TYPE_GETSUBTYPES_RESPART.containing_type = _TYPE_GETSUBTYPES
 _TYPE_GETSUBTYPES.containing_type = _TYPE
+_TYPE_GETSUBTYPESEXPLICIT_REQ.containing_type = _TYPE_GETSUBTYPESEXPLICIT
+_TYPE_GETSUBTYPESEXPLICIT_RESPART.fields_by_name['types'].message_type = _TYPE
+_TYPE_GETSUBTYPESEXPLICIT_RESPART.containing_type = _TYPE_GETSUBTYPESEXPLICIT
+_TYPE_GETSUBTYPESEXPLICIT.containing_type = _TYPE
 _TYPE.fields_by_name['encoding'].enum_type = _TYPE_ENCODING
 _TYPE.fields_by_name['value_type'].enum_type = _ATTRIBUTETYPE_VALUETYPE
 _TYPE_ENCODING.containing_type = _TYPE
 _ROLETYPE_GETRELATIONTYPES_REQ.containing_type = _ROLETYPE_GETRELATIONTYPES
 _ROLETYPE_GETRELATIONTYPES_RESPART.fields_by_name['relation_types'].message_type = _TYPE
 _ROLETYPE_GETRELATIONTYPES_RESPART.containing_type = _ROLETYPE_GETRELATIONTYPES
 _ROLETYPE_GETRELATIONTYPES.containing_type = _ROLETYPE
@@ -5879,69 +6819,112 @@
 _THINGTYPE_UNSETABSTRACT_REQ.containing_type = _THINGTYPE_UNSETABSTRACT
 _THINGTYPE_UNSETABSTRACT_RES.containing_type = _THINGTYPE_UNSETABSTRACT
 _THINGTYPE_UNSETABSTRACT.containing_type = _THINGTYPE
 _THINGTYPE_GETINSTANCES_REQ.containing_type = _THINGTYPE_GETINSTANCES
 _THINGTYPE_GETINSTANCES_RESPART.fields_by_name['things'].message_type = _THING
 _THINGTYPE_GETINSTANCES_RESPART.containing_type = _THINGTYPE_GETINSTANCES
 _THINGTYPE_GETINSTANCES.containing_type = _THINGTYPE
+_THINGTYPE_GETINSTANCESEXPLICIT_REQ.containing_type = _THINGTYPE_GETINSTANCESEXPLICIT
+_THINGTYPE_GETINSTANCESEXPLICIT_RESPART.fields_by_name['things'].message_type = _THING
+_THINGTYPE_GETINSTANCESEXPLICIT_RESPART.containing_type = _THINGTYPE_GETINSTANCESEXPLICIT
+_THINGTYPE_GETINSTANCESEXPLICIT.containing_type = _THINGTYPE
 _THINGTYPE_GETOWNS_REQ.fields_by_name['value_type'].enum_type = _ATTRIBUTETYPE_VALUETYPE
 _THINGTYPE_GETOWNS_REQ.containing_type = _THINGTYPE_GETOWNS
 _THINGTYPE_GETOWNS_REQ.oneofs_by_name['filter'].fields.append(
   _THINGTYPE_GETOWNS_REQ.fields_by_name['value_type'])
 _THINGTYPE_GETOWNS_REQ.fields_by_name['value_type'].containing_oneof = _THINGTYPE_GETOWNS_REQ.oneofs_by_name['filter']
 _THINGTYPE_GETOWNS_RESPART.fields_by_name['attribute_types'].message_type = _TYPE
 _THINGTYPE_GETOWNS_RESPART.containing_type = _THINGTYPE_GETOWNS
 _THINGTYPE_GETOWNS.containing_type = _THINGTYPE
-_THINGTYPE_GETPLAYS_REQ.containing_type = _THINGTYPE_GETPLAYS
-_THINGTYPE_GETPLAYS_RESPART.fields_by_name['roles'].message_type = _TYPE
-_THINGTYPE_GETPLAYS_RESPART.containing_type = _THINGTYPE_GETPLAYS
-_THINGTYPE_GETPLAYS.containing_type = _THINGTYPE
+_THINGTYPE_GETOWNSEXPLICIT_REQ.fields_by_name['value_type'].enum_type = _ATTRIBUTETYPE_VALUETYPE
+_THINGTYPE_GETOWNSEXPLICIT_REQ.containing_type = _THINGTYPE_GETOWNSEXPLICIT
+_THINGTYPE_GETOWNSEXPLICIT_REQ.oneofs_by_name['filter'].fields.append(
+  _THINGTYPE_GETOWNSEXPLICIT_REQ.fields_by_name['value_type'])
+_THINGTYPE_GETOWNSEXPLICIT_REQ.fields_by_name['value_type'].containing_oneof = _THINGTYPE_GETOWNSEXPLICIT_REQ.oneofs_by_name['filter']
+_THINGTYPE_GETOWNSEXPLICIT_RESPART.fields_by_name['attribute_types'].message_type = _TYPE
+_THINGTYPE_GETOWNSEXPLICIT_RESPART.containing_type = _THINGTYPE_GETOWNSEXPLICIT
+_THINGTYPE_GETOWNSEXPLICIT.containing_type = _THINGTYPE
+_THINGTYPE_GETOWNSOVERRIDDEN_REQ.fields_by_name['attribute_type'].message_type = _TYPE
+_THINGTYPE_GETOWNSOVERRIDDEN_REQ.containing_type = _THINGTYPE_GETOWNSOVERRIDDEN
+_THINGTYPE_GETOWNSOVERRIDDEN_RES.fields_by_name['attribute_type'].message_type = _TYPE
+_THINGTYPE_GETOWNSOVERRIDDEN_RES.containing_type = _THINGTYPE_GETOWNSOVERRIDDEN
+_THINGTYPE_GETOWNSOVERRIDDEN_RES.oneofs_by_name['res'].fields.append(
+  _THINGTYPE_GETOWNSOVERRIDDEN_RES.fields_by_name['attribute_type'])
+_THINGTYPE_GETOWNSOVERRIDDEN_RES.fields_by_name['attribute_type'].containing_oneof = _THINGTYPE_GETOWNSOVERRIDDEN_RES.oneofs_by_name['res']
+_THINGTYPE_GETOWNSOVERRIDDEN.containing_type = _THINGTYPE
 _THINGTYPE_SETOWNS_REQ.fields_by_name['attribute_type'].message_type = _TYPE
 _THINGTYPE_SETOWNS_REQ.fields_by_name['overridden_type'].message_type = _TYPE
 _THINGTYPE_SETOWNS_REQ.containing_type = _THINGTYPE_SETOWNS
 _THINGTYPE_SETOWNS_REQ.oneofs_by_name['overridden'].fields.append(
   _THINGTYPE_SETOWNS_REQ.fields_by_name['overridden_type'])
 _THINGTYPE_SETOWNS_REQ.fields_by_name['overridden_type'].containing_oneof = _THINGTYPE_SETOWNS_REQ.oneofs_by_name['overridden']
 _THINGTYPE_SETOWNS_RES.containing_type = _THINGTYPE_SETOWNS
 _THINGTYPE_SETOWNS.containing_type = _THINGTYPE
-_THINGTYPE_SETPLAYS_REQ.fields_by_name['role'].message_type = _TYPE
-_THINGTYPE_SETPLAYS_REQ.fields_by_name['overridden_role'].message_type = _TYPE
-_THINGTYPE_SETPLAYS_REQ.containing_type = _THINGTYPE_SETPLAYS
-_THINGTYPE_SETPLAYS_REQ.oneofs_by_name['overridden'].fields.append(
-  _THINGTYPE_SETPLAYS_REQ.fields_by_name['overridden_role'])
-_THINGTYPE_SETPLAYS_REQ.fields_by_name['overridden_role'].containing_oneof = _THINGTYPE_SETPLAYS_REQ.oneofs_by_name['overridden']
-_THINGTYPE_SETPLAYS_RES.containing_type = _THINGTYPE_SETPLAYS
-_THINGTYPE_SETPLAYS.containing_type = _THINGTYPE
 _THINGTYPE_UNSETOWNS_REQ.fields_by_name['attribute_type'].message_type = _TYPE
 _THINGTYPE_UNSETOWNS_REQ.containing_type = _THINGTYPE_UNSETOWNS
 _THINGTYPE_UNSETOWNS_RES.containing_type = _THINGTYPE_UNSETOWNS
 _THINGTYPE_UNSETOWNS.containing_type = _THINGTYPE
-_THINGTYPE_UNSETPLAYS_REQ.fields_by_name['role'].message_type = _TYPE
+_THINGTYPE_GETPLAYS_REQ.containing_type = _THINGTYPE_GETPLAYS
+_THINGTYPE_GETPLAYS_RESPART.fields_by_name['role_types'].message_type = _TYPE
+_THINGTYPE_GETPLAYS_RESPART.containing_type = _THINGTYPE_GETPLAYS
+_THINGTYPE_GETPLAYS.containing_type = _THINGTYPE
+_THINGTYPE_GETPLAYSEXPLICIT_REQ.containing_type = _THINGTYPE_GETPLAYSEXPLICIT
+_THINGTYPE_GETPLAYSEXPLICIT_RESPART.fields_by_name['role_types'].message_type = _TYPE
+_THINGTYPE_GETPLAYSEXPLICIT_RESPART.containing_type = _THINGTYPE_GETPLAYSEXPLICIT
+_THINGTYPE_GETPLAYSEXPLICIT.containing_type = _THINGTYPE
+_THINGTYPE_GETPLAYSOVERRIDDEN_REQ.fields_by_name['role_type'].message_type = _TYPE
+_THINGTYPE_GETPLAYSOVERRIDDEN_REQ.containing_type = _THINGTYPE_GETPLAYSOVERRIDDEN
+_THINGTYPE_GETPLAYSOVERRIDDEN_RES.fields_by_name['role_type'].message_type = _TYPE
+_THINGTYPE_GETPLAYSOVERRIDDEN_RES.containing_type = _THINGTYPE_GETPLAYSOVERRIDDEN
+_THINGTYPE_GETPLAYSOVERRIDDEN_RES.oneofs_by_name['res'].fields.append(
+  _THINGTYPE_GETPLAYSOVERRIDDEN_RES.fields_by_name['role_type'])
+_THINGTYPE_GETPLAYSOVERRIDDEN_RES.fields_by_name['role_type'].containing_oneof = _THINGTYPE_GETPLAYSOVERRIDDEN_RES.oneofs_by_name['res']
+_THINGTYPE_GETPLAYSOVERRIDDEN.containing_type = _THINGTYPE
+_THINGTYPE_SETPLAYS_REQ.fields_by_name['role_type'].message_type = _TYPE
+_THINGTYPE_SETPLAYS_REQ.fields_by_name['overridden_type'].message_type = _TYPE
+_THINGTYPE_SETPLAYS_REQ.containing_type = _THINGTYPE_SETPLAYS
+_THINGTYPE_SETPLAYS_REQ.oneofs_by_name['overridden'].fields.append(
+  _THINGTYPE_SETPLAYS_REQ.fields_by_name['overridden_type'])
+_THINGTYPE_SETPLAYS_REQ.fields_by_name['overridden_type'].containing_oneof = _THINGTYPE_SETPLAYS_REQ.oneofs_by_name['overridden']
+_THINGTYPE_SETPLAYS_RES.containing_type = _THINGTYPE_SETPLAYS
+_THINGTYPE_SETPLAYS.containing_type = _THINGTYPE
+_THINGTYPE_UNSETPLAYS_REQ.fields_by_name['role_type'].message_type = _TYPE
 _THINGTYPE_UNSETPLAYS_REQ.containing_type = _THINGTYPE_UNSETPLAYS
 _THINGTYPE_UNSETPLAYS_RES.containing_type = _THINGTYPE_UNSETPLAYS
 _THINGTYPE_UNSETPLAYS.containing_type = _THINGTYPE
 _ENTITYTYPE_CREATE_REQ.containing_type = _ENTITYTYPE_CREATE
 _ENTITYTYPE_CREATE_RES.fields_by_name['entity'].message_type = _THING
 _ENTITYTYPE_CREATE_RES.containing_type = _ENTITYTYPE_CREATE
 _ENTITYTYPE_CREATE.containing_type = _ENTITYTYPE
 _RELATIONTYPE_CREATE_REQ.containing_type = _RELATIONTYPE_CREATE
 _RELATIONTYPE_CREATE_RES.fields_by_name['relation'].message_type = _THING
 _RELATIONTYPE_CREATE_RES.containing_type = _RELATIONTYPE_CREATE
 _RELATIONTYPE_CREATE.containing_type = _RELATIONTYPE
 _RELATIONTYPE_GETRELATES_REQ.containing_type = _RELATIONTYPE_GETRELATES
-_RELATIONTYPE_GETRELATES_RESPART.fields_by_name['roles'].message_type = _TYPE
+_RELATIONTYPE_GETRELATES_RESPART.fields_by_name['role_types'].message_type = _TYPE
 _RELATIONTYPE_GETRELATES_RESPART.containing_type = _RELATIONTYPE_GETRELATES
 _RELATIONTYPE_GETRELATES.containing_type = _RELATIONTYPE
+_RELATIONTYPE_GETRELATESEXPLICIT_REQ.containing_type = _RELATIONTYPE_GETRELATESEXPLICIT
+_RELATIONTYPE_GETRELATESEXPLICIT_RESPART.fields_by_name['role_types'].message_type = _TYPE
+_RELATIONTYPE_GETRELATESEXPLICIT_RESPART.containing_type = _RELATIONTYPE_GETRELATESEXPLICIT
+_RELATIONTYPE_GETRELATESEXPLICIT.containing_type = _RELATIONTYPE
 _RELATIONTYPE_GETRELATESFORROLELABEL_REQ.containing_type = _RELATIONTYPE_GETRELATESFORROLELABEL
 _RELATIONTYPE_GETRELATESFORROLELABEL_RES.fields_by_name['role_type'].message_type = _TYPE
 _RELATIONTYPE_GETRELATESFORROLELABEL_RES.containing_type = _RELATIONTYPE_GETRELATESFORROLELABEL
 _RELATIONTYPE_GETRELATESFORROLELABEL_RES.oneofs_by_name['role'].fields.append(
   _RELATIONTYPE_GETRELATESFORROLELABEL_RES.fields_by_name['role_type'])
 _RELATIONTYPE_GETRELATESFORROLELABEL_RES.fields_by_name['role_type'].containing_oneof = _RELATIONTYPE_GETRELATESFORROLELABEL_RES.oneofs_by_name['role']
 _RELATIONTYPE_GETRELATESFORROLELABEL.containing_type = _RELATIONTYPE
+_RELATIONTYPE_GETRELATESOVERRIDDEN_REQ.containing_type = _RELATIONTYPE_GETRELATESOVERRIDDEN
+_RELATIONTYPE_GETRELATESOVERRIDDEN_RES.fields_by_name['role_type'].message_type = _TYPE
+_RELATIONTYPE_GETRELATESOVERRIDDEN_RES.containing_type = _RELATIONTYPE_GETRELATESOVERRIDDEN
+_RELATIONTYPE_GETRELATESOVERRIDDEN_RES.oneofs_by_name['res'].fields.append(
+  _RELATIONTYPE_GETRELATESOVERRIDDEN_RES.fields_by_name['role_type'])
+_RELATIONTYPE_GETRELATESOVERRIDDEN_RES.fields_by_name['role_type'].containing_oneof = _RELATIONTYPE_GETRELATESOVERRIDDEN_RES.oneofs_by_name['res']
+_RELATIONTYPE_GETRELATESOVERRIDDEN.containing_type = _RELATIONTYPE
 _RELATIONTYPE_SETRELATES_REQ.containing_type = _RELATIONTYPE_SETRELATES
 _RELATIONTYPE_SETRELATES_REQ.oneofs_by_name['overridden'].fields.append(
   _RELATIONTYPE_SETRELATES_REQ.fields_by_name['overridden_label'])
 _RELATIONTYPE_SETRELATES_REQ.fields_by_name['overridden_label'].containing_oneof = _RELATIONTYPE_SETRELATES_REQ.oneofs_by_name['overridden']
 _RELATIONTYPE_SETRELATES_RES.containing_type = _RELATIONTYPE_SETRELATES
 _RELATIONTYPE_SETRELATES.containing_type = _RELATIONTYPE
 _RELATIONTYPE_UNSETRELATES_REQ.containing_type = _RELATIONTYPE_UNSETRELATES
@@ -5957,37 +6940,41 @@
 _ATTRIBUTETYPE_GET_RES.fields_by_name['attribute'].message_type = _THING
 _ATTRIBUTETYPE_GET_RES.containing_type = _ATTRIBUTETYPE_GET
 _ATTRIBUTETYPE_GET_RES.oneofs_by_name['res'].fields.append(
   _ATTRIBUTETYPE_GET_RES.fields_by_name['attribute'])
 _ATTRIBUTETYPE_GET_RES.fields_by_name['attribute'].containing_oneof = _ATTRIBUTETYPE_GET_RES.oneofs_by_name['res']
 _ATTRIBUTETYPE_GET.containing_type = _ATTRIBUTETYPE
 _ATTRIBUTETYPE_GETOWNERS_REQ.containing_type = _ATTRIBUTETYPE_GETOWNERS
-_ATTRIBUTETYPE_GETOWNERS_RESPART.fields_by_name['owners'].message_type = _TYPE
+_ATTRIBUTETYPE_GETOWNERS_RESPART.fields_by_name['thing_types'].message_type = _TYPE
 _ATTRIBUTETYPE_GETOWNERS_RESPART.containing_type = _ATTRIBUTETYPE_GETOWNERS
 _ATTRIBUTETYPE_GETOWNERS.containing_type = _ATTRIBUTETYPE
+_ATTRIBUTETYPE_GETOWNERSEXPLICIT_REQ.containing_type = _ATTRIBUTETYPE_GETOWNERSEXPLICIT
+_ATTRIBUTETYPE_GETOWNERSEXPLICIT_RESPART.fields_by_name['thing_types'].message_type = _TYPE
+_ATTRIBUTETYPE_GETOWNERSEXPLICIT_RESPART.containing_type = _ATTRIBUTETYPE_GETOWNERSEXPLICIT
+_ATTRIBUTETYPE_GETOWNERSEXPLICIT.containing_type = _ATTRIBUTETYPE
 _ATTRIBUTETYPE_GETREGEX_REQ.containing_type = _ATTRIBUTETYPE_GETREGEX
 _ATTRIBUTETYPE_GETREGEX_RES.containing_type = _ATTRIBUTETYPE_GETREGEX
 _ATTRIBUTETYPE_GETREGEX.containing_type = _ATTRIBUTETYPE
 _ATTRIBUTETYPE_SETREGEX_REQ.containing_type = _ATTRIBUTETYPE_SETREGEX
 _ATTRIBUTETYPE_SETREGEX_RES.containing_type = _ATTRIBUTETYPE_SETREGEX
 _ATTRIBUTETYPE_SETREGEX.containing_type = _ATTRIBUTETYPE
 _ATTRIBUTETYPE_GETSUBTYPES_REQ.fields_by_name['value_type'].enum_type = _ATTRIBUTETYPE_VALUETYPE
 _ATTRIBUTETYPE_GETSUBTYPES_REQ.containing_type = _ATTRIBUTETYPE_GETSUBTYPES
 _ATTRIBUTETYPE_GETSUBTYPES_REQ.oneofs_by_name['req'].fields.append(
   _ATTRIBUTETYPE_GETSUBTYPES_REQ.fields_by_name['value_type'])
 _ATTRIBUTETYPE_GETSUBTYPES_REQ.fields_by_name['value_type'].containing_oneof = _ATTRIBUTETYPE_GETSUBTYPES_REQ.oneofs_by_name['req']
-_ATTRIBUTETYPE_GETSUBTYPES_RESPART.fields_by_name['types'].message_type = _TYPE
+_ATTRIBUTETYPE_GETSUBTYPES_RESPART.fields_by_name['attribute_types'].message_type = _TYPE
 _ATTRIBUTETYPE_GETSUBTYPES_RESPART.containing_type = _ATTRIBUTETYPE_GETSUBTYPES
 _ATTRIBUTETYPE_GETSUBTYPES.containing_type = _ATTRIBUTETYPE
 _ATTRIBUTETYPE_GETINSTANCES_REQ.fields_by_name['value_type'].enum_type = _ATTRIBUTETYPE_VALUETYPE
 _ATTRIBUTETYPE_GETINSTANCES_REQ.containing_type = _ATTRIBUTETYPE_GETINSTANCES
 _ATTRIBUTETYPE_GETINSTANCES_REQ.oneofs_by_name['req'].fields.append(
   _ATTRIBUTETYPE_GETINSTANCES_REQ.fields_by_name['value_type'])
 _ATTRIBUTETYPE_GETINSTANCES_REQ.fields_by_name['value_type'].containing_oneof = _ATTRIBUTETYPE_GETINSTANCES_REQ.oneofs_by_name['req']
-_ATTRIBUTETYPE_GETINSTANCES_RESPART.fields_by_name['things'].message_type = _THING
+_ATTRIBUTETYPE_GETINSTANCES_RESPART.fields_by_name['attributes'].message_type = _THING
 _ATTRIBUTETYPE_GETINSTANCES_RESPART.containing_type = _ATTRIBUTETYPE_GETINSTANCES
 _ATTRIBUTETYPE_GETINSTANCES.containing_type = _ATTRIBUTETYPE
 _ATTRIBUTETYPE_VALUETYPE.containing_type = _ATTRIBUTETYPE
 DESCRIPTOR.message_types_by_name['ConceptManager'] = _CONCEPTMANAGER
 DESCRIPTOR.message_types_by_name['Concept'] = _CONCEPT
 DESCRIPTOR.message_types_by_name['Thing'] = _THING
 DESCRIPTOR.message_types_by_name['Relation'] = _RELATION
@@ -6688,14 +7675,35 @@
       ))
     ,
     DESCRIPTOR = _TYPE_GETSUBTYPES,
     __module__ = 'common.concept_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.Type.GetSubtypes)
     ))
   ,
+
+  GetSubtypesExplicit = _reflection.GeneratedProtocolMessageType('GetSubtypesExplicit', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _TYPE_GETSUBTYPESEXPLICIT_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.Type.GetSubtypesExplicit.Req)
+      ))
+    ,
+
+    ResPart = _reflection.GeneratedProtocolMessageType('ResPart', (_message.Message,), dict(
+      DESCRIPTOR = _TYPE_GETSUBTYPESEXPLICIT_RESPART,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.Type.GetSubtypesExplicit.ResPart)
+      ))
+    ,
+    DESCRIPTOR = _TYPE_GETSUBTYPESEXPLICIT,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.Type.GetSubtypesExplicit)
+    ))
+  ,
   DESCRIPTOR = _TYPE,
   __module__ = 'common.concept_pb2'
   # @@protoc_insertion_point(class_scope:typedb.protocol.Type)
   ))
 _sym_db.RegisterMessage(Type)
 _sym_db.RegisterMessage(Type.Req)
 _sym_db.RegisterMessage(Type.Res)
@@ -6717,14 +7725,17 @@
 _sym_db.RegisterMessage(Type.SetSupertype.Res)
 _sym_db.RegisterMessage(Type.GetSupertypes)
 _sym_db.RegisterMessage(Type.GetSupertypes.Req)
 _sym_db.RegisterMessage(Type.GetSupertypes.ResPart)
 _sym_db.RegisterMessage(Type.GetSubtypes)
 _sym_db.RegisterMessage(Type.GetSubtypes.Req)
 _sym_db.RegisterMessage(Type.GetSubtypes.ResPart)
+_sym_db.RegisterMessage(Type.GetSubtypesExplicit)
+_sym_db.RegisterMessage(Type.GetSubtypesExplicit.Req)
+_sym_db.RegisterMessage(Type.GetSubtypesExplicit.ResPart)
 
 RoleType = _reflection.GeneratedProtocolMessageType('RoleType', (_message.Message,), dict(
 
   GetRelationTypes = _reflection.GeneratedProtocolMessageType('GetRelationTypes', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _ROLETYPE_GETRELATIONTYPES_REQ,
@@ -6838,14 +7849,35 @@
     ,
     DESCRIPTOR = _THINGTYPE_GETINSTANCES,
     __module__ = 'common.concept_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetInstances)
     ))
   ,
 
+  GetInstancesExplicit = _reflection.GeneratedProtocolMessageType('GetInstancesExplicit', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETINSTANCESEXPLICIT_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetInstancesExplicit.Req)
+      ))
+    ,
+
+    ResPart = _reflection.GeneratedProtocolMessageType('ResPart', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETINSTANCESEXPLICIT_RESPART,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetInstancesExplicit.ResPart)
+      ))
+    ,
+    DESCRIPTOR = _THINGTYPE_GETINSTANCESEXPLICIT,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetInstancesExplicit)
+    ))
+  ,
+
   GetOwns = _reflection.GeneratedProtocolMessageType('GetOwns', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _THINGTYPE_GETOWNS_REQ,
       __module__ = 'common.concept_pb2'
       # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwns.Req)
       ))
@@ -6859,74 +7891,74 @@
     ,
     DESCRIPTOR = _THINGTYPE_GETOWNS,
     __module__ = 'common.concept_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwns)
     ))
   ,
 
-  GetPlays = _reflection.GeneratedProtocolMessageType('GetPlays', (_message.Message,), dict(
+  GetOwnsExplicit = _reflection.GeneratedProtocolMessageType('GetOwnsExplicit', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
-      DESCRIPTOR = _THINGTYPE_GETPLAYS_REQ,
+      DESCRIPTOR = _THINGTYPE_GETOWNSEXPLICIT_REQ,
       __module__ = 'common.concept_pb2'
-      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlays.Req)
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwnsExplicit.Req)
       ))
     ,
 
     ResPart = _reflection.GeneratedProtocolMessageType('ResPart', (_message.Message,), dict(
-      DESCRIPTOR = _THINGTYPE_GETPLAYS_RESPART,
+      DESCRIPTOR = _THINGTYPE_GETOWNSEXPLICIT_RESPART,
       __module__ = 'common.concept_pb2'
-      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlays.ResPart)
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwnsExplicit.ResPart)
       ))
     ,
-    DESCRIPTOR = _THINGTYPE_GETPLAYS,
+    DESCRIPTOR = _THINGTYPE_GETOWNSEXPLICIT,
     __module__ = 'common.concept_pb2'
-    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlays)
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwnsExplicit)
     ))
   ,
 
-  SetOwns = _reflection.GeneratedProtocolMessageType('SetOwns', (_message.Message,), dict(
+  GetOwnsOverridden = _reflection.GeneratedProtocolMessageType('GetOwnsOverridden', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
-      DESCRIPTOR = _THINGTYPE_SETOWNS_REQ,
+      DESCRIPTOR = _THINGTYPE_GETOWNSOVERRIDDEN_REQ,
       __module__ = 'common.concept_pb2'
-      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetOwns.Req)
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwnsOverridden.Req)
       ))
     ,
 
     Res = _reflection.GeneratedProtocolMessageType('Res', (_message.Message,), dict(
-      DESCRIPTOR = _THINGTYPE_SETOWNS_RES,
+      DESCRIPTOR = _THINGTYPE_GETOWNSOVERRIDDEN_RES,
       __module__ = 'common.concept_pb2'
-      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetOwns.Res)
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwnsOverridden.Res)
       ))
     ,
-    DESCRIPTOR = _THINGTYPE_SETOWNS,
+    DESCRIPTOR = _THINGTYPE_GETOWNSOVERRIDDEN,
     __module__ = 'common.concept_pb2'
-    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetOwns)
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetOwnsOverridden)
     ))
   ,
 
-  SetPlays = _reflection.GeneratedProtocolMessageType('SetPlays', (_message.Message,), dict(
+  SetOwns = _reflection.GeneratedProtocolMessageType('SetOwns', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
-      DESCRIPTOR = _THINGTYPE_SETPLAYS_REQ,
+      DESCRIPTOR = _THINGTYPE_SETOWNS_REQ,
       __module__ = 'common.concept_pb2'
-      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetPlays.Req)
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetOwns.Req)
       ))
     ,
 
     Res = _reflection.GeneratedProtocolMessageType('Res', (_message.Message,), dict(
-      DESCRIPTOR = _THINGTYPE_SETPLAYS_RES,
+      DESCRIPTOR = _THINGTYPE_SETOWNS_RES,
       __module__ = 'common.concept_pb2'
-      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetPlays.Res)
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetOwns.Res)
       ))
     ,
-    DESCRIPTOR = _THINGTYPE_SETPLAYS,
+    DESCRIPTOR = _THINGTYPE_SETOWNS,
     __module__ = 'common.concept_pb2'
-    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetPlays)
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetOwns)
     ))
   ,
 
   UnsetOwns = _reflection.GeneratedProtocolMessageType('UnsetOwns', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _THINGTYPE_UNSETOWNS_REQ,
@@ -6943,14 +7975,98 @@
     ,
     DESCRIPTOR = _THINGTYPE_UNSETOWNS,
     __module__ = 'common.concept_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.UnsetOwns)
     ))
   ,
 
+  GetPlays = _reflection.GeneratedProtocolMessageType('GetPlays', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETPLAYS_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlays.Req)
+      ))
+    ,
+
+    ResPart = _reflection.GeneratedProtocolMessageType('ResPart', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETPLAYS_RESPART,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlays.ResPart)
+      ))
+    ,
+    DESCRIPTOR = _THINGTYPE_GETPLAYS,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlays)
+    ))
+  ,
+
+  GetPlaysExplicit = _reflection.GeneratedProtocolMessageType('GetPlaysExplicit', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETPLAYSEXPLICIT_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlaysExplicit.Req)
+      ))
+    ,
+
+    ResPart = _reflection.GeneratedProtocolMessageType('ResPart', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETPLAYSEXPLICIT_RESPART,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlaysExplicit.ResPart)
+      ))
+    ,
+    DESCRIPTOR = _THINGTYPE_GETPLAYSEXPLICIT,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlaysExplicit)
+    ))
+  ,
+
+  GetPlaysOverridden = _reflection.GeneratedProtocolMessageType('GetPlaysOverridden', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETPLAYSOVERRIDDEN_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlaysOverridden.Req)
+      ))
+    ,
+
+    Res = _reflection.GeneratedProtocolMessageType('Res', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_GETPLAYSOVERRIDDEN_RES,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlaysOverridden.Res)
+      ))
+    ,
+    DESCRIPTOR = _THINGTYPE_GETPLAYSOVERRIDDEN,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.GetPlaysOverridden)
+    ))
+  ,
+
+  SetPlays = _reflection.GeneratedProtocolMessageType('SetPlays', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_SETPLAYS_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetPlays.Req)
+      ))
+    ,
+
+    Res = _reflection.GeneratedProtocolMessageType('Res', (_message.Message,), dict(
+      DESCRIPTOR = _THINGTYPE_SETPLAYS_RES,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetPlays.Res)
+      ))
+    ,
+    DESCRIPTOR = _THINGTYPE_SETPLAYS,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.SetPlays)
+    ))
+  ,
+
   UnsetPlays = _reflection.GeneratedProtocolMessageType('UnsetPlays', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _THINGTYPE_UNSETPLAYS_REQ,
       __module__ = 'common.concept_pb2'
       # @@protoc_insertion_point(class_scope:typedb.protocol.ThingType.UnsetPlays.Req)
       ))
@@ -6977,29 +8093,44 @@
 _sym_db.RegisterMessage(ThingType.SetAbstract.Res)
 _sym_db.RegisterMessage(ThingType.UnsetAbstract)
 _sym_db.RegisterMessage(ThingType.UnsetAbstract.Req)
 _sym_db.RegisterMessage(ThingType.UnsetAbstract.Res)
 _sym_db.RegisterMessage(ThingType.GetInstances)
 _sym_db.RegisterMessage(ThingType.GetInstances.Req)
 _sym_db.RegisterMessage(ThingType.GetInstances.ResPart)
+_sym_db.RegisterMessage(ThingType.GetInstancesExplicit)
+_sym_db.RegisterMessage(ThingType.GetInstancesExplicit.Req)
+_sym_db.RegisterMessage(ThingType.GetInstancesExplicit.ResPart)
 _sym_db.RegisterMessage(ThingType.GetOwns)
 _sym_db.RegisterMessage(ThingType.GetOwns.Req)
 _sym_db.RegisterMessage(ThingType.GetOwns.ResPart)
-_sym_db.RegisterMessage(ThingType.GetPlays)
-_sym_db.RegisterMessage(ThingType.GetPlays.Req)
-_sym_db.RegisterMessage(ThingType.GetPlays.ResPart)
+_sym_db.RegisterMessage(ThingType.GetOwnsExplicit)
+_sym_db.RegisterMessage(ThingType.GetOwnsExplicit.Req)
+_sym_db.RegisterMessage(ThingType.GetOwnsExplicit.ResPart)
+_sym_db.RegisterMessage(ThingType.GetOwnsOverridden)
+_sym_db.RegisterMessage(ThingType.GetOwnsOverridden.Req)
+_sym_db.RegisterMessage(ThingType.GetOwnsOverridden.Res)
 _sym_db.RegisterMessage(ThingType.SetOwns)
 _sym_db.RegisterMessage(ThingType.SetOwns.Req)
 _sym_db.RegisterMessage(ThingType.SetOwns.Res)
-_sym_db.RegisterMessage(ThingType.SetPlays)
-_sym_db.RegisterMessage(ThingType.SetPlays.Req)
-_sym_db.RegisterMessage(ThingType.SetPlays.Res)
 _sym_db.RegisterMessage(ThingType.UnsetOwns)
 _sym_db.RegisterMessage(ThingType.UnsetOwns.Req)
 _sym_db.RegisterMessage(ThingType.UnsetOwns.Res)
+_sym_db.RegisterMessage(ThingType.GetPlays)
+_sym_db.RegisterMessage(ThingType.GetPlays.Req)
+_sym_db.RegisterMessage(ThingType.GetPlays.ResPart)
+_sym_db.RegisterMessage(ThingType.GetPlaysExplicit)
+_sym_db.RegisterMessage(ThingType.GetPlaysExplicit.Req)
+_sym_db.RegisterMessage(ThingType.GetPlaysExplicit.ResPart)
+_sym_db.RegisterMessage(ThingType.GetPlaysOverridden)
+_sym_db.RegisterMessage(ThingType.GetPlaysOverridden.Req)
+_sym_db.RegisterMessage(ThingType.GetPlaysOverridden.Res)
+_sym_db.RegisterMessage(ThingType.SetPlays)
+_sym_db.RegisterMessage(ThingType.SetPlays.Req)
+_sym_db.RegisterMessage(ThingType.SetPlays.Res)
 _sym_db.RegisterMessage(ThingType.UnsetPlays)
 _sym_db.RegisterMessage(ThingType.UnsetPlays.Req)
 _sym_db.RegisterMessage(ThingType.UnsetPlays.Res)
 
 EntityType = _reflection.GeneratedProtocolMessageType('EntityType', (_message.Message,), dict(
 
   Create = _reflection.GeneratedProtocolMessageType('Create', (_message.Message,), dict(
@@ -7071,14 +8202,35 @@
     ,
     DESCRIPTOR = _RELATIONTYPE_GETRELATES,
     __module__ = 'common.concept_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelates)
     ))
   ,
 
+  GetRelatesExplicit = _reflection.GeneratedProtocolMessageType('GetRelatesExplicit', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _RELATIONTYPE_GETRELATESEXPLICIT_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesExplicit.Req)
+      ))
+    ,
+
+    ResPart = _reflection.GeneratedProtocolMessageType('ResPart', (_message.Message,), dict(
+      DESCRIPTOR = _RELATIONTYPE_GETRELATESEXPLICIT_RESPART,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesExplicit.ResPart)
+      ))
+    ,
+    DESCRIPTOR = _RELATIONTYPE_GETRELATESEXPLICIT,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesExplicit)
+    ))
+  ,
+
   GetRelatesForRoleLabel = _reflection.GeneratedProtocolMessageType('GetRelatesForRoleLabel', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _RELATIONTYPE_GETRELATESFORROLELABEL_REQ,
       __module__ = 'common.concept_pb2'
       # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesForRoleLabel.Req)
       ))
@@ -7092,14 +8244,35 @@
     ,
     DESCRIPTOR = _RELATIONTYPE_GETRELATESFORROLELABEL,
     __module__ = 'common.concept_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesForRoleLabel)
     ))
   ,
 
+  GetRelatesOverridden = _reflection.GeneratedProtocolMessageType('GetRelatesOverridden', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _RELATIONTYPE_GETRELATESOVERRIDDEN_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesOverridden.Req)
+      ))
+    ,
+
+    Res = _reflection.GeneratedProtocolMessageType('Res', (_message.Message,), dict(
+      DESCRIPTOR = _RELATIONTYPE_GETRELATESOVERRIDDEN_RES,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesOverridden.Res)
+      ))
+    ,
+    DESCRIPTOR = _RELATIONTYPE_GETRELATESOVERRIDDEN,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.GetRelatesOverridden)
+    ))
+  ,
+
   SetRelates = _reflection.GeneratedProtocolMessageType('SetRelates', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _RELATIONTYPE_SETRELATES_REQ,
       __module__ = 'common.concept_pb2'
       # @@protoc_insertion_point(class_scope:typedb.protocol.RelationType.SetRelates.Req)
       ))
@@ -7144,17 +8317,23 @@
 _sym_db.RegisterMessage(RelationType)
 _sym_db.RegisterMessage(RelationType.Create)
 _sym_db.RegisterMessage(RelationType.Create.Req)
 _sym_db.RegisterMessage(RelationType.Create.Res)
 _sym_db.RegisterMessage(RelationType.GetRelates)
 _sym_db.RegisterMessage(RelationType.GetRelates.Req)
 _sym_db.RegisterMessage(RelationType.GetRelates.ResPart)
+_sym_db.RegisterMessage(RelationType.GetRelatesExplicit)
+_sym_db.RegisterMessage(RelationType.GetRelatesExplicit.Req)
+_sym_db.RegisterMessage(RelationType.GetRelatesExplicit.ResPart)
 _sym_db.RegisterMessage(RelationType.GetRelatesForRoleLabel)
 _sym_db.RegisterMessage(RelationType.GetRelatesForRoleLabel.Req)
 _sym_db.RegisterMessage(RelationType.GetRelatesForRoleLabel.Res)
+_sym_db.RegisterMessage(RelationType.GetRelatesOverridden)
+_sym_db.RegisterMessage(RelationType.GetRelatesOverridden.Req)
+_sym_db.RegisterMessage(RelationType.GetRelatesOverridden.Res)
 _sym_db.RegisterMessage(RelationType.SetRelates)
 _sym_db.RegisterMessage(RelationType.SetRelates.Req)
 _sym_db.RegisterMessage(RelationType.SetRelates.Res)
 _sym_db.RegisterMessage(RelationType.UnsetRelates)
 _sym_db.RegisterMessage(RelationType.UnsetRelates.Req)
 _sym_db.RegisterMessage(RelationType.UnsetRelates.Res)
 
@@ -7219,14 +8398,35 @@
     ,
     DESCRIPTOR = _ATTRIBUTETYPE_GETOWNERS,
     __module__ = 'common.concept_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.AttributeType.GetOwners)
     ))
   ,
 
+  GetOwnersExplicit = _reflection.GeneratedProtocolMessageType('GetOwnersExplicit', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _ATTRIBUTETYPE_GETOWNERSEXPLICIT_REQ,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.AttributeType.GetOwnersExplicit.Req)
+      ))
+    ,
+
+    ResPart = _reflection.GeneratedProtocolMessageType('ResPart', (_message.Message,), dict(
+      DESCRIPTOR = _ATTRIBUTETYPE_GETOWNERSEXPLICIT_RESPART,
+      __module__ = 'common.concept_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.AttributeType.GetOwnersExplicit.ResPart)
+      ))
+    ,
+    DESCRIPTOR = _ATTRIBUTETYPE_GETOWNERSEXPLICIT,
+    __module__ = 'common.concept_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.AttributeType.GetOwnersExplicit)
+    ))
+  ,
+
   GetRegex = _reflection.GeneratedProtocolMessageType('GetRegex', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _ATTRIBUTETYPE_GETREGEX_REQ,
       __module__ = 'common.concept_pb2'
       # @@protoc_insertion_point(class_scope:typedb.protocol.AttributeType.GetRegex.Req)
       ))
@@ -7316,14 +8516,17 @@
 _sym_db.RegisterMessage(AttributeType.Put.Res)
 _sym_db.RegisterMessage(AttributeType.Get)
 _sym_db.RegisterMessage(AttributeType.Get.Req)
 _sym_db.RegisterMessage(AttributeType.Get.Res)
 _sym_db.RegisterMessage(AttributeType.GetOwners)
 _sym_db.RegisterMessage(AttributeType.GetOwners.Req)
 _sym_db.RegisterMessage(AttributeType.GetOwners.ResPart)
+_sym_db.RegisterMessage(AttributeType.GetOwnersExplicit)
+_sym_db.RegisterMessage(AttributeType.GetOwnersExplicit.Req)
+_sym_db.RegisterMessage(AttributeType.GetOwnersExplicit.ResPart)
 _sym_db.RegisterMessage(AttributeType.GetRegex)
 _sym_db.RegisterMessage(AttributeType.GetRegex.Req)
 _sym_db.RegisterMessage(AttributeType.GetRegex.Res)
 _sym_db.RegisterMessage(AttributeType.SetRegex)
 _sym_db.RegisterMessage(AttributeType.SetRegex.Req)
 _sym_db.RegisterMessage(AttributeType.SetRegex.Res)
 _sym_db.RegisterMessage(AttributeType.GetSubtypes)
```

### Comparing `typedb-protocol-2.6.1/typedb_protocol/common/logic_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/common/logic_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/common/answer_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/common/answer_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/common/session_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/common/session_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_server_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_server_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_user_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_user_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_database_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_database_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_service_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/cluster/cluster_service_pb2_grpc.py` & `typedb-protocol-2.9.0/typedb_protocol/cluster/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/typedb_protocol/core/core_service_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/core/core_service_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='core/core_service.proto',
   package='typedb.protocol',
   syntax='proto3',
   serialized_options=_b('\n\033com.vaticle.typedb.protocolB\020CoreServiceProto\210\001\001'),
-  serialized_pb=_b('\n\x17\x63ore/core_service.proto\x12\x0ftypedb.protocol\x1a\x18\x63ore/core_database.proto\x1a\x14\x63ommon/session.proto\x1a\x18\x63ommon/transaction.proto2\x9a\x07\n\x06TypeDB\x12z\n\x12\x64\x61tabases_contains\x12\x31.typedb.protocol.CoreDatabaseManager.Contains.Req\x1a\x31.typedb.protocol.CoreDatabaseManager.Contains.Res\x12t\n\x10\x64\x61tabases_create\x12/.typedb.protocol.CoreDatabaseManager.Create.Req\x1a/.typedb.protocol.CoreDatabaseManager.Create.Res\x12k\n\rdatabases_all\x12,.typedb.protocol.CoreDatabaseManager.All.Req\x1a,.typedb.protocol.CoreDatabaseManager.All.Res\x12\x65\n\x0f\x64\x61tabase_schema\x12(.typedb.protocol.CoreDatabase.Schema.Req\x1a(.typedb.protocol.CoreDatabase.Schema.Res\x12\x65\n\x0f\x64\x61tabase_delete\x12(.typedb.protocol.CoreDatabase.Delete.Req\x1a(.typedb.protocol.CoreDatabase.Delete.Res\x12T\n\x0csession_open\x12!.typedb.protocol.Session.Open.Req\x1a!.typedb.protocol.Session.Open.Res\x12W\n\rsession_close\x12\".typedb.protocol.Session.Close.Req\x1a\".typedb.protocol.Session.Close.Res\x12W\n\rsession_pulse\x12\".typedb.protocol.Session.Pulse.Req\x1a\".typedb.protocol.Session.Pulse.Res\x12[\n\x0btransaction\x12#.typedb.protocol.Transaction.Client\x1a#.typedb.protocol.Transaction.Server(\x01\x30\x01\x42\x32\n\x1b\x63om.vaticle.typedb.protocolB\x10\x43oreServiceProto\x88\x01\x01\x62\x06proto3')
+  serialized_pb=_b('\n\x17\x63ore/core_service.proto\x12\x0ftypedb.protocol\x1a\x18\x63ore/core_database.proto\x1a\x14\x63ommon/session.proto\x1a\x18\x63ommon/transaction.proto2\x82\t\n\x06TypeDB\x12z\n\x12\x64\x61tabases_contains\x12\x31.typedb.protocol.CoreDatabaseManager.Contains.Req\x1a\x31.typedb.protocol.CoreDatabaseManager.Contains.Res\x12t\n\x10\x64\x61tabases_create\x12/.typedb.protocol.CoreDatabaseManager.Create.Req\x1a/.typedb.protocol.CoreDatabaseManager.Create.Res\x12k\n\rdatabases_all\x12,.typedb.protocol.CoreDatabaseManager.All.Req\x1a,.typedb.protocol.CoreDatabaseManager.All.Res\x12\x65\n\x0f\x64\x61tabase_schema\x12(.typedb.protocol.CoreDatabase.Schema.Req\x1a(.typedb.protocol.CoreDatabase.Schema.Res\x12r\n\x14\x64\x61tabase_type_schema\x12,.typedb.protocol.CoreDatabase.TypeSchema.Req\x1a,.typedb.protocol.CoreDatabase.TypeSchema.Res\x12r\n\x14\x64\x61tabase_rule_schema\x12,.typedb.protocol.CoreDatabase.RuleSchema.Req\x1a,.typedb.protocol.CoreDatabase.RuleSchema.Res\x12\x65\n\x0f\x64\x61tabase_delete\x12(.typedb.protocol.CoreDatabase.Delete.Req\x1a(.typedb.protocol.CoreDatabase.Delete.Res\x12T\n\x0csession_open\x12!.typedb.protocol.Session.Open.Req\x1a!.typedb.protocol.Session.Open.Res\x12W\n\rsession_close\x12\".typedb.protocol.Session.Close.Req\x1a\".typedb.protocol.Session.Close.Res\x12W\n\rsession_pulse\x12\".typedb.protocol.Session.Pulse.Req\x1a\".typedb.protocol.Session.Pulse.Res\x12[\n\x0btransaction\x12#.typedb.protocol.Transaction.Client\x1a#.typedb.protocol.Transaction.Server(\x01\x30\x01\x42\x32\n\x1b\x63om.vaticle.typedb.protocolB\x10\x43oreServiceProto\x88\x01\x01\x62\x06proto3')
   ,
   dependencies=[core_dot_core__database__pb2.DESCRIPTOR,common_dot_session__pb2.DESCRIPTOR,common_dot_transaction__pb2.DESCRIPTOR,])
 
 
 
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
@@ -36,15 +36,15 @@
 _TYPEDB = _descriptor.ServiceDescriptor(
   name='TypeDB',
   full_name='typedb.protocol.TypeDB',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   serialized_start=119,
-  serialized_end=1041,
+  serialized_end=1273,
   methods=[
   _descriptor.MethodDescriptor(
     name='databases_contains',
     full_name='typedb.protocol.TypeDB.databases_contains',
     index=0,
     containing_service=None,
     input_type=core_dot_core__database__pb2._COREDATABASEMANAGER_CONTAINS_REQ,
@@ -75,53 +75,71 @@
     index=3,
     containing_service=None,
     input_type=core_dot_core__database__pb2._COREDATABASE_SCHEMA_REQ,
     output_type=core_dot_core__database__pb2._COREDATABASE_SCHEMA_RES,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
+    name='database_type_schema',
+    full_name='typedb.protocol.TypeDB.database_type_schema',
+    index=4,
+    containing_service=None,
+    input_type=core_dot_core__database__pb2._COREDATABASE_TYPESCHEMA_REQ,
+    output_type=core_dot_core__database__pb2._COREDATABASE_TYPESCHEMA_RES,
+    serialized_options=None,
+  ),
+  _descriptor.MethodDescriptor(
+    name='database_rule_schema',
+    full_name='typedb.protocol.TypeDB.database_rule_schema',
+    index=5,
+    containing_service=None,
+    input_type=core_dot_core__database__pb2._COREDATABASE_RULESCHEMA_REQ,
+    output_type=core_dot_core__database__pb2._COREDATABASE_RULESCHEMA_RES,
+    serialized_options=None,
+  ),
+  _descriptor.MethodDescriptor(
     name='database_delete',
     full_name='typedb.protocol.TypeDB.database_delete',
-    index=4,
+    index=6,
     containing_service=None,
     input_type=core_dot_core__database__pb2._COREDATABASE_DELETE_REQ,
     output_type=core_dot_core__database__pb2._COREDATABASE_DELETE_RES,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
     name='session_open',
     full_name='typedb.protocol.TypeDB.session_open',
-    index=5,
+    index=7,
     containing_service=None,
     input_type=common_dot_session__pb2._SESSION_OPEN_REQ,
     output_type=common_dot_session__pb2._SESSION_OPEN_RES,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
     name='session_close',
     full_name='typedb.protocol.TypeDB.session_close',
-    index=6,
+    index=8,
     containing_service=None,
     input_type=common_dot_session__pb2._SESSION_CLOSE_REQ,
     output_type=common_dot_session__pb2._SESSION_CLOSE_RES,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
     name='session_pulse',
     full_name='typedb.protocol.TypeDB.session_pulse',
-    index=7,
+    index=9,
     containing_service=None,
     input_type=common_dot_session__pb2._SESSION_PULSE_REQ,
     output_type=common_dot_session__pb2._SESSION_PULSE_RES,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
     name='transaction',
     full_name='typedb.protocol.TypeDB.transaction',
-    index=8,
+    index=10,
     containing_service=None,
     input_type=common_dot_transaction__pb2._TRANSACTION_CLIENT,
     output_type=common_dot_transaction__pb2._TRANSACTION_SERVER,
     serialized_options=None,
   ),
 ])
 _sym_db.RegisterServiceDescriptor(_TYPEDB)
```

### Comparing `typedb-protocol-2.6.1/typedb_protocol/core/core_service_pb2_grpc.py` & `typedb-protocol-2.9.0/typedb_protocol/core/core_service_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,24 @@
         response_deserializer=core_dot_core__database__pb2.CoreDatabaseManager.All.Res.FromString,
         )
     self.database_schema = channel.unary_unary(
         '/typedb.protocol.TypeDB/database_schema',
         request_serializer=core_dot_core__database__pb2.CoreDatabase.Schema.Req.SerializeToString,
         response_deserializer=core_dot_core__database__pb2.CoreDatabase.Schema.Res.FromString,
         )
+    self.database_type_schema = channel.unary_unary(
+        '/typedb.protocol.TypeDB/database_type_schema',
+        request_serializer=core_dot_core__database__pb2.CoreDatabase.TypeSchema.Req.SerializeToString,
+        response_deserializer=core_dot_core__database__pb2.CoreDatabase.TypeSchema.Res.FromString,
+        )
+    self.database_rule_schema = channel.unary_unary(
+        '/typedb.protocol.TypeDB/database_rule_schema',
+        request_serializer=core_dot_core__database__pb2.CoreDatabase.RuleSchema.Req.SerializeToString,
+        response_deserializer=core_dot_core__database__pb2.CoreDatabase.RuleSchema.Res.FromString,
+        )
     self.database_delete = channel.unary_unary(
         '/typedb.protocol.TypeDB/database_delete',
         request_serializer=core_dot_core__database__pb2.CoreDatabase.Delete.Req.SerializeToString,
         response_deserializer=core_dot_core__database__pb2.CoreDatabase.Delete.Res.FromString,
         )
     self.session_open = channel.unary_unary(
         '/typedb.protocol.TypeDB/session_open',
@@ -91,14 +101,28 @@
   def database_schema(self, request, context):
     # missing associated documentation comment in .proto file
     pass
     context.set_code(grpc.StatusCode.UNIMPLEMENTED)
     context.set_details('Method not implemented!')
     raise NotImplementedError('Method not implemented!')
 
+  def database_type_schema(self, request, context):
+    # missing associated documentation comment in .proto file
+    pass
+    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+    context.set_details('Method not implemented!')
+    raise NotImplementedError('Method not implemented!')
+
+  def database_rule_schema(self, request, context):
+    # missing associated documentation comment in .proto file
+    pass
+    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+    context.set_details('Method not implemented!')
+    raise NotImplementedError('Method not implemented!')
+
   def database_delete(self, request, context):
     # missing associated documentation comment in .proto file
     pass
     context.set_code(grpc.StatusCode.UNIMPLEMENTED)
     context.set_details('Method not implemented!')
     raise NotImplementedError('Method not implemented!')
 
@@ -149,14 +173,24 @@
           response_serializer=core_dot_core__database__pb2.CoreDatabaseManager.All.Res.SerializeToString,
       ),
       'database_schema': grpc.unary_unary_rpc_method_handler(
           servicer.database_schema,
           request_deserializer=core_dot_core__database__pb2.CoreDatabase.Schema.Req.FromString,
           response_serializer=core_dot_core__database__pb2.CoreDatabase.Schema.Res.SerializeToString,
       ),
+      'database_type_schema': grpc.unary_unary_rpc_method_handler(
+          servicer.database_type_schema,
+          request_deserializer=core_dot_core__database__pb2.CoreDatabase.TypeSchema.Req.FromString,
+          response_serializer=core_dot_core__database__pb2.CoreDatabase.TypeSchema.Res.SerializeToString,
+      ),
+      'database_rule_schema': grpc.unary_unary_rpc_method_handler(
+          servicer.database_rule_schema,
+          request_deserializer=core_dot_core__database__pb2.CoreDatabase.RuleSchema.Req.FromString,
+          response_serializer=core_dot_core__database__pb2.CoreDatabase.RuleSchema.Res.SerializeToString,
+      ),
       'database_delete': grpc.unary_unary_rpc_method_handler(
           servicer.database_delete,
           request_deserializer=core_dot_core__database__pb2.CoreDatabase.Delete.Req.FromString,
           response_serializer=core_dot_core__database__pb2.CoreDatabase.Delete.Res.SerializeToString,
       ),
       'session_open': grpc.unary_unary_rpc_method_handler(
           servicer.session_open,
```

### Comparing `typedb-protocol-2.6.1/typedb_protocol/core/core_database_pb2.py` & `typedb-protocol-2.9.0/typedb_protocol/core/core_database_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='core/core_database.proto',
   package='typedb.protocol',
   syntax='proto3',
   serialized_options=_b('\n\033com.vaticle.typedb.protocolB\021CoreDatabaseProto'),
-  serialized_pb=_b('\n\x18\x63ore/core_database.proto\x12\x0ftypedb.protocol\"\xb6\x01\n\x13\x43oreDatabaseManager\x1aH\n\x08\x43ontains\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a!\n\x03Res\x12\x1a\n\x08\x63ontains\x18\x01 \x01(\x08R\x08\x63ontains\x1a*\n\x06\x43reate\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x05\n\x03Res\x1a)\n\x03\x41ll\x1a\x05\n\x03Req\x1a\x1b\n\x03Res\x12\x14\n\x05names\x18\x01 \x03(\tR\x05names\"~\n\x0c\x43oreDatabase\x1a\x42\n\x06Schema\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x1d\n\x03Res\x12\x16\n\x06schema\x18\x01 \x01(\tR\x06schema\x1a*\n\x06\x44\x65lete\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x05\n\x03ResB0\n\x1b\x63om.vaticle.typedb.protocolB\x11\x43oreDatabaseProtob\x06proto3')
+  serialized_pb=_b('\n\x18\x63ore/core_database.proto\x12\x0ftypedb.protocol\"\xb6\x01\n\x13\x43oreDatabaseManager\x1aH\n\x08\x43ontains\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a!\n\x03Res\x12\x1a\n\x08\x63ontains\x18\x01 \x01(\x08R\x08\x63ontains\x1a*\n\x06\x43reate\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x05\n\x03Res\x1a)\n\x03\x41ll\x1a\x05\n\x03Req\x1a\x1b\n\x03Res\x12\x14\n\x05names\x18\x01 \x03(\tR\x05names\"\x8e\x02\n\x0c\x43oreDatabase\x1a\x42\n\x06Schema\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x1d\n\x03Res\x12\x16\n\x06schema\x18\x01 \x01(\tR\x06schema\x1a\x46\n\nTypeSchema\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x1d\n\x03Res\x12\x16\n\x06schema\x18\x01 \x01(\tR\x06schema\x1a\x46\n\nRuleSchema\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x1d\n\x03Res\x12\x16\n\x06schema\x18\x01 \x01(\tR\x06schema\x1a*\n\x06\x44\x65lete\x1a\x19\n\x03Req\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a\x05\n\x03ResB0\n\x1b\x63om.vaticle.typedb.protocolB\x11\x43oreDatabaseProtob\x06proto3')
 )
 
 
 
 
 _COREDATABASEMANAGER_CONTAINS_REQ = _descriptor.Descriptor(
   name='Req',
@@ -336,16 +336,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=283,
-  serialized_end=312,
+  serialized_start=284,
+  serialized_end=313,
 )
 
 _COREDATABASE_SCHEMA = _descriptor.Descriptor(
   name='Schema',
   full_name='typedb.protocol.CoreDatabase.Schema',
   filename=None,
   file=DESCRIPTOR,
@@ -359,16 +359,182 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=246,
-  serialized_end=312,
+  serialized_start=247,
+  serialized_end=313,
+)
+
+_COREDATABASE_TYPESCHEMA_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.CoreDatabase.TypeSchema.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='typedb.protocol.CoreDatabase.TypeSchema.Req.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='name', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=81,
+  serialized_end=106,
+)
+
+_COREDATABASE_TYPESCHEMA_RES = _descriptor.Descriptor(
+  name='Res',
+  full_name='typedb.protocol.CoreDatabase.TypeSchema.Res',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='schema', full_name='typedb.protocol.CoreDatabase.TypeSchema.Res.schema', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='schema', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=284,
+  serialized_end=313,
+)
+
+_COREDATABASE_TYPESCHEMA = _descriptor.Descriptor(
+  name='TypeSchema',
+  full_name='typedb.protocol.CoreDatabase.TypeSchema',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_COREDATABASE_TYPESCHEMA_REQ, _COREDATABASE_TYPESCHEMA_RES, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=315,
+  serialized_end=385,
+)
+
+_COREDATABASE_RULESCHEMA_REQ = _descriptor.Descriptor(
+  name='Req',
+  full_name='typedb.protocol.CoreDatabase.RuleSchema.Req',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='typedb.protocol.CoreDatabase.RuleSchema.Req.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='name', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=81,
+  serialized_end=106,
+)
+
+_COREDATABASE_RULESCHEMA_RES = _descriptor.Descriptor(
+  name='Res',
+  full_name='typedb.protocol.CoreDatabase.RuleSchema.Res',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='schema', full_name='typedb.protocol.CoreDatabase.RuleSchema.Res.schema', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='schema', file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=284,
+  serialized_end=313,
+)
+
+_COREDATABASE_RULESCHEMA = _descriptor.Descriptor(
+  name='RuleSchema',
+  full_name='typedb.protocol.CoreDatabase.RuleSchema',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[_COREDATABASE_RULESCHEMA_REQ, _COREDATABASE_RULESCHEMA_RES, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=387,
+  serialized_end=457,
 )
 
 _COREDATABASE_DELETE_REQ = _descriptor.Descriptor(
   name='Req',
   full_name='typedb.protocol.CoreDatabase.Delete.Req',
   filename=None,
   file=DESCRIPTOR,
@@ -435,53 +601,59 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=314,
-  serialized_end=356,
+  serialized_start=459,
+  serialized_end=501,
 )
 
 _COREDATABASE = _descriptor.Descriptor(
   name='CoreDatabase',
   full_name='typedb.protocol.CoreDatabase',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
   ],
   extensions=[
   ],
-  nested_types=[_COREDATABASE_SCHEMA, _COREDATABASE_DELETE, ],
+  nested_types=[_COREDATABASE_SCHEMA, _COREDATABASE_TYPESCHEMA, _COREDATABASE_RULESCHEMA, _COREDATABASE_DELETE, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=230,
-  serialized_end=356,
+  serialized_start=231,
+  serialized_end=501,
 )
 
 _COREDATABASEMANAGER_CONTAINS_REQ.containing_type = _COREDATABASEMANAGER_CONTAINS
 _COREDATABASEMANAGER_CONTAINS_RES.containing_type = _COREDATABASEMANAGER_CONTAINS
 _COREDATABASEMANAGER_CONTAINS.containing_type = _COREDATABASEMANAGER
 _COREDATABASEMANAGER_CREATE_REQ.containing_type = _COREDATABASEMANAGER_CREATE
 _COREDATABASEMANAGER_CREATE_RES.containing_type = _COREDATABASEMANAGER_CREATE
 _COREDATABASEMANAGER_CREATE.containing_type = _COREDATABASEMANAGER
 _COREDATABASEMANAGER_ALL_REQ.containing_type = _COREDATABASEMANAGER_ALL
 _COREDATABASEMANAGER_ALL_RES.containing_type = _COREDATABASEMANAGER_ALL
 _COREDATABASEMANAGER_ALL.containing_type = _COREDATABASEMANAGER
 _COREDATABASE_SCHEMA_REQ.containing_type = _COREDATABASE_SCHEMA
 _COREDATABASE_SCHEMA_RES.containing_type = _COREDATABASE_SCHEMA
 _COREDATABASE_SCHEMA.containing_type = _COREDATABASE
+_COREDATABASE_TYPESCHEMA_REQ.containing_type = _COREDATABASE_TYPESCHEMA
+_COREDATABASE_TYPESCHEMA_RES.containing_type = _COREDATABASE_TYPESCHEMA
+_COREDATABASE_TYPESCHEMA.containing_type = _COREDATABASE
+_COREDATABASE_RULESCHEMA_REQ.containing_type = _COREDATABASE_RULESCHEMA
+_COREDATABASE_RULESCHEMA_RES.containing_type = _COREDATABASE_RULESCHEMA
+_COREDATABASE_RULESCHEMA.containing_type = _COREDATABASE
 _COREDATABASE_DELETE_REQ.containing_type = _COREDATABASE_DELETE
 _COREDATABASE_DELETE_RES.containing_type = _COREDATABASE_DELETE
 _COREDATABASE_DELETE.containing_type = _COREDATABASE
 DESCRIPTOR.message_types_by_name['CoreDatabaseManager'] = _COREDATABASEMANAGER
 DESCRIPTOR.message_types_by_name['CoreDatabase'] = _COREDATABASE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
@@ -583,14 +755,56 @@
     ,
     DESCRIPTOR = _COREDATABASE_SCHEMA,
     __module__ = 'core.core_database_pb2'
     # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.Schema)
     ))
   ,
 
+  TypeSchema = _reflection.GeneratedProtocolMessageType('TypeSchema', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _COREDATABASE_TYPESCHEMA_REQ,
+      __module__ = 'core.core_database_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.TypeSchema.Req)
+      ))
+    ,
+
+    Res = _reflection.GeneratedProtocolMessageType('Res', (_message.Message,), dict(
+      DESCRIPTOR = _COREDATABASE_TYPESCHEMA_RES,
+      __module__ = 'core.core_database_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.TypeSchema.Res)
+      ))
+    ,
+    DESCRIPTOR = _COREDATABASE_TYPESCHEMA,
+    __module__ = 'core.core_database_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.TypeSchema)
+    ))
+  ,
+
+  RuleSchema = _reflection.GeneratedProtocolMessageType('RuleSchema', (_message.Message,), dict(
+
+    Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
+      DESCRIPTOR = _COREDATABASE_RULESCHEMA_REQ,
+      __module__ = 'core.core_database_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.RuleSchema.Req)
+      ))
+    ,
+
+    Res = _reflection.GeneratedProtocolMessageType('Res', (_message.Message,), dict(
+      DESCRIPTOR = _COREDATABASE_RULESCHEMA_RES,
+      __module__ = 'core.core_database_pb2'
+      # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.RuleSchema.Res)
+      ))
+    ,
+    DESCRIPTOR = _COREDATABASE_RULESCHEMA,
+    __module__ = 'core.core_database_pb2'
+    # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.RuleSchema)
+    ))
+  ,
+
   Delete = _reflection.GeneratedProtocolMessageType('Delete', (_message.Message,), dict(
 
     Req = _reflection.GeneratedProtocolMessageType('Req', (_message.Message,), dict(
       DESCRIPTOR = _COREDATABASE_DELETE_REQ,
       __module__ = 'core.core_database_pb2'
       # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase.Delete.Req)
       ))
@@ -611,14 +825,20 @@
   __module__ = 'core.core_database_pb2'
   # @@protoc_insertion_point(class_scope:typedb.protocol.CoreDatabase)
   ))
 _sym_db.RegisterMessage(CoreDatabase)
 _sym_db.RegisterMessage(CoreDatabase.Schema)
 _sym_db.RegisterMessage(CoreDatabase.Schema.Req)
 _sym_db.RegisterMessage(CoreDatabase.Schema.Res)
+_sym_db.RegisterMessage(CoreDatabase.TypeSchema)
+_sym_db.RegisterMessage(CoreDatabase.TypeSchema.Req)
+_sym_db.RegisterMessage(CoreDatabase.TypeSchema.Res)
+_sym_db.RegisterMessage(CoreDatabase.RuleSchema)
+_sym_db.RegisterMessage(CoreDatabase.RuleSchema.Req)
+_sym_db.RegisterMessage(CoreDatabase.RuleSchema.Res)
 _sym_db.RegisterMessage(CoreDatabase.Delete)
 _sym_db.RegisterMessage(CoreDatabase.Delete.Req)
 _sym_db.RegisterMessage(CoreDatabase.Delete.Res)
 
 
 DESCRIPTOR._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `typedb-protocol-2.6.1/typedb_protocol.egg-info/PKG-INFO` & `typedb-protocol-2.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,15 @@
 Metadata-Version: 2.1
 Name: typedb-protocol
-Version: 2.6.1
+Version: 2.9.0
 Summary: TypeDB Protocol
 Home-page: https://github.com/vaticle/typedb-protocol/
 Author: Vaticle
 Author-email: community@vaticle.com
 License: AGPL-3.0
-Description: # TypeDB Client RPC (Remote Procedure Call) Protocol
-        
-        A protocol for implementing a TypeDB client driver, in many popular programming languages, using [GRPC (Google's Remote Procedure Call)](https://grpc.io) framework.
-        
-        ---
-        
-        ## Licensing
-        
-        The TypeDB protocol is distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
-        
-        Exception to AGPL 3.0: Any driver or client library (in each case) that implements the TypeDB protocol, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeDB software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
-        
-        - The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
-        - The MIT License: https://opensource.org/licenses/MIT
-        - The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
-        
-        As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Limited.
-        
-        If you make any change to, or contribute to, (in each case) the TypeDB protocol, then this exception will apply to any driver or client library that uses or implements that change/contribution.
-        
 Keywords: typedb typeql type-system strongly-typed database knowledge-base
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -37,7 +17,29 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
+
+# TypeDB Client RPC (Remote Procedure Call) Protocol
+
+A protocol for implementing a TypeDB client driver, in many popular programming languages, using [GRPC (Google's Remote Procedure Call)](https://grpc.io) framework.
+
+---
+
+## Licensing
+
+The TypeDB protocol is distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
+
+Exception to AGPL 3.0: Any driver or client library (in each case) that implements the TypeDB protocol, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeDB software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
+
+- The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
+- The MIT License: https://opensource.org/licenses/MIT
+- The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
+
+As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Limited.
+
+If you make any change to, or contribute to, (in each case) the TypeDB protocol, then this exception will apply to any driver or client library that uses or implements that change/contribution.
+
+
```

### Comparing `typedb-protocol-2.6.1/typedb_protocol.egg-info/SOURCES.txt` & `typedb-protocol-2.9.0/typedb_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/PKG-INFO` & `typedb-protocol-2.9.0/typedb_protocol.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,15 @@
 Metadata-Version: 2.1
 Name: typedb-protocol
-Version: 2.6.1
+Version: 2.9.0
 Summary: TypeDB Protocol
 Home-page: https://github.com/vaticle/typedb-protocol/
 Author: Vaticle
 Author-email: community@vaticle.com
 License: AGPL-3.0
-Description: # TypeDB Client RPC (Remote Procedure Call) Protocol
-        
-        A protocol for implementing a TypeDB client driver, in many popular programming languages, using [GRPC (Google's Remote Procedure Call)](https://grpc.io) framework.
-        
-        ---
-        
-        ## Licensing
-        
-        The TypeDB protocol is distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
-        
-        Exception to AGPL 3.0: Any driver or client library (in each case) that implements the TypeDB protocol, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeDB software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
-        
-        - The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
-        - The MIT License: https://opensource.org/licenses/MIT
-        - The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
-        
-        As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Limited.
-        
-        If you make any change to, or contribute to, (in each case) the TypeDB protocol, then this exception will apply to any driver or client library that uses or implements that change/contribution.
-        
 Keywords: typedb typeql type-system strongly-typed database knowledge-base
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -37,7 +17,29 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
+
+# TypeDB Client RPC (Remote Procedure Call) Protocol
+
+A protocol for implementing a TypeDB client driver, in many popular programming languages, using [GRPC (Google's Remote Procedure Call)](https://grpc.io) framework.
+
+---
+
+## Licensing
+
+The TypeDB protocol is distributed under the terms GNU Affero General Public License v3.0 ("AGPL 3.0") as published by the Free Software Foundation, but with the following special exception.
+
+Exception to AGPL 3.0: Any driver or client library (in each case) that implements the TypeDB protocol, and that is used to communicate or interact (in each case) with a database created or managed or accessed (in each case) using a version of the TypeDB software that is made available by or on behalf of Vaticle Limited (UK Company Number 08766237) or any successor entity (but excluding any forked version of that software), may be distributed under one of the following licences:
+
+- The Apache License version 2: https://www.apache.org/licenses/LICENSE-2.0.txt
+- The MIT License: https://opensource.org/licenses/MIT
+- The BSD License (2-Clause): https://opensource.org/licenses/BSD-2-Clause
+
+As used above "successor entity" means any entity then owning copyrights in the TypeDB software that were previously owned by Vaticle Limited.
+
+If you make any change to, or contribute to, (in each case) the TypeDB protocol, then this exception will apply to any driver or client library that uses or implements that change/contribution.
+
+
```

### Comparing `typedb-protocol-2.6.1/README.md` & `typedb-protocol-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `typedb-protocol-2.6.1/setup.py` & `typedb-protocol-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import setup
 from setuptools import find_packages
 
 packages = find_packages()
 
 setup(
     name = "typedb-protocol",
-    version = "2.6.1",
+    version = "2.9.0",
     description = "TypeDB Protocol",
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     classifiers = ["Programming Language :: Python", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)", "Operating System :: OS Independent", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "Environment :: Console", "Topic :: Database :: Front-Ends"],
     keywords = "typedb typeql type-system strongly-typed database knowledge-base",
     url = "https://github.com/vaticle/typedb-protocol/",
     author = "Vaticle",
```

