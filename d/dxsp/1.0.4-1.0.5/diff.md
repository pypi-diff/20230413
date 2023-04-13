# Comparing `tmp/dxsp-1.0.4.tar.gz` & `tmp/dxsp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.0.4.tar", max compression
+gzip compressed data, was "dxsp-1.0.5.tar", max compression
```

## Comparing `dxsp-1.0.4.tar` & `dxsp-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-13 08:23:27.739268 dxsp-1.0.4/LICENSE
--rw-r--r--   0        0        0     2889 2023-04-13 08:23:27.739268 dxsp-1.0.4/README.md
--rw-r--r--   0        0        0       48 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8588 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    15814 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/main.py
--rw-r--r--   0        0        0      678 2023-04-13 08:23:28.423281 dxsp-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 dxsp-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 08:47:58.222262 dxsp-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2877 2023-04-13 08:47:58.222262 dxsp-1.0.5/README.md
+-rw-r--r--   0        0        0       47 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8589 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    15819 2023-04-13 08:47:58.222262 dxsp-1.0.5/dxsp/main.py
+-rw-r--r--   0        0        0      678 2023-04-13 08:47:58.870270 dxsp-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.5/PKG-INFO
```

### Comparing `dxsp-1.0.4/LICENSE` & `dxsp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.4/README.md` & `dxsp-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - Use Base symbol like stablecoin
 
 [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/)
 ![Pypi](https://img.shields.io/pypi/dm/dxsp) ![Version](https://img.shields.io/pypi/v/dxsp)
 
 [![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko) 
 
-[![🧼CodeCheck](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%A7%BCCodeCheck.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%A7%BCCodeCheck.yml)
+[![🐍Build](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml)
 
 # Install
 `pip install dxsp`
 
 # How to use it
 ```
 from dxsp import DexSwap
```

### Comparing `dxsp-1.0.4/dxsp/assets/blockchains.py` & `dxsp-1.0.5/dxsp/assets/blockchains.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,24 @@
         "rpc": "https://rpc.ankr.com/eth_goerli",
         "uniswap_v2": "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D",
         "uniswap_v3": "",
         "1inch": "",
         "1inch_limit": "",
         "0x": "https://goerli.api.0x.org/"
     },
+    # Optimism
+    10: {
+        "block_explorer_url": "https://api-optimistic.etherscan.io/api?",
+        "rpc": "https://rpc.ankr.com/optimism",
+        "uniswap_v2": "0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f",
+        "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
+        "1inch": "https://api.1inch.exchange/v5.0/10",
+        "1inch_limit": "https://limit-orders.1inch.io/v3.0/10",
+        "0x": "https://optimism.api.0x.org/"
+    },
     # ETHEREUM Sepolia
     11155111: {
         "block_explorer_url": "https://api-Sepolia.etherscan.io/api?",
         "rpc": "https://rpc.ankr.com/eth_sepolia",
         "uniswap_v2": "",
         "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
         "1inch": "",
@@ -105,24 +115,15 @@
         "rpc": "https://rpc.ankr.com/polygon_zkevm_testnet",
         "uniswap_v2": "",
         "uniswap_v3": "",
         "1inch": "",
         "1inch_limit": "h",
         "0x": ""
     },
-    # Optimism
-    10: {
-        "block_explorer_url": "https://api-optimistic.etherscan.io/api?",
-        "rpc": "https://rpc.ankr.com/optimism",
-        "uniswap_v2": "0x5c69bee701ef814a2b6a3edd4b1652cb9cc5aa6f",
-        "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
-        "1inch": "https://api.1inch.exchange/v5.0/10",
-        "1inch_limit": "https://limit-orders.1inch.io/v3.0/10",
-        "0x": "https://optimism.api.0x.org/"
-    },
+
     # Optimism goerli
     69: {
         "block_explorer_url": "https://api-Goerli.etherscan.io/api? ne",
         "rpc": "https://rpc.ankr.com/optimism_testnet",
         "uniswap_v2": "",
         "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
         "1inch": "",
```

### Comparing `dxsp-1.0.4/dxsp/main.py` & `dxsp-1.0.5/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 
 
     def __init__(self,
                  chain_id: int = 1, 
                  wallet_address: str = None,
                  private_key: str = None,
                  block_explorer_api: str = None,
-
                  block_explorer_url: str = None,
                  rpc: str = None,
                  w3: Web3 = None,
                  protocol_type: str = None,
                  dex_exchange: str = None,
                  base_trading_symbol: str = None,
                  amount_trading_option: int = 1,
                  ):
-        self.chain_id = chain_id
-        blockchain = blockchains[self.chain_id]
+        self.chain_id = int(chain_id)
+        blockchain = blockchains[self.chain_id ]
 
         self.wallet_address = wallet_address
         self.private_key = private_key
         self.block_explorer_api = block_explorer_api
 
         self.block_explorer_url = block_explorer_url
         if self.block_explorer_url is None:
```

### Comparing `dxsp-1.0.4/pyproject.toml` & `dxsp-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.0.4"
+version = "1.0.5"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dxsp-1.0.4/PKG-INFO` & `dxsp-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.0.4
+Version: 1.0.5
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,15 @@
 - Use Base symbol like stablecoin
 
 [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/)
 ![Pypi](https://img.shields.io/pypi/dm/dxsp) ![Version](https://img.shields.io/pypi/v/dxsp)
 
 [![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko) 
 
-[![🧼CodeCheck](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%A7%BCCodeCheck.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%A7%BCCodeCheck.yml)
+[![🐍Build](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%90%8Dbuild.yml)
 
 # Install
 `pip install dxsp`
 
 # How to use it
 ```
 from dxsp import DexSwap
```

