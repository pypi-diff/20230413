# Comparing `tmp/dissect.xfs-3.4.dev2.tar.gz` & `tmp/dissect.xfs-3.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.xfs-3.4.dev2.tar", last modified: Thu Mar 16 13:05:31 2023, max compression
+gzip compressed data, was "dissect.xfs-3.5.dev4.tar", last modified: Thu Apr 13 07:42:29 2023, max compression
```

## Comparing `dissect.xfs-3.4.dev2.tar` & `dissect.xfs-3.5.dev4.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:31.488075 dissect.xfs-3.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-16 13:05:31.488075 dissect.xfs-3.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:31.484075 dissect.xfs-3.4.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:31.484075 dissect.xfs-3.4.dev2/dissect/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/dissect/xfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/dissect/xfs/c_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/dissect/xfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/dissect/xfs/xfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:31.484075 dissect.xfs-3.4.dev2/dissect.xfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-16 13:05:31.000000 dissect.xfs-3.4.dev2/dissect.xfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-16 13:05:31.000000 dissect.xfs-3.4.dev2/dissect.xfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:05:31.000000 dissect.xfs-3.4.dev2/dissect.xfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:05:31.000000 dissect.xfs-3.4.dev2/dissect.xfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:05:31.000000 dissect.xfs-3.4.dev2/dissect.xfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-16 13:05:22.000000 dissect.xfs-3.4.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:05:31.488075 dissect.xfs-3.4.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:31.484075 dissect.xfs-3.4.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:18.000000 dissect.xfs-3.4.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:05:31.484075 dissect.xfs-3.4.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/tests/data/xfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/tests/data/xfs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/tests/data/xfs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/tests/data/xfs_symlink_test3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/tests/test_xfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:05:17.000000 dissect.xfs-3.4.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.405170 dissect.xfs-3.5.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.409170 dissect.xfs-3.5.dev4/dissect/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41820 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/c_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/dissect/xfs/xfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.409170 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:42:29.000000 dissect.xfs-3.5.dev4/dissect.xfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-13 07:42:15.000000 dissect.xfs-3.5.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.409170 dissect.xfs-3.5.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:29.413170 dissect.xfs-3.5.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_bigtime.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    45520 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    42015 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    41936 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tests/test_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 07:42:09.000000 dissect.xfs-3.5.dev4/tox.ini
```

### Comparing `dissect.xfs-3.4.dev2/LICENSE` & `dissect.xfs-3.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.4.dev2/PKG-INFO` & `dissect.xfs-3.5.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.4.dev2
+Version: 3.5.dev4
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.xfs-3.4.dev2/README.md` & `dissect.xfs-3.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.4.dev2/dissect/xfs/xfs.py` & `dissect.xfs-3.5.dev4/dissect/xfs/xfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from __future__ import annotations
+
 import io
 import logging
 import os
 import stat
+from datetime import datetime
 from functools import lru_cache
+from typing import BinaryIO, Iterator, Optional, Union
 from uuid import UUID
 
+from dissect.cstruct import Instance
 from dissect.util import ts
 from dissect.util.stream import RangeStream, RunlistStream
 
 from dissect.xfs.c_xfs import FILETYPES, c_xfs
 from dissect.xfs.exceptions import (
     Error,
     FileNotFoundError,
@@ -19,15 +24,15 @@
 )
 
 log = logging.getLogger(__name__)
 log.setLevel(os.getenv("DISSECT_LOG_XFS", "CRITICAL"))
 
 
 class XFS:
-    def __init__(self, fh):
+    def __init__(self, fh: BinaryIO):
         self.fh = fh
         self.ag = {0: AllocationGroup(self, fh, 0)}
         self.sb = self.ag[0].sb
 
         self.block_size = self.sb.sb_blocksize
         self.version = self.sb.sb_versionnum & c_xfs.XFS_SB_VERSION_NUMBITS
         self._has_ftype = (self.version == 5 and self.sb.sb_features_incompat & c_xfs.XFS_SB_FEAT_INCOMPAT_FTYPE) or (
@@ -38,85 +43,88 @@
         # This should be the same across all AG's
         self._inum_bits = self.sb.sb_agblklog + self.sb.sb_inopblog
         self._inum_mask = (1 << self._inum_bits) - 1
         self._inum_max = self.sb.sb_agblocks * self.sb.sb_inopblock
         # Not necessarily correct for the last AG, but doesn't harm
         self._ag_size = self.sb.sb_agblocks * self.block_size
 
-        self._lblock_s = c_xfs.xfs_btree_lblock_v5 if self._has_crc else c_xfs.xfs_btree_lblock
-        self._sblock_s = c_xfs.xfs_btree_sblock_v5 if self._has_crc else c_xfs.xfs_btree_sblock
+        self._lblock_s = c_xfs.xfs_btree_lblock_crc if self._has_crc else c_xfs.xfs_btree_lblock
+        self._sblock_s = c_xfs.xfs_btree_sblock_crc if self._has_crc else c_xfs.xfs_btree_sblock
 
         self.name = self.sb.sb_fname.split(b"\x00")[0].decode(errors="surrogateescape")
         self.uuid = UUID(bytes=self.sb.sb_uuid)
         self.meta_uuid = UUID(bytes=self.sb.sb_meta_uuid)
 
         self.root = self.get_inode(self.sb.sb_rootino)
 
-    def get(self, path, node=None):
+    def get(self, path: Union[int, str], node: Optional[INode] = None) -> INode:
         if isinstance(path, int):
             return self.get_inode(path)
 
         node = node if node else self.root
 
         parts = path.split("/")
-        for i, p in enumerate(parts):
-            if not p:
+        for part in parts:
+            if not part:
                 continue
 
-            while node.filetype == stat.S_IFLNK and i < len(parts):
+            while node.filetype == stat.S_IFLNK:
                 node = node.link_inode
 
-            dirlist = node.listdir()
-            if p not in dirlist:
+            for entry in node.iterdir():
+                if entry.filename == part:
+                    node = entry
+                    break
+            else:
                 raise FileNotFoundError(f"File not found: {path}")
 
-            node = dirlist[p]
-
         return node
 
-    def get_allocation_group(self, agnum):
+    def get_allocation_group(self, agnum: int) -> AllocationGroup:
         if agnum not in self.ag:
             self.ag[agnum] = AllocationGroup(self, RangeStream(self.fh, agnum * self._ag_size, self._ag_size), agnum)
         return self.ag[agnum]
 
-    def get_inode(self, absinum, *args, **kwargs):
+    def get_inode(self, absinum: int, *args, **kwargs) -> INode:
         return self.get_relative_inode(absinum >> self._inum_bits, absinum & self._inum_mask, *args, **kwargs)
 
-    def get_relative_inode(self, agnum, inum, *args, **kwargs):
+    def get_relative_inode(self, agnum: int, inum: int, *args, **kwargs) -> INode:
         if agnum >= self.sb.sb_agcount:
             raise Error(f"Allocation group num exceeds number of allocation groups: {agnum} >= {self.sb.sb_agcount}")
         elif inum >= self._inum_max:
             raise Error(f"inode number exceeds number of inodes per allocation group: {inum} >= {self._inum_max}")
 
         return self.get_allocation_group(agnum).get_inode(inum, *args, **kwargs)
 
-    def walk_agi(self, block, agnum):
+    def walk_agi(self, block: int, agnum: int) -> Iterator[Instance]:
         for record in self.walk_small_tree(block, agnum, 16, (c_xfs.XFS_IBT_MAGIC, c_xfs.XFS_IBT_CRC_MAGIC)):
             yield c_xfs.xfs_inobt_rec(record)
 
-    def walk_extents(self, block):
+    def walk_extents(self, block: int) -> Iterator[tuple[int, int, int, int]]:
         for record in self.walk_large_tree(block, 16, (c_xfs.XFS_BMAP_MAGIC, c_xfs.XFS_BMAP_CRC_MAGIC)):
             yield parse_fsblock(record)
 
-    def walk_large_tree(self, block, leaf_size, magic=None):
+    def walk_large_tree(self, block: int, leaf_size: int, magic: Optional[list[int]] = None) -> Iterator[bytes]:
         self.fh.seek(block * self.block_size)
         root = self._lblock_s(self.fh)
 
-        for record in self._walk_large_tree(root, leaf_size, magic):
-            yield record
+        yield from self._walk_large_tree(root, leaf_size, magic)
 
-    def walk_small_tree(self, block, agnum, leaf_size, magic=None):
+    def walk_small_tree(
+        self, block: int, agnum: int, leaf_size: int, magic: Optional[list[int]] = None
+    ) -> Iterator[bytes]:
         block = agnum * self.sb.sb_agblocks + block
         self.fh.seek(block * self.block_size)
         root = self._sblock_s(self.fh)
 
-        for record in self._walk_small_tree(root, leaf_size, agnum, magic):
-            yield record
+        yield from self._walk_small_tree(root, leaf_size, agnum, magic)
 
-    def _walk_small_tree(self, node, leaf_size, agnum, magic=None):
+    def _walk_small_tree(
+        self, node: Instance, leaf_size: int, agnum: int, magic: Optional[list[int]] = None
+    ) -> Iterator[bytes]:
         fh = self.fh
         if magic and node.bb_magic not in magic:
             magic_values = ", ".join([f"0x{magic_value:x}" for magic_value in magic])
             raise Error(f"B+Tree node has invalid magic. Expected one of ({magic_values}), got 0x{node.bb_magic:x}")
 
         if node.bb_level == 0:
             buf = fh.read(node.bb_numrecs * leaf_size)
@@ -127,18 +135,17 @@
             maxrecs = (self.block_size - len(self._sblock_s)) // 8
             fh.seek(maxrecs * 4, io.SEEK_CUR)
             ptrs = c_xfs.uint32[node.bb_numrecs](fh)
             for ptr in ptrs:
                 block = agnum * self.sb.sb_agblocks + ptr
                 fh.seek(block * self.block_size)
 
-                for res in self._walk_small_tree(self._sblock_s(fh), leaf_size, agnum, magic):
-                    yield res
+                yield from self._walk_small_tree(self._sblock_s(fh), leaf_size, agnum, magic)
 
-    def _walk_large_tree(self, node, leaf_size, magic=None):
+    def _walk_large_tree(self, node: Instance, leaf_size: int, magic: Optional[list[int]] = None) -> Iterator[bytes]:
         fh = self.fh
         if magic and node.bb_magic not in magic:
             magic_values = ", ".join([f"0x{magic_value:x}" for magic_value in magic])
             raise Error(f"B+Tree node has invalid magic. Expected one of ({magic_values}), got 0x{node.bb_magic:x}")
 
         if node.bb_level == 0:
             buf = fh.read(node.bb_numrecs * leaf_size)
@@ -150,20 +157,19 @@
             fh.seek(maxrecs * 8, io.SEEK_CUR)
             ptrs = c_xfs.uint64[node.bb_numrecs](fh)
             for ptr in ptrs:
                 agnum, blknum = fsb_to_bb(ptr, self.sb.sb_agblklog)
                 block = agnum * self.sb.sb_agblocks + blknum
                 fh.seek(block * self.block_size)
 
-                for res in self._walk_large_tree(self._lblock_s(fh), leaf_size, magic):
-                    yield res
+                yield from self._walk_large_tree(self._lblock_s(fh), leaf_size, magic)
 
 
 class AllocationGroup:
-    def __init__(self, xfs, fh, num):
+    def __init__(self, xfs: XFS, fh: BinaryIO, num: int):
         self.xfs = xfs
         self.fh = fh
         self.num = num
 
         fh.seek(0)
 
         self.sb = c_xfs.xfs_sb(fh)
@@ -187,42 +193,58 @@
             raise Error("Not a valid XFS filesystem (AGI magic mismatch)")
 
         # This should be the same across all AG's
         self._inum_bits = sb.sb_agblklog + sb.sb_inopblog
         self._inum_mask = (1 << self._inum_bits) - 1
         self._inum_max = sb.sb_agblocks * sb.sb_inopblock
 
-    @lru_cache(1024)
-    def get_inode(self, inum, filename=None, filetype=None, parent=None, lazy=False):
+        self.get_inode = lru_cache(4096)(self.get_inode)
+
+    def get_inode(
+        self,
+        inum: int,
+        filename: Optional[str] = None,
+        filetype: Optional[int] = None,
+        parent: Optional[INode] = None,
+        lazy: bool = False,
+    ) -> INode:
         inode = INode(self, inum, filename, filetype, parent=parent)
 
         if not lazy:
             inode._inode = inode._read_inode()
 
         return inode
 
-    def walk_extents(self, fsb):
+    def walk_extents(self, fsb: int) -> Iterator[tuple[int, int, int, int]]:
         agnum, blknum = fsb_to_bb(fsb, self.sb.sb_agblklog)
         block = agnum * self.xfs.sb.sb_agblocks + blknum
-        for fs_block in self.xfs.walk_extents(block):
-            yield fs_block
+        yield from self.xfs.walk_extents(block)
 
-    def walk_agi(self):
-        for inobt_record in self.xfs.walk_agi(self.agi.agi_root, self.num):
-            yield inobt_record
+    def walk_agi(self) -> Iterator[Instance]:
+        yield from self.xfs.walk_agi(self.agi.agi_root, self.num)
 
-    def walk_tree(self, fsb, magic=None, small=False):
+    def walk_tree(self, fsb: int, magic: Optional[list[int]] = None, small: bool = False):
         agnum, blknum = fsb_to_bb(fsb, self.sb.sb_agblklog)
         block = agnum * self.xfs.sb.sb_agblocks + blknum
-        for record in self.xfs.walk_tree(block, magic, small):
-            yield record
+
+        if small:
+            yield from self.xfs.walk_small_tree(block, agnum, 16, magic)
+        else:
+            yield from self.xfs.walk_large_tree(block, 16, magic)
 
 
 class INode:
-    def __init__(self, ag, inum, filename=None, filetype=None, parent=None):
+    def __init__(
+        self,
+        ag: AllocationGroup,
+        inum: int,
+        filename: Optional[str] = None,
+        filetype: Optional[int] = None,
+        parent: Optional[INode] = None,
+    ):
         self.ag = ag
         self.xfs = ag.xfs
         self.inum = inum + (ag.num << ag._inum_bits)
         self.relative_inum = inum
         self.parent = parent
         self._inode = None
         self._buf = None
@@ -231,45 +253,65 @@
         self._filetype = filetype
         self._link = None
         self._link_inode = None
 
         self._dirlist = None
         self._runlist = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<inode {self.inum} ({self.ag.num}:{self.relative_inum})>"
 
-    def _read_inode(self):
+    def _read_inode(self) -> Instance:
         self.ag.fh.seek(self.relative_inum * self.ag.sb.sb_inodesize)
         self._buf = io.BytesIO(self.ag.fh.read(self.ag.sb.sb_inodesize))
         inode = c_xfs.xfs_dinode(self._buf)
 
         if inode.di_magic != c_xfs.XFS_DINODE_MAGIC:
             raise Error(f"{self!r} has invalid inode magic")
 
         return inode
 
     @property
-    def inode(self):
+    def inode(self) -> Instance:
         if not self._inode:
             self._inode = self._read_inode()
         return self._inode
 
+    def _has_bigtime(self) -> bool:
+        return self.inode.di_version >= 3 and self.inode.di_flags2 & c_xfs.XFS_DIFLAG2_BIGTIME != 0
+
+    def _has_large_extent_counts(self) -> bool:
+        return self.inode.di_version >= 3 and self.inode.di_flags2 & c_xfs.XFS_DIFLAG2_NREXT64 != 0
+
     @property
-    def size(self):
+    def size(self) -> int:
         return self.inode.di_size
 
     @property
-    def filetype(self):
+    def data_extents(self) -> int:
+        if self._has_large_extent_counts():
+            return self.inode.di_big_nextents
+        # Actually di_nextents, but we optimized the union away
+        return self.inode.di_big_anextents
+
+    @property
+    def attr_extents(self) -> int:
+        if self._has_large_extent_counts():
+            return self.inode.di_big_anextents
+        # Actually di_anextents, but we optimized the union away
+        return self.inode.di_nrext64_pad
+
+    @property
+    def filetype(self) -> int:
         if not self._filetype:
             self._filetype = stat.S_IFMT(self.inode.di_mode)
         return self._filetype
 
     @property
-    def link(self):
+    def link(self) -> str:
         if self.filetype != stat.S_IFLNK:
             raise NotASymlinkError(f"{self!r} is not a symlink")
 
         if not self._link:
             if self.inode.di_format != c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_LOCAL and self.xfs.version == 5:
                 fh = self.open()
 
@@ -279,15 +321,15 @@
 
                 self._link = fh.read(header.sl_bytes).decode(errors="surrogateescape")
             else:
                 self._link = self.open().read().decode(errors="surrogateescape")
         return self._link
 
     @property
-    def link_inode(self):
+    def link_inode(self) -> INode:
         if not self._link_inode:
             # Relative lookups work because . and .. are actual directory entries
             link = self.link
             if link.startswith("/"):
                 relnode = None
             elif link.startswith("../"):
                 relnode = self.parent
@@ -295,240 +337,234 @@
                     raise SymlinkUnavailableException(f"{self!r} is a symlink to another filesystem")
             else:
                 relnode = self.parent
             self._link_inode = self.xfs.get(self.link, relnode)
         return self._link_inode
 
     @property
-    def atime(self):
+    def atime(self) -> datetime:
         return ts.from_unix_ns(self.atime_ns)
 
     @property
-    def atime_ns(self):
-        return (self.inode.di_atime.t_sec * 1000000000) + self.inode.di_atime.t_nsec
+    def atime_ns(self) -> int:
+        return _parse_ts(self.inode.di_atime, self._has_bigtime())
 
     @property
-    def mtime(self):
+    def mtime(self) -> datetime:
         return ts.from_unix_ns(self.mtime_ns)
 
     @property
-    def mtime_ns(self):
-        return (self.inode.di_mtime.t_sec * 1000000000) + self.inode.di_mtime.t_nsec
+    def mtime_ns(self) -> int:
+        return _parse_ts(self.inode.di_mtime, self._has_bigtime())
 
     @property
-    def ctime(self):
+    def ctime(self) -> datetime:
         return ts.from_unix_ns(self.ctime_ns)
 
     @property
-    def ctime_ns(self):
-        return (self.inode.di_ctime.t_sec * 1000000000) + self.inode.di_ctime.t_nsec
+    def ctime_ns(self) -> int:
+        return _parse_ts(self.inode.di_ctime, self._has_bigtime())
 
     @property
-    def crtime(self):
+    def crtime(self) -> datetime:
         return ts.from_unix_ns(self.crtime_ns)
 
     @property
-    def crtime_ns(self):
-        return (self.inode.di_crtime.t_sec * 1000000000) + self.inode.di_crtime.t_nsec
-
-    def listdir(self):
-        if self.filetype != stat.S_IFDIR:
-            raise NotADirectoryError(f"{self!r} is not a directory")
+    def crtime_ns(self) -> int:
+        return _parse_ts(self.inode.di_crtime, self._has_bigtime())
 
+    def listdir(self) -> dict[str, INode]:
         if not self._dirlist:
-            dirs = {}
-
-            buf = self.open()
-            if self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_LOCAL:
-                header = c_xfs.xfs_dir2_sf_hdr(buf)
-                inum_s = c_xfs.uint64 if header.i8count else c_xfs.uint32
-
-                if header.i8count:
-                    header.parent = (header.parent << 32) | c_xfs.uint32(buf)
-
-                dirs["."] = self
-                dirs[".."] = self.xfs.get_inode(header.parent)
+            self._dirlist = {node.filename: node for node in self.iterdir()}
+        return self._dirlist
 
-                for _ in range(header.count):
-                    entry = c_xfs.xfs_dir2_sf_entry(buf)
-                    fname = entry.name.decode(errors="surrogateescape")
-                    ftype = c_xfs.uint8(buf) if self.xfs._has_ftype else 0
-                    inum = inum_s(buf)
+    dirlist = listdir
 
-                    ftype = FILETYPES[ftype]
+    def iterdir(self) -> Iterator[INode]:
+        if self.filetype != stat.S_IFDIR:
+            raise NotADirectoryError(f"{self!r} is not a directory")
 
-                    dirs[fname] = self.xfs.get_inode(inum, fname, ftype, parent=self, lazy=True)
-            elif self.inode.di_format in (
-                c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_EXTENTS,
-                c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_BTREE,
-            ):
-                for block_num in range(self.size // self.xfs.block_size):
-                    buf.seek(block_num * self.xfs.block_size)
-
-                    block_data = buf.read(self.xfs.block_size)
-                    block = io.BytesIO(block_data)
-
-                    block.seek(-len(c_xfs.xfs_dir2_block_tail), io.SEEK_END)
-                    tail = c_xfs.xfs_dir2_block_tail(block)
-                    block.seek(0)
+        buf = self.open()
+        if self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_LOCAL:
+            header = c_xfs.xfs_dir2_sf_hdr(buf)
+            inum_s = c_xfs.uint64 if header.i8count else c_xfs.uint32
 
-                    if self.inode.di_nextents > 1:
-                        entries_end = self.xfs.block_size
-                    else:
-                        entries_end = self.xfs.block_size
-                        entries_end -= len(c_xfs.xfs_dir2_block_tail)
-                        entries_end -= len(c_xfs.xfs_dir2_leaf_entry) * tail.count
-
-                    if self.xfs.version == 5:
-                        header = c_xfs.xfs_dir3_data_hdr(block)
-                        if header.magic not in (c_xfs.XFS_DIR3_BLOCK_MAGIC, c_xfs.XFS_DIR3_DATA_MAGIC):
-                            # Probably a sparse block
-                            continue
-                    else:
-                        header = c_xfs.xfs_dir2_data_hdr(block)
-                        if header.magic not in (c_xfs.XFS_DIR2_BLOCK_MAGIC, c_xfs.XFS_DIR2_DATA_MAGIC):
-                            # Probably a sparse block
-                            continue
+            if header.i8count:
+                header.parent = (header.parent << 32) | c_xfs.uint32(buf)
 
-                    if self.xfs._has_ftype:
-                        data_entry = c_xfs.xfs_dir2_data_entry_ftype
-                    else:
-                        data_entry = c_xfs.xfs_dir2_data_entry
+            yield self.xfs.get_inode(self.inum, filename=".")
+            yield self.xfs.get_inode(header.parent, filename="..")
 
-                    while True:
-                        if block.tell() >= entries_end:
-                            break
+            for _ in range(header.count):
+                entry = c_xfs.xfs_dir2_sf_entry(buf)
+                fname = entry.name.decode(errors="surrogateescape")
+                ftype = c_xfs.uint8(buf) if self.xfs._has_ftype else 0
+                inum = inum_s(buf)
 
-                        try:
-                            if block_data[block.tell() : block.tell() + 2] == b"\xff\xff":
-                                unused = c_xfs.xfs_dir2_data_unused(block)
+                ftype = FILETYPES[ftype]
 
-                                block.read(unused.length - 6)
+                yield self.xfs.get_inode(inum, fname, ftype, parent=self, lazy=True)
+        elif self.inode.di_format in (
+            c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_EXTENTS,
+            c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_BTREE,
+        ):
+            for block_num in range(self.size // self.xfs.block_size):
+                buf.seek(block_num * self.xfs.block_size)
 
-                                misalign = block.tell() % 8
-                                if misalign:
-                                    block.seek(8 - misalign, io.SEEK_CUR)
+                block_data = buf.read(self.xfs.block_size)
+                block = io.BytesIO(block_data)
 
-                                continue
+                block.seek(-len(c_xfs.xfs_dir2_block_tail), io.SEEK_END)
+                tail = c_xfs.xfs_dir2_block_tail(block)
+                block.seek(0)
+
+                if self.data_extents > 1:
+                    entries_end = self.xfs.block_size
+                else:
+                    entries_end = self.xfs.block_size
+                    entries_end -= len(c_xfs.xfs_dir2_block_tail)
+                    entries_end -= len(c_xfs.xfs_dir2_leaf_entry) * tail.count
+
+                if self.xfs.version == 5:
+                    header = c_xfs.xfs_dir3_data_hdr(block)
+                    if header.magic not in (c_xfs.XFS_DIR3_BLOCK_MAGIC, c_xfs.XFS_DIR3_DATA_MAGIC):
+                        # Probably a sparse block
+                        continue
+                else:
+                    header = c_xfs.xfs_dir2_data_hdr(block)
+                    if header.magic not in (c_xfs.XFS_DIR2_BLOCK_MAGIC, c_xfs.XFS_DIR2_DATA_MAGIC):
+                        # Probably a sparse block
+                        continue
+
+                if self.xfs._has_ftype:
+                    data_entry = c_xfs.xfs_dir2_data_entry_ftype
+                else:
+                    data_entry = c_xfs.xfs_dir2_data_entry
+
+                while True:
+                    if block.tell() >= entries_end:
+                        break
+
+                    try:
+                        if block_data[block.tell() : block.tell() + 2] == b"\xff\xff":
+                            unused = c_xfs.xfs_dir2_data_unused(block)
 
-                            entry = data_entry(block)
+                            block.read(unused.length - 6)
 
-                            # Entries are 8 byte aligned
-                            # uint64 inum | uint8 namelen | variable name | uint8 ftype | uint16 tag
                             misalign = block.tell() % 8
                             if misalign:
                                 block.seek(8 - misalign, io.SEEK_CUR)
-                        except EOFError:
-                            break
-
-                        inum = entry.inumber
-                        if inum >> 48 == 0xFFFF:  # XFS_DIR2_DATA_FREE_TAG
-                            break
 
-                        if self.xfs._has_ftype:
-                            ftype = FILETYPES[entry.ftype]
-                        else:
-                            ftype = None
+                            continue
 
-                        fname = entry.name.decode(errors="surrogateescape")
+                        entry = data_entry(block)
 
-                        dirs[fname] = self.xfs.get_inode(inum, fname, ftype, parent=self, lazy=True)
-            else:
-                raise Error(f"{self!r} has invalid inode format for dirlist")
+                        # Entries are 8 byte aligned
+                        # uint64 inum | uint8 namelen | variable name | uint8 ftype | uint16 tag
+                        misalign = block.tell() % 8
+                        if misalign:
+                            block.seek(8 - misalign, io.SEEK_CUR)
+                    except EOFError:
+                        break
+
+                    inum = entry.inumber
+                    if inum >> 48 == 0xFFFF:  # XFS_DIR2_DATA_FREE_TAG
+                        break
 
-            self._dirlist = dirs
+                    if self.xfs._has_ftype:
+                        ftype = FILETYPES[entry.ftype]
+                    else:
+                        ftype = None
 
-        return self._dirlist
+                    fname = entry.name.decode(errors="surrogateescape")
 
-    dirlist = listdir
+                    yield self.xfs.get_inode(inum, fname, ftype, parent=self, lazy=True)
+        else:
+            raise Error(f"{self!r} has invalid inode format for dirlist")
 
-    def datafork(self):
+    def datafork(self) -> BinaryIO:
         offset = 0xB0 if self.inode.di_version == 0x3 else 0x64
         if self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_LOCAL:
             size = self.size
         elif self.inode.di_forkoff:
             size = self.inode.di_forkoff * 8
         else:
             size = self.ag.sb.sb_inodesize - offset
 
         return RangeStream(self._buf, offset, size)
 
-    def attrfork(self):
+    def attrfork(self) -> BinaryIO:
         if self.inode.di_forkoff == 0:
             raise Error(f"{self!r} has no extended attributes")
 
         offset = 0xB0 if self.inode.di_version == 0x3 else 0x64
         offset += self.inode.di_forkoff * 8
         size = self.ag.sb.sb_inodesize - offset
 
         return RangeStream(self._buf, offset, size)
 
-    def dataruns(self):
+    def dataruns(self) -> list[tuple[Optional[int], int]]:
         if not self._runlist:
             runs = []
             run_offset = 0
+            expected_runs = (self.size + self.xfs.block_size - 1) // self.xfs.block_size
+
+            for offset, block, count, _ in self._iter_blocks():
+                if offset != run_offset:
+                    gap = offset - run_offset
+                    runs.append((None, gap))
+                    run_offset += gap
+
+                # Convert filesystem blocks to logical blocks
+                agnum, blknum = fsb_to_bb(block, self.ag.sb.sb_agblklog)
+                block = agnum * self.xfs.sb.sb_agblocks + blknum
 
-            if self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_EXTENTS:
-                buf = self.datafork().read(self.inode.di_nextents * 16)
-                for extent_num in range(self.inode.di_nextents):
-                    offset, block, count, _ = parse_fsblock(buf[extent_num * 16 : (extent_num + 1) * 16])
-
-                    # Sparse gaps
-                    if offset != run_offset:
-                        gap = offset - run_offset
-                        runs.append((None, gap))
-                        run_offset += gap
-
-                    # Convert filesystem blocks to logical blocks
-                    agnum, blknum = fsb_to_bb(block, self.ag.sb.sb_agblklog)
-                    block = agnum * self.xfs.sb.sb_agblocks + blknum
-
-                    runs.append((block, count))
-                    run_offset += count
-            elif self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_BTREE:
-                # B+tree extent lists are always large trees (64bit block numbers)
-                df = self.datafork()
-                root = c_xfs.xfs_bmdr_block(df)
-
-                # Pointers start around halfway
-                maxrecs = (df.size - 4) // 16
-                df.seek(4 + maxrecs * 8)
-                ptrs = c_xfs.uint64[root.bb_numrecs](df)
-
-                for ptr in ptrs:
-                    for offset, block, count, _ in self.ag.walk_extents(ptr):
-                        if offset != run_offset:
-                            gap = offset - run_offset
-                            runs.append((None, gap))
-                            run_offset += gap
-
-                        agnum, blknum = fsb_to_bb(block, self.ag.sb.sb_agblklog)
-                        block = agnum * self.xfs.sb.sb_agblocks + blknum
-                        runs.append((block, count))
-                        run_offset += count
+                runs.append((block, count))
+                run_offset += count
+
+            if run_offset < expected_runs:
+                runs.append((None, expected_runs - run_offset))
 
             self._runlist = runs
         return self._runlist
 
-    def open(self):
+    def _iter_blocks(self) -> Iterator[tuple[int, int, int, int]]:
+        if self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_EXTENTS:
+            buf = self.datafork().read(self.data_extents * 16)
+            for extent_num in range(self.data_extents):
+                yield parse_fsblock(buf[extent_num * 16 : (extent_num + 1) * 16])
+        elif self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_BTREE:
+            # B+tree extent lists are always large trees (64bit block numbers)
+            df = self.datafork()
+            root = c_xfs.xfs_bmdr_block(df)
+
+            # Pointers start around halfway
+            maxrecs = (df.size - 4) // 16
+            df.seek(4 + maxrecs * 8)
+            ptrs = c_xfs.uint64[root.bb_numrecs](df)
+
+            for ptr in ptrs:
+                yield from self.ag.walk_extents(ptr)
+
+    def open(self) -> BinaryIO:
         if self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_LOCAL:
             return self.datafork()
         elif self.inode.di_format in (
             c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_EXTENTS,
             c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_BTREE,
         ):
             return RunlistStream(self.xfs.fh, self.dataruns(), self.size, self.xfs.block_size)
         elif self.inode.di_format == c_xfs.xfs_dinode_fmt.XFS_DINODE_FMT_DEV:
             raise UnsupportedDataforkException(f"{self!r} is a character/block device.")
         else:
             dinode_type = c_xfs.xfs_dinode_fmt(self.inode.di_format)
             raise UnsupportedDataforkException(f"{self!r} is an unsupported datafork: {dinode_type}")
 
 
-def parse_fsblock(s):
+def parse_fsblock(s: bytes) -> tuple[int, int, int, int]:
     # MSB -> LSB
     # flag = 1 bit
     # offset = 54 bits
     # block = 52 bits
     # count = 21 bits
     l0, l1 = c_xfs.uint64[2](s)
 
@@ -536,11 +572,20 @@
     offset = (l0 & ((1 << 63) - 1)) >> 9
     block = (l0 & ((1 << 9) - 1)) << 43 | (l1 >> 21)
     count = l1 & ((1 << 21) - 1)
 
     return offset, block, count, flag
 
 
-def fsb_to_bb(block, agblklog):
+def fsb_to_bb(block: int, agblklog: int) -> tuple[int, int]:
     agnum = block >> agblklog
     blknum = block & ((1 << agblklog) - 1)
     return agnum, blknum
+
+
+def _parse_ts(ts: int, is_bigtime: bool) -> int:
+    if is_bigtime:
+        sec, nsec = divmod(ts, 1000000000)
+        sec -= 1 << 31
+    else:
+        sec, nsec = ts >> 32, ts & 0xFFFFFFFF
+    return (sec * 1000000000) + nsec
```

### Comparing `dissect.xfs-3.4.dev2/dissect.xfs.egg-info/PKG-INFO` & `dissect.xfs-3.5.dev4/dissect.xfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.4.dev2
+Version: 3.5.dev4
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.xfs-3.4.dev2/pyproject.toml` & `dissect.xfs-3.5.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.4.dev2/tests/data/xfs.bin.gz` & `dissect.xfs-3.5.dev4/tests/data/xfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.4.dev2/tests/data/xfs_symlink_test1.bin.gz` & `dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.4.dev2/tests/data/xfs_symlink_test2.bin.gz` & `dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.4.dev2/tests/data/xfs_symlink_test3.bin.gz` & `dissect.xfs-3.5.dev4/tests/data/xfs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.4.dev2/tox.ini` & `dissect.xfs-3.5.dev4/tox.ini`

 * *Files identical despite different names*

