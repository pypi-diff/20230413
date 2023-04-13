# Comparing `tmp/azure-storage-blob-2.0.1.tar.gz` & `tmp/azure-storage-blob-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../dist/azure-storage-blob-2.0.1.tar", last modified: Thu May  9 19:54:07 2019, max compression
+gzip compressed data, was "../dist/azure-storage-blob-2.1.0.tar", last modified: Fri Aug  2 04:12:45 2019, max compression
```

## Comparing `azure-storage-blob-2.0.1.tar` & `azure-storage-blob-2.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/
--rw-r--r--   0 zed        (501) staff       (20)     1075 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/LICENSE.txt
--rw-r--r--   0 zed        (501) staff       (20)       94 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/MANIFEST.in
--rw-r--r--   0 zed        (501) staff       (20)     9755 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/PKG-INFO
--rw-r--r--   0 zed        (501) staff       (20)     7067 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/README.rst
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure/
--rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/azure/__init__.py
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure/storage/
--rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/azure/storage/__init__.py
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure/storage/blob/
--rw-r--r--   0 zed        (501) staff       (20)      888 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/azure/storage/blob/__init__.py
--rw-r--r--   0 zed        (501) staff       (20)      562 2019-05-09 19:45:45.000000 azure-storage-blob-2.0.1/azure/storage/blob/_constants.py
--rw-r--r--   0 zed        (501) staff       (20)    20674 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/_deserialization.py
--rw-r--r--   0 zed        (501) staff       (20)     7264 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/azure/storage/blob/_download_chunking.py
--rw-r--r--   0 zed        (501) staff       (20)     7169 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/azure/storage/blob/_encryption.py
--rw-r--r--   0 zed        (501) staff       (20)     1103 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/azure/storage/blob/_error.py
--rw-r--r--   0 zed        (501) staff       (20)     5254 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/_serialization.py
--rw-r--r--   0 zed        (501) staff       (20)    18855 2019-05-09 02:25:10.000000 azure-storage-blob-2.0.1/azure/storage/blob/_upload_chunking.py
--rw-r--r--   0 zed        (501) staff       (20)    41877 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/appendblobservice.py
--rw-r--r--   0 zed        (501) staff       (20)   177356 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/baseblobservice.py
--rw-r--r--   0 zed        (501) staff       (20)    61664 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/blockblobservice.py
--rw-r--r--   0 zed        (501) staff       (20)    29587 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/models.py
--rw-r--r--   0 zed        (501) staff       (20)    82060 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/pageblobservice.py
--rw-r--r--   0 zed        (501) staff       (20)    15010 2019-05-09 02:25:39.000000 azure-storage-blob-2.0.1/azure/storage/blob/sharedaccesssignature.py
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure_storage_blob.egg-info/
--rw-r--r--   0 zed        (501) staff       (20)     9755 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure_storage_blob.egg-info/PKG-INFO
--rw-r--r--   0 zed        (501) staff       (20)      858 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure_storage_blob.egg-info/SOURCES.txt
--rw-r--r--   0 zed        (501) staff       (20)        1 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure_storage_blob.egg-info/dependency_links.txt
--rw-r--r--   0 zed        (501) staff       (20)        1 2019-05-09 19:54:06.000000 azure-storage-blob-2.0.1/azure_storage_blob.egg-info/not-zip-safe
--rw-r--r--   0 zed        (501) staff       (20)       79 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure_storage_blob.egg-info/requires.txt
--rw-r--r--   0 zed        (501) staff       (20)        6 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/azure_storage_blob.egg-info/top_level.txt
--rw-r--r--   0 zed        (501) staff       (20)       67 2019-05-09 19:54:07.000000 azure-storage-blob-2.0.1/setup.cfg
--rw-r--r--   0 zed        (501) staff       (20)     2453 2019-05-09 19:45:45.000000 azure-storage-blob-2.0.1/setup.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/
+-rw-r--r--   0 zed        (501) staff       (20)     1075 2019-06-07 07:59:17.000000 azure-storage-blob-2.1.0/LICENSE.txt
+-rw-r--r--   0 zed        (501) staff       (20)       94 2019-06-07 07:59:17.000000 azure-storage-blob-2.1.0/MANIFEST.in
+-rw-r--r--   0 zed        (501) staff       (20)     9755 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/PKG-INFO
+-rw-r--r--   0 zed        (501) staff       (20)     7067 2019-05-09 02:25:10.000000 azure-storage-blob-2.1.0/README.rst
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure/
+-rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-blob-2.1.0/azure/__init__.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure/storage/
+-rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-blob-2.1.0/azure/storage/__init__.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure/storage/blob/
+-rw-r--r--   0 zed        (501) staff       (20)     1063 2019-08-01 21:38:37.000000 azure-storage-blob-2.1.0/azure/storage/blob/__init__.py
+-rw-r--r--   0 zed        (501) staff       (20)      562 2019-08-02 04:01:26.000000 azure-storage-blob-2.1.0/azure/storage/blob/_constants.py
+-rw-r--r--   0 zed        (501) staff       (20)    24384 2019-07-29 19:41:49.000000 azure-storage-blob-2.1.0/azure/storage/blob/_deserialization.py
+-rw-r--r--   0 zed        (501) staff       (20)     7347 2019-07-29 19:41:49.000000 azure-storage-blob-2.1.0/azure/storage/blob/_download_chunking.py
+-rw-r--r--   0 zed        (501) staff       (20)     7169 2019-06-07 07:59:17.000000 azure-storage-blob-2.1.0/azure/storage/blob/_encryption.py
+-rw-r--r--   0 zed        (501) staff       (20)     1103 2019-05-09 02:25:10.000000 azure-storage-blob-2.1.0/azure/storage/blob/_error.py
+-rw-r--r--   0 zed        (501) staff       (20)    10670 2019-07-29 19:41:49.000000 azure-storage-blob-2.1.0/azure/storage/blob/_serialization.py
+-rw-r--r--   0 zed        (501) staff       (20)    19067 2019-07-29 19:41:49.000000 azure-storage-blob-2.1.0/azure/storage/blob/_upload_chunking.py
+-rw-r--r--   0 zed        (501) staff       (20)    44835 2019-08-02 01:22:32.000000 azure-storage-blob-2.1.0/azure/storage/blob/appendblobservice.py
+-rw-r--r--   0 zed        (501) staff       (20)   188084 2019-08-02 04:01:06.000000 azure-storage-blob-2.1.0/azure/storage/blob/baseblobservice.py
+-rw-r--r--   0 zed        (501) staff       (20)    73061 2019-08-02 01:24:41.000000 azure-storage-blob-2.1.0/azure/storage/blob/blockblobservice.py
+-rw-r--r--   0 zed        (501) staff       (20)    36668 2019-07-29 19:41:49.000000 azure-storage-blob-2.1.0/azure/storage/blob/models.py
+-rw-r--r--   0 zed        (501) staff       (20)    85085 2019-08-02 01:24:41.000000 azure-storage-blob-2.1.0/azure/storage/blob/pageblobservice.py
+-rw-r--r--   0 zed        (501) staff       (20)    15010 2019-06-07 07:59:17.000000 azure-storage-blob-2.1.0/azure/storage/blob/sharedaccesssignature.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure_storage_blob.egg-info/
+-rw-r--r--   0 zed        (501) staff       (20)     9755 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure_storage_blob.egg-info/PKG-INFO
+-rw-r--r--   0 zed        (501) staff       (20)      858 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure_storage_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 zed        (501) staff       (20)        1 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure_storage_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 zed        (501) staff       (20)        1 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure_storage_blob.egg-info/not-zip-safe
+-rw-r--r--   0 zed        (501) staff       (20)       79 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure_storage_blob.egg-info/requires.txt
+-rw-r--r--   0 zed        (501) staff       (20)        6 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/azure_storage_blob.egg-info/top_level.txt
+-rw-r--r--   0 zed        (501) staff       (20)       67 2019-08-02 04:12:45.000000 azure-storage-blob-2.1.0/setup.cfg
+-rw-r--r--   0 zed        (501) staff       (20)     2453 2019-08-02 04:02:02.000000 azure-storage-blob-2.1.0/setup.py
```

### Comparing `azure-storage-blob-2.0.1/LICENSE.txt` & `azure-storage-blob-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azure-storage-blob-2.0.1/PKG-INFO` & `azure-storage-blob-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-storage-blob
-Version: 2.0.1
+Version: 2.1.0
 Summary: Microsoft Azure Storage Blob Client Library for Python
 Home-page: https://github.com/Azure/azure-storage-python
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Description: Microsoft Azure Storage SDK for Python
         ======================================
```

### Comparing `azure-storage-blob-2.0.1/README.rst` & `azure-storage-blob-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/__init__.py` & `azure-storage-blob-2.1.0/azure/storage/blob/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,9 +23,15 @@
     ResourceProperties,
     Include,
     SequenceNumberAction,
     BlockListType,
     PublicAccess,
     BlobPrefix,
     DeleteSnapshot,
+    BatchDeleteSubRequest,
+    BatchSetBlobTierSubRequest,
+    BatchSubResponse,
+    CustomerProvidedEncryptionKey,
+    RehydratePriority,
 )
 from .pageblobservice import PageBlobService
+from ._constants import __version__
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/_constants.py` & `azure-storage-blob-2.1.0/azure/storage/blob/_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 __author__ = 'Microsoft Corp. <ptvshelp@microsoft.com>'
-__version__ = '2.0.1'
+__version__ = '2.1.0'
 
 # x-ms-version for storage service.
-X_MS_VERSION = '2018-11-09'
+X_MS_VERSION = '2019-02-02'
 
 # internal configurations, should not be changed
 _LARGE_BLOB_UPLOAD_MAX_READ_BUFFER_SIZE = 4 * 1024 * 1024
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/_deserialization.py` & `azure-storage-blob-2.1.0/azure/storage/blob/_deserialization.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from azure.common import AzureException
 from dateutil import parser
 
+from azure.storage.common._http import HTTPResponse
+
 try:
     from xml.etree import cElementTree as ETree
 except ImportError:
     from xml.etree import ElementTree as ETree
 from azure.storage.common._common_conversion import (
     _decode_base64_to_text,
     _to_str,
@@ -32,56 +34,68 @@
     PageRange,
     ContainerProperties,
     AppendBlockProperties,
     PageBlobProperties,
     ResourceProperties,
     BlobPrefix,
     AccountInformation,
-    UserDelegationKey,
-)
+    UserDelegationKey, BatchSubResponse)
 from ._encryption import _decrypt_blob
 from azure.storage.common.models import _list
 from azure.storage.common._error import (
     _validate_content_match,
     _ERROR_DECRYPTION_FAILURE,
 )
+from io import BytesIO
+
+_HTTP_LINE_ENDING = "\r\n"
+
+def _parse_cpk_headers(response, properties):
+    server_encrypted = response.headers.get('x-ms-request-server-encrypted')
+    if server_encrypted is not None:
+        properties.request_server_encrypted = _bool(server_encrypted)
+
+    properties.encryption_key_sha256 = response.headers.get('x-ms-encryption-key-sha256')
 
 
 def _parse_base_properties(response):
     '''
     Extracts basic response headers.
     '''
     resource_properties = ResourceProperties()
     resource_properties.last_modified = parser.parse(response.headers.get('last-modified'))
     resource_properties.etag = response.headers.get('etag')
+    _parse_cpk_headers(response, resource_properties)
 
     return resource_properties
 
 
 def _parse_page_properties(response):
     '''
     Extracts page response headers.
     '''
     put_page = PageBlobProperties()
     put_page.last_modified = parser.parse(response.headers.get('last-modified'))
     put_page.etag = response.headers.get('etag')
     put_page.sequence_number = _to_int(response.headers.get('x-ms-blob-sequence-number'))
+    _parse_cpk_headers(response, put_page)
 
     return put_page
 
 
 def _parse_append_block(response):
     '''
     Extracts append block response headers.
     '''
     append_block = AppendBlockProperties()
     append_block.last_modified = parser.parse(response.headers.get('last-modified'))
     append_block.etag = response.headers.get('etag')
     append_block.append_offset = _to_int(response.headers.get('x-ms-blob-append-offset'))
     append_block.committed_block_count = _to_int(response.headers.get('x-ms-blob-committed-block-count'))
+    _parse_cpk_headers(response, append_block)
 
     return append_block
 
 
 def _parse_snapshot_blob(response, name):
     '''
     Extracts snapshot return header.
@@ -286,15 +300,15 @@
             <AccessTier>P4 | P6 | P10 | P20 | P30 | P40 | P50 | P60 | Archive | Cool | Hot</AccessTier>
             <AccessTierChangeTime>date-time-value</AccessTierChangeTime>
             <AccessTierInferred>true</AccessTierInferred>
             <DeletedTime>datetime</DeletedTime>
             <RemainingRetentionDays>int</RemainingRetentionDays>
             <Creation-Time>date-time-value</Creation-Time>
           </Properties>
-          <Metadata>   
+          <Metadata>
             <Name>value</Name>
           </Metadata>
         </Blob>
         <BlobPrefix>
           <Name>blob-prefix</Name>
         </BlobPrefix>
       </Blobs>
@@ -388,15 +402,15 @@
             <AccessTier>P4 | P6 | P10 | P20 | P30 | P40 | P50 | P60 | Archive | Cool | Hot</AccessTier>
             <AccessTierChangeTime>date-time-value</AccessTierChangeTime>
             <AccessTierInferred>true</AccessTierInferred>
             <DeletedTime>datetime</DeletedTime>
             <RemainingRetentionDays>int</RemainingRetentionDays>
             <Creation-Time>date-time-value</Creation-Time>
           </Properties>
-          <Metadata>   
+          <Metadata>
             <Name>value</Name>
           </Metadata>
         </Blob>
         <BlobPrefix>
           <Name>blob-prefix</Name>
         </BlobPrefix>
       </Blobs>
@@ -471,27 +485,27 @@
     return block_list
 
 
 def _convert_xml_to_page_ranges(response):
     '''
     <?xml version="1.0" encoding="utf-8"?>
     <PageList>
