# Comparing `tmp/dxsp-1.0.2.tar.gz` & `tmp/dxsp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.0.2.tar", max compression
+gzip compressed data, was "dxsp-1.0.3.tar", max compression
```

## Comparing `dxsp-1.0.2.tar` & `dxsp-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-13 06:48:08.521218 dxsp-1.0.2/LICENSE
--rw-r--r--   0        0        0     2889 2023-04-13 06:48:08.521218 dxsp-1.0.2/README.md
--rw-r--r--   0        0        0       47 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8588 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    15860 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/main.py
--rw-r--r--   0        0        0      678 2023-04-13 06:48:09.217226 dxsp-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 dxsp-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 07:40:35.667131 dxsp-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2889 2023-04-13 07:40:35.667131 dxsp-1.0.3/README.md
+-rw-r--r--   0        0        0       48 2023-04-13 07:40:35.667131 dxsp-1.0.3/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-13 07:40:35.667131 dxsp-1.0.3/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8588 2023-04-13 07:40:35.667131 dxsp-1.0.3/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    15992 2023-04-13 07:40:35.671131 dxsp-1.0.3/dxsp/main.py
+-rw-r--r--   0        0        0      678 2023-04-13 07:40:36.459186 dxsp-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 dxsp-1.0.3/PKG-INFO
```

### Comparing `dxsp-1.0.2/LICENSE` & `dxsp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.2/README.md` & `dxsp-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.2/dxsp/assets/blockchains.py` & `dxsp-1.0.3/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.2/dxsp/main.py` & `dxsp-1.0.3/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,72 +5,83 @@
 import requests
 import asyncio
 from web3 import Web3
 from pycoingecko import CoinGeckoAPI
 
 from dxsp.assets.blockchains import blockchains
 
-logging.getLogger('dxsp').addHandler(logging.NullHandler())
+logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 class DexSwap:
 
 
     def __init__(self,
-                 chain_id = 1, 
-                 wallet_address = 0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE,
-                 private_key = 0x111111111117dc0aa78b770fa6a738034120c302,
+                 chain_id: int = 1, 
+                 wallet_address: str = None,
+                 private_key: str = None,
                  block_explorer_api: str = None,
-                 w3: Web3 = None,
-                 protocol_type= "1inch",
+
                  block_explorer_url: str = None,
                  rpc: str = None,
+                 w3: Web3 = None,
+                 protocol_type: str = None,
                  dex_exchange: str = None,
-                 base_trading_symbol = 'USDC',
-                 amount_trading_option = 1,
+                 base_trading_symbol: str = None,
+                 amount_trading_option: int = 1,
                  ):
         self.chain_id = int(chain_id)
+        blockchain = blockchains[self.chain_id]
+
         self.wallet_address = wallet_address
         self.private_key = private_key
         self.block_explorer_api = block_explorer_api
-        self.block_explorer_url = block_explorer_url
-        self.rpc = rpc
-        self.w3 = w3
-        self.protocol_type = protocol_type
-        self.dex_exchange = dex_exchange
-        self.base_trading_symbol = base_trading_symbol
-        self.amount_trading_option = amount_trading_option
-
-        #🦎GECKO
-        self.gecko_api = CoinGeckoAPI() # llama_api = f"https://api.llama.fi/" maybe as backup to be reviewed
-        blockchain = blockchains[self.chain_id]
 
+        self.block_explorer_url = block_explorer_url
         if self.block_explorer_url is None:
             self.block_explorer_url = blockchain["block_explorer_url"]
+
+        self.rpc = rpc
         if self.rpc is None:
             self.rpc = blockchain["rpc"]
+
+        self.w3 = w3
         if self.w3 is None:
             self.w3 = Web3(Web3.HTTPProvider(self.rpc))
 
-        if self.protocol_type == "0x":
-            base_url = blockchain["0x"]
-            self.dex_url = f"{base_url}"
-
-        elif self.protocol_type == "1inch":
-            base_url = blockchain["1inch"]
-            self.dex_url = f"{base_url}"
-        elif self.protocol_type == "1inch_limit":
-            base_url = blockchain["1inch_limit"]
-            self.dex_url = f"{base_url}"
+        self.protocol_type = protocol_type
+        if self.protocol_type is None:
+            if self.protocol_type == "1inch_limit":
+                base_url = blockchain["1inch_limit"]
+                self.dex_url = f"{base_url}"
+            elif self.protocol_type == "0x":
+                base_url = blockchain["0x"]
+                self.dex_url = f"{base_url}"
+            else:
+                base_url = blockchain["1inch"]
+                self.dex_url = f"{base_url}"
+
+        self.dex_exchange = dex_exchange
+        if self.dex_exchange is None:
         if self.dex_exchange == blockchain["uniswap_v3"]:
             self.router = blockchain["uniswap_v3"]
         elif self.dex_exchange == blockchain["uniswap_v2"]:
             self.router = blockchain["uniswap_v2"]
         else:
             self.router = self.dex_exchange
 
+        self.base_trading_symbol = base_trading_symbol
+        if self.base_trading_symbol is None:
+            self.base_trading_symbol= 'USDC'
+
+        self.amount_trading_option = amount_trading_option
+
+        #🦎GECKO
+        self.gecko_api = CoinGeckoAPI() # llama_api = f"https://api.llama.fi/" maybe as backup to be reviewed
+
+
     @staticmethod
     def _get(url, params=None, headers=None):
         headers = { "User-Agent": "Mozilla/5.0" }
         response = requests.get(url,params =params,headers=headers)
         return response.json()
 
     async def get_quote(self, symbol):
```

### Comparing `dxsp-1.0.2/pyproject.toml` & `dxsp-1.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.0.2"
+version = "1.0.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dxsp-1.0.2/PKG-INFO` & `dxsp-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.0.2
+Version: 1.0.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

