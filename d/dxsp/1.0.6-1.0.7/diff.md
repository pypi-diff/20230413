# Comparing `tmp/dxsp-1.0.6.tar.gz` & `tmp/dxsp-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.0.6.tar", max compression
+gzip compressed data, was "dxsp-1.0.7.tar", max compression
```

## Comparing `dxsp-1.0.6.tar` & `dxsp-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-13 12:57:29.227748 dxsp-1.0.6/LICENSE
--rw-r--r--   0        0        0     2877 2023-04-13 12:57:29.227748 dxsp-1.0.6/README.md
--rw-r--r--   0        0        0      137 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8589 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    15819 2023-04-13 12:57:29.227748 dxsp-1.0.6/dxsp/main.py
--rw-r--r--   0        0        0      678 2023-04-13 12:57:30.143748 dxsp-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 13:37:21.902501 dxsp-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2877 2023-04-13 13:37:21.902501 dxsp-1.0.7/README.md
+-rw-r--r--   0        0        0      137 2023-04-13 13:37:21.902501 dxsp-1.0.7/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-13 13:37:21.902501 dxsp-1.0.7/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8589 2023-04-13 13:37:21.902501 dxsp-1.0.7/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    15979 2023-04-13 13:37:21.902501 dxsp-1.0.7/dxsp/main.py
+-rw-r--r--   0        0        0      678 2023-04-13 13:37:22.770506 dxsp-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.7/PKG-INFO
```

### Comparing `dxsp-1.0.6/LICENSE` & `dxsp-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.6/README.md` & `dxsp-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.6/dxsp/assets/blockchains.py` & `dxsp-1.0.7/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.6/dxsp/main.py` & `dxsp-1.0.7/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import requests
 import asyncio
 from web3 import Web3
 from pycoingecko import CoinGeckoAPI
 
 from dxsp.assets.blockchains import blockchains
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__).addHandler(logging.NullHandler())
+
 
 class DexSwap:
 
 
     def __init__(self,
                  chain_id: int = 1, 
                  wallet_address: str = None,
@@ -23,14 +24,15 @@
                  rpc: str = None,
                  w3: Web3 = None,
                  protocol_type: str = None,
                  dex_exchange: str = None,
                  base_trading_symbol: str = None,
                  amount_trading_option: int = 1,
                  ):
+        logger.debug("dxsp setup started")
         self.chain_id = int(chain_id)
         blockchain = blockchains[self.chain_id ]
 
         self.wallet_address = wallet_address
         self.private_key = private_key
         self.block_explorer_api = block_explorer_api
 
@@ -41,15 +43,15 @@
         self.rpc = rpc
         if self.rpc is None:
             self.rpc = blockchain["rpc"]
 
         self.w3 = w3
         if self.w3 is None:
             self.w3 = Web3(Web3.HTTPProvider(self.rpc))
-
+        logger.debug(f"self.w3 {self.w3}")
         self.protocol_type = protocol_type
         if self.protocol_type is None:
             if self.protocol_type == "0x":
                 base_url = blockchain["0x"]
             elif self.protocol_type == "1inch_limit":
                 base_url = blockchain["1inch_limit"]
             else:
@@ -77,14 +79,15 @@
     def _get(url, params=None, headers=None):
         headers = { "User-Agent": "Mozilla/5.0" }
         response = requests.get(url,params =params,headers=headers)
         return response.json()
 
     async def get_quote(self, symbol):
             asset_in_address = await self.search_contract(symbol)
+            logger.debug(f"asset_in_address {asset_in_address}")
             asset_out_address = await self.search_contract(self.base_trading_symbol)
             try:
                 if self.protocol_type == "1inch":
                     asset_out_amount=1000000000000
                     quote_url = f"{self.dex_url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
                     quote = self._get(quote_url)
                     return quote['toTokenAmount']
```

### Comparing `dxsp-1.0.6/pyproject.toml` & `dxsp-1.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.0.6"
+version = "1.0.7"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dxsp-1.0.6/PKG-INFO` & `dxsp-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.0.6
+Version: 1.0.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

