# Comparing `tmp/sev-snp-measure-0.0.3.tar.gz` & `tmp/sev-snp-measure-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sev-snp-measure-0.0.3.tar", last modified: Tue May 17 12:51:29 2022, max compression
+gzip compressed data, was "sev-snp-measure-0.0.4.tar", last modified: Thu Apr 13 07:30:54 2023, max compression
```

## Comparing `sev-snp-measure-0.0.3.tar` & `sev-snp-measure-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2022-05-17 12:51:29.559290 sev-snp-measure-0.0.3/
--rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.3/LICENSE
--rw-r--r--   0 dubek     (1000) dubek     (1000)     4776 2022-05-17 12:51:29.559290 sev-snp-measure-0.0.3/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)     4031 2022-05-17 12:50:22.000000 sev-snp-measure-0.0.3/README.md
--rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2022-04-11 09:47:58.000000 sev-snp-measure-0.0.3/pyproject.toml
--rw-r--r--   0 dubek     (1000) dubek     (1000)      858 2022-05-17 12:51:29.559290 sev-snp-measure-0.0.3/setup.cfg
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2022-05-17 12:51:29.559290 sev-snp-measure-0.0.3/sev_snp_measure.egg-info/
--rw-r--r--   0 dubek     (1000) dubek     (1000)     4776 2022-05-17 12:51:29.000000 sev-snp-measure-0.0.3/sev_snp_measure.egg-info/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)      458 2022-05-17 12:51:29.000000 sev-snp-measure-0.0.3/sev_snp_measure.egg-info/SOURCES.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2022-05-17 12:51:29.000000 sev-snp-measure-0.0.3/sev_snp_measure.egg-info/dependency_links.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       59 2022-05-17 12:51:29.000000 sev-snp-measure-0.0.3/sev_snp_measure.egg-info/entry_points.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2022-05-17 12:51:29.000000 sev-snp-measure-0.0.3/sev_snp_measure.egg-info/top_level.txt
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2022-05-17 12:51:29.559290 sev-snp-measure-0.0.3/sevsnpmeasure/
--rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.3/sevsnpmeasure/__init__.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3315 2022-05-17 12:50:22.000000 sev-snp-measure-0.0.3/sevsnpmeasure/cli.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     2442 2022-03-09 18:23:20.000000 sev-snp-measure-0.0.3/sevsnpmeasure/gctx.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     2831 2022-05-17 08:48:05.000000 sev-snp-measure-0.0.3/sevsnpmeasure/guest.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3966 2022-04-04 18:59:40.000000 sev-snp-measure-0.0.3/sevsnpmeasure/ovmf.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     2508 2022-05-10 07:32:24.000000 sev-snp-measure-0.0.3/sevsnpmeasure/sev_hashes.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2022-04-24 09:17:37.000000 sev-snp-measure-0.0.3/sevsnpmeasure/sev_mode.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     1310 2022-05-17 08:48:18.000000 sev-snp-measure-0.0.3/sevsnpmeasure/vcpu_types.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5684 2022-05-17 08:30:05.000000 sev-snp-measure-0.0.3/sevsnpmeasure/vmsa.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.4/LICENSE
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6713 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5968 2023-04-13 06:53:56.000000 sev-snp-measure-0.0.4/README.md
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2022-04-11 09:47:58.000000 sev-snp-measure-0.0.4/pyproject.toml
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      973 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/setup.cfg
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6713 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      590 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/SOURCES.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/dependency_links.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      109 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/entry_points.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       40 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/requires.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2023-04-13 07:30:54.000000 sev-snp-measure-0.0.4/sev_snp_measure.egg-info/top_level.txt
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/sevsnpmeasure/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.4/sevsnpmeasure/__init__.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3616 2023-04-13 07:27:01.000000 sev-snp-measure-0.0.4/sevsnpmeasure/cli.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     2462 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.4/sevsnpmeasure/gctx.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3626 2023-04-10 12:19:02.000000 sev-snp-measure-0.0.4/sevsnpmeasure/guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5591 2023-04-10 12:20:41.000000 sev-snp-measure-0.0.4/sevsnpmeasure/id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     4736 2023-04-10 12:19:02.000000 sev-snp-measure-0.0.4/sevsnpmeasure/ovmf.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3488 2022-06-08 14:31:05.000000 sev-snp-measure-0.0.4/sevsnpmeasure/sev_hashes.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2022-04-24 09:17:37.000000 sev-snp-measure-0.0.4/sevsnpmeasure/sev_mode.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1609 2023-03-07 15:16:17.000000 sev-snp-measure-0.0.4/sevsnpmeasure/vcpu_types.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5727 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.4/sevsnpmeasure/vmsa.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 07:30:54.317440 sev-snp-measure-0.0.4/tests/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3130 2023-04-10 12:19:02.000000 sev-snp-measure-0.0.4/tests/test_guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1149 2023-04-10 12:20:41.000000 sev-snp-measure-0.0.4/tests/test_id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      480 2022-06-08 12:42:41.000000 sev-snp-measure-0.0.4/tests/test_vcpu_types.py
```

### Comparing `sev-snp-measure-0.0.3/LICENSE` & `sev-snp-measure-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.3/PKG-INFO` & `sev-snp-measure-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.3
+Version: 0.0.4
 Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 Home-page: https://github.com/IBM/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik1@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -41,28 +41,30 @@
 
     git clone https://github.com/IBM/sev-snp-measure.git
     cd sev-snp-measure
     ./sev-snp-measure.py --help
 
 ## Command-line usage
 