-       <PageRange> 
-          <Start>Start Byte</Start> 
-          <End>End Byte</End> 
-       </PageRange> 
-       <ClearRange> 
-          <Start>Start Byte</Start> 
-          <End>End Byte</End> 
-       </ClearRange> 
-       <PageRange> 
-          <Start>Start Byte</Start> 
-          <End>End Byte</End> 
-       </PageRange> 
-    </PageList> 
+       <PageRange>
+          <Start>Start Byte</Start>
+          <End>End Byte</End>
+       </PageRange>
+       <ClearRange>
+          <Start>Start Byte</Start>
+          <End>End Byte</End>
+       </ClearRange>
+       <PageRange>
+          <Start>Start Byte</Start>
+          <End>End Byte</End>
+       </PageRange>
+    </PageList>
     '''
     if response is None or response.body is None:
         return None
 
     page_list = list()
 
     list_element = ETree.fromstring(response.body)
@@ -550,7 +564,87 @@
     delegation_key.signed_start = key_element.findtext('SignedStart')
     delegation_key.signed_expiry = key_element.findtext('SignedExpiry')
     delegation_key.signed_service = key_element.findtext('SignedService')
     delegation_key.signed_version = key_element.findtext('SignedVersion')
     delegation_key.value = key_element.findtext('Value')
 
     return delegation_key
+
+
+def _ingest_batch_response(batch_response, batch_sub_requests):
+    """
+    Takes the response to a batch request and parses the response into the separate responses.
+
+    :param :class:`~azure.storage.common._http.HTTPResponse` batch_response:
+        batchResponse The response of the HTTP batch request generated by this object.
+    :return: sub-responses parsed from batch HTTP response
+    :rtype: list of :class:`~azure.storage.common._http.HTTPResponse`
+    """
+    parsed_batch_sub_response_list = []
+
+    # header value format: `multipart/mixed; boundary=<delimiter>`
+    response_delimiter = batch_response.headers.get('content-type').split("=")[1]
+
+    response_body = batch_response.body.decode('utf-8')
+
+    # split byte[] on the "substring" "--<delim>\r\n"
+    sub_response_list = response_body.split("--" + response_delimiter + _HTTP_LINE_ENDING)
+
+    # strip final, slightly different delim "\r\n--<delim>--" off last entry
+    sub_response_list[len(sub_response_list) - 1] = \
+        sub_response_list[len(sub_response_list) - 1].split(_HTTP_LINE_ENDING + "--" + response_delimiter + "--")[0]
+
+    for sub_response in sub_response_list:
+        if len(sub_response) != 0:
+            http_response = _parse_sub_response_to_http_response(sub_response)
+            is_successful = 200 <= http_response.status < 300
+            index_of_sub_request = _to_int(http_response.headers.get('Content-ID'))
+            batch_sub_request = batch_sub_requests[index_of_sub_request]
+
+            parsed_batch_sub_response_list.append(BatchSubResponse(is_successful, http_response, batch_sub_request))
+
+    return parsed_batch_sub_response_list
+
+
+def _parse_sub_response_to_http_response(sub_response):
+    """
+    Header: Value (1 or more times)
+
+    HTTP/<version> <statusCode> <statusName>
+    Header: Value (1 or more times)
+
+    body (if any)
+
+    :param sub_response:
+        The raw bytes of this sub-response.
+    :return: An HttpResponse object.
+    """
+
+    empty_line = _HTTP_LINE_ENDING.encode('utf-8')
+    num_empty_lines = 0
+    batch_http_sub_response = HTTPResponse(None, '', dict(), b'')
+    try:
+        body_stream = BytesIO()
+        body_stream.write(sub_response.encode('utf-8'))
+        body_stream.seek(0)
+
+        while True:
+            line = body_stream.readline()
+            if line == b'':
+                return batch_http_sub_response
+
+            if line.startswith("HTTP".encode('utf-8')):
+                batch_http_sub_response.status = _to_int(line.decode('utf-8').split(" ")[1])
+            elif line == empty_line:
+                num_empty_lines += 1
+            elif line.startswith("x-ms-error-code".encode('utf-8')):
+                batch_http_sub_response.message = line.decode('utf-8').split(": ")[1].rstrip()
+            elif num_empty_lines is 2:
+                batch_http_sub_response.body += line
+            else:
+                header = line.decode('utf-8').split(": ")[0]
+                value = line.decode('utf-8').split(": ")[1].rstrip()
+                batch_http_sub_response.headers[header] = value
+    finally:
+        body_stream.close()
+
+    return batch_http_sub_response
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/_download_chunking.py` & `azure-storage-blob-2.1.0/azure/storage/blob/_download_chunking.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import threading
 
 
 def _download_blob_chunks(blob_service, container_name, blob_name, snapshot,
                           download_size, block_size, progress, start_range, end_range,
                           stream, max_connections, progress_callback, validate_content,
                           lease_id, if_modified_since, if_unmodified_since, if_match,
-                          if_none_match, timeout, operation_context):
+                          if_none_match, timeout, operation_context, cpk):
 
     downloader_class = _ParallelBlobChunkDownloader if max_connections > 1 else _SequentialBlobChunkDownloader
 
     downloader = downloader_class(
         blob_service,
         container_name,
         blob_name,
@@ -30,14 +30,15 @@
         lease_id,
         if_modified_since,
         if_unmodified_since,
         if_match,
         if_none_match,
         timeout,
         operation_context,
+        cpk,
     )
 
     if max_connections > 1:
         import concurrent.futures
         executor = concurrent.futures.ThreadPoolExecutor(max_connections)
         list(executor.map(downloader.process_chunk, downloader.get_chunk_offsets()))
     else:
@@ -45,15 +46,15 @@
             downloader.process_chunk(chunk)
 
 
 class _BlobChunkDownloader(object):
     def __init__(self, blob_service, container_name, blob_name, snapshot, download_size,
                  chunk_size, progress, start_range, end_range, stream,
                  progress_callback, validate_content, lease_id, if_modified_since,
-                 if_unmodified_since, if_match, if_none_match, timeout, operation_context):
+                 if_unmodified_since, if_match, if_none_match, timeout, operation_context, cpk):
         # identifiers for the blob
         self.blob_service = blob_service
         self.container_name = container_name
         self.blob_name = blob_name
         self.snapshot = snapshot
 
         # information on the download range/chunk size
@@ -74,14 +75,15 @@
         self.operation_context = operation_context
         self.validate_content = validate_content
         self.lease_id = lease_id
         self.if_modified_since = if_modified_since
         self.if_unmodified_since = if_unmodified_since
         self.if_match = if_match
         self.if_none_match = if_none_match
+        self.cpk = cpk
 
     def get_chunk_offsets(self):
         index = self.start_index
         while index < self.blob_end:
             yield index
             index += self.chunk_size
 
@@ -115,36 +117,37 @@
             validate_content=self.validate_content,
             lease_id=self.lease_id,
             if_modified_since=self.if_modified_since,
             if_unmodified_since=self.if_unmodified_since,
             if_match=self.if_match,
             if_none_match=self.if_none_match,
             timeout=self.timeout,
-            _context=self.operation_context
+            _context=self.operation_context,
+            cpk=self.cpk,
         )
 
         # This makes sure that if_match is set so that we can validate 
         # that subsequent downloads are to an unmodified blob
         self.if_match = response.properties.etag
         return response
 
 
 class _ParallelBlobChunkDownloader(_BlobChunkDownloader):
     def __init__(self, blob_service, container_name, blob_name, snapshot, download_size,
                  chunk_size, progress, start_range, end_range, stream,
                  progress_callback, validate_content, lease_id, if_modified_since,
-                 if_unmodified_since, if_match, if_none_match, timeout, operation_context):
+                 if_unmodified_since, if_match, if_none_match, timeout, operation_context, cpk):
 
         super(_ParallelBlobChunkDownloader, self).__init__(blob_service, container_name, blob_name, snapshot,
                                                            download_size,
                                                            chunk_size, progress, start_range, end_range, stream,
                                                            progress_callback, validate_content, lease_id,
                                                            if_modified_since,
                                                            if_unmodified_since, if_match, if_none_match, timeout,
-                                                           operation_context)
+                                                           operation_context, cpk)
 
         # for a parallel download, the stream is always seekable, so we note down the current position
         # in order to seek to the right place when out-of-order chunks come in
         self.stream_start = stream.tell()
 
         # since parallel operations are going on
         # it is essential to protect the writing and progress reporting operations
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/_encryption.py` & `azure-storage-blob-2.1.0/azure/storage/blob/_encryption.py`

 * *Files identical despite different names*

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/_error.py` & `azure-storage-blob-2.1.0/azure/storage/blob/_error.py`

 * *Files identical despite different names*

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/_upload_chunking.py` & `azure-storage-blob-2.1.0/azure/storage/blob/_upload_chunking.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 from azure.storage.common._common_conversion import _encode_base64
 from azure.storage.common._error import _ERROR_VALUE_SHOULD_BE_SEEKABLE_STREAM
 from azure.storage.common._serialization import (
     url_quote,
     _get_data_bytes_only,
     _len_plus
 )
+from ._deserialization import _parse_base_properties
 from ._constants import (
     _LARGE_BLOB_UPLOAD_MAX_READ_BUFFER_SIZE
 )
 from ._encryption import (
     _get_blob_encryptor_and_padder,
 )
 from .models import BlobBlock
 
 
 def _upload_blob_chunks(blob_service, container_name, blob_name,
                         blob_size, block_size, stream, max_connections,
                         progress_callback, validate_content, lease_id, uploader_class,
                         maxsize_condition=None, if_modified_since=None, if_unmodified_since=None, if_match=None,
-                        if_none_match=None, timeout=None,
+                        if_none_match=None, timeout=None, cpk=None,
                         content_encryption_key=None, initialization_vector=None, resource_properties=None):
     encryptor, padder = _get_blob_encryptor_and_padder(content_encryption_key, initialization_vector,
                                                        uploader_class is not _PageBlobChunkUploader)
 
     uploader = uploader_class(
         blob_service,
         container_name,
@@ -42,15 +43,16 @@
         stream,
         max_connections > 1,
         progress_callback,
         validate_content,
         lease_id,
         timeout,
         encryptor,
-        padder
+        padder,
+        cpk,
     )
 
     uploader.maxsize_condition = maxsize_condition
 
     # Access conditions do not work with parallelism
     if max_connections > 1:
         uploader.if_match = uploader.if_none_match = uploader.if_modified_since = uploader.if_unmodified_since = None
@@ -96,39 +98,39 @@
             running_futures.append(future)
 
         # result() will wait until completion and also raise any exceptions that may have been set.
         range_ids = [f.result() for f in futures]
     else:
         range_ids = [uploader.process_chunk(result) for result in uploader.get_chunk_streams()]
 
-    if resource_properties:
-        resource_properties.last_modified = uploader.last_modified
-        resource_properties.etag = uploader.etag
+    if resource_properties and uploader.response_properties is not None:
+        resource_properties.clone(uploader.response_properties)
 
     return range_ids
 
 
 def _upload_blob_substream_blocks(blob_service, container_name, blob_name,
                                   blob_size, block_size, stream, max_connections,
                                   progress_callback, validate_content, lease_id, uploader_class,
-                                  maxsize_condition=None, if_match=None, timeout=None):
+                                  maxsize_condition=None, if_match=None, timeout=None, cpk=None):
     uploader = uploader_class(
         blob_service,
         container_name,
         blob_name,
         blob_size,
         block_size,
         stream,
         max_connections > 1,
         progress_callback,
         validate_content,
         lease_id,
         timeout,
         None,
-        None
+        None,
+        cpk,
     )
 
     uploader.maxsize_condition = maxsize_condition
 
     # ETag matching does not work with parallelism as a ranged upload may start
     # before the previous finishes and provides an etag
     uploader.if_match = if_match if not max_connections > 1 else None
@@ -145,15 +147,15 @@
 
     return range_ids
 
 
 class _BlobChunkUploader(object):
     def __init__(self, blob_service, container_name, blob_name, blob_size,
                  chunk_size, stream, parallel, progress_callback,
-                 validate_content, lease_id, timeout, encryptor, padder):
+                 validate_content, lease_id, timeout, encryptor, padder, cpk):
         self.blob_service = blob_service
         self.container_name = container_name
         self.blob_name = blob_name
         self.blob_size = blob_size
         self.chunk_size = chunk_size
         self.stream = stream
         self.parallel = parallel
@@ -163,16 +165,16 @@
         self.progress_total = 0
         self.progress_lock = Lock() if parallel else None
         self.validate_content = validate_content
         self.lease_id = lease_id
         self.timeout = timeout
         self.encryptor = encryptor
         self.padder = padder
-        self.last_modified = None
-        self.etag = None
+        self.response_properties = None
+        self.cpk = cpk
 
     def get_chunk_streams(self):
         index = 0
         while True:
             data = b''
             read_size = self.chunk_size
 
@@ -249,42 +251,43 @@
 
     def _upload_substream_block_with_progress(self, block_id, block_stream):
         range_id = self._upload_substream_block(block_id, block_stream)
         self._update_progress(len(block_stream))
         return range_id
 
     def set_response_properties(self, resp):
-        self.etag = resp.etag
-        self.last_modified = resp.last_modified
+        self.response_properties = resp
 
 
 class _BlockBlobChunkUploader(_BlobChunkUploader):
     def _upload_chunk(self, chunk_offset, chunk_data):
         block_id = url_quote(_encode_base64('{0:032d}'.format(chunk_offset)))
         self.blob_service._put_block(
             self.container_name,
             self.blob_name,
             chunk_data,
             block_id,
             validate_content=self.validate_content,
             lease_id=self.lease_id,
             timeout=self.timeout,
+            cpk=self.cpk,
         )
         return BlobBlock(block_id)
 
     def _upload_substream_block(self, block_id, block_stream):
         try:
             self.blob_service._put_block(
                 self.container_name,
                 self.blob_name,
                 block_stream,
                 block_id,
                 validate_content=self.validate_content,
                 lease_id=self.lease_id,
                 timeout=self.timeout,
+                cpk=self.cpk,
             )
         finally:
             block_stream.close()
         return BlobBlock(block_id)
 
 
 class _PageBlobChunkUploader(_BlobChunkUploader):
@@ -306,14 +309,15 @@
                 chunk_data,
                 chunk_start,
                 chunk_end,
                 validate_content=self.validate_content,
                 lease_id=self.lease_id,
                 if_match=self.if_match,
                 timeout=self.timeout,
+                cpk=self.cpk,
             )
 
             if not self.parallel:
                 self.if_match = resp.etag
 
             self.set_response_properties(resp)
 
@@ -328,28 +332,30 @@
                 validate_content=self.validate_content,
                 lease_id=self.lease_id,
                 maxsize_condition=self.maxsize_condition,
                 timeout=self.timeout,
                 if_modified_since=self.if_modified_since,
                 if_unmodified_since=self.if_unmodified_since,
                 if_match=self.if_match,
-                if_none_match=self.if_none_match
+                if_none_match=self.if_none_match,
+                cpk=self.cpk,
             )
 
             self.current_length = resp.append_offset
         else:
             resp = self.blob_service.append_block(
                 self.container_name,
                 self.blob_name,
                 chunk_data,
                 validate_content=self.validate_content,
                 lease_id=self.lease_id,
                 maxsize_condition=self.maxsize_condition,
                 appendpos_condition=self.current_length + chunk_offset,
                 timeout=self.timeout,
+                cpk=self.cpk,
             )
 
         self.set_response_properties(resp)
 
 
 class _SubStream(IOBase):
     def __init__(self, wrapped_stream, stream_begin_index, length, lockObj):
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/appendblobservice.py` & `azure-storage-blob-2.1.0/azure/storage/blob/appendblobservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from ._deserialization import (
     _parse_append_block,
     _parse_base_properties,
 )
 from ._serialization import (
     _get_path,
     _validate_and_format_range_headers,
+    _validate_and_add_cpk_headers,
 )
 from ._upload_chunking import (
     _AppendBlobChunkUploader,
     _upload_blob_chunks,
 )
 from .baseblobservice import BaseBlobService
 from .models import (
@@ -119,15 +120,15 @@
         super(AppendBlobService, self).__init__(
             account_name, account_key, sas_token, is_emulated, protocol, endpoint_suffix,
             custom_domain, request_session, connection_string, socket_timeout, token_credential)
 
     def create_blob(self, container_name, blob_name, content_settings=None,
                     metadata=None, lease_id=None,
                     if_modified_since=None, if_unmodified_since=None,
-                    if_match=None, if_none_match=None, timeout=None):
+                    if_match=None, if_none_match=None, timeout=None, cpk=None):
         '''
         Creates a blob or overrides an existing blob. Use if_none_match=* to
         prevent overriding an existing blob. 
 
         See create_blob_from_* for high level
         functions that handle the creation and upload of large blobs with
         automatic chunking and progress notifications.
