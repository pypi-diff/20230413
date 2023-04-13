# Comparing `tmp/iconsdk-2.3.0.tar.gz` & `tmp/iconsdk-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iconsdk-2.3.0.tar", last modified: Mon Jan 30 03:49:19 2023, max compression
+gzip compressed data, was "dist/iconsdk-2.4.0.tar", last modified: Thu Apr 13 08:23:05 2023, max compression
```

## Comparing `iconsdk-2.3.0.tar` & `iconsdk-2.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-01-30 03:49:19.000000 iconsdk-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-01-30 03:49:11.000000 iconsdk-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/builder/call_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/builder/transaction_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    21956 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/icon_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk/libs/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/libs/in_memory_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/libs/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/libs/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/providers/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/signed_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/convert_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/gen_tx_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/hexadecimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk/utils/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/typing/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-01-30 03:49:11.000000 iconsdk-2.3.0/iconsdk/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-30 03:49:19.000000 iconsdk-2.3.0/iconsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-30 03:49:19.000000 iconsdk-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-30 03:49:11.000000 iconsdk-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 08:23:05.000000 iconsdk-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-04-13 08:23:00.000000 iconsdk-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/builder/call_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/builder/transaction_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/icon_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/in_memory_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/providers/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/signed_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/convert_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/hexadecimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/utils/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/typing/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 08:23:05.000000 iconsdk-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 08:23:00.000000 iconsdk-2.4.0/setup.py
```

### Comparing `iconsdk-2.3.0/PKG-INFO` & `iconsdk-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.3.0
+Version: 2.4.0
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
```

### Comparing `iconsdk-2.3.0/README.md` & `iconsdk-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/__init__.py` & `iconsdk-2.4.0/iconsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/builder/__init__.py` & `iconsdk-2.4.0/iconsdk/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/builder/call_builder.py` & `iconsdk-2.4.0/iconsdk/builder/call_builder.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/builder/transaction_builder.py` & `iconsdk-2.4.0/iconsdk/builder/transaction_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 from iconsdk.exception import DataTypeException
 from iconsdk.utils.hexadecimal import remove_0x_prefix, is_0x_prefixed, is_lowercase_hex_string
+from iconsdk.utils.typing.conversion import object_to_str
 
 
 class Transaction:
     """Super class `Transaction` which is read-only."""
 
     def __init__(self, from_: str, to: str, value: int, step_limit: int, nid: int, nonce: int, version: int,
                  timestamp: int):
@@ -68,15 +71,15 @@
         return self.__timestamp
 
     @property
     def data_type(self):
         return None
 
     @property
-    def data(self):
+    def data(self) -> dict | str | None:
         return None
 
     def to_dict(self) -> dict:
         return {"from_": self.from_, "to": self.to, "value": self.value, "step_limit": self.step_limit, "nid": self.nid,
                 "nonce": self.nonce, "version": self.version, "timestamp": self.timestamp}
 
 
@@ -107,14 +110,21 @@
     def data_type(self) -> str:
         return "deploy"
 
     @property
     def params(self) -> dict:
         return self.__params
 
+    @property
+    def data(self) -> dict | None:
+        data = {"contentType": self.__content_type, "content": self.__content}
+        if self.__params:
+            data["params"] = self.__params
+        return object_to_str(data)
+
     def to_dict(self) -> dict:
         transaction_as_dict = super().to_dict()
         transaction_as_dict.update({"content_type": self.content_type, "content": self.content,
                                     "data_type": self.data_type, "params": self.params})
         return transaction_as_dict
 
 
@@ -135,14 +145,21 @@
     def data_type(self) -> str:
         return "call"
 
     @property
     def params(self) -> dict:
         return self.__params
 
+    @property
+    def data(self) -> dict | None:
+        data = {"method": self.__method}
+        if self.__params:
+            data["params"] = self.__params
+        return object_to_str(data)
+
     def to_dict(self) -> dict:
         transaction_as_dict = super().to_dict()
         transaction_as_dict.update({"method": self.method, "data_type": self.data_type, "params": self.params})
         return transaction_as_dict
 
 
 class MessageTransaction(Transaction):