+### sev-snp-measure
 ```
 $ sev-snp-measure --help
-usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp} [--vcpus N]
+usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash} [--vcpus N]
                        [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
                        [--vcpu-model MODEL] [--vcpu-stepping STEPPING] --ovmf PATH [--kernel PATH]
                        [--initrd PATH] [--append CMDLINE] [--output-format {hex,base64}]
+                       [--snp-ovmf-hash HASH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 optional arguments:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
-  --mode {sev,seves,snp}
+  --mode {sev,seves,snp,snp:ovmf-hash}
                         Guest mode
   --vcpus N             Number of guest vcpus
   --vcpu-type CPUTYPE   Type of guest vcpu (EPYC, EPYC-v1, EPYC-v2, EPYC-IBPB, EPYC-v3, EPYC-v4,
                         EPYC-Rome, EPYC-Rome-v1, EPYC-Rome-v2, EPYC-Rome-v3, EPYC-Milan, EPYC-
                         Milan-v1, EPYC-Milan-v2)
   --vcpu-sig VALUE      Guest vcpu signature value
   --vcpu-family FAMILY  Guest vcpu family
@@ -71,34 +73,52 @@
                         Guest vcpu stepping
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
   --output-format {hex,base64}
                         Measurement output format
+  --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
 ```
 
 For example:
 
     $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
     1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
 
+### snp-create-id-block
+```
+$ snp-create-id-block --help
+usage: snp-create-id-block [-h] [--measurement VALUE] [--idkey PATH] [--authorkey PATH]
+
+Calculate AMD SEV-SNP guest id block
+
+optional arguments:
+  -h, --help           show this help message and exit
+  --measurement VALUE  Guest launch measurement in Base64 encoding
+  --idkey PATH         id private key file
+  --authorkey PATH     author private key file
+```
+
 ## Programmatic usage
 
 After installing the `sev-snp-measure` package with pip, you can call it from
 another Python application:
 
 ```python3
-from sevsnpmeasure import guest
+from sevsnpmeasure import guest,id_block
 from sevsnpmeasure import vcpu_types
 from sevsnpmeasure.sev_mode import SevMode
 
 ld = guest.calc_launch_digest(SevMode.SEV_SNP, vcpus_num, vcpu_types.CPU_SIGS["EPYC-v4"],
                               ovmf_path, kernel_path, initrd_path, cmdline_str)
 print("Calculated measurement:", ld.hex())
+
+block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
+print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
 
 For SEV-ES and SEV-SNP, the initial CPU state (VMSA) includes the guest CPU
 signature in the edx register.  Therefore, starting the VM with a different
 type of guest CPU will modify the content of the VMSA, and therefore modify the
@@ -108,19 +128,40 @@
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
 3. `sev-snp-measure --vcpu-family=23 --vcpu-model=1 --vcpu-stepping=2 ...`
 
+## Precalculated OVMF hashes
+
+The SEV-SNP digest gets generated in multiple steps that each have a digest as output. With that digest output, you can stop at any of these steps and continue generation of the full digest later. These are the steps:
+
+1. OVMF
+2. (optional) -kernel, -initrd, -append arguments
+3. Initial state of all vCPUs
+
+In situations where only minor OVMF changes happen, you may not want to copy the full OVMF binary to the validation system. In these situations, you can cut digest calculation after the `OVMF` step and use its hash instead of the full binary.
+
+To generate a hash, use the `--mode snp:ovmf-hash` parameter:
+
+    $ sev-snp-measure --mode snp:ovmf-hash --ovmf OVMF.fd
+    cab7e085874b3acfdbe2d96dcaa3125111f00c35c6fc9708464c2ae74bfdb048a198cb9a9ccae0b3e5e1a33f5f249819
+
+On a different machine that only has access to an older but compatible OVMF binary, you can then ingest the hash again to generate a full measurement:
+
+    $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd.old --ovmf-hash cab7e[...]
+    d52697c3e056fb8d698d19cc29adfbed5a8ec9170cb9eb63c2ac957d22b4eb647e25780162036d063a0cf418b8830acc
+
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
 * [sev Rust crate](https://github.com/virtee/sev)
+* [snp-digest-rs](https://github.com/slp/snp-digest-rs)
 * [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
```