@@ -160,14 +161,19 @@
             perform the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return: ETag and last modified properties for the updated Append Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
@@ -182,26 +188,27 @@
             'x-ms-blob-type': _to_str(self.blob_type),
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _add_metadata_headers(metadata, request)
         if content_settings is not None:
             request.headers.update(content_settings._to_headers())
 
         return self._perform_request(request, _parse_base_properties)
 
     def append_block(self, container_name, blob_name, block,
                      validate_content=False, maxsize_condition=None,
                      appendpos_condition=None,
                      lease_id=None, if_modified_since=None,
                      if_unmodified_since=None, if_match=None,
-                     if_none_match=None, timeout=None):
+                     if_none_match=None, timeout=None, cpk=None):
         '''
         Commits a new block of data to the end of an existing append blob.
         
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of existing blob.
@@ -246,14 +253,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return:
             ETag, last modified, append offset, and committed block count 
             properties for the updated Append Blob
         :rtype: :class:`~azure.storage.blob.models.AppendBlockProperties`
         '''
@@ -275,29 +287,30 @@
             'x-ms-blob-condition-appendpos': _to_str(appendpos_condition),
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         request.body = _get_data_bytes_only('block', block)
 
         if validate_content:
             computed_md5 = _get_content_md5(request.body)
             request.headers['Content-MD5'] = _to_str(computed_md5)
 
         return self._perform_request(request, _parse_append_block)
 
     def append_block_from_url(self, container_name, blob_name, copy_source_url, source_range_start=None,
                               source_range_end=None, source_content_md5=None, source_if_modified_since=None,
                               source_if_unmodified_since=None, source_if_match=None,
                               source_if_none_match=None, maxsize_condition=None,
                               appendpos_condition=None, lease_id=None, if_modified_since=None,
                               if_unmodified_since=None, if_match=None,
-                              if_none_match=None, timeout=None):
+                              if_none_match=None, timeout=None, cpk=None):
         """
         Creates a new block to be committed as part of a blob, where the contents are read from a source url.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of blob.
@@ -363,14 +376,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         """
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('copy_source_url', copy_source_url)
@@ -394,29 +412,29 @@
             'x-ms-blob-condition-appendpos': _to_str(appendpos_condition),
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match)
         }
-
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _validate_and_format_range_headers(request, source_range_start, source_range_end,
                                            start_range_required=False,
                                            end_range_required=False,
                                            range_header_name="x-ms-source-range")
 
         return self._perform_request(request, _parse_append_block)
 
     # ----Convenience APIs----------------------------------------------
 
     def append_blob_from_path(
             self, container_name, blob_name, file_path, validate_content=False,
             maxsize_condition=None, progress_callback=None, lease_id=None, timeout=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None):
+            if_none_match=None, cpk=None):
         '''
         Appends to the content of an existing blob from a file path, with automatic
         chunking and progress notifications.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -464,14 +482,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the Append Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('file_path', file_path)
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
@@ -487,21 +510,22 @@
                 maxsize_condition=maxsize_condition,
                 progress_callback=progress_callback,
                 lease_id=lease_id,
                 timeout=timeout,
                 if_modified_since=if_modified_since,
                 if_unmodified_since=if_unmodified_since,
                 if_match=if_match,
-                if_none_match=if_none_match)
+                if_none_match=if_none_match,
+                cpk=cpk)
 
     def append_blob_from_bytes(
             self, container_name, blob_name, blob, index=0, count=None,
             validate_content=False, maxsize_condition=None, progress_callback=None,
             lease_id=None, timeout=None, if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None):
+            if_none_match=None, cpk=None):
         '''
         Appends to the content of an existing blob from an array of bytes, with
         automatic chunking and progress notifications.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -554,14 +578,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the Append Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('blob', blob)
         _validate_not_none('index', index)
@@ -586,21 +615,22 @@
             maxsize_condition=maxsize_condition,
             lease_id=lease_id,
             progress_callback=progress_callback,
             timeout=timeout,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
-            if_none_match=if_none_match)
+            if_none_match=if_none_match,
+            cpk=cpk)
 
     def append_blob_from_text(
             self, container_name, blob_name, text, encoding='utf-8',
             validate_content=False, maxsize_condition=None, progress_callback=None,
             lease_id=None, timeout=None, if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None):
+            if_none_match=None, cpk=None):
         '''
         Appends to the content of an existing blob from str/unicode, with
         automatic chunking and progress notifications.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -650,14 +680,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the Append Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('text', text)
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
@@ -676,21 +711,22 @@
             maxsize_condition=maxsize_condition,
             lease_id=lease_id,
             progress_callback=progress_callback,
             timeout=timeout,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
-            if_none_match=if_none_match)
+            if_none_match=if_none_match,
+            cpk=cpk)
 
     def append_blob_from_stream(
             self, container_name, blob_name, stream, count=None,
             validate_content=False, maxsize_condition=None, progress_callback=None,
             lease_id=None, timeout=None, if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None):
+            if_none_match=None, cpk=None):
         '''
         Appends to the content of an existing blob from a file/stream, with
         automatic chunking and progress notifications.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -741,14 +777,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the Append Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('stream', stream)
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
@@ -771,11 +812,12 @@
             uploader_class=_AppendBlobChunkUploader,
             maxsize_condition=maxsize_condition,
             timeout=timeout,
             resource_properties=resource_properties,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
-            if_none_match=if_none_match
+            if_none_match=if_none_match,
+            cpk=cpk,
         )
 
         return resource_properties
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/baseblobservice.py` & `azure-storage-blob-2.1.0/azure/storage/blob/baseblobservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import sys
+import uuid
 from abc import ABCMeta
 
 from azure.common import AzureHttpError
 
 from azure.storage.common._auth import (
     _StorageSASAuthentication,
     _StorageSharedKeyAuthentication,
@@ -41,15 +42,15 @@
 )
 from azure.storage.common._http import HTTPRequest
 from azure.storage.common._serialization import (
     _get_request_body,
     _convert_signed_identifiers_to_xml,
     _convert_service_properties_to_xml,
     _add_metadata_headers,
-)
+    _update_request, _add_date_header)
 from azure.storage.common.models import (
     Services,
     ListGenerator,
     _OperationContext,
 )
 from .sharedaccesssignature import (
     BlobSharedAccessSignature,
@@ -63,24 +64,27 @@
     _parse_container,
     _parse_snapshot_blob,
     _parse_lease,
     _convert_xml_to_signed_identifiers_and_access,
     _parse_base_properties,
     _parse_account_information,
     _convert_xml_to_user_delegation_key,
-)
+    _ingest_batch_response)
 from ._download_chunking import _download_blob_chunks
 from ._error import (
     _ERROR_INVALID_LEASE_DURATION,
     _ERROR_INVALID_LEASE_BREAK_PERIOD,
 )
 from ._serialization import (
     _get_path,
     _validate_and_format_range_headers,
     _convert_delegation_key_info_to_xml,
+    _get_batch_request_delimiter,
+    _serialize_batch_body,
+    _validate_and_add_cpk_headers,
 )
 from .models import (
     BlobProperties,
     _LeaseActions,
     ContainerPermissions,
     BlobPermissions,
 )
@@ -545,15 +549,16 @@
 
         :param datetime key_start_time:
             A DateTime value. Indicates when the key becomes valid.
         :param datetime key_expiry_time:
             A DateTime value. Indicates when the key stops being valid.
         :param int timeout:
             The timeout parameter is expressed in seconds.
