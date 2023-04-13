# Comparing `tmp/dissect.shellitem-3.5.dev1.tar.gz` & `tmp/dissect.shellitem-3.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.shellitem-3.5.dev1.tar", last modified: Tue Apr 11 17:44:53 2023, max compression
+gzip compressed data, was "dissect.shellitem-3.5.dev2.tar", last modified: Thu Apr 13 08:53:32 2023, max compression
```

## Comparing `dissect.shellitem-3.5.dev1.tar` & `dissect.shellitem-3.5.dev2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/shellitem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/c_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17346 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/shellitem/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/tools/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-11 17:44:43.000000 dissect.shellitem-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/downloads.win81.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/local.directory.seven.lnk
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/remote.directory.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/remote.file.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.744938 dissect.shellitem-3.5.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-13 08:53:32.744938 dissect.shellitem-3.5.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.732938 dissect.shellitem-3.5.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.736938 dissect.shellitem-3.5.dev2/dissect/shellitem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:17.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.736938 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/c_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17611 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.740938 dissect.shellitem-3.5.dev2/dissect/shellitem/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:17.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/dissect/shellitem/tools/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.736938 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:53:32.000000 dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-13 08:53:22.000000 dissect.shellitem-3.5.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:53:32.744938 dissect.shellitem-3.5.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.740938 dissect.shellitem-3.5.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:17.000000 dissect.shellitem-3.5.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:53:32.740938 dissect.shellitem-3.5.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/downloads.win81.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/local.directory.seven.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/modified_remote.file.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/remote.directory.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/data/remote.file.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tests/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 08:53:16.000000 dissect.shellitem-3.5.dev2/tox.ini
```

### Comparing `dissect.shellitem-3.5.dev1/LICENSE` & `dissect.shellitem-3.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/PKG-INFO` & `dissect.shellitem-3.5.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.shellitem-3.5.dev1/README.md` & `dissect.shellitem-3.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/c_lnk.py` & `dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/c_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/lnk.py` & `dissect.shellitem-3.5.dev2/dissect/shellitem/lnk/lnk.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 
 log = logging.getLogger(__name__)
 logging.lastResort = None
 logging.raiseExceptions = False
 
 
 class LnkExtraData:
-    """Class that represents the a LNK file's EXTRA_DATA stucture
+    """Class that represents the a LNK file's EXTRA_DATA structure
     This optional structure hold additional optional structures that convey additional information about a link target
 
     Args:
         fh: A file-like object to an EXTRA_DATA structure
     """
 
     # EXTRA_DATA = *EXTRA_DATA_BLOCK TERMINAL_BLOCK
 
     # EXTRA_DATA_BLOCK = CONSOLE_PROPS / CONSOLE_FE_PROPS / DARWIN_PROPS /
     #                    ENVIRONMENT_PROPS / ICON_ENVIRONMENT_PROPS /
     #                    KNOWN_FOLDER_PROPS / PROPERTY_STORE_PROPS /
     #                    SHIM_PROPS / SPECIAL_FOLDER_PROPS /
     #                    TRACKER_PROPS / VISTA_AND_ABOVE_IDLIST_PROPS
-    # This is kinda the same as LnkStringData only that the defined extra stuctures can wildly vary
+    # This is kinda the same as LnkStringData only that the defined extra structures can wildly vary
     def __init__(self, fh: Optional[BinaryIO] = None):
         self.extradata = {}
 
         if fh:
             self._parse(fh)
 
     def _parse(self, fh: BinaryIO) -> None:
@@ -54,15 +54,15 @@
         block_name = EXTRA_DATA_BLOCK_SIGNATURES.get_name(signature)
 
         if block_name:
             read_size = self.size - LINK_EXTRA_DATA_HEADER_SIZE
             block_data = memoryview(fh.read(read_size))
 
             if len(block_data) != read_size:
-                # Some malicous lnk files have a mismatch in the size indicated in the data block and actual bytes red.
+                # Some malicious lnk files have a mismatch in the size indicated in the data block and actual bytes red.
                 # This causes cstruct to have an EOFError when trying to parse the actual size. Which is not reflected.
                 log.warning(
                     "Mismatch in read size (%i) and actual EXTRA_DATA_BLOCK length (%i) for data block (%s)",
                     read_size,
                     len(block_data),
                     block_name,
                 )
@@ -101,15 +101,15 @@
                     struct.target_unicode = struct.target_unicode.decode("utf-16").rstrip("\x00")
 
             self.extradata.update({block_name: struct})
 
         else:
             log.warning(f"Unknown extra data block encountered with signature 0x{signature:x}")
 
-        # keep calling parse untill the TERMINAL_BLOCK is hit.
+        # keep calling parse until the TERMINAL_BLOCK is hit.
         self._parse(fh)
 
     def _parse_guid(self, guid: bytes, endianness: str = "<") -> UUID:
         if endianness == "<":
             return UUID(bytes_le=guid)
         else:
             return UUID(bytes=guid)
@@ -179,16 +179,17 @@
     def __repr__(self) -> str:
         value_string = " ".join(f"{value}" for value in self.string_data.values())
         return value_string
 
 
 class LnkInfo:
     """This class represents a LNK file's LINK_INFO structure. The optional LINK_INFO structure specifies information