### Comparing `sev-snp-measure-0.0.3/setup.cfg` & `sev-snp-measure-0.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sev-snp-measure
-version = 0.0.3
+version = 0.0.4
 author = Dov Murik
 author_email = dov.murik1@il.ibm.com
 description = Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/sev-snp-measure
 project_urls = 
@@ -17,15 +17,20 @@
 	Operating System :: OS Independent
 	Topic :: Security
 	Topic :: Software Development :: Libraries
 
 [options]
 packages = sevsnpmeasure
 python_requires = >=3.7
+install_requires = 
+	cryptography>=39.0.1
+	types-cryptography
 
 [options.entry_points]
-console_scripts = sev-snp-measure = sevsnpmeasure.cli:main
+console_scripts = 
+	sev-snp-measure = sevsnpmeasure.cli:main
+	snp-create-id-block = sevsnpmeasure.id_block:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sev-snp-measure-0.0.3/sev_snp_measure.egg-info/PKG-INFO` & `sev-snp-measure-0.0.4/sev_snp_measure.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.3
+Version: 0.0.4
 Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 Home-page: https://github.com/IBM/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik1@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -41,28 +41,30 @@
 
     git clone https://github.com/IBM/sev-snp-measure.git
     cd sev-snp-measure
     ./sev-snp-measure.py --help
 
 ## Command-line usage
 
+### sev-snp-measure
 ```
 $ sev-snp-measure --help
-usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp} [--vcpus N]
+usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash} [--vcpus N]
                        [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
                        [--vcpu-model MODEL] [--vcpu-stepping STEPPING] --ovmf PATH [--kernel PATH]
                        [--initrd PATH] [--append CMDLINE] [--output-format {hex,base64}]
+                       [--snp-ovmf-hash HASH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 optional arguments:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
-  --mode {sev,seves,snp}
+  --mode {sev,seves,snp,snp:ovmf-hash}
                         Guest mode
   --vcpus N             Number of guest vcpus
   --vcpu-type CPUTYPE   Type of guest vcpu (EPYC, EPYC-v1, EPYC-v2, EPYC-IBPB, EPYC-v3, EPYC-v4,
                         EPYC-Rome, EPYC-Rome-v1, EPYC-Rome-v2, EPYC-Rome-v3, EPYC-Milan, EPYC-
                         Milan-v1, EPYC-Milan-v2)
   --vcpu-sig VALUE      Guest vcpu signature value
   --vcpu-family FAMILY  Guest vcpu family
@@ -71,34 +73,52 @@
                         Guest vcpu stepping
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
   --output-format {hex,base64}
                         Measurement output format
+  --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
 ```
 
 For example:
 
     $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
     1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
 