-        :return:
+        :return: The user delegation key.
+        :rtype: ~azure.storage.blob.models.UserDelegationKey
         """
         _validate_not_none('key_start_time', key_start_time)
         _validate_not_none('key_end_time', key_expiry_time)
 
         request = HTTPRequest()
         request.method = 'POST'
         request.host_locations = self._get_host_locations(secondary=True)
@@ -649,14 +654,17 @@
         '''
         Creates a new container under the specified account. If the container
         with the same name already exists, the operation fails if
         fail_on_exist is True.
 
         :param str container_name:
             Name of container to create.
+            The container name may only contain lowercase letters, numbers, and hyphens, and must begin with a letter or
+            a number. Each hyphen must be preceded and followed by a non-hyphen character. The name must also be
+            between 3 and 63 characters long.
         :param metadata:
             A dict with name_value pairs to associate with the
             container as metadata. Example:{'Category':'test'}
         :type metadata: dict(str, str)
         :param ~azure.storage.blob.models.PublicAccess public_access:
             Possible values include: container, blob.
         :param bool fail_on_exist:
@@ -1575,15 +1583,15 @@
         }
 
         return self._perform_request(request, _convert_xml_to_service_properties)
 
     def get_blob_properties(
             self, container_name, blob_name, snapshot=None, lease_id=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+            if_none_match=None, timeout=None, cpk=None):
         '''
         Returns all user-defined metadata, standard HTTP properties, and
         system properties for the blob. It does not return the content of the blob.
         Returns :class:`~azure.storage.blob.models.Blob`
         with :class:`~azure.storage.blob.models.BlobProperties` and a metadata dict.
         
         :param str container_name:
@@ -1612,14 +1620,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Decrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return: a blob object including properties and metadata.
         :rtype: :class:`~azure.storage.blob.models.Blob`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
@@ -1634,21 +1647,21 @@
         request.headers = {
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match),
         }
-
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         return self._perform_request(request, _parse_blob, [blob_name, snapshot])
 
     def set_blob_properties(
             self, container_name, blob_name, content_settings=None, lease_id=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+            if_none_match=None, timeout=None, cpk=None):
         '''
         Sets system properties on the blob. If one property is set for the
         content_settings, all properties will be overriden.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -1674,14 +1687,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return: ETag and last modified properties for the updated Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
@@ -1696,14 +1714,15 @@
         request.headers = {
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match),
             'x-ms-lease-id': _to_str(lease_id)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         if content_settings is not None:
             request.headers.update(content_settings._to_headers())
 
         return self._perform_request(request, _parse_base_properties)
 
     def exists(self, container_name, blob_name=None, snapshot=None, timeout=None):
         '''
@@ -1743,15 +1762,15 @@
         except AzureHttpError as ex:
             _dont_fail_not_exist(ex)
             return False
 
     def _get_blob(
             self, container_name, blob_name, snapshot=None, start_range=None,
             end_range=None, validate_content=False, lease_id=None, if_modified_since=None,
-            if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None,
+            if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None, cpk=None,
             _context=None):
         '''
         Downloads a blob's content, metadata, and properties. You can also
         call this API to read a snapshot. You can specify a range if you don't
         need to download the blob in its entirety. If no range is specified,
         the full blob will be downloaded.
 
@@ -1798,14 +1817,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Decrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return: A Blob with content, properties, and metadata.
         :rtype: :class:`~azure.storage.blob.models.Blob`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
@@ -1843,14 +1867,15 @@
         request.headers = {
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match),
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _validate_and_format_range_headers(
             request,
             start_range,
             end_range,
             start_range_required=False,
             end_range_required=False,
             check_content_md5=validate_content)
@@ -1862,16 +1887,15 @@
                                      operation_context=_context)
 
     def get_blob_to_path(
             self, container_name, blob_name, file_path, open_mode='wb',
             snapshot=None, start_range=None, end_range=None,
             validate_content=False, progress_callback=None,
             max_connections=2, lease_id=None, if_modified_since=None,
-            if_unmodified_since=None, if_match=None, if_none_match=None,
-            timeout=None):
+            if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None, cpk=None):
         '''
         Downloads a blob to a file path, with automatic chunking and progress
         notifications. Returns an instance of :class:`~azure.storage.blob.models.Blob` with
         properties and metadata.
 
         :param str container_name:
             Name of existing container.
@@ -1943,14 +1967,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Decrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make 
             multiple calls to the Azure service and the timeout will apply to 
             each call individually.
         :return: A Blob with properties and metadata. If max_connections is greater 
             than 1, the content_md5 (if set on the blob) will not be returned. If you 
             require this value, either use get_blob_properties or set max_connections 
@@ -1977,24 +2006,25 @@
                 progress_callback,
                 max_connections,
                 lease_id,
                 if_modified_since,
                 if_unmodified_since,
                 if_match,
                 if_none_match,
-                timeout)
+                timeout=timeout,
+                cpk=cpk)
 
         return blob
 
     def get_blob_to_stream(
             self, container_name, blob_name, stream, snapshot=None,
             start_range=None, end_range=None, validate_content=False,
             progress_callback=None, max_connections=2, lease_id=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+            if_none_match=None, timeout=None, cpk=None):
 
         '''
         Downloads a blob to a stream, with automatic chunking and progress
         notifications. Returns an instance of :class:`~azure.storage.blob.models.Blob` with
         properties and metadata.
 
         :param str container_name:
@@ -2063,14 +2093,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Decrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make 
             multiple calls to the Azure service and the timeout will apply to 
             each call individually.
         :return: A Blob with properties and metadata. If max_connections is greater 
             than 1, the content_md5 (if set on the blob) will not be returned. If you 
             require this value, either use get_blob_properties or set max_connections 
@@ -2117,15 +2152,16 @@
                                   validate_content=validate_content,
                                   lease_id=lease_id,
                                   if_modified_since=if_modified_since,
                                   if_unmodified_since=if_unmodified_since,
                                   if_match=if_match,
                                   if_none_match=if_none_match,
                                   timeout=timeout,
-                                  _context=operation_context)
+                                  _context=operation_context,
+                                  cpk=cpk)
 
             # Parse the total blob size and adjust the download size if ranges
             # were specified
             blob_size = _parse_length_from_content_range(blob.properties.content_range)
             if end_range is not None:
                 # Use the end_range unless it is over the end of the blob
                 download_size = min(blob_size, end_range - start_range + 1)
@@ -2144,15 +2180,16 @@
                                       validate_content=validate_content,
                                       lease_id=lease_id,
                                       if_modified_since=if_modified_since,
                                       if_unmodified_since=if_unmodified_since,
                                       if_match=if_match,
                                       if_none_match=if_none_match,
                                       timeout=timeout,
-                                      _context=operation_context)
+                                      _context=operation_context,
+                                      cpk=cpk)
 
                 # Set the download size to empty
                 download_size = 0
             else:
                 raise ex
 
         # Mark the first progress chunk. If the blob is small or this is a single
@@ -2193,15 +2230,16 @@
                 validate_content,
                 lease_id,
                 if_modified_since,
                 if_unmodified_since,
                 if_match,
                 if_none_match,
                 timeout,
-                operation_context
+                operation_context,
+                cpk,
             )
 
             # Set the content length to the download size instead of the size of
             # the last range
             blob.properties.content_length = download_size
 
             # Overwrite the content range to the user requested range
@@ -2215,15 +2253,15 @@
         return blob
 
     def get_blob_to_bytes(
             self, container_name, blob_name, snapshot=None,
             start_range=None, end_range=None, validate_content=False,
             progress_callback=None, max_connections=2, lease_id=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+            if_none_match=None, timeout=None, cpk=None):
         '''
         Downloads a blob as an array of bytes, with automatic chunking and
         progress notifications. Returns an instance of :class:`~azure.storage.blob.models.Blob` with
         properties, metadata, and content.
 
         :param str container_name:
             Name of existing container.
@@ -2289,14 +2327,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Decrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make 
             multiple calls to the Azure service and the timeout will apply to 
             each call individually.
         :return: A Blob with properties and metadata. If max_connections is greater 
             than 1, the content_md5 (if set on the blob) will not be returned. If you 
             require this value, either use get_blob_properties or set max_connections 
@@ -2318,25 +2361,26 @@
             progress_callback,
             max_connections,
             lease_id,
             if_modified_since,
             if_unmodified_since,
             if_match,
             if_none_match,
-            timeout)
+            timeout=timeout,
+            cpk=cpk)
 
         blob.content = stream.getvalue()
         return blob
 
     def get_blob_to_text(
             self, container_name, blob_name, encoding='utf-8', snapshot=None,
             start_range=None, end_range=None, validate_content=False,
             progress_callback=None, max_connections=2, lease_id=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+            if_none_match=None, timeout=None, cpk=None):
         '''
         Downloads a blob as unicode text, with automatic chunking and progress
         notifications. Returns an instance of :class:`~azure.storage.blob.models.Blob` with
         properties, metadata, and content.
 
         :param str container_name:
             Name of existing container.
@@ -2404,14 +2448,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Decrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make 
             multiple calls to the Azure service and the timeout will apply to 
             each call individually.
         :return: A Blob with properties and metadata. If max_connections is greater 
             than 1, the content_md5 (if set on the blob) will not be returned. If you 
             require this value, either use get_blob_properties or set max_connections 
@@ -2431,22 +2480,23 @@
                                       progress_callback,
                                       max_connections,
                                       lease_id,
                                       if_modified_since,
                                       if_unmodified_since,
                                       if_match,
                                       if_none_match,
-                                      timeout)
+                                      timeout=timeout,
+                                      cpk=cpk)
         blob.content = blob.content.decode(encoding)
         return blob
 
     def get_blob_metadata(
             self, container_name, blob_name, snapshot=None, lease_id=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+            if_none_match=None, timeout=None, cpk=None):
         '''
         Returns all user-defined metadata for the specified blob or snapshot.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of existing blob.
@@ -2472,14 +2522,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Decrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return:
             A dictionary representing the blob metadata name, value pairs.
         :rtype: dict(str, str)
         '''
         _validate_not_none('container_name', container_name)
@@ -2496,21 +2551,21 @@
         request.headers = {
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match),
         }
-
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         return self._perform_request(request, _parse_metadata)
 
     def set_blob_metadata(self, container_name, blob_name,
                           metadata=None, lease_id=None,
                           if_modified_since=None, if_unmodified_since=None,
-                          if_match=None, if_none_match=None, timeout=None):
+                          if_match=None, if_none_match=None, timeout=None, cpk=None):
         '''
         Sets user-defined metadata for the specified blob as one or more
         name-value pairs.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -2539,14 +2594,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return: ETag and last modified properties for the updated Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
@@ -2562,15 +2622,15 @@
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match),
             'x-ms-lease-id': _to_str(lease_id),
         }
         _add_metadata_headers(metadata, request)
-
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         return self._perform_request(request, _parse_base_properties)
 
     def _lease_blob_impl(self, container_name, blob_name,
                          lease_action, lease_id,
                          lease_duration, lease_break_period,
                          proposed_lease_id, if_modified_since,
                          if_unmodified_since, if_match, if_none_match, timeout=None):
@@ -2976,15 +3036,15 @@
                               if_match,
                               if_none_match,
                               timeout)
 
     def snapshot_blob(self, container_name, blob_name,
                       metadata=None, if_modified_since=None,
                       if_unmodified_since=None, if_match=None,
-                      if_none_match=None, lease_id=None, timeout=None):
+                      if_none_match=None, lease_id=None, timeout=None, cpk=None):
         '''
         Creates a read-only snapshot of a blob.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of existing blob.
@@ -3014,14 +3074,19 @@
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
         :param str lease_id:
             Required if the blob has an active lease.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return: snapshot properties
         :rtype: :class:`~azure.storage.blob.models.Blob`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
@@ -3036,14 +3101,15 @@
         request.headers = {
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match),
             'x-ms-lease-id': _to_str(lease_id)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _add_metadata_headers(metadata, request)
 
         return self._perform_request(request, _parse_snapshot_blob, [blob_name])
 
     def copy_blob(self, container_name, blob_name, copy_source,
                   metadata=None,
                   source_if_modified_since=None,
@@ -3193,15 +3259,17 @@
                    destination_if_modified_since=None,
                    destination_if_unmodified_since=None,
                    destination_if_match=None,
                    destination_if_none_match=None,
                    destination_lease_id=None,
                    source_lease_id=None, timeout=None,
                    incremental_copy=False,
-                   requires_sync=None):
+                   requires_sync=None,
+                   standard_blob_tier=None,
+                   rehydrate_priority=None):
         '''
         See copy_blob for more details. This helper method
         allows for standard copies as well as incremental copies which are only supported for page blobs and sync
         copies which are only supported for block blobs.
         :param bool incremental_copy:
             Performs an incremental copy operation on a page blob instead of a standard copy operation.
         :param bool requires_sync:
@@ -3248,16 +3316,17 @@
             'x-ms-source-if-none-match': _to_str(source_if_none_match),
             'If-Modified-Since': _datetime_to_utc_string(destination_if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(destination_if_unmodified_since),
             'If-Match': _to_str(destination_if_match),
             'If-None-Match': _to_str(destination_if_none_match),
             'x-ms-lease-id': _to_str(destination_lease_id),
             'x-ms-source-lease-id': _to_str(source_lease_id),
-            'x-ms-access-tier': _to_str(premium_page_blob_tier),
-            'x-ms-requires-sync': _to_str(requires_sync)
+            'x-ms-access-tier': _to_str(premium_page_blob_tier) or _to_str(standard_blob_tier),
+            'x-ms-requires-sync': _to_str(requires_sync),
+            'x-ms-rehydrate-priority': _to_str(rehydrate_priority)
         }
 
         _add_metadata_headers(metadata, request)
 
         return self._perform_request(request, _parse_properties, [BlobProperties]).copy
 
     def abort_copy_blob(self, container_name, blob_name, copy_id,
@@ -3346,14 +3415,112 @@
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         '''
+        request = self._get_basic_delete_blob_http_request(container_name,
+                                                           blob_name,
+                                                           snapshot=snapshot,
+                                                           lease_id=lease_id,
+                                                           delete_snapshots=delete_snapshots,
+                                                           if_modified_since=if_modified_since,
+                                                           if_unmodified_since=if_unmodified_since,
+                                                           if_match=if_match,
+                                                           if_none_match=if_none_match,
+                                                           timeout=timeout)
+
+        self._perform_request(request)
+
+    def batch_delete_blobs(self, batch_delete_sub_requests, timeout=None):
+        '''
+        Sends a batch of multiple blob delete requests.
+
+        The blob delete method deletes the specified blob or snapshot. Note that deleting a blob also deletes all its
+        snapshots. For more information, see https://docs.microsoft.com/rest/api/storageservices/delete-blob
+
+        :param list(BatchDeleteSubRequest) batch_delete_sub_requests:
+            The blob delete requests to send as a batch.
+        :param int timeout:
+            The timeout parameter is expressed in seconds.
+        :return: parsed batch delete HTTP response
+        :rtype: list of :class:`~azure.storage.blob.models.BatchSubResponse`
+        '''
+        self._check_batch_request(batch_delete_sub_requests)
+
+        request = HTTPRequest()
+        request.method = 'POST'
+        request.host_locations = self._get_host_locations()
+        request.path = _get_path()
+        batch_id = str(uuid.uuid1())
+        request.headers = {
+            'Content-Type': "multipart/mixed; boundary=" + _get_batch_request_delimiter(batch_id, False, False),
+        }
+        request.query = {
+            'comp': 'batch',
+            'timeout': _int_to_str(timeout)
+        }
+
+        batch_http_requests = []
+        for batch_delete_sub_request in batch_delete_sub_requests:
+            batch_delete_sub_http_request = self._construct_batch_delete_sub_http_request(len(batch_http_requests),
+                                                                                          batch_delete_sub_request)
+            batch_http_requests.append(batch_delete_sub_http_request)
+
+        request.body = _serialize_batch_body(batch_http_requests, batch_id)
+
+        return self._perform_request(request, parser=_ingest_batch_response, parser_args=[batch_delete_sub_requests])
+
+    def _construct_batch_delete_sub_http_request(self, content_id, batch_delete_sub_request):
+        """
+        Construct an HTTPRequest instance from a batch delete sub-request.
+
+        :param int content_id:
+            the index of sub-request in the list of sub-requests
+        :param ~azure.storage.blob.models.BatchDeleteSubRequest batch_delete_sub_request:
+            one of the delete request to be sent in a batch
+        :return: HTTPRequest parsed from batch delete sub-request
+        :rtype: :class:`~azure.storage.common._http.HTTPRequest`
+        """
+        request = self._get_basic_delete_blob_http_request(batch_delete_sub_request.container_name,
+                                                           batch_delete_sub_request.blob_name,
+                                                           snapshot=batch_delete_sub_request.snapshot,
+                                                           lease_id=batch_delete_sub_request.lease_id,
+                                                           delete_snapshots=batch_delete_sub_request.delete_snapshots,
+                                                           if_modified_since=batch_delete_sub_request.if_modified_since,
+                                                           if_unmodified_since=batch_delete_sub_request.if_unmodified_since,
+                                                           if_match=batch_delete_sub_request.if_match,
+                                                           if_none_match=batch_delete_sub_request.if_none_match)
+        request.headers.update({
+            'Content-ID': _int_to_str(content_id),
+            'Content-Length': _int_to_str(0),
+            'Content-Transfer-Encoding': 'binary',
+        })
+
+        _update_request(request, None, self._USER_AGENT_STRING)
+        # sub-request will use the batch request id automatically, no need to generate a separate one
+        request.headers.pop('x-ms-client-request-id', None)
+
+        _add_date_header(request)
+        self.authentication.sign_request(request)
+
+        return request
+
+    def _get_basic_delete_blob_http_request(self, container_name, blob_name, snapshot=None, lease_id=None,
+                                            delete_snapshots=None, if_modified_since=None, if_unmodified_since=None,
+                                            if_match=None, if_none_match=None, timeout=None):
+        """
+        Construct a basic HTTPRequest instance for delete blob
+
+        For more information about the parameters please see delete_blob
+
+        :return: an HTTPRequest for delete blob
+        :rtype :class:`~azure.storage.common._http.HTTPRequest`
+        """
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         request = HTTPRequest()
         request.method = 'DELETE'
         request.host_locations = self._get_host_locations()
         request.path = _get_path(container_name, blob_name)
         request.headers = {
@@ -3365,15 +3532,20 @@
             'If-None-Match': _to_str(if_none_match),
         }
         request.query = {
             'snapshot': _to_str(snapshot),
             'timeout': _int_to_str(timeout)
         }
 
-        self._perform_request(request)
+        return request
+
+    @staticmethod
+    def _check_batch_request(request):
+        if request is None or len(request) < 1 or len(request) > 256:
+            raise ValueError("Batch request should take 1 to 256 sub-requests")
 
     def undelete_blob(self, container_name, blob_name, timeout=None):
         '''
         The undelete Blob operation restores the contents and metadata of soft deleted blob or snapshot.
         Attempting to undelete a blob or snapshot that is not soft deleted will succeed without any changes.
 
         :param str container_name:
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/blockblobservice.py` & `azure-storage-blob-2.1.0/azure/storage/blob/blockblobservice.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
+import uuid
 from io import (
     BytesIO
 )
 from os import (
     path,
 )
 
@@ -31,30 +32,33 @@
 )
 from azure.storage.common._http import HTTPRequest
 from azure.storage.common._serialization import (
     _get_request_body,
     _get_data_bytes_only,
     _get_data_bytes_or_stream_only,
     _add_metadata_headers,
-)
+    _add_date_header, _update_request)
 from azure.storage.common._serialization import (
     _len_plus
 )
 from ._deserialization import (
     _convert_xml_to_block_list,
     _parse_base_properties,
-)
+    _ingest_batch_response)
 from ._encryption import (
     _encrypt_blob,
     _generate_blob_encryption_data,
 )
 from ._serialization import (
     _convert_block_list_to_xml,
     _get_path,
     _validate_and_format_range_headers,
+    _get_batch_request_delimiter,
+    _serialize_batch_body,
+    _validate_and_add_cpk_headers,
 )
 from ._upload_chunking import (
     _BlockBlobChunkUploader,
     _upload_blob_chunks,
     _upload_blob_substream_blocks,
 )
 from .baseblobservice import BaseBlobService
@@ -142,60 +146,64 @@
         '''
         self.blob_type = _BlobTypes.BlockBlob
         super(BlockBlobService, self).__init__(
             account_name, account_key, sas_token, is_emulated, protocol, endpoint_suffix,
             custom_domain, request_session, connection_string, socket_timeout, token_credential)
 
     def put_block(self, container_name, blob_name, block, block_id,
-                  validate_content=False, lease_id=None, timeout=None):
+                  validate_content=False, lease_id=None, timeout=None, cpk=None):
         '''
         Creates a new block to be committed as part of a blob.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of blob.
         :param block: Content of the block.
         :type block: io.IOBase or bytes
             Content of the block.
         :param str block_id:
-            A valid Base64 string value that identifies the block. Prior to
-            encoding, the string must be less than or equal to 64 bytes in size.
-            For a given blob, the length of the value specified for the blockid
-            parameter must be the same size for each block. Note that the Base64
-            string must be URL-encoded.
+            A string value that identifies the block. The string should be less than
+            or equal to 64 bytes in size.
+            For a given blob, the block_id must be the same size for each block.
         :param bool validate_content:
             If true, calculates an MD5 hash of the block content. The storage
             service checks the hash of the content that has arrived
             with the hash that was sent. This is primarily valuable for detecting
             bitflips on the wire if using http instead of https as https (the default)
             will already validate. Note that this MD5 hash is not stored with the
             blob.
         :param str lease_id:
             Required if the blob has an active lease.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         '''
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
 
         self._put_block(
             container_name,
             blob_name,
             block,
             block_id,
             validate_content=validate_content,
             lease_id=lease_id,
-            timeout=timeout
+            timeout=timeout,
+            cpk=cpk,
         )
 
     def put_block_list(
             self, container_name, blob_name, block_list, content_settings=None,
             metadata=None, validate_content=False, lease_id=None, if_modified_since=None,
             if_unmodified_since=None, if_match=None, if_none_match=None,
-            timeout=None):
+            timeout=None, standard_blob_tier=None, cpk=None):
         '''
         Writes a blob by specifying the list of block IDs that make up the blob.
         In order to be written as part of a blob, a block must have been
         successfully written to the server in a prior Put Block operation.
 
         You can call Put Block List to update a blob by uploading only those
         blocks that have changed, then committing the new and existing blocks
@@ -242,16 +250,24 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
+        :param StandardBlobTier standard_blob_tier:
+            A standard blob tier value to set the blob to. For this version of the library,
+            this is only applicable to block blobs on standard storage accounts.
         :return: ETag and last modified properties for the updated Block Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
 
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
 
         return self._put_block_list(
@@ -262,15 +278,17 @@
             metadata=metadata,
             validate_content=validate_content,
             lease_id=lease_id,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
             if_none_match=if_none_match,
-            timeout=timeout
+            timeout=timeout,
+            standard_blob_tier=standard_blob_tier,
+            cpk=cpk,
         )
 
     def get_block_list(self, container_name, blob_name, snapshot=None,
                        block_list_type=None, lease_id=None, timeout=None):
         '''
         Retrieves the list of blocks that have been uploaded as part of a
         block blob. There are two block lists maintained for a blob:
@@ -314,15 +332,15 @@
         }
         request.headers = {'x-ms-lease-id': _to_str(lease_id)}
 
         return self._perform_request(request, _convert_xml_to_block_list)
 
     def put_block_from_url(self, container_name, blob_name, copy_source_url, block_id,
                            source_range_start=None, source_range_end=None,
-                           source_content_md5=None, lease_id=None, timeout=None):
+                           source_content_md5=None, lease_id=None, timeout=None, cpk=None):
         """
         Creates a new block to be committed as part of a blob.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of blob.
