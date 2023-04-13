# Comparing `tmp/types-netaddr-0.8.0.7.tar.gz` & `tmp/types-netaddr-0.8.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-netaddr-0.8.0.7.tar", last modified: Mon Mar 27 18:24:54 2023, max compression
+gzip compressed data, was "types-netaddr-0.8.0.8.tar", last modified: Thu Apr 13 12:31:03 2023, max compression
```

## Comparing `types-netaddr-0.8.0.7.tar` & `types-netaddr-0.8.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-27 18:24:53.000000 types-netaddr-0.8.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:53.000000 types-netaddr-0.8.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/netaddr-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:24:53.000000 types-netaddr-0.8.0.7/netaddr-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/netaddr-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/contrib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/contrib/subnet_splitter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/netaddr-stubs/eui/
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/eui/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/eui/ieee.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/fbsocket.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/netaddr-stubs/ip/
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/ip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/ip/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/ip/iana.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/ip/nmap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/ip/rfc1924.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/ip/sets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/netaddr-stubs/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/strategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/strategy/eui48.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/strategy/eui64.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/strategy/ipv4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-27 18:21:24.000000 types-netaddr-0.8.0.7/netaddr-stubs/strategy/ipv6.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-27 18:24:53.000000 types-netaddr-0.8.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:54.279496 types-netaddr-0.8.0.7/types_netaddr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-27 18:24:54.000000 types-netaddr-0.8.0.7/types_netaddr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-27 18:24:54.000000 types-netaddr-0.8.0.7/types_netaddr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:54.000000 types-netaddr-0.8.0.7/types_netaddr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-27 18:24:54.000000 types-netaddr-0.8.0.7/types_netaddr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/netaddr-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/contrib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/contrib/subnet_splitter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/eui/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/eui/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/eui/ieee.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/fbsocket.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/ip/
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/iana.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/nmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/rfc1924.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/ip/sets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/netaddr-stubs/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui48.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui64.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-13 12:30:41.000000 types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv6.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:31:03.676277 types-netaddr-0.8.0.8/types_netaddr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 12:31:03.000000 types-netaddr-0.8.0.8/types_netaddr.egg-info/top_level.txt
```

### Comparing `types-netaddr-0.8.0.7/CHANGELOG.md` & `types-netaddr-0.8.0.8/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.8.0.8 (2023-04-13)
+
+Style: prefer `type[Foo | Bar]` over `type[Foo] | type[Bar]` (#10039)
+
 ## 0.8.0.7 (2023-03-27)
 
 Add defaults for third-party stubs M-O (#9956)
 
 ## 0.8.0.6 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
```

### Comparing `types-netaddr-0.8.0.7/PKG-INFO` & `types-netaddr-0.8.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-netaddr
-Version: 0.8.0.7
+Version: 0.8.0.8
 Summary: Typing stubs for netaddr
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `netaddr`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
```

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/__init__.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/core.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/eui/__init__.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/eui/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -31,24 +31,24 @@
     def __init__(self, iab: str | int, strict: bool = False) -> None: ...
     def __eq__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     def registration(self) -> DictDotLookup: ...
 
 class EUI(BaseIdentifier):
     def __init__(
-        self, addr: EUI | int | str, version: int | None = None, dialect: type[mac_eui48] | type[eui64_base] | None = None
+        self, addr: EUI | int | str, version: int | None = None, dialect: type[mac_eui48 | eui64_base] | None = None
     ) -> None: ...
     @property
     def value(self) -> int: ...
     @value.setter
     def value(self, value: str | SupportsInt | SupportsIndex) -> None: ...
     @property
-    def dialect(self) -> type[mac_eui48] | type[eui64_base]: ...
+    def dialect(self) -> type[mac_eui48 | eui64_base]: ...
     @dialect.setter
-    def dialect(self, value: type[mac_eui48] | type[eui64_base] | None) -> None: ...
+    def dialect(self, value: type[mac_eui48 | eui64_base] | None) -> None: ...
     @property
     def oui(self) -> OUI: ...
     @property
     def ei(self) -> str: ...
     def is_iab(self) -> bool: ...
     @property
     def iab(self) -> IAB | None: ...
@@ -77,8 +77,8 @@
     def bin(self) -> str: ...
     def eui64(self) -> Self: ...
     def modified_eui64(self) -> Self: ...
     def ipv6(self, prefix: str | SupportsInt | SupportsIndex) -> IPAddress: ...
     def ipv6_link_local(self) -> IPAddress: ...
     @property
     def info(self) -> DictDotLookup: ...
-    def format(self, dialect: type[mac_eui48] | type[eui64_base] | None = None) -> str: ...
+    def format(self, dialect: type[mac_eui48 | eui64_base] | None = None) -> str: ...
```

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/eui/ieee.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/eui/ieee.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
 class IABIndexParser(Publisher):
     fh: BinaryIO
     def __init__(self, ieee_file: BinaryIO | FileDescriptorOrPath) -> None: ...
     def parse(self) -> None: ...
 
 def create_index_from_registry(
-    registry_fh: BinaryIO | FileDescriptorOrPath, index_path: StrOrBytesPath, parser: type[OUIIndexParser] | type[IABIndexParser]
+    registry_fh: BinaryIO | FileDescriptorOrPath, index_path: StrOrBytesPath, parser: type[OUIIndexParser | IABIndexParser]
 ) -> None: ...
 def create_indices() -> None: ...
 def load_index(index: _INDEX, fp: Iterable[bytes]) -> None: ...
 def load_indices() -> None: ...
```

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/ip/__init__.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/ip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/ip/glob.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/ip/glob.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/ip/iana.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/ip/iana.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/ip/sets.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/ip/sets.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/strategy/__init__.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/strategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/strategy/eui48.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui48.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/strategy/eui64.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/strategy/eui64.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/strategy/ipv4.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv4.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/netaddr-stubs/strategy/ipv6.pyi` & `types-netaddr-0.8.0.8/netaddr-stubs/strategy/ipv6.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-0.8.0.7/setup.py` & `types-netaddr-0.8.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `netaddr`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.8.0.7",
+      version="0.8.0.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md",
```

### Comparing `types-netaddr-0.8.0.7/types_netaddr.egg-info/PKG-INFO` & `types-netaddr-0.8.0.8/types_netaddr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-netaddr
-Version: 0.8.0.7
+Version: 0.8.0.8
 Summary: Typing stubs for netaddr
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `netaddr`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
```

### Comparing `types-netaddr-0.8.0.7/types_netaddr.egg-info/SOURCES.txt` & `types-netaddr-0.8.0.8/types_netaddr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