+### snp-create-id-block
+```
+$ snp-create-id-block --help
+usage: snp-create-id-block [-h] [--measurement VALUE] [--idkey PATH] [--authorkey PATH]
+
+Calculate AMD SEV-SNP guest id block
+
+optional arguments:
+  -h, --help           show this help message and exit
+  --measurement VALUE  Guest launch measurement in Base64 encoding
+  --idkey PATH         id private key file
+  --authorkey PATH     author private key file
+```
+
 ## Programmatic usage
 
 After installing the `sev-snp-measure` package with pip, you can call it from
 another Python application:
 
 ```python3
-from sevsnpmeasure import guest
+from sevsnpmeasure import guest,id_block
 from sevsnpmeasure import vcpu_types
 from sevsnpmeasure.sev_mode import SevMode
 
 ld = guest.calc_launch_digest(SevMode.SEV_SNP, vcpus_num, vcpu_types.CPU_SIGS["EPYC-v4"],
                               ovmf_path, kernel_path, initrd_path, cmdline_str)
 print("Calculated measurement:", ld.hex())
+
+block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
+print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
 
 For SEV-ES and SEV-SNP, the initial CPU state (VMSA) includes the guest CPU
 signature in the edx register.  Therefore, starting the VM with a different
 type of guest CPU will modify the content of the VMSA, and therefore modify the
@@ -108,19 +128,40 @@
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
 3. `sev-snp-measure --vcpu-family=23 --vcpu-model=1 --vcpu-stepping=2 ...`
 
+## Precalculated OVMF hashes
+
+The SEV-SNP digest gets generated in multiple steps that each have a digest as output. With that digest output, you can stop at any of these steps and continue generation of the full digest later. These are the steps:
+
+1. OVMF
+2. (optional) -kernel, -initrd, -append arguments
+3. Initial state of all vCPUs
+
+In situations where only minor OVMF changes happen, you may not want to copy the full OVMF binary to the validation system. In these situations, you can cut digest calculation after the `OVMF` step and use its hash instead of the full binary.
+
+To generate a hash, use the `--mode snp:ovmf-hash` parameter:
+
+    $ sev-snp-measure --mode snp:ovmf-hash --ovmf OVMF.fd
+    cab7e085874b3acfdbe2d96dcaa3125111f00c35c6fc9708464c2ae74bfdb048a198cb9a9ccae0b3e5e1a33f5f249819
+
+On a different machine that only has access to an older but compatible OVMF binary, you can then ingest the hash again to generate a full measurement:
+
+    $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd.old --ovmf-hash cab7e[...]
+    d52697c3e056fb8d698d19cc29adfbed5a8ec9170cb9eb63c2ac957d22b4eb647e25780162036d063a0cf418b8830acc
+
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
 * [sev Rust crate](https://github.com/virtee/sev)
+* [snp-digest-rs](https://github.com/slp/snp-digest-rs)
 * [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
```

### Comparing `sev-snp-measure-0.0.3/sevsnpmeasure/cli.py` & `sev-snp-measure-0.0.4/sevsnpmeasure/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 import base64
 import sys
 
 from sevsnpmeasure import guest
 from sevsnpmeasure import vcpu_types
 from .sev_mode import SevMode
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 
 def auto_base_int(s: str) -> int:
     return int(s, 0)
 
 
 def main() -> int:
     parser = argparse.ArgumentParser(prog='sev-snp-measure',
                                      description='Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement')
     parser.add_argument('--version', action='version', version=f'%(prog)s {VERSION}')
     parser.add_argument('-v', '--verbose', action='store_true')
-    parser.add_argument('--mode', choices=['sev', 'seves', 'snp'], help='Guest mode', required=True)
+    parser.add_argument('--mode', choices=['sev', 'seves', 'snp', 'snp:ovmf-hash'], help='Guest mode', required=True)
     parser.add_argument('--vcpus', metavar='N', type=int, help='Number of guest vcpus', default=None)
     parser.add_argument('--vcpu-type', metavar='CPUTYPE', choices=list(vcpu_types.CPU_SIGS.keys()),
                         help=f"Type of guest vcpu ({', '.join(vcpu_types.CPU_SIGS.keys())})",
                         default=None)
     parser.add_argument('--vcpu-sig', metavar='VALUE', type=auto_base_int, help='Guest vcpu signature value', default=None)
     parser.add_argument('--vcpu-family', metavar='FAMILY', type=int, help='Guest vcpu family', default=None)
     parser.add_argument('--vcpu-model', metavar='MODEL', type=int, help='Guest vcpu model', default=None)