@@ -330,23 +348,26 @@
             The URL of the source data. It can point to any Azure Blob or File, that is either public or has a
             shared access signature attached.
         :param int source_range_start:
             This indicates the start of the range of bytes(inclusive) that has to be taken from the copy source.
         :param int source_range_end:
             This indicates the end of the range of bytes(inclusive) that has to be taken from the copy source.
         :param str block_id:
-            A valid Base64 string value that identifies the block. Prior to
-            encoding, the string must be less than or equal to 64 bytes in size.
-            For a given blob, the length of the value specified for the blockid
-            parameter must be the same size for each block. Note that the Base64
-            string must be URL-encoded.
+            A string value that identifies the block. The string should be less than
+            or equal to 64 bytes in size.
+            For a given blob, the block_id must be the same size for each block.
         :param str source_content_md5:
             If given, the service will calculate the MD5 hash of the block content and compare against this value.
         :param str lease_id:
             Required if the blob has an active lease.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         """
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('copy_source_url', copy_source_url)
@@ -362,32 +383,32 @@
             'timeout': _int_to_str(timeout),
         }
         request.headers = {
             'x-ms-lease-id': _to_str(lease_id),
             'x-ms-copy-source': copy_source_url,
             'x-ms-source-content-md5': source_content_md5,
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _validate_and_format_range_headers(
             request,
             source_range_start,
             source_range_end,
             start_range_required=False,
             end_range_required=False,
             range_header_name="x-ms-source-range"
         )
 
         self._perform_request(request)
 
     # ----Convenience APIs-----------------------------------------------------
 
-    def create_blob_from_path(
-            self, container_name, blob_name, file_path, content_settings=None,
-            metadata=None, validate_content=False, progress_callback=None,
-            max_connections=2, lease_id=None, if_modified_since=None,
-            if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None):
+    def create_blob_from_path(self, container_name, blob_name, file_path, content_settings=None, metadata=None,
+                              validate_content=False, progress_callback=None, max_connections=2, lease_id=None,
+                              if_modified_since=None, if_unmodified_since=None, if_match=None, if_none_match=None,
+                              timeout=None, standard_blob_tier=None, cpk=None):
         '''
         Creates a new blob from a file path, or updates the content of an
         existing blob, with automatic chunking and progress notifications.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -435,50 +456,49 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make
             multiple calls to the Azure service and the timeout will apply to
             each call individually.
+        :param StandardBlobTier standard_blob_tier:
+            A standard blob tier value to set the blob to. For this version of the library,
+            this is only applicable to block blobs on standard storage accounts.
         :return: ETag and last modified properties for the Block Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('file_path', file_path)
 
         count = path.getsize(file_path)
         with open(file_path, 'rb') as stream:
-            return self.create_blob_from_stream(
-                container_name=container_name,
-                blob_name=blob_name,
-                stream=stream,
-                count=count,
-                content_settings=content_settings,
-                metadata=metadata,
-                validate_content=validate_content,
-                lease_id=lease_id,
-                progress_callback=progress_callback,
-                max_connections=max_connections,
-                if_modified_since=if_modified_since,
-                if_unmodified_since=if_unmodified_since,
-                if_match=if_match,
-                if_none_match=if_none_match,
-                timeout=timeout)
-
-    def create_blob_from_stream(
-            self, container_name, blob_name, stream, count=None,
-            content_settings=None, metadata=None, validate_content=False,
-            progress_callback=None, max_connections=2, lease_id=None,
-            if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None, use_byte_buffer=False):
+            return self.create_blob_from_stream(container_name=container_name, blob_name=blob_name, stream=stream,
+                                                count=count, content_settings=content_settings, metadata=metadata,
+                                                validate_content=validate_content, progress_callback=progress_callback,
+                                                max_connections=max_connections, lease_id=lease_id,
+                                                if_modified_since=if_modified_since,
+                                                if_unmodified_since=if_unmodified_since, if_match=if_match,
+                                                if_none_match=if_none_match, timeout=timeout,
+                                                standard_blob_tier=standard_blob_tier, cpk=cpk)
+
+    def create_blob_from_stream(self, container_name, blob_name, stream, count=None, content_settings=None,
+                                metadata=None, validate_content=False, progress_callback=None, max_connections=2,
+                                lease_id=None, if_modified_since=None, if_unmodified_since=None, if_match=None,
+                                if_none_match=None, timeout=None, use_byte_buffer=False, standard_blob_tier=None,
+                                cpk=None):
         '''
         Creates a new blob from a file/stream, or updates the content of
         an existing blob, with automatic chunking and progress
         notifications.
 
         :param str container_name:
             Name of existing container.
@@ -530,14 +550,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make
             multiple calls to the Azure service and the timeout will apply to
             each call individually.
         :param bool use_byte_buffer:
             If True, this will force usage of the original full block buffering upload path.
             By default, this value is False and will employ a memory-efficient,
@@ -551,14 +576,17 @@
             If max_connections > 1, the concurrency will result in a considerable amount of seeking on
             the underlying stream. For the most common inputs such as a file-like stream object, seeking
             is an inexpensive operation and this is not much of a concern. However, for other variants of streams
             this may not be the case. The trade-off for memory-efficiency must be weighed against the cost of seeking
             with your input stream.
             The SubStream class will attempt to buffer up to 4 MB internally to reduce the amount of
             seek and read calls to the underlying stream. This is particularly beneficial when uploading larger blocks.
+        :param StandardBlobTier standard_blob_tier:
+            A standard blob tier value to set the blob to. For this version of the library,
+            this is only applicable to block blobs on standard storage accounts.
         :return: ETag and last modified properties for the Block Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('stream', stream)
         _validate_encryption_required(self.require_encryption, self.key_encryption_key)
@@ -570,26 +598,42 @@
 
         # Do single put if the size is smaller than MAX_SINGLE_PUT_SIZE
         if adjusted_count is not None and (adjusted_count < self.MAX_SINGLE_PUT_SIZE):
             if progress_callback:
                 progress_callback(0, count)
 
             data = stream.read(count)
+            data_chunk = data  # to store the chunk of data read from stream each time
+
+            # keep reading from stream util length of data >= count or reaching the end of stream
+            while len(data) < count and len(data_chunk) is not 0:
+                data_chunk = stream.read(count - len(data))
+                data += data_chunk
+
+            if len(data) < count:
+                raise ValueError('Parameter:count is greater than the amount of data in the stream,'
+                                 'please specify a valid count')
+
+            if len(data) > count:
+                data = data[0:count]
+
             resp = self._put_blob(
                 container_name=container_name,
                 blob_name=blob_name,
                 blob=data,
                 content_settings=content_settings,
                 metadata=metadata,
                 validate_content=validate_content,
                 lease_id=lease_id,
                 if_modified_since=if_modified_since,
                 if_unmodified_since=if_unmodified_since,
                 if_match=if_match,
                 if_none_match=if_none_match,
+                standard_blob_tier=standard_blob_tier,
+                cpk=cpk,
                 timeout=timeout)
 
             if progress_callback:
                 progress_callback(count, count)
 
             return resp
         else:  # Size is larger than MAX_SINGLE_PUT_SIZE, must upload with multiple put_block calls
@@ -614,15 +658,16 @@
                     max_connections=max_connections,
                     progress_callback=progress_callback,
                     validate_content=validate_content,
                     lease_id=lease_id,
                     uploader_class=_BlockBlobChunkUploader,
                     timeout=timeout,
                     content_encryption_key=cek,
-                    initialization_vector=iv
+                    initialization_vector=iv,
+                    cpk=cpk,
                 )
             else:
                 block_ids = _upload_blob_substream_blocks(
                     blob_service=self,
                     container_name=container_name,
                     blob_name=blob_name,
                     blob_size=count,
@@ -630,14 +675,15 @@
                     stream=stream,
                     max_connections=max_connections,
                     progress_callback=progress_callback,
                     validate_content=validate_content,
                     lease_id=lease_id,
                     uploader_class=_BlockBlobChunkUploader,
                     timeout=timeout,
+                    cpk=cpk,
                 )
 
             return self._put_block_list(
                 container_name=container_name,
                 blob_name=blob_name,
                 block_list=block_ids,
                 content_settings=content_settings,
@@ -645,23 +691,23 @@
                 validate_content=validate_content,
                 lease_id=lease_id,
                 if_modified_since=if_modified_since,
                 if_unmodified_since=if_unmodified_since,
                 if_match=if_match,
                 if_none_match=if_none_match,
                 timeout=timeout,
-                encryption_data=encryption_data
+                encryption_data=encryption_data,
+                standard_blob_tier=standard_blob_tier,
+                cpk=cpk,
             )
 
-    def create_blob_from_bytes(
-            self, container_name, blob_name, blob, index=0, count=None,
-            content_settings=None, metadata=None, validate_content=False,
-            progress_callback=None, max_connections=2, lease_id=None,
-            if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+    def create_blob_from_bytes(self, container_name, blob_name, blob, index=0, count=None, content_settings=None,
+                               metadata=None, validate_content=False, progress_callback=None, max_connections=2,
+                               lease_id=None, if_modified_since=None, if_unmodified_since=None, if_match=None,
+                               if_none_match=None, timeout=None, standard_blob_tier=None, cpk=None):
         '''
         Creates a new blob from an array of bytes, or updates the content
         of an existing blob, with automatic chunking and progress
         notifications.
 
         :param str container_name:
             Name of existing container.
@@ -713,18 +759,26 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make
             multiple calls to the Azure service and the timeout will apply to
             each call individually.
+        :param StandardBlobTier standard_blob_tier:
+            A standard blob tier value to set the blob to. For this version of the library,
+            this is only applicable to block blobs on standard storage accounts.
         :return: ETag and last modified properties for the Block Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('blob', blob)
         _validate_not_none('index', index)
@@ -735,39 +789,27 @@
 
         if count is None or count < 0:
             count = len(blob) - index
 
         stream = BytesIO(blob)
         stream.seek(index)
 
-        return self.create_blob_from_stream(
-            container_name=container_name,
-            blob_name=blob_name,
-            stream=stream,
-            count=count,
-            content_settings=content_settings,
-            metadata=metadata,
-            validate_content=validate_content,
-            progress_callback=progress_callback,
-            max_connections=max_connections,
-            lease_id=lease_id,
-            if_modified_since=if_modified_since,
-            if_unmodified_since=if_unmodified_since,
-            if_match=if_match,
-            if_none_match=if_none_match,
-            timeout=timeout,
-            use_byte_buffer=True
-        )
-
-    def create_blob_from_text(
-            self, container_name, blob_name, text, encoding='utf-8',
-            content_settings=None, metadata=None, validate_content=False,
-            progress_callback=None, max_connections=2, lease_id=None,
-            if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None):
+        return self.create_blob_from_stream(container_name=container_name, blob_name=blob_name, stream=stream,
+                                            count=count, content_settings=content_settings, metadata=metadata,
+                                            validate_content=validate_content, progress_callback=progress_callback,
+                                            max_connections=max_connections, lease_id=lease_id,
+                                            if_modified_since=if_modified_since,
+                                            if_unmodified_since=if_unmodified_since, if_match=if_match,
+                                            if_none_match=if_none_match, timeout=timeout, use_byte_buffer=True,
+                                            standard_blob_tier=standard_blob_tier, cpk=cpk)
+
+    def create_blob_from_text(self, container_name, blob_name, text, encoding='utf-8', content_settings=None,
+                              metadata=None, validate_content=False, progress_callback=None, max_connections=2,
+                              lease_id=None, if_modified_since=None, if_unmodified_since=None, if_match=None,
+                              if_none_match=None, timeout=None, standard_blob_tier=None, cpk=None):
         '''
         Creates a new blob from str/unicode, or updates the content of an
         existing blob, with automatic chunking and progress notifications.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
@@ -815,89 +857,180 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make
             multiple calls to the Azure service and the timeout will apply to
             each call individually.
+        :param StandardBlobTier standard_blob_tier:
+            A standard blob tier value to set the blob to. For this version of the library,
+            this is only applicable to block blobs on standard storage accounts.
         :return: ETag and last modified properties for the Block Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('text', text)
 
         if not isinstance(text, bytes):
             _validate_not_none('encoding', encoding)
             text = text.encode(encoding)
 
-        return self.create_blob_from_bytes(
-            container_name=container_name,
-            blob_name=blob_name,
-            blob=text,
-            index=0,
-            count=len(text),
-            content_settings=content_settings,
-            metadata=metadata,
-            validate_content=validate_content,
-            lease_id=lease_id,
-            progress_callback=progress_callback,
-            max_connections=max_connections,
-            if_modified_since=if_modified_since,
-            if_unmodified_since=if_unmodified_since,
-            if_match=if_match,
-            if_none_match=if_none_match,
-            timeout=timeout)
+        return self.create_blob_from_bytes(container_name=container_name, blob_name=blob_name, blob=text, index=0,
+                                           count=len(text), content_settings=content_settings, metadata=metadata,
+                                           validate_content=validate_content, progress_callback=progress_callback,
+                                           max_connections=max_connections, lease_id=lease_id,
+                                           if_modified_since=if_modified_since, if_unmodified_since=if_unmodified_since,
+                                           if_match=if_match, if_none_match=if_none_match, timeout=timeout,
+                                           standard_blob_tier=standard_blob_tier, cpk=cpk)
 
     def set_standard_blob_tier(
-            self, container_name, blob_name, standard_blob_tier, timeout=None):
+            self, container_name, blob_name, standard_blob_tier, timeout=None, rehydrate_priority=None):
         '''
         Sets the block blob tiers on the blob. This API is only supported for block blobs on standard storage accounts.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of blob to update.
         :param StandardBlobTier standard_blob_tier:
             A standard blob tier value to set the blob to. For this version of the library,
             this is only applicable to block blobs on standard storage accounts.
         :param int timeout:
             The timeout parameter is expressed in seconds. This method may make
             multiple calls to the Azure service and the timeout will apply to
             each call individually.
+        :param :class:`~azure.storage.blob.models.RehydratePriority` rehydrate_priority:
+            Indicates the priority with which to rehydrate an archived blob
         '''
+        request = self._get_basic_set_blob_tier_http_request(container_name, blob_name, standard_blob_tier,
+                                                             timeout=timeout, rehydrate_priority=rehydrate_priority)
+
+        self._perform_request(request)
+
+    def batch_set_standard_blob_tier(
+            self, batch_set_blob_tier_sub_requests, timeout=None):
+        """
+        Sends a batch of multiple set block blob tiers requests.
+        This API is only supported for block blobs on standard storage accounts.
+
+        :param list(BatchSetBlobTierSubRequest) batch_set_blob_tier_sub_requests:
+            The set block blob tier requests to send as a batch.
+        :param int timeout:
+            The timeout parameter is expressed in seconds. This method may make
+            multiple calls to the Azure service and the timeout will apply to
+            each call individually.
+        :return: parsed batch set tier HTTP response which indicates if each sub-request is successful.
+        :rtype: list of :class:`~azure.storage.blob.models.BatchSubResponse`
+        """
+        self._check_batch_request(batch_set_blob_tier_sub_requests)
+
+        request = HTTPRequest()
+        request.method = 'POST'
+        request.host_locations = self._get_host_locations()
+        request.path = _get_path()
+        batch_id = str(uuid.uuid1())
+        request.headers = {
+            'Content-Type': "multipart/mixed; boundary=" + _get_batch_request_delimiter(batch_id, False, False),
+        }
+        request.query = {
+            'comp': 'batch',
+            'timeout': _int_to_str(timeout),
+        }
+
+        batch_http_requests = []
+        for batch_set_blob_tier_sub_request in batch_set_blob_tier_sub_requests:
+            batch_sub_http_request = \
+                self._construct_batch_set_blob_tier_sub_http_request(
+                    len(batch_http_requests), batch_set_blob_tier_sub_request)
+
+            batch_http_requests.append(batch_sub_http_request)
+
+        request.body = _serialize_batch_body(batch_http_requests, batch_id)
+
+        return self._perform_request(request, parser=_ingest_batch_response,
+                                     parser_args=[batch_set_blob_tier_sub_requests])
+
+    def _construct_batch_set_blob_tier_sub_http_request(self, content_id, batch_set_blob_tier_sub_request):
+        """
+        Construct an HTTPRequest instance from a batch set tier sub-request.
+
+        :param int content_id:
+            the index of sub-request in the list of sub-requests
+        :param ~azure.storage.blob.models.BatchSetBlobTierSubRequest batch_set_blob_tier_sub_request:
+            one of the set tier requests to be sent in a batch
+        :return: HTTPRequest parsed from batch set tier sub-request
+        :rtype: :class:`~azure.storage.common._http.HTTPRequest`
+        """
+        request = self._get_basic_set_blob_tier_http_request(
+            batch_set_blob_tier_sub_request.container_name,
+            batch_set_blob_tier_sub_request.blob_name,
+            batch_set_blob_tier_sub_request.standard_blob_tier,
+            rehydrate_priority=batch_set_blob_tier_sub_request.rehydrate_priority)
+        request.headers.update({
+            'Content-ID': _int_to_str(content_id),
+            'Content-Length': _int_to_str(0),
+            'Content-Transfer-Encoding': 'binary',
+            'User-Agent': self._USER_AGENT_STRING,
+        })
+
+        _update_request(request, None, self._USER_AGENT_STRING)
+        # sub-request will use the batch request id automatically, no need to generate a separate one
+        request.headers.pop('x-ms-client-request-id', None)
+
+        _add_date_header(request)
+        self.authentication.sign_request(request)
+
+        return request
+
+    def _get_basic_set_blob_tier_http_request(self, container_name, blob_name, standard_blob_tier, timeout=None,
+                                              rehydrate_priority=None):
+        """
+        Construct a basic HTTPRequest instance for set standard blob tier
+
+        For more information about the parameters please see set_standard_blob_tier
+
+        :return: an HTTPRequest for set standard blob tier
+        :rtype :class:`~azure.storage.common._http.HTTPRequest`
+        """
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('standard_blob_tier', standard_blob_tier)
 
         request = HTTPRequest()
         request.method = 'PUT'
         request.host_locations = self._get_host_locations()
         request.path = _get_path(container_name, blob_name)
         request.query = {
             'comp': 'tier',
             'timeout': _int_to_str(timeout),
         }
         request.headers = {
-            'x-ms-access-tier': _to_str(standard_blob_tier)
+            'x-ms-access-tier': _to_str(standard_blob_tier),
+            'x-ms-rehydrate-priority': _to_str(rehydrate_priority)
         }
-
-        self._perform_request(request)
+        return request
 
     def copy_blob(self, container_name, blob_name, copy_source,
                   metadata=None, source_if_modified_since=None,
                   source_if_unmodified_since=None, source_if_match=None,
                   source_if_none_match=None, destination_if_modified_since=None,
                   destination_if_unmodified_since=None, destination_if_match=None,
                   destination_if_none_match=None, destination_lease_id=None,
-                  source_lease_id=None, timeout=None, requires_sync=None):
+                  source_lease_id=None, timeout=None, requires_sync=None, standard_blob_tier=None,
+                  rehydrate_priority=None):
 
         '''
         Copies a blob. This operation returns a copy operation
         properties object. The copy operation may be configured to either be an
         asynchronous, best-effort operation, or a synchronous operation.
 
         The source must be a block blob if requires_sync is true. Any existing
@@ -993,14 +1126,19 @@
         :param str source_lease_id:
         Specify this to perform the Copy Blob operation only if
         the lease ID given matches the active lease ID of the source blob.
         :param int timeout:
         The timeout parameter is expressed in seconds.
         :param bool requires_sync:
         Enforces that the service will not return a response until the copy is complete.
+        :param StandardBlobTier standard_blob_tier:
+        A standard blob tier value to set the blob to. For this version of the library,
+        this is only applicable to block blobs on standard storage accounts.
+        :param :class:`~azure.storage.blob.models.RehydratePriority` rehydrate_priority:
+        Indicates the priority with which to rehydrate an archived blob
         :return: Copy operation properties such as status, source, and ID.
         :rtype: :class:`~azure.storage.blob.models.CopyProperties`
         '''
 
         return self._copy_blob(container_name, blob_name, copy_source,
                                metadata,
                                premium_page_blob_tier=None,
@@ -1011,21 +1149,23 @@
                                destination_if_modified_since=destination_if_modified_since,
                                destination_if_unmodified_since=destination_if_unmodified_since,
                                destination_if_match=destination_if_match,
                                destination_if_none_match=destination_if_none_match,
                                destination_lease_id=destination_lease_id,
                                source_lease_id=source_lease_id, timeout=timeout,
                                incremental_copy=False,
-                               requires_sync=requires_sync)
+                               requires_sync=requires_sync,
+                               standard_blob_tier=standard_blob_tier,
+                               rehydrate_priority=rehydrate_priority)
 
     # -----Helper methods------------------------------------
     def _put_blob(self, container_name, blob_name, blob, content_settings=None,
                   metadata=None, validate_content=False, lease_id=None, if_modified_since=None,
                   if_unmodified_since=None, if_match=None, if_none_match=None,
-                  timeout=None):
+                  cpk=None, timeout=None, standard_blob_tier=None):
         '''
         Creates a blob or updates an existing blob.
 
         See create_blob_from_* for high level
         functions that handle the creation and upload of large blobs with
         automatic chunking and progress notifications.
 
@@ -1066,16 +1206,24 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
+        :param StandardBlobTier standard_blob_tier:
+            A standard blob tier value to set the blob to. For this version of the library,
+            this is only applicable to block blobs on standard storage accounts.
         :return: ETag and last modified properties for the new Block Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_encryption_required(self.require_encryption, self.key_encryption_key)
 
@@ -1086,16 +1234,18 @@
         request.query = {'timeout': _int_to_str(timeout)}
         request.headers = {
             'x-ms-blob-type': _to_str(self.blob_type),
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
-            'If-None-Match': _to_str(if_none_match)
+            'If-None-Match': _to_str(if_none_match),
+            'x-ms-access-tier': _to_str(standard_blob_tier)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _add_metadata_headers(metadata, request)
         if content_settings is not None:
             request.headers.update(content_settings._to_headers())
         blob = _get_data_bytes_only('blob', blob)
         if self.key_encryption_key:
             encryption_data, blob = _encrypt_blob(blob, self.key_encryption_key)
             request.headers['x-ms-meta-encryptiondata'] = encryption_data
@@ -1104,15 +1254,15 @@
         if validate_content:
             computed_md5 = _get_content_md5(request.body)
             request.headers['Content-MD5'] = _to_str(computed_md5)
 
         return self._perform_request(request, _parse_base_properties)
 
     def _put_block(self, container_name, blob_name, block, block_id,
-                   validate_content=False, lease_id=None, timeout=None):
+                   validate_content=False, lease_id=None, cpk=None, timeout=None):
         '''
         See put_block for more details. This helper method
         allows for encryption or other such special behavior because
         it is safely handled by the library. These behaviors are
         prohibited in the public version of this function.
         '''
 
@@ -1128,14 +1278,15 @@
             'comp': 'block',
             'blockid': _encode_base64(_to_str(block_id)),
             'timeout': _int_to_str(timeout),
         }
         request.headers = {
             'x-ms-lease-id': _to_str(lease_id)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         request.body = _get_data_bytes_or_stream_only('block', block)
         if hasattr(request.body, 'read'):
             if _len_plus(request.body) is None:
                 try:
                     data = b''
                     for chunk in iter(lambda: request.body.read(4096), b""):
                         data += chunk
@@ -1149,15 +1300,15 @@
 
         self._perform_request(request)
 
     def _put_block_list(
             self, container_name, blob_name, block_list, content_settings=None,
             metadata=None, validate_content=False, lease_id=None, if_modified_since=None,
             if_unmodified_since=None, if_match=None, if_none_match=None,
-            timeout=None, encryption_data=None):
+            timeout=None, encryption_data=None, cpk=None, standard_blob_tier=None):
         '''
         See put_block_list for more details. This helper method
         allows for encryption or other such special behavior because
         it is safely handled by the library. These behaviors are
         prohibited in the public version of this function.
         :param str encryption_data:
             A JSON formatted string containing the encryption metadata generated for this 
@@ -1178,15 +1329,17 @@
         }
         request.headers = {
             'x-ms-lease-id': _to_str(lease_id),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match),
+            'x-ms-access-tier': _to_str(standard_blob_tier)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _add_metadata_headers(metadata, request)
         if content_settings is not None:
             request.headers.update(content_settings._to_headers())
         request.body = _get_request_body(
             _convert_block_list_to_xml(block_list))
 
         if validate_content:
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/models.py` & `azure-storage-blob-2.1.0/azure/storage/blob/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -108,14 +108,17 @@
     :ivar int append_blob_committed_block_count:
         (For Append Blobs) Number of committed blocks in the blob.
     :ivar int page_blob_sequence_number:
         (For Page Blobs) Sequence number for page blob used for coordinating
         concurrent writes.
     :ivar bool server_encrypted:
         Set to true if the blob is encrypted on the server.
+    :ivar str encryption_key_sha256:
+        The server will echo the SHA256 of the customer-provided encryption key
+        to validate the key used in the operation.
     :ivar ~azure.storage.blob.models.CopyProperties copy:
         Stores all the copy properties for the blob.
     :ivar ~azure.storage.blob.models.ContentSettings content_settings:
         Stores all the content settings for the blob.
     :ivar ~azure.storage.blob.models.LeaseProperties lease:
         Stores all the lease information for the blob.
     :ivar StandardBlobTier blob_tier:
@@ -143,14 +146,15 @@
         self.last_modified = None
         self.etag = None
         self.content_length = None
         self.content_range = None
         self.append_blob_committed_block_count = None
         self.page_blob_sequence_number = None
         self.server_encrypted = None
+        self.encryption_key_sha256 = None
         self.copy = CopyProperties()
         self.content_settings = ContentSettings()
         self.lease = LeaseProperties()
         self.blob_tier = None
         self.blob_tier_change_time = None
         self.blob_tier_inferred = False
         self.deleted_time = None
@@ -364,19 +368,33 @@
     Base response for a resource request.
     
     :ivar str etag:
         Opaque etag value that can be used to check if resource
         has been modified.
     :ivar datetime last_modified:
         Datetime for last time resource was modified.
+    :ivar bool server_encrypted:
+        The value is set to true if the contents of the request are successfully
+        encrypted using the specified algorithm.
+    :ivar str encryption_key_sha256:
+        The server will echo the SHA256 of the customer-provided encryption key
+        to validate the key used in the operation.
     '''
 
     def __init__(self):
         self.last_modified = None
         self.etag = None
+        self.request_server_encrypted = None
+        self.encryption_key_sha256 = None
+
+    def clone(self, src):
+        self.last_modified = src.last_modified
+        self.etag = src.etag
+        self.request_server_encrypted = src.request_server_encrypted
+        self.encryption_key_sha256 = src.encryption_key_sha256
 
 
 class AppendBlockProperties(ResourceProperties):
     '''
     Response for an append block request.
     
     :ivar int append_offset:
@@ -772,14 +790,26 @@
     Cool = 'Cool'
     ''' Cool '''
 
     Hot = 'Hot'
     ''' Hot '''
 
 
+class RehydratePriority(object):
+    """
+    Indicates the priority with which to rehydrate an archived blob
+    """
+
+    Standard = 'Standard'
+    ''' The rehydrate priority is standard. '''
+
+    High = 'High'
+    ''' The rehydrate priority is high. '''
+
+
 class AccountInformation(object):
     """
     Holds information related to the storage account.
 
     :ivar str sku_name:
         Name of the storage SKU, also known as account type.
         Example: Standard_LRS, Standard_ZRS, Standard_GRS, Standard_RAGRS, Premium_LRS, Premium_ZRS