-    necesarry to resolve a link target if it is not found in its original location. This includes information about the
-    volume that the target was stored on, the mapped drive letter, and a UNC path if existed when the link was created.
+    necessary to resolve a link target if it is not found in its original location. This includes information about
+    the volume that the target was stored on, the mapped drive letter, and a UNC path if existed when the link was
+    created.
 
     Args:
         fh: A file-like objet to a LINK_INFO structure
     """
 
     def __init__(self, fh: Optional[BinaryIO] = None):
         self.fh = fh
@@ -199,15 +200,15 @@
         self.linkinfo_header = None
         self.linkinfo_body = None
 
         if fh:
             self.linkinfo_header = c_lnk.LINK_INFO_HEADER(fh.read(LINK_INFO_HEADER_SIZE))
             self.flags = self.linkinfo_header.link_info_flags
 
-            # values higher than 0x24 indicate the presense of optional fields in the link info structure
+            # values higher than 0x24 indicate the presence of optional fields in the link info structure
             # if so the LocalBasePathOffsetUnicode and CommonPathSuffixOffsetUnicode fields are present
             if self.linkinfo_header.link_info_header_size >= 0x00000024:
                 log.error(
                     "Unicode link_info_header encountered. Size bigger than 0x00000024. Size encountered:"
                     f"{self.linkinfo_header.link_info_header_size}"
                 )
                 # TODO parse unicode headers. none encountered yet.
@@ -286,15 +287,15 @@
             volumeid=volumeid,
             local_base_path=local_base_path,
             common_network_relative_link=common_network_relative_link,
             common_path_suffix=common_path_suffix,
         )
 
     def flag(self, name: str) -> int:
-        """Retuns whether supplied flag is set.
+        """Returns whether supplied flag is set.
 
         Args:
             name: Name of the flag
 
         Returns:
             int: >0 if flag is set
         """
@@ -348,15 +349,15 @@
     def __repr__(self) -> str:
         return repr(self.target_idlist)
 
 
 class Lnk:
     """This class represents a LNK file's SHELL_LINK_HEADER, and the remainder of the parsed LNK file structures.
     This SHELL_LINK_HEADER structure contains identification information, timestamps, and flags that specify the
-    pressence of optional structures.
+    presence of optional structures.
 
     Parses a .lnk file (aka Microsoft Shell Item) according to the MS-SHLLINK specification
     reference: https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/%5bMS-SHLLINK%5d.pdf
 
     Args:
         path: (string) Path to a link file.
         target_idlist: A LnkTargetIdList object.
@@ -399,27 +400,38 @@
                 or self.flag("has_icon_location")
             ):
                 self.stringdata = LnkStringData(self.fh, self.flags)
 
             self.extradata = LnkExtraData(self.fh)
 
     def flag(self, name: str) -> int:
-        """Retuns whether supplied flag is set.
+        """Returns whether supplied flag is set.
 
         Args:
             name: Name of the flag
 
         Returns:
             int: >0 if flag is set
         """
         return self.flags & c_lnk.LINK_FLAGS[name]
 
     def _parse_header(self, fh: Optional[BinaryIO]) -> Optional[c_lnk.SHELL_LINK_HEADER]:
+        """Returns LINK header.
+
+        Parse the header in a buffer that does not start at offset 0
+
+        Args:
+            fh: File object
+
+        Returns:
+            LINK header if size is 0x4C, else none
+        """
+        offset = fh.tell()
         header_size = unpack("I", fh.read(4))[0]
-        fh.seek(0)
+        fh.seek(offset)
 
         if header_size == LINK_HEADER_SIZE:
             link_header = c_lnk.SHELL_LINK_HEADER(fh.read(LINK_HEADER_SIZE))
             link_clsid = str(UUID(bytes_le=link_header.link_clsid))
 
             if link_clsid == "00021401-0000-0000-c000-000000000046":
                 return link_header
```

### Comparing `dissect.shellitem-3.5.dev1/dissect/shellitem/tools/lnk.py` & `dissect.shellitem-3.5.dev2/dissect/shellitem/tools/lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/PKG-INFO` & `dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.5.dev1
+Version: 3.5.dev2
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/SOURCES.txt` & `dissect.shellitem-3.5.dev2/dissect.shellitem.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 dissect/shellitem/tools/__init__.py
 dissect/shellitem/tools/lnk.py
 tests/__init__.py
 tests/conftest.py
 tests/test_lnk.py
 tests/data/downloads.win81.lnk
 tests/data/local.directory.seven.lnk
+tests/data/modified_remote.file.xp.lnk
 tests/data/remote.directory.xp.lnk
 tests/data/remote.file.xp.lnk
```

### Comparing `dissect.shellitem-3.5.dev1/pyproject.toml` & `dissect.shellitem-3.5.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/tests/conftest.py` & `dissect.shellitem-3.5.dev2/tests/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 
 def absolute_path(filename):
     return os.path.join(os.path.dirname(__file__), filename)
 
 
 @pytest.fixture
+def xp_modified_remote_lnk_file():
+    return Path(absolute_path("data/modified_remote.file.xp.lnk"))
+
+
+@pytest.fixture
 def xp_remote_lnk_file():
     return Path(absolute_path("data/remote.file.xp.lnk"))
 
 
 @pytest.fixture
 def xp_remote_lnk_dir():
     return Path(absolute_path("data/remote.directory.xp.lnk"))
```

### Comparing `dissect.shellitem-3.5.dev1/tests/data/downloads.win81.lnk` & `dissect.shellitem-3.5.dev2/tests/data/downloads.win81.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/tests/data/local.directory.seven.lnk` & `dissect.shellitem-3.5.dev2/tests/data/local.directory.seven.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/tests/data/remote.directory.xp.lnk` & `dissect.shellitem-3.5.dev2/tests/data/remote.directory.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/tests/data/remote.file.xp.lnk` & `dissect.shellitem-3.5.dev2/tests/data/remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.5.dev1/tests/test_lnk.py` & `dissect.shellitem-3.5.dev2/tests/test_lnk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 from dissect.util.ts import uuid1timestamp
 
 from dissect.shellitem.lnk import Lnk, c_lnk
 
 
+def test_xp_custom_destination_remote_lnk_file(xp_modified_remote_lnk_file):
+    # The first 16 bytes contain the LNK GUID a to simulate a Jumplist CustomDestination file
+    fh = xp_modified_remote_lnk_file.open("rb")
+    fh.seek(16)
+
+    lnk_file = Lnk(fh)
+
+    assert lnk_file.link_header.header_size == 0x4C
+    assert str(lnk_file.clsid) == "00021401-0000-0000-c000-000000000046"
+
+
 def test_xp_remote_lnk_file(xp_remote_lnk_file):
     fh = xp_remote_lnk_file.open("rb")
     lnk_file = Lnk(fh)
 
     assert lnk_file.link_header.header_size == 0x4C
     assert str(lnk_file.clsid) == "00021401-0000-0000-c000-000000000046"
```

### Comparing `dissect.shellitem-3.5.dev1/tox.ini` & `dissect.shellitem-3.5.dev2/tox.ini`

 * *Files identical despite different names*

