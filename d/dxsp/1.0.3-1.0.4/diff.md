# Comparing `tmp/dxsp-1.0.3.tar.gz` & `tmp/dxsp-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.0.3.tar", max compression
+gzip compressed data, was "dxsp-1.0.4.tar", max compression
```

## Comparing `dxsp-1.0.3.tar` & `dxsp-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-13 07:40:35.667131 dxsp-1.0.3/LICENSE
--rw-r--r--   0        0        0     2889 2023-04-13 07:40:35.667131 dxsp-1.0.3/README.md
--rw-r--r--   0        0        0       48 2023-04-13 07:40:35.667131 dxsp-1.0.3/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-13 07:40:35.667131 dxsp-1.0.3/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8588 2023-04-13 07:40:35.667131 dxsp-1.0.3/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    15992 2023-04-13 07:40:35.671131 dxsp-1.0.3/dxsp/main.py
--rw-r--r--   0        0        0      678 2023-04-13 07:40:36.459186 dxsp-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 dxsp-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 08:23:27.739268 dxsp-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2889 2023-04-13 08:23:27.739268 dxsp-1.0.4/README.md
+-rw-r--r--   0        0        0       48 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8588 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    15814 2023-04-13 08:23:27.739268 dxsp-1.0.4/dxsp/main.py
+-rw-r--r--   0        0        0      678 2023-04-13 08:23:28.423281 dxsp-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 dxsp-1.0.4/PKG-INFO
```

### Comparing `dxsp-1.0.3/LICENSE` & `dxsp-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.3/README.md` & `dxsp-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.3/dxsp/assets/blockchains.py` & `dxsp-1.0.4/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.3/dxsp/main.py` & `dxsp-1.0.4/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                  rpc: str = None,
                  w3: Web3 = None,
                  protocol_type: str = None,
                  dex_exchange: str = None,
                  base_trading_symbol: str = None,
                  amount_trading_option: int = 1,
                  ):
-        self.chain_id = int(chain_id)
+        self.chain_id = chain_id
         blockchain = blockchains[self.chain_id]
 
         self.wallet_address = wallet_address
         self.private_key = private_key
         self.block_explorer_api = block_explorer_api
 
         self.block_explorer_url = block_explorer_url
@@ -45,33 +45,29 @@
 
         self.w3 = w3
         if self.w3 is None:
             self.w3 = Web3(Web3.HTTPProvider(self.rpc))
 
         self.protocol_type = protocol_type
         if self.protocol_type is None:
-            if self.protocol_type == "1inch_limit":
-                base_url = blockchain["1inch_limit"]
-                self.dex_url = f"{base_url}"
-            elif self.protocol_type == "0x":
+            if self.protocol_type == "0x":
                 base_url = blockchain["0x"]
-                self.dex_url = f"{base_url}"
+            elif self.protocol_type == "1inch_limit":
+                base_url = blockchain["1inch_limit"]
             else:
                 base_url = blockchain["1inch"]
-                self.dex_url = f"{base_url}"
-
+            self.dex_url = f"{base_url}"
         self.dex_exchange = dex_exchange
-        if self.dex_exchange is None:
-        if self.dex_exchange == blockchain["uniswap_v3"]:
-            self.router = blockchain["uniswap_v3"]
-        elif self.dex_exchange == blockchain["uniswap_v2"]:
+        if (
+            self.dex_exchange is None
+            or self.dex_exchange != blockchain["uniswap_v3"]
+        ):
             self.router = blockchain["uniswap_v2"]
         else:
-            self.router = self.dex_exchange
-
+            self.router = blockchain["uniswap_v3"]
         self.base_trading_symbol = base_trading_symbol
         if self.base_trading_symbol is None:
             self.base_trading_symbol= 'USDC'
 
         self.amount_trading_option = amount_trading_option
 
         #🦎GECKO
```

### Comparing `dxsp-1.0.3/pyproject.toml` & `dxsp-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.0.3"
+version = "1.0.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dxsp-1.0.3/PKG-INFO` & `dxsp-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.0.3
+Version: 1.0.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