@@ -819,7 +849,129 @@
         self.signed_oid = None
         self.signed_tid = None
         self.signed_start = None
         self.signed_expiry = None
         self.signed_service = None
         self.signed_version = None
         self.value = None
+
+
+class BatchDeleteSubRequest(object):
+    """
+    Represents one request in batch of multiple blob delete requests
+
+    Organizes HttpRequest objects together for batch REST operations to a single host endpoint.
+
+    :ivar str container_name:
+            Name of existing container.
+    :ivar str blob_name:
+            Name of existing blob.
+    :ivar str snapshot:
+            The snapshot parameter is an opaque DateTime value that,
+            when present, specifies the blob snapshot to delete.
+    :ivar str lease_id:
+            Required if the blob has an active lease.
+    :ivar ~azure.storage.blob.models.DeleteSnapshot delete_snapshots:
+            Required if the blob has associated snapshots.
+    :ivar datetime if_modified_since:
+            A DateTime value. Azure expects the date value passed in to be UTC.
+            If timezone is included, any non-UTC datetimes will be converted to UTC.
+            If a date is passed in without timezone info, it is assumed to be UTC.
+            Specify this header to perform the operation only
+            if the resource has been modified since the specified time.
+    :ivar datetime if_unmodified_since:
+            A DateTime value. Azure expects the date value passed in to be UTC.
+            If timezone is included, any non-UTC datetimes will be converted to UTC.
+            If a date is passed in without timezone info, it is assumed to be UTC.
+            Specify this header to perform the operation only if
+            the resource has not been modified since the specified date/time.
+    :ivar str if_match:
+            An ETag value, or the wildcard character (*). Specify this header to perform
+            the operation only if the resource's ETag matches the value specified.
+    :ivar str if_none_match:
+            An ETag value, or the wildcard character (*). Specify this header
+            to perform the operation only if the resource's ETag does not match
+            the value specified. Specify the wildcard character (*) to perform
+            the operation only if the resource does not exist, and fail the
+            operation if it does exist.
+    """
+    def __init__(self, container_name, blob_name, snapshot=None,
+                 lease_id=None, delete_snapshots=None,
+                 if_modified_since=None, if_unmodified_since=None,
+                 if_match=None, if_none_match=None):
+        self.container_name = container_name
+        self.blob_name = blob_name
+        self.snapshot = snapshot
+        self.lease_id = lease_id
+        self.delete_snapshots = delete_snapshots
+        self.if_modified_since = if_modified_since
+        self.if_unmodified_since = if_unmodified_since
+        self.if_match = if_match
+        self.if_none_match = if_none_match
+
+
+class BatchSubResponse(object):
+    """
+    Sub-response parsed from batch http sub-response
+
+    Organizes batch sub-response info and batch sub-request together for easier processing
+
+    :ivar bool is_successful:
+        Represent if the batch sub-request is successful
+    :ivar :class:`~azure.storage.common._http.HTTPResponse` http_response:
+        Parsed batch sub-response, in HTTPResponse format
+    :ivar batch_sub_request:
+        Represent the batch sub-request corresponding to the batch sub-response.
+        This could be any type of sub-request. One example is class: ~azure.storage.blob.models.BatchDeleteSubRequest
+    """
+    def __init__(self, is_successful, http_response, batch_sub_request):
+        self.is_successful = is_successful
+        self.http_response = http_response
+        self.batch_sub_request = batch_sub_request
+
+
+class BatchSetBlobTierSubRequest(object):
+    """
+    Represents one request in batch of multiple set block blob tier requests
+
+    Organizes HttpRequest objects together for batch REST operations to a single host endpoint.
+
+    :ivar str container_name:
+        Name of existing container.
+    :ivar str blob_name:
+        Name of existing blob.
+    :ivar StandardBlobTier standard_blob_tier:
+        A standard blob tier value to set the blob to. For this version of the library,
+        this is only applicable to block blobs on standard storage accounts.
+    """
+    def __init__(self, container_name, blob_name, standard_blob_tier, rehydrate_priority=None):
+        self.container_name = container_name
+        self.blob_name = blob_name
+        self.standard_blob_tier = standard_blob_tier
+        self.rehydrate_priority = rehydrate_priority
+
+class CustomerProvidedEncryptionKey(object):
+    """
+    All data in Azure Storage is encrypted at-rest using an account-level encryption key.
+    In versions 2018-06-17 and newer, you can manage the key used to encrypt blob contents
+    and application metadata per-blob by providing an AES-256 encryption key in requests to the storage service.
+
+    When you use a customer-provided key, Azure Storage does not manage or persist your key.
+    When writing data to a blob, the provided key is used to encrypt your data before writing it to disk.
+    A SHA-256 hash of the encryption key is written alongside the blob contents,
+    and is used to verify that all subsequent operations against the blob use the same encryption key.
+    This hash cannot be used to retrieve the encryption key or decrypt the contents of the blob.
+    When reading a blob, the provided key is used to decrypt your data after reading it from disk.
+    In both cases, the provided encryption key is securely discarded
+    as soon as the encryption or decryption process completes.
+
+    :ivar str key_value:
+        Base64-encoded AES-256 encryption key value.
+    :ivar str key_hash:
+        Base64-encoded SHA256 of the encryption key.
+    :ivar str algorithm:
+        Specifies the algorithm to use when encrypting data using the given key. Must be AES256.
+    """
+    def __init__(self, key_value, key_hash):
+        self.key_value = key_value
+        self.key_hash = key_hash
+        self.algorithm = 'AES256'
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/pageblobservice.py` & `azure-storage-blob-2.1.0/azure/storage/blob/pageblobservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ._encryption import _generate_blob_encryption_data
 from ._error import (
     _ERROR_PAGE_BLOB_SIZE_ALIGNMENT,
 )
 from ._serialization import (
     _get_path,
     _validate_and_format_range_headers,
+    _validate_and_add_cpk_headers,
 )
 from ._upload_chunking import (
     _PageBlobChunkUploader,
     _upload_blob_chunks,
 )
 from .baseblobservice import BaseBlobService
 from .models import (
@@ -128,15 +129,16 @@
         super(PageBlobService, self).__init__(
             account_name, account_key, sas_token, is_emulated, protocol, endpoint_suffix,
             custom_domain, request_session, connection_string, socket_timeout, token_credential)
 
     def create_blob(
             self, container_name, blob_name, content_length, content_settings=None,
             sequence_number=None, metadata=None, lease_id=None, if_modified_since=None,
-            if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None, premium_page_blob_tier=None):
+            if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None,
+            premium_page_blob_tier=None, cpk=None):
         '''
         Creates a new Page Blob.
 
         See create_blob_from_* for high level functions that handle the
         creation and upload of large blobs with automatic chunking and
         progress notifications.
 
@@ -182,14 +184,19 @@
             operation if it does exist.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :param PremiumPageBlobTier premium_page_blob_tier:
             A page blob tier value to set the blob to. The tier correlates to the size of the
             blob and number of allowed IOPS. This is only applicable to page blobs on
             premium storage accounts.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the new Page Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
 
         return self._create_blob(
             container_name,
@@ -200,15 +207,16 @@
             metadata=metadata,
             lease_id=lease_id,
             premium_page_blob_tier=premium_page_blob_tier,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
             if_none_match=if_none_match,
-            timeout=timeout
+            timeout=timeout,
+            cpk=cpk,
         )
 
     def incremental_copy_blob(self, container_name, blob_name, copy_source,
                               metadata=None, destination_if_modified_since=None, destination_if_unmodified_since=None,
                               destination_if_match=None, destination_if_none_match=None, destination_lease_id=None,
                               source_lease_id=None, timeout=None):
         '''
