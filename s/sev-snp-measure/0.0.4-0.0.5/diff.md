# Comparing `tmp/sev-snp-measure-0.0.4.tar.gz` & `tmp/sev-snp-measure-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sev-snp-measure-0.0.4.tar", last modified: Thu Apr 13 07:30:54 2023, max compression
+gzip compressed data, was "sev-snp-measure-0.0.5.tar", last modified: Thu Apr 13 09:52:59 2023, max compression
```

## Comparing `sev-snp-measure-0.0.4.tar` & `sev-snp-measure-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/
--rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.4/LICENSE
--rw-r--r--   0 dubek     (1000) dubek     (1000)     6713 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5968 2023-04-13 06:53:56.000000 sev-snp-measure-0.0.4/README.md
--rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2022-04-11 09:47:58.000000 sev-snp-measure-0.0.4/pyproject.toml
--rw-r--r--   0 dubek     (1000) dubek     (1000)      973 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/setup.cfg
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/
--rw-r--r--   0 dubek     (1000) dubek     (1000)     6713 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)      590 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/SOURCES.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/dependency_links.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)      109 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/entry_points.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       40 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/requires.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/top_level.txt
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/sevsnpmeasure/
--rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.4/sevsnpmeasure/__init__.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3616 2023-04-13 07:27:01.000000 sev-snp-measure-0.0.4/sevsnpmeasure/cli.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     2462 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.4/sevsnpmeasure/gctx.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3626 2023-04-10 12:19:02.000000 sev-snp-measure-0.0.4/sevsnpmeasure/guest.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5591 2023-04-10 12:20:41.000000 sev-snp-measure-0.0.4/sevsnpmeasure/id_block.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     4736 2023-04-10 12:19:02.000000 sev-snp-measure-0.0.4/sevsnpmeasure/ovmf.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3488 2022-06-08 14:31:05.000000 sev-snp-measure-0.0.4/sevsnpmeasure/sev_hashes.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2022-04-24 09:17:37.000000 sev-snp-measure-0.0.4/sevsnpmeasure/sev_mode.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     1609 2023-03-07 15:16:17.000000 sev-snp-measure-0.0.4/sevsnpmeasure/vcpu_types.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5727 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.4/sevsnpmeasure/vmsa.py
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/tests/
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3130 2023-04-10 12:19:02.000000 sev-snp-measure-0.0.4/tests/test_guest.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     1149 2023-04-10 12:20:41.000000 sev-snp-measure-0.0.4/tests/test_id_block.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)      480 2022-06-08 12:42:41.000000 sev-snp-measure-0.0.4/tests/test_vcpu_types.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.5/LICENSE
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6770 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6025 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.5/README.md
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2022-04-11 09:47:58.000000 sev-snp-measure-0.0.5/pyproject.toml
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      973 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/setup.cfg
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6770 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      590 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/SOURCES.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/dependency_links.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      109 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/entry_points.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       40 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/requires.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/top_level.txt
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/sevsnpmeasure/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.5/sevsnpmeasure/__init__.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3616 2023-04-13 09:51:04.000000 sev-snp-measure-0.0.5/sevsnpmeasure/cli.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     2462 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.5/sevsnpmeasure/gctx.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     4035 2023-04-13 07:59:29.000000 sev-snp-measure-0.0.5/sevsnpmeasure/guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5591 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.5/sevsnpmeasure/id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     4765 2023-04-13 07:59:29.000000 sev-snp-measure-0.0.5/sevsnpmeasure/ovmf.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3488 2022-06-08 14:31:05.000000 sev-snp-measure-0.0.5/sevsnpmeasure/sev_hashes.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2022-04-24 09:17:37.000000 sev-snp-measure-0.0.5/sevsnpmeasure/sev_mode.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1609 2023-03-07 15:16:17.000000 sev-snp-measure-0.0.5/sevsnpmeasure/vcpu_types.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5727 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.5/sevsnpmeasure/vmsa.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/tests/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3130 2023-04-13 07:59:29.000000 sev-snp-measure-0.0.5/tests/test_guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1149 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.5/tests/test_id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      480 2022-06-08 12:42:41.000000 sev-snp-measure-0.0.5/tests/test_vcpu_types.py
```

### Comparing `sev-snp-measure-0.0.4/LICENSE` & `sev-snp-measure-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/PKG-INFO` & `sev-snp-measure-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 Home-page: https://github.com/IBM/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik1@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -155,14 +155,15 @@
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
 * [sev Rust crate](https://github.com/virtee/sev)
 * [snp-digest-rs](https://github.com/slp/snp-digest-rs)
 * [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
+* [go-sev-guest](https://github.com/google/go-sev-guest)
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
```

### Comparing `sev-snp-measure-0.0.4/README.md` & `sev-snp-measure-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
 * [sev Rust crate](https://github.com/virtee/sev)
 * [snp-digest-rs](https://github.com/slp/snp-digest-rs)
 * [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
+* [go-sev-guest](https://github.com/google/go-sev-guest)
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
```

### Comparing `sev-snp-measure-0.0.4/setup.cfg` & `sev-snp-measure-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sev-snp-measure
-version = 0.0.4
+version = 0.0.5
 author = Dov Murik
 author_email = dov.murik1@il.ibm.com
 description = Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/sev-snp-measure
 project_urls =
```

### Comparing `sev-snp-measure-0.0.4/sev_snp_measure.egg-info/PKG-INFO` & `sev-snp-measure-0.0.5/sev_snp_measure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 Home-page: https://github.com/IBM/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik1@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -155,14 +155,15 @@
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
 * [sev Rust crate](https://github.com/virtee/sev)
 * [snp-digest-rs](https://github.com/slp/snp-digest-rs)
 * [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
+* [go-sev-guest](https://github.com/google/go-sev-guest)
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
```

### Comparing `sev-snp-measure-0.0.4/sev_snp_measure.egg-info/SOURCES.txt` & `sev-snp-measure-0.0.5/sev_snp_measure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/cli.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import base64
 import sys
 
 from sevsnpmeasure import guest
 from sevsnpmeasure import vcpu_types
 from .sev_mode import SevMode
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 
 def auto_base_int(s: str) -> int:
     return int(s, 0)
 
 
 def main() -> int:
```

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/gctx.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/gctx.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/guest.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/guest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 # Copyright 2022- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import hashlib
+from typing import Optional
 
 from .gctx import GCTX
 from .ovmf import OVMF, SectionType
 from .sev_hashes import SevHashes
 from .vmsa import VMSA
 from .sev_mode import SevMode
 
@@ -25,22 +26,35 @@
         return seves_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append)
     elif mode == SevMode.SEV:
         return sev_calc_launch_digest(ovmf_file, kernel, initrd, append)
     else:
         raise ValueError("unknown mode")
 
 
-def snp_update_metadata_pages(gctx, ovmf) -> None:
+def snp_update_kernel_hashes(gctx: GCTX, ovmf: OVMF, sev_hashes: Optional[SevHashes], gpa: int, size: int) -> None:
+    if sev_hashes:
+        sev_hashes_table_gpa = ovmf.sev_hashes_table_gpa()
+        offset_in_page = sev_hashes_table_gpa & PAGE_MASK
+        sev_hashes_page = sev_hashes.construct_page(offset_in_page)
+        assert size == len(sev_hashes_page)
+        gctx.update_normal_pages(gpa, sev_hashes_page)
+    else:
+        gctx.update_zero_pages(gpa, size)
+
+
+def snp_update_metadata_pages(gctx: GCTX, ovmf: OVMF, sev_hashes: Optional[SevHashes]) -> None:
     for desc in ovmf.metadata_items():
         if desc.section_type() == SectionType.SNP_SEC_MEM:
             gctx.update_zero_pages(desc.gpa, desc.size)
         elif desc.section_type() == SectionType.SNP_SECRETS:
             gctx.update_secrets_page(desc.gpa)
         elif desc.section_type() == SectionType.CPUID:
             gctx.update_cpuid_page(desc.gpa)
+        elif desc.section_type() == SectionType.SNP_KERNEL_HASHES:
+            snp_update_kernel_hashes(gctx, ovmf, sev_hashes, desc.gpa, desc.size)
         else:
             raise ValueError("unknown OVMF metadata section type")
 
 
 def calc_snp_ovmf_hash(ovmf_file: str) -> bytes:
     ovmf = OVMF(ovmf_file)
 
@@ -59,23 +73,19 @@
     # Ignores the contents of the OVMF file in front of us.
     if ovmf_hash_str:
         ovmf_hash = bytearray.fromhex(ovmf_hash_str)
         gctx = GCTX(seed=ovmf_hash)
     else:
         gctx.update_normal_pages(ovmf.gpa(), ovmf.data())
 
+    sev_hashes = None
     if kernel:
-        sev_hashes_table_gpa = ovmf.sev_hashes_table_gpa()
-        offset_in_page = sev_hashes_table_gpa & PAGE_MASK
-        sev_hashes_page_gpa = sev_hashes_table_gpa & ~PAGE_MASK
         sev_hashes = SevHashes(kernel, initrd, append)
-        sev_hashes_page = sev_hashes.construct_page(offset_in_page)
-        gctx.update_normal_pages(sev_hashes_page_gpa, sev_hashes_page)
 
-    snp_update_metadata_pages(gctx, ovmf)
+    snp_update_metadata_pages(gctx, ovmf, sev_hashes)
 
     vmsa = VMSA(SevMode.SEV_SNP, ovmf.sev_es_reset_eip(), vcpu_sig)
     for vmsa_page in vmsa.pages(vcpus):
         gctx.update_vmsa_page(vmsa_page)
 
     return gctx.ld()
```

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/id_block.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/id_block.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/ovmf.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/ovmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # Types of sections declared by OVMF SEV Metadata, as appears in:
 # https://github.com/tianocore/edk2/blob/edk2-stable202205/OvmfPkg/ResetVector/X64/OvmfSevMetadata.asm
 class SectionType(Enum):
     SNP_SEC_MEM = 1
     SNP_SECRETS = 2
     CPUID = 3
+    SNP_KERNEL_HASHES = 0x10
 
 
 class OvmfSevMetadataSectionDesc(ctypes.LittleEndianStructure):
     _pack_ = 1
     _fields_ = [
         ("gpa", c_uint32),
         ("size", c_uint32),
```

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/sev_hashes.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/sev_hashes.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/sev_mode.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/sev_mode.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/vcpu_types.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/vcpu_types.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/sevsnpmeasure/vmsa.py` & `sev-snp-measure-0.0.5/sevsnpmeasure/vmsa.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.4/tests/test_guest.py` & `sev-snp-measure-0.0.5/tests/test_guest.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,16 @@
                 "tests/fixtures/ovmf_suffix.bin",
                 "/dev/null",
                 "/dev/null",
                 "",
                 snp_ovmf_hash_str=ovmf_hash)
         self.assertEqual(
                 ld.hex(),
-                '6a23d4774a60f6238506b531e0cb60a698a198db100476f6'
-                'fadb724f60c144bed9c71a3903b9ca425ff82b376c381b33')
+                '228c6b5fe659c179041ed98ccc13e1199a2d85575ef28b7b'
+                '851e4a0b3a178f5401620cc67b1aa22bca198566defb63e1')
 
     # Test of we can a full LD from the OVMF hash
     def test_snp_ovmf_hash_full(self):
         ovmf_hash = guest.calc_snp_ovmf_hash("tests/fixtures/ovmf_suffix.bin").hex()
         self.assertEqual(
                 ovmf_hash,
                 '4ef91bfd7241908300ac19305a694753cbc8db28104f356f'
@@ -44,30 +44,30 @@
                 "/dev/null",
                 "/dev/null",
                 "",
                 snp_ovmf_hash_str=ovmf_hash)
 
         self.assertEqual(
                 ld.hex(),
-                '38859e76ac5fa5009c8249eb2f44dafb33a2a1f41efd65ce'
-                'b13f042864abab87d018dc64da21628b320a98642f25ae6c')
+                'd68382026a91989d9428675e9b220548b76db03c75234403'
+                '16b90f0a72c33b5fee2ade72791fb1c0ff0a923741e5190d')
 
     def test_snp(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_suffix.bin",
                 "/dev/null",
                 "/dev/null",
                 "")
         self.assertEqual(
                 ld.hex(),
-                '38859e76ac5fa5009c8249eb2f44dafb33a2a1f41efd65ce'
-                'b13f042864abab87d018dc64da21628b320a98642f25ae6c')
+                'd68382026a91989d9428675e9b220548b76db03c75234403'
+                '16b90f0a72c33b5fee2ade72791fb1c0ff0a923741e5190d')
 
     def test_seves(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_ES,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_suffix.bin",
```

### Comparing `sev-snp-measure-0.0.4/tests/test_id_block.py` & `sev-snp-measure-0.0.5/tests/test_id_block.py`

 * *Files identical despite different names*