@@ -158,15 +175,15 @@
             raise DataTypeException("Message data should be hex string prefixed with '0x'.")
 
     @property
     def data_type(self) -> str:
         return "message"
 
     @property
-    def data(self) -> str:
+    def data(self) -> str | None:
         return self.__data
 
     def to_dict(self) -> dict:
         transaction_as_dict = super().to_dict()
         transaction_as_dict.update({"data_type": self.data_type, "data": self.data})
         return transaction_as_dict
 
@@ -182,14 +199,24 @@
         self.__amount = amount
 
     @property
     def data_type(self) -> str:
         return "deposit"
 
     @property
+    def data(self) -> dict | None:
+        data = {"action": self.__action}
+        if self.__action == 'withdraw':
+            if self.__id is not None:
+                data['id'] = self.__id
+            if self.__amount is not None:
+                data['amount'] = self.__amount
+        return object_to_str(data)
+
+    @property
     def action(self) -> str:
         return self.__action
 
     @property
     def id(self) -> str:
         return self.__id
```

### Comparing `iconsdk-2.3.0/iconsdk/exception.py` & `iconsdk-2.4.0/iconsdk/exception.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/icon_service.py` & `iconsdk-2.4.0/iconsdk/icon_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Union, Tuple, Any, List
+from typing import Union, Tuple, Any, List, Optional
 
 from iconsdk.builder.call_builder import Call
 from iconsdk.builder.transaction_builder import Transaction
 from iconsdk.exception import AddressException, DataTypeException
-from iconsdk.providers.provider import Provider
+from iconsdk.providers.provider import Provider, MonitorSpec, Monitor
 from iconsdk.signed_transaction import SignedTransaction
 from iconsdk.utils import get_timestamp
 from iconsdk.utils.convert_type import convert_int_to_hex_str
 from iconsdk.utils.converter import convert, \
     get_block_template_to_convert_transactions_for_genesis