@@ -291,15 +299,15 @@
                                incremental_copy=True)
 
     def update_page(
             self, container_name, blob_name, page, start_range, end_range,
             validate_content=False, lease_id=None, if_sequence_number_lte=None,
             if_sequence_number_lt=None, if_sequence_number_eq=None,
             if_modified_since=None, if_unmodified_since=None,
-            if_match=None, if_none_match=None, timeout=None):
+            if_match=None, if_none_match=None, cpk=None, timeout=None):
         '''
         Updates a range of pages.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of existing blob.
@@ -350,14 +358,19 @@
             header to write the page only if the blob's ETag value matches the
             value specified. If the values do not match, the Blob service fails.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify an ETag value for this conditional
             header to write the page only if the blob's ETag value does not
             match the value specified. If the values are identical, the Blob
             service fails.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         :return: ETag and last modified properties for the updated Page Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
 
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
@@ -373,23 +386,24 @@
             if_sequence_number_lte=if_sequence_number_lte,
             if_sequence_number_lt=if_sequence_number_lt,
             if_sequence_number_eq=if_sequence_number_eq,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
             if_none_match=if_none_match,
+            cpk=cpk,
             timeout=timeout
         )
 
     def update_page_from_url(self, container_name, blob_name, start_range, end_range, copy_source_url,
                              source_range_start, source_content_md5=None, source_if_modified_since=None,
                              source_if_unmodified_since=None, source_if_match=None, source_if_none_match=None,
                              lease_id=None, if_sequence_number_lte=None, if_sequence_number_lt=None,
                              if_sequence_number_eq=None, if_modified_since=None, if_unmodified_since=None,
-                             if_match=None, if_none_match=None, timeout=None):
+                             if_match=None, if_none_match=None, cpk=None, timeout=None):
         """
         Updates a range of pages to a page blob where the contents are read from a URL.
 
         :param str container_name:
             Name of existing container.
         :param str blob_name:
             Name of blob.
@@ -460,14 +474,19 @@
             the operation only if the resource's ETag matches the value specified.
         :param str if_none_match:
             An ETag value, or the wildcard character (*). Specify this header
             to perform the operation only if the resource's ETag does not match
             the value specified. Specify the wildcard character (*) to perform
             the operation only if the resource does not exist, and fail the
             operation if it does exist.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :param int timeout:
             The timeout parameter is expressed in seconds.
         """
         _validate_encryption_unsupported(self.require_encryption, self.key_encryption_key)
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('copy_source_url', copy_source_url)
@@ -493,14 +512,15 @@
             'x-ms-if-sequence-number-lt': _to_str(if_sequence_number_lt),
             'x-ms-if-sequence-number-eq': _to_str(if_sequence_number_eq),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _validate_and_format_range_headers(
             request,
             start_range,
             end_range,
             align_to_page=True)
         _validate_and_format_range_headers(
             request,
@@ -919,15 +939,15 @@
 
     # ----Convenience APIs-----------------------------------------------------
 
     def create_blob_from_path(
             self, container_name, blob_name, file_path, content_settings=None,
             metadata=None, validate_content=False, progress_callback=None, max_connections=2,
             lease_id=None, if_modified_since=None, if_unmodified_since=None,
-            if_match=None, if_none_match=None, timeout=None, premium_page_blob_tier=None):
+            if_match=None, if_none_match=None, timeout=None, premium_page_blob_tier=None, cpk=None):
         '''
         Creates a new blob from a file path, or updates the content of an
         existing blob, with automatic chunking and progress notifications.
         Empty chunks are skipped, while non-emtpy ones(even if only partly filled) are uploaded.
 
         :param str container_name:
             Name of existing container.