@@ -37,16 +37,21 @@
     parser.add_argument('--kernel', metavar='PATH',
                         help='Kernel file to calculate hash from')
     parser.add_argument('--initrd', metavar='PATH',
                         help='Initrd file to calculate hash from (use with --kernel)')
     parser.add_argument('--append', metavar='CMDLINE',
                         help='Kernel command line to calculate hash from (use with --kernel)')
     parser.add_argument('--output-format', choices=['hex', 'base64'], help='Measurement output format', default='hex')
+    parser.add_argument('--snp-ovmf-hash', metavar='HASH', help='Precalculated hash of the OVMF binary (hex string)')
     args = parser.parse_args()
 
+    if args.mode == 'snp:ovmf-hash':
+        print(guest.calc_snp_ovmf_hash(args.ovmf).hex())
+        return 0
+
     if args.mode != 'sev' and args.vcpus is None:
         parser.error(f"missing --vcpus N in guest mode '{args.mode}'")
 
     vcpu_sig = 0
     if args.mode != 'sev':
         if args.vcpu_family:
             vcpu_sig = vcpu_types.cpu_sig(args.vcpu_family, args.vcpu_model, args.vcpu_stepping)
@@ -54,15 +59,16 @@
             vcpu_sig = args.vcpu_sig
         elif args.vcpu_type:
             vcpu_sig = vcpu_types.CPU_SIGS[args.vcpu_type]
         else:
             parser.error(f"missing --vcpu-type or --vcpu-sig or --vcpu-family in guest mode '{args.mode}'")
 
     sev_mode = SevMode.from_str(args.mode)
-    ld = guest.calc_launch_digest(sev_mode, args.vcpus, vcpu_sig, args.ovmf, args.kernel, args.initrd, args.append)
+    ld = guest.calc_launch_digest(sev_mode, args.vcpus, vcpu_sig, args.ovmf,
+                                  args.kernel, args.initrd, args.append, args.snp_ovmf_hash)
 
     if args.output_format == "hex":
         measurement = ld.hex()
     elif args.output_format == "base64":
         measurement = base64.b64encode(ld).decode()
 
     if args.verbose:
```

### Comparing `sev-snp-measure-0.0.3/sevsnpmeasure/gctx.py` & `sev-snp-measure-0.0.4/sevsnpmeasure/gctx.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     """
 
     # VMSA page is recorded in the RMP table with GPA (u64)(-1).
     # However, the address is page-aligned, and also all the bits above
     # 51 are cleared.
     VMSA_GPA = 0xFFFFFFFFF000
 
-    def __init__(self):
-        self._ld = ZEROS
+    def __init__(self, seed: bytes = ZEROS):
+        self._ld = seed
 
     def ld(self) -> bytes:
         return self._ld
 
     def hex_ld(self) -> str:
         return self._ld.hex()
```

### Comparing `sev-snp-measure-0.0.3/sevsnpmeasure/guest.py` & `sev-snp-measure-0.0.4/sevsnpmeasure/guest.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,49 +2,70 @@
 # Copyright 2022- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import hashlib
 
 from .gctx import GCTX
-from .ovmf import OVMF
+from .ovmf import OVMF, SectionType
 from .sev_hashes import SevHashes
 from .vmsa import VMSA
 from .sev_mode import SevMode
 
 PAGE_MASK = 0xfff
 
 
 def calc_launch_digest(mode: SevMode, vcpus: int, vcpu_sig: int, ovmf_file: str,
-                       kernel: str, initrd: str, append: str) -> bytes:
+                       kernel: str, initrd: str, append: str, snp_ovmf_hash_str: str = '') -> bytes:
+    if snp_ovmf_hash_str and mode != SevMode.SEV_SNP:
+        raise ValueError("SNP OVMF hash only works with SNP")
+
     if mode == SevMode.SEV_SNP:
-        return snp_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append)
+        return snp_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append, snp_ovmf_hash_str)
     elif mode == SevMode.SEV_ES:
         return seves_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append)
     elif mode == SevMode.SEV:
         return sev_calc_launch_digest(ovmf_file, kernel, initrd, append)
     else:
         raise ValueError("unknown mode")
 
 
 def snp_update_metadata_pages(gctx, ovmf) -> None:
     for desc in ovmf.metadata_items():
-        if desc.page_type == 1:
+        if desc.section_type() == SectionType.SNP_SEC_MEM:
             gctx.update_zero_pages(desc.gpa, desc.size)
-        elif desc.page_type == 2:
+        elif desc.section_type() == SectionType.SNP_SECRETS:
             gctx.update_secrets_page(desc.gpa)
-        elif desc.page_type == 3:
+        elif desc.section_type() == SectionType.CPUID:
             gctx.update_cpuid_page(desc.gpa)
+        else:
+            raise ValueError("unknown OVMF metadata section type")
 
 
-def snp_calc_launch_digest(vcpus: int, vcpu_sig: int, ovmf_file: str, kernel: str, initrd: str, append: str) -> bytes:
+def calc_snp_ovmf_hash(ovmf_file: str) -> bytes:
     ovmf = OVMF(ovmf_file)
 
     gctx = GCTX()
     gctx.update_normal_pages(ovmf.gpa(), ovmf.data())
+    return gctx.ld()
+
+
+def snp_calc_launch_digest(vcpus: int, vcpu_sig: int, ovmf_file: str,
+                           kernel: str, initrd: str, append: str, ovmf_hash_str: str) -> bytes:
+
+    gctx = GCTX()
+    ovmf = OVMF(ovmf_file)
+
+    # Allow users to provide a precalculated OVMF hash.
+    # Ignores the contents of the OVMF file in front of us.
+    if ovmf_hash_str:
+        ovmf_hash = bytearray.fromhex(ovmf_hash_str)
+        gctx = GCTX(seed=ovmf_hash)
+    else:
+        gctx.update_normal_pages(ovmf.gpa(), ovmf.data())
 
     if kernel:
         sev_hashes_table_gpa = ovmf.sev_hashes_table_gpa()
         offset_in_page = sev_hashes_table_gpa & PAGE_MASK
         sev_hashes_page_gpa = sev_hashes_table_gpa & ~PAGE_MASK
         sev_hashes = SevHashes(kernel, initrd, append)
         sev_hashes_page = sev_hashes.construct_page(offset_in_page)
```

### Comparing `sev-snp-measure-0.0.3/sevsnpmeasure/sev_mode.py` & `sev-snp-measure-0.0.4/sevsnpmeasure/sev_mode.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.3/sevsnpmeasure/vcpu_types.py` & `sev-snp-measure-0.0.4/sevsnpmeasure/vcpu_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 def cpu_sig(family: int, model: int, stepping: int) -> int:
+    """Compute the 32-bit CPUID signature from family, model, and stepping.
+
+    This computation is described in AMD's CPUID Specification, publication #25481
+    https://www.amd.com/system/files/TechDocs/25481.pdf
+    See section: CPUID Fn0000_0001_EAX Family, Model, Stepping Identifiers
+    """
     if family > 0xf:
         family_low = 0xf
         family_high = (family - 0x0f) & 0xff
     else:
         family_low = family
         family_high = 0
```

### Comparing `sev-snp-measure-0.0.3/sevsnpmeasure/vmsa.py` & `sev-snp-measure-0.0.4/sevsnpmeasure/vmsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             efer=0x1000,  # KVM enables EFER_SVME
             cr4=0x40,     # KVM enables X86_CR4_MCE
             cr0=0x10,
             dr7=0x400,
             dr6=0xffff0ff0,
             rflags=0x2,
             rip=eip & 0xffff,
-            g_pat=0x7040600070406,
+            g_pat=0x7040600070406,  # PAT MSR: See AMD APM Vol 2, Section A.3
             rdx=vcpu_sig,
             sev_features=sev_features,
             xcr0=0x1,
         )
 
     def __init__(self, sev_mode: SevMode, ap_eip: int, vcpu_sig: int):
         if sev_mode == SevMode.SEV_SNP:
```