-from iconsdk.utils.gen_tx_data import generate_data_value
 from iconsdk.utils.hexadecimal import add_0x_prefix, remove_0x_prefix
 from iconsdk.utils.templates import BLOCK_0_1a, BLOCK_0_3, TRANSACTION_RESULT, TRANSACTION, BLOCK_0_1A_VERSION
 from iconsdk.utils.validation import (
     is_block_height,
     is_hex_block_hash,
     is_predefined_block_value,
     is_score_address,
@@ -342,17 +341,15 @@
 
         if transaction.nonce is not None:
             params["nonce"] = convert_int_to_hex_str(transaction.nonce)
 
         if transaction.data_type is not None:
             params["dataType"] = transaction.data_type
 
-        if transaction.data_type in ('deploy', 'call'):
-            params["data"] = generate_data_value(transaction)
-        elif transaction.data_type == 'message':
+        if transaction.data is not None:
             params["data"] = transaction.data
 
         result = self.__provider.make_request('debug_estimateStep', params, full_response)
         return result if full_response else int(result, 16)
 
     def get_trace(self, tx_hash: str) -> dict:
         """
@@ -519,7 +516,18 @@
         Returns BTP source network information.
         Delegates to btp_getSourceInformation RPC method.
         https://github.com/icon-project/goloop/blob/master/doc/btp2_extension.md#btp_getSourceInformation
 
         :return: A BTP network information object
         """
         return self.__provider.make_request('btp_getSourceInformation')
+
+    def monitor(self, spec: MonitorSpec, keep_alive: Optional[float]) -> Monitor:
+        """
+        Monitor events specified in the spec
+
+        :param spec: Monitor specification
+        :param keep_alive: interval to send keep-alive while it reads a message
+        in fraction of seconds
+        :return: Monitoring handle
+        """
+        return self.__provider.make_monitor(spec, keep_alive)
```

### Comparing `iconsdk-2.3.0/iconsdk/libs/__init__.py` & `iconsdk-2.4.0/iconsdk/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/libs/in_memory_zip.py` & `iconsdk-2.4.0/iconsdk/libs/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/libs/serializer.py` & `iconsdk-2.4.0/iconsdk/libs/serializer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/libs/signer.py` & `iconsdk-2.4.0/iconsdk/libs/signer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/providers/__init__.py` & `iconsdk-2.4.0/iconsdk/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/providers/http_provider.py` & `iconsdk-2.4.0/iconsdk/monitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,155 @@
-# Copyright 2018 ICON Foundation
+#  Copyright 2023 ICON Foundation
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json
-import re
-from json.decoder import JSONDecodeError
-from time import time
-from typing import Union
-from urllib.parse import urlparse
-
-import requests
-from multimethod import multimethod
-
-from iconsdk.exception import JSONRPCException, URLException
-from iconsdk.providers.provider import Provider
-from iconsdk.utils import to_dict
-
-
-class HTTPProvider(Provider):
-    """
-    The HTTPProvider takes the full URI where the server can be found.
-    For local development this would be something like 'http://localhost:9000'.
-    """
-
-    @multimethod
-    def __init__(self, base_domain_url: str, version: int, request_kwargs: dict = None):
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+from __future__ import annotations
+
+from typing import List
+
+from iconsdk.providers.provider import MonitorSpec
+from iconsdk.utils.typing.conversion import object_to_str
+
+
+class EventFilter:
+    def __init__(self, addr: str, event: str, indexed: int, *args):
+        self.__addr = addr
+        self.__event = event
+        self.__indexed = list(args[0:indexed])
+        self.__data = list(args[indexed:])
+
+    def apply_to(self, obj: dict):
+        obj.update({
+            "event": self.__event,
+            "indexed": self.__indexed,
+            "data": self.__data,
+        })
+        if self.__addr is not None:
+            obj.update({
+                "addr": self.__addr
+            })
+
+    def as_dict(self) -> dict:
+        obj = {}
+        self.apply_to(obj)
+        return obj
+
+
+class EventMonitorSpec(MonitorSpec):
+    def __init__(self, height: int | None,
+                 filters: EventFilter | List[EventFilter],
+                 logs: bool = False,
+                 progress_interval: int = 0):
+        self.__height = height
+        self.__logs = logs
+        if type(filters) is EventFilter:
+            self.__filters = list([filters])
+        else:
+            self.__filters = filters
+        self.__progress_interval = progress_interval
+
+    def get_path(self) -> str:
+        return 'event'
+
+    def get_request(self) -> any:
+        params = {}
+        if self.__height is not None:
+            params["height"] = self.__height
+        if self.__logs:
+            params["logs"] = True
+        if self.__progress_interval > 0:
+            params["progressInterval"] = self.__progress_interval
+        if len(self.__filters) == 1:
+            self.__filters[0].apply_to(params)
+        else:
+            params["filters"] = list(map(lambda a: a.as_dict(), self.__filters))
+        return object_to_str(params)
+
+
+class BlockMonitorSpec(MonitorSpec):
+    def __init__(self, height: int | None,
+                 filters: EventFilter|List[EventFilter]|None = None,
+                 logs: bool = False):
         """
-        The initializer to be set with base domain URL and version.
+        Block monitoring spec
 
-        :param base_domain_url: base domain URL as like <scheme>://<host>:<port>
-        :param version: version for RPC server
-        :param request_kwargs: kwargs for setting to head of request
+        :param height: Block height to start monitoring
+        :param filters: One event filter or list of event filters
+        :param logs: Whether the notification includes logs or not
         """
-        uri = urlparse(base_domain_url)
-        if uri.path != '':
-            raise URLException('Path is not allowed')
-        self._serverUri = f'{uri.scheme}://{uri.netloc}'
-        self._channel = ''
-        self._version = version
-        self._request_kwargs = request_kwargs or {}
-        self._generate_url_map()
-
-    @multimethod
-    def __init__(self, full_path_url: str, request_kwargs: dict = None):
+        self.__height = height
+        self.__logs = logs
+        if type(filters) is EventFilter:
+            self.__filters = list([filters])
+        else:
+            self.__filters = filters
+
+    def get_path(self) -> str:
+        return 'block'
+
+    def get_request(self) -> any:
+        params = {}
+        if self.__height is not None:
+            params["height"] = self.__height
+        if self.__logs:
+            params["logs"] = True
+        if len(self.__filters) == 1:
+            self.__filters[0].apply_to(params)
+        else:
+            params["eventFilters"] = list(map(lambda a: a.as_dict(), self.__filters))
+        return object_to_str(params)
+
+
+class BTPMonitorSpec(MonitorSpec):
+    def __init__(self, height: int | None,
+                 network_id: int,
+                 proof_flag: bool = False,
+                 progress_interval: int = 0):
         """
-        The initializer to be set with full path url as like <scheme>://<host>:<port>/api/v3.
-        If you need to use a channel, you can use it such as <scheme>://<host>:<port>/api/v3/{channel}.
+        BTP Block event monitoring specification.
+        https://github.com/icon-project/goloop/blob/master/doc/btp2_extension.md#block
 
-        :param full_path_url: full path URL as like <scheme>://<host>:<port>/api/v3
-        :param request_kwargs: kwargs for setting to head of request
+        :param height: Height of the block to start monitoring
+        :param network_id: Network ID of the BTP Network
+        :param proof_flag: Whether it includes proof data or not
+        :param progress_interval: Progress interval to notify progress
         """
-        uri = urlparse(full_path_url)
-        self._serverUri = f'{uri.scheme}://{uri.netloc}'
-        self._channel = self._get_channel(uri.path)
-        self._version = 3
-        self._request_kwargs = request_kwargs or {}
-        self._generate_url_map()
-
-    def _generate_url_map(self):
-        def _add_channel_path(url: str):
-            if self._channel:
-                return f"{url}/{self._channel}"
-            return url
-
-        self._URL_MAP = {
-            'icx': _add_channel_path(f"{self._serverUri}/api/v{self._version}"),
-            'btp': _add_channel_path(f"{self._serverUri}/api/v{self._version}"),
-            'debug': _add_channel_path(f"{self._serverUri}/api/v{self._version}d"),
+        self.__height = height
+        self.__network_id = network_id
+        self.__proof_flag = proof_flag
+        self.__progress_interval = progress_interval
+
+    def get_path(self) -> str:
+        return 'btp'
+
+    def get_request(self) -> any:
+        params = {
+            "networkID": self.__network_id,
         }
-
-    @staticmethod
-    def _get_channel(path: str):
-        tokens = re.split("/(?=[^/]+$)", path.rstrip('/'))
-        if tokens[0] == '/api/v3':
-            return tokens[1]
-        elif tokens == ['/api', 'v3']:
-            return ''
-        raise URLException('Invalid URI path')
-
-    def __str__(self):
-        return "RPC connection to {0}".format(self._serverUri)
-
-    @to_dict
-    def _get_request_kwargs(self) -> dict:
-        if 'headers' not in self._request_kwargs:
-            yield 'headers', {'Content-Type': 'application/json'}
-        for key, value in self._request_kwargs.items():
-            yield key, value
-
-    @staticmethod
-    def _make_post_request(request_url: str, data: dict, **kwargs) -> requests.Response:
-        kwargs.setdefault('timeout', 10)
-        with requests.Session() as session:
-            response = session.post(url=request_url, data=json.dumps(data), **kwargs)
-        return response
-
-    def _make_id(self) -> int:
-        return int(time())
-
-    def make_request(self, method: str, params=None, full_response: bool = False) -> Union[str, list, dict]:
-        rpc_dict = {
-            'jsonrpc': '2.0',
-            'method': method,
-            'id': self._make_id()
-        }
-        if params:
-            rpc_dict['params'] = params
-
-        req_key = method.split('_')[0]
-        request_url = self._URL_MAP.get(req_key)
-        response = self._make_post_request(request_url, rpc_dict, **self._get_request_kwargs())
-        try:
-            return self._return_custom_response(response, full_response)
-        except JSONDecodeError:
-            raw_response = response.content.decode()
-            raise JSONRPCException(f'Unknown response: {raw_response}')
-
-    @staticmethod
-    def _return_custom_response(response: requests.Response, full_response: bool = False) -> Union[str, list, dict]:
-        content = json.loads(response.content)
-        if full_response:
-            return content
-        if response.ok:
-            return content['result']
-        raise JSONRPCException(content["error"])
+        if self.__height is not None:
+            params["height"] = self.__height
+        if self.__proof_flag:
+            params['proofFlag'] = True
+        if self.__progress_interval > 0:
+            params["progressInterval"] = self.__progress_interval
+        return object_to_str(params)
```

### Comparing `iconsdk-2.3.0/iconsdk/signed_transaction.py` & `iconsdk-2.4.0/iconsdk/signed_transaction.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from hashlib import sha3_256
 
 from iconsdk.builder.transaction_builder import Transaction
 from iconsdk.exception import DataTypeException
 from iconsdk.libs.serializer import serialize
 from iconsdk.utils import get_timestamp
 from iconsdk.utils.convert_type import convert_int_to_hex_str
-from iconsdk.utils.gen_tx_data import generate_data_value
 from iconsdk.wallet.wallet import Wallet
 
 
 class SignedTransaction:
 
     def __init__(self, transaction: Transaction, wallet: Wallet, step_limit: int = None):
         """Converts raw transaction into the signed transaction object having a signature.
@@ -64,20 +63,11 @@
 
         if transaction.nonce is not None:
             dict_tx["nonce"] = convert_int_to_hex_str(transaction.nonce)
 
         if transaction.data_type is not None:
             dict_tx["dataType"] = transaction.data_type
 
-        if transaction.data_type in ('deploy', 'call'):
-            dict_tx["data"] = generate_data_value(transaction)
-        elif transaction.data_type == 'message':
+        if transaction.data is not None:
             dict_tx["data"] = transaction.data
-        elif transaction.data_type == "deposit":
-            dict_tx["data"] = {"action": transaction.action}
-            if transaction.action == "withdraw":
-                if transaction.id is not None:
-                    dict_tx["data"]["id"] = transaction.id
-                elif transaction.amount is not None:
-                    dict_tx["data"]["amount"] = convert_int_to_hex_str(transaction.amount)
 
         return dict_tx
```

### Comparing `iconsdk-2.3.0/iconsdk/utils/__init__.py` & `iconsdk-2.4.0/iconsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/convert_type.py` & `iconsdk-2.4.0/iconsdk/utils/convert_type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/converter.py` & `iconsdk-2.4.0/iconsdk/utils/converter.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/hexadecimal.py` & `iconsdk-2.4.0/iconsdk/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/templates.py` & `iconsdk-2.4.0/iconsdk/utils/templates.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/type.py` & `iconsdk-2.4.0/iconsdk/utils/type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/typing/__init__.py` & `iconsdk-2.4.0/iconsdk/utils/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/typing/conversion.py` & `iconsdk-2.4.0/iconsdk/utils/typing/conversion.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/utils/validation.py` & `iconsdk-2.4.0/iconsdk/utils/validation.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/wallet/__init__.py` & `iconsdk-2.4.0/iconsdk/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk/wallet/wallet.py` & `iconsdk-2.4.0/iconsdk/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.3.0/iconsdk.egg-info/PKG-INFO` & `iconsdk-2.4.0/iconsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.3.0
+Version: 2.4.0
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
```

### Comparing `iconsdk-2.3.0/iconsdk.egg-info/SOURCES.txt` & `iconsdk-2.4.0/iconsdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.cfg
 setup.py
 iconsdk/__init__.py
 iconsdk/exception.py
 iconsdk/icon_service.py
+iconsdk/monitor.py
 iconsdk/signed_transaction.py
 iconsdk/version.py
 iconsdk.egg-info/PKG-INFO
 iconsdk.egg-info/SOURCES.txt
 iconsdk.egg-info/dependency_links.txt
 iconsdk.egg-info/requires.txt
 iconsdk.egg-info/top_level.txt
@@ -20,15 +21,14 @@
 iconsdk/libs/signer.py
 iconsdk/providers/__init__.py
 iconsdk/providers/http_provider.py
 iconsdk/providers/provider.py
 iconsdk/utils/__init__.py
 iconsdk/utils/convert_type.py
 iconsdk/utils/converter.py
-iconsdk/utils/gen_tx_data.py
 iconsdk/utils/hexadecimal.py
 iconsdk/utils/templates.py
 iconsdk/utils/type.py
 iconsdk/utils/validation.py
 iconsdk/utils/typing/__init__.py
 iconsdk/utils/typing/conversion.py
 iconsdk/wallet/__init__.py
```

### Comparing `iconsdk-2.3.0/setup.py` & `iconsdk-2.4.0/setup.py`

 * *Files identical despite different names*