@@ -981,14 +1001,19 @@
             The timeout parameter is expressed in seconds. This method may make 
             multiple calls to the Azure service and the timeout will apply to 
             each call individually.
         :param premium_page_blob_tier:
             A page blob tier value to set the blob to. The tier correlates to the size of the
             blob and number of allowed IOPS. This is only applicable to page blobs on
             premium storage accounts.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the Page Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('file_path', file_path)
 
@@ -1006,22 +1031,23 @@
                 max_connections=max_connections,
                 lease_id=lease_id,
                 if_modified_since=if_modified_since,
                 if_unmodified_since=if_unmodified_since,
                 if_match=if_match,
                 if_none_match=if_none_match,
                 timeout=timeout,
-                premium_page_blob_tier=premium_page_blob_tier)
+                premium_page_blob_tier=premium_page_blob_tier,
+                cpk=cpk)
 
     def create_blob_from_stream(
             self, container_name, blob_name, stream, count, content_settings=None,
             metadata=None, validate_content=False, progress_callback=None,
             max_connections=2, lease_id=None, if_modified_since=None,
             if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None,
-            premium_page_blob_tier=None):
+            premium_page_blob_tier=None, cpk=None):
         '''
         Creates a new blob from a file/stream, or updates the content of an
         existing blob, with automatic chunking and progress notifications.
         Empty chunks are skipped, while non-emtpy ones(even if only partly filled) are uploaded.
 
         :param str container_name:
             Name of existing container.
@@ -1079,14 +1105,19 @@
             The timeout parameter is expressed in seconds. This method may make 
             multiple calls to the Azure service and the timeout will apply to 
             each call individually.
         :param premium_page_blob_tier:
             A page blob tier value to set the blob to. The tier correlates to the size of the
             blob and number of allowed IOPS. This is only applicable to page blobs on
             premium storage accounts.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the Page Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('stream', stream)
         _validate_not_none('count', count)
@@ -1111,15 +1142,16 @@
             lease_id=lease_id,
             premium_page_blob_tier=premium_page_blob_tier,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
             if_none_match=if_none_match,
             timeout=timeout,
-            encryption_data=encryption_data
+            encryption_data=encryption_data,
+            cpk=cpk,
         )
 
         if count == 0:
             return response
 
         # _upload_blob_chunks returns the block ids for block blobs so resource_properties
         # is passed as a parameter to get the last_modified and etag for page and append blobs.
@@ -1137,25 +1169,26 @@
             validate_content=validate_content,
             lease_id=lease_id,
             uploader_class=_PageBlobChunkUploader,
             if_match=response.etag,
             timeout=timeout,
             content_encryption_key=cek,
             initialization_vector=iv,
-            resource_properties=resource_properties
+            resource_properties=resource_properties,
+            cpk=cpk,
         )
 
         return resource_properties
 
     def create_blob_from_bytes(
             self, container_name, blob_name, blob, index=0, count=None,
             content_settings=None, metadata=None, validate_content=False,
             progress_callback=None, max_connections=2, lease_id=None,
             if_modified_since=None, if_unmodified_since=None, if_match=None,
-            if_none_match=None, timeout=None, premium_page_blob_tier=None):
+            if_none_match=None, timeout=None, premium_page_blob_tier=None, cpk=None):
         '''
         Creates a new blob from an array of bytes, or updates the content
         of an existing blob, with automatic chunking and progress
         notifications. Empty chunks are skipped, while non-emtpy ones(even if only partly filled) are uploaded.
 
         :param str container_name:
             Name of existing container.
@@ -1214,14 +1247,19 @@
             The timeout parameter is expressed in seconds. This method may make 
             multiple calls to the Azure service and the timeout will apply to 
             each call individually.
         :param premium_page_blob_tier:
             A page blob tier value to set the blob to. The tier correlates to the size of the
             blob and number of allowed IOPS. This is only applicable to page blobs on
             premium storage accounts.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         :return: ETag and last modified properties for the Page Blob
         :rtype: :class:`~azure.storage.blob.models.ResourceProperties`
         '''
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('blob', blob)
         _validate_type_bytes('blob', blob)
@@ -1247,15 +1285,16 @@
             progress_callback=progress_callback,
             max_connections=max_connections,
             if_modified_since=if_modified_since,
             if_unmodified_since=if_unmodified_since,
             if_match=if_match,
             if_none_match=if_none_match,
             timeout=timeout,
-            premium_page_blob_tier=premium_page_blob_tier)
+            premium_page_blob_tier=premium_page_blob_tier,
+            cpk=cpk)
 
     def set_premium_page_blob_tier(
             self, container_name, blob_name, premium_page_blob_tier,
             timeout=None):
         '''
         Sets the page blob tiers on the blob. This API is only supported for page blobs on premium accounts.
 
@@ -1432,24 +1471,29 @@
 
     # -----Helper methods-----------------------------------------------------
 
     def _create_blob(
             self, container_name, blob_name, content_length, content_settings=None,
             sequence_number=None, metadata=None, lease_id=None, premium_page_blob_tier=None, if_modified_since=None,
             if_unmodified_since=None, if_match=None, if_none_match=None, timeout=None,
-            encryption_data=None):
+            encryption_data=None, cpk=None):
         '''
         See create_blob for more details. This helper method
         allows for encryption or other such special behavior because
         it is safely handled by the library. These behaviors are
         prohibited in the public version of this function.
         :param str encryption_data:
             The JSON formatted encryption metadata to upload as a part of the blob.
             This should only be passed internally from other methods and only applied
             when uploading entire blob contents immediately follows creation of the blob.
+        :param ~azure.storage.blob.models.CustomerProvidedEncryptionKey cpk:
+            Encrypts the data on the service-side with the given key.
+            Use of customer-provided keys must be done over HTTPS.
+            As the encryption key itself is provided in the request,
+            a secure connection must be established to transfer the key.
         '''
 
         _validate_not_none('container_name', container_name)
         _validate_not_none('blob_name', blob_name)
         _validate_not_none('content_length', content_length)
         request = HTTPRequest()
         request.method = 'PUT'
@@ -1463,29 +1507,30 @@
             'x-ms-blob-sequence-number': _to_str(sequence_number),
             'x-ms-access-tier': _to_str(premium_page_blob_tier),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _add_metadata_headers(metadata, request)
         if content_settings is not None:
             request.headers.update(content_settings._to_headers())
 
         if encryption_data is not None:
             request.headers['x-ms-meta-encryptiondata'] = encryption_data
 
         return self._perform_request(request, _parse_base_properties)
 
     def _update_page(
             self, container_name, blob_name, page, start_range, end_range,
             validate_content=False, lease_id=None, if_sequence_number_lte=None,
             if_sequence_number_lt=None, if_sequence_number_eq=None,
             if_modified_since=None, if_unmodified_since=None,
-            if_match=None, if_none_match=None, timeout=None):
+            if_match=None, if_none_match=None, cpk=None, timeout=None):
         '''
         See update_page for more details. This helper method
         allows for encryption or other such special behavior because
         it is safely handled by the library. These behaviors are
         prohibited in the public version of this function.
         '''
 
@@ -1504,14 +1549,15 @@
             'x-ms-if-sequence-number-lt': _to_str(if_sequence_number_lt),
             'x-ms-if-sequence-number-eq': _to_str(if_sequence_number_eq),
             'If-Modified-Since': _datetime_to_utc_string(if_modified_since),
             'If-Unmodified-Since': _datetime_to_utc_string(if_unmodified_since),
             'If-Match': _to_str(if_match),
             'If-None-Match': _to_str(if_none_match)
         }
+        _validate_and_add_cpk_headers(request, encryption_key=cpk, protocol=self.protocol)
         _validate_and_format_range_headers(
             request,
             start_range,
             end_range,
             align_to_page=True)
         request.body = _get_data_bytes_only('page', page)
```

### Comparing `azure-storage-blob-2.0.1/azure/storage/blob/sharedaccesssignature.py` & `azure-storage-blob-2.1.0/azure/storage/blob/sharedaccesssignature.py`

 * *Files identical despite different names*

### Comparing `azure-storage-blob-2.0.1/azure_storage_blob.egg-info/PKG-INFO` & `azure-storage-blob-2.1.0/azure_storage_blob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-storage-blob
-Version: 2.0.1
+Version: 2.1.0
 Summary: Microsoft Azure Storage Blob Client Library for Python
 Home-page: https://github.com/Azure/azure-storage-python
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Description: Microsoft Azure Storage SDK for Python
         ======================================
```

### Comparing `azure-storage-blob-2.0.1/azure_storage_blob.egg-info/SOURCES.txt` & `azure-storage-blob-2.1.0/azure_storage_blob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-storage-blob-2.0.1/setup.py` & `azure-storage-blob-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     except AttributeError:
         pass
 except ImportError:
     pass
 
 setup(
     name='azure-storage-blob',
-    version='2.0.1',
+    version='2.1.0',
     description='Microsoft Azure Storage Blob Client Library for Python',
     long_description=open('README.rst', 'r').read(),
     license='MIT License',
     author='Microsoft Corporation',
     author_email='ascl@microsoft.com',
     url='https://github.com/Azure/azure-storage-python',
     classifiers=[
@@ -68,13 +68,13 @@
     packages=find_packages(exclude=[
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.storage',
     ]),
     install_requires=[
         'azure-common>=1.1.5',
-        'azure-storage-common~=2.0'
+        'azure-storage-common~=2.1'
     ],
     extras_require={
         ":python_version<'3.0'": ['futures'],
     },
 )
```

