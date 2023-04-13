# Comparing `tmp/snapper-ont-0.4.4.tar.gz` & `tmp/snapper-ont-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snapper-ont-0.4.4.tar", last modified: Fri Apr  7 06:34:08 2023, max compression
+gzip compressed data, was "dist/snapper-ont-0.4.5.tar", last modified: Thu Apr 13 14:46:28 2023, max compression
```

## Comparing `snapper-ont-0.4.4.tar` & `snapper-ont-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)     1074 2023-02-27 11:26:28.000000 snapper-ont-0.4.4/LICENSE
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)      475 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/PKG-INFO
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)     2922 2023-02-27 11:28:05.000000 snapper-ont-0.4.4/README.md
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)       38 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/setup.cfg
--rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     1064 2023-04-07 06:33:31.000000 snapper-ont-0.4.4/setup.py
-drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper/
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)     7813 2023-04-03 14:46:52.000000 snapper-ont-0.4.4/snapper/snapper.py
-drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper/src/
--rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     6983 2023-03-30 14:19:03.000000 snapper-ont-0.4.4/snapper/src/data_processing.py
--rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)    15983 2023-03-30 14:18:56.000000 snapper-ont-0.4.4/snapper/src/methods.py
--rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     5804 2023-04-03 14:56:18.000000 snapper-ont-0.4.4/snapper/src/motif_extraction.py
--rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     5460 2023-04-07 06:33:13.000000 snapper-ont-0.4.4/snapper/src/plotting.py
--rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     1465 2023-02-27 11:26:28.000000 snapper-ont-0.4.4/snapper/src/seq_processing.py
--rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     3120 2023-03-30 14:17:30.000000 snapper-ont-0.4.4/snapper/src/statistics_methods.py
--rwx------   0 konanov_dn  (1002) konanov_dn  (1002)     8829 2023-03-30 11:35:53.000000 snapper-ont-0.4.4/snapper/src/type_I_RM_system.py
-drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper_ont.egg-info/
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)      475 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper_ont.egg-info/PKG-INFO
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)      463 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper_ont.egg-info/SOURCES.txt
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)        1 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper_ont.egg-info/dependency_links.txt
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)       49 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper_ont.egg-info/entry_points.txt
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)       45 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper_ont.egg-info/requires.txt
--rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)        8 2023-04-07 06:34:08.000000 snapper-ont-0.4.4/snapper_ont.egg-info/top_level.txt
+drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)     1074 2023-02-27 11:26:28.000000 snapper-ont-0.4.5/LICENSE
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)      475 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/PKG-INFO
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)     3487 2023-04-13 14:45:02.000000 snapper-ont-0.4.5/README.md
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)       38 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/setup.cfg
+-rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     1064 2023-04-13 14:39:37.000000 snapper-ont-0.4.5/setup.py
+drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper/
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)     8205 2023-04-13 14:32:21.000000 snapper-ont-0.4.5/snapper/snapper.py
+drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper/src/
+-rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     6983 2023-03-30 14:19:03.000000 snapper-ont-0.4.5/snapper/src/data_processing.py
+-rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)    15983 2023-03-30 14:18:56.000000 snapper-ont-0.4.5/snapper/src/methods.py
+-rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     5804 2023-04-03 14:56:18.000000 snapper-ont-0.4.5/snapper/src/motif_extraction.py
+-rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     5460 2023-04-07 06:33:13.000000 snapper-ont-0.4.5/snapper/src/plotting.py
+-rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     1465 2023-02-27 11:26:28.000000 snapper-ont-0.4.5/snapper/src/seq_processing.py
+-rwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)     3120 2023-03-30 14:17:30.000000 snapper-ont-0.4.5/snapper/src/statistics_methods.py
+-rwx------   0 konanov_dn  (1002) konanov_dn  (1002)     8829 2023-03-30 11:35:53.000000 snapper-ont-0.4.5/snapper/src/type_I_RM_system.py
+drwxrwxr-x   0 konanov_dn  (1002) konanov_dn  (1002)        0 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper_ont.egg-info/
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)      475 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper_ont.egg-info/PKG-INFO
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)      463 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper_ont.egg-info/SOURCES.txt
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)        1 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper_ont.egg-info/dependency_links.txt
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)       49 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper_ont.egg-info/entry_points.txt
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)       45 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper_ont.egg-info/requires.txt
+-rw-rw-r--   0 konanov_dn  (1002) konanov_dn  (1002)        8 2023-04-13 14:46:28.000000 snapper-ont-0.4.5/snapper_ont.egg-info/top_level.txt
```

### Comparing `snapper-ont-0.4.4/LICENSE` & `snapper-ont-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snapper-ont-0.4.4/README.md` & `snapper-ont-0.4.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -29,31 +29,44 @@
 
 Firstly, fast5 files should be resquiggled using [Tombo](https://github.com/nanoporetech/tombo) software. 
 After resquiggling, fast5 files should be converted to the multi-fast5 format using [ont_fast5_api](https://github.com/nanoporetech/ont_fast5_api).
 
 A more detailed usage guideline and few usercases are available in [Snapper's documentation](https://snapper-tutorial.readthedocs.io/en/latest/index.html)
 
 ```
-usage: snapper [-h] [-sample_fast5dir SAMPLE_FAST5DIR] [-control_fast5dir CONTROL_FAST5DIR] [-reference REFERENCE] [-ks_t KS_T]
-               [-outdir OUTDIR] [-n_batches N_BATCHES] [-threads THREADS] [-max_motifs MAX_MOTIFS] [-min_conf MIN_CONF]
+usage: snapper [-h] -sample_fast5dir SAMPLE_FAST5DIR -control_fast5dir
+               CONTROL_FAST5DIR -reference REFERENCE [-ks_t KS_T]
+               [-outdir OUTDIR] [-coverage COVERAGE] [-threads THREADS]
+               [-k_size K_SIZE] [-long_k_size LONG_K_SIZE]
+               [-max_motifs MAX_MOTIFS] [-min_conf MIN_CONF]
+               [-target_chr TARGET_CHR]
 
 optional arguments:
   -h, --help            show this help message and exit
   -sample_fast5dir SAMPLE_FAST5DIR
                         sample multi fast5 dir
   -control_fast5dir CONTROL_FAST5DIR
-                        control multi fast54 dir
-  -reference REFERENCE  reference fasta
-  -ks_t KS_T            -log ks_test p-value (default 5)
+                        control multi fast5 dir
+  -reference REFERENCE  reference genome in the fasta format
+  -ks_t KS_T            -log ks_test p-value (default 3).
   -outdir OUTDIR        output directory name
-  -n_batches N_BATCHES  number of parsed fast5 batches
-  -threads THREADS      number of threads used (derfault is 8)
+  -coverage COVERAGE    minimal genome coverage depth (default 40)
+  -threads THREADS      number of threads used (default 8)
+  -k_size K_SIZE        k-mer size, must be odd, 
+                        should not be less than 11 (default 15)
+  -long_k_size LONG_K_SIZE
+                        k-mer size, must be odd, 
+                        should not be less than 21 (default 29)
   -max_motifs MAX_MOTIFS
                         the maximum expected number of motifs extracted
-  -min_conf MIN_CONF    the minimal confidence value. Default is 1000
+  -min_conf MIN_CONF    the minimal confidence value (default is 100)
+  -target_chr TARGET_CHR
+                        target chromosome name (by default all
+                        contigs/replicons are considered)
+
 
 ```
 
 
 Typical run command:
 ```
 snapper -sample_fast5dir ../HelicobacterMod/fast5/J99_multi/ -control_fast5dir ../HelicobacterMod/fast5/J99_wga_multi/ -reference ../HelicobacterMod/genome/J99.fasta -n_batches 5
```

### Comparing `snapper-ont-0.4.4/setup.py` & `snapper-ont-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="snapper-ont",
-    version="0.4.4",
+    version="0.4.5",
     author="D.N. Konanov",
     author_email="konanovdmitriy@gmail.com",
     description="Nanopore-based methylation sites caller",
     long_description="snapper",
     long_description_content_type="",
     url="https://github.com/DNKonanov/Snapper",
     project_urls={
```

### Comparing `snapper-ont-0.4.4/snapper/snapper.py` & `snapper-ont-0.4.5/snapper/snapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 
 def main():
 
     parser = ArgumentParser()
 
     parser.add_argument('-sample_fast5dir', type=str, help='sample multi fast5 dir', required=True)
-    parser.add_argument('-control_fast5dir', type=str, help='control multi fast54 dir', required=True)
+    parser.add_argument('-control_fast5dir', type=str, help='control multi fast5 dir', required=True)
     parser.add_argument('-reference', type=str, help='reference genome in the fasta format', required=True)
     parser.add_argument('-ks_t', type=int, default=3, help='-log ks_test p-value (default 3).')
     parser.add_argument('-outdir', type=str, default='default', help='output directory name')
     parser.add_argument('-coverage', type=float, help='minimal genome coverage depth (default 40)', default=40)
     parser.add_argument('-threads', type=int, default=8, help='number of threads used (default 8)')
-    parser.add_argument('-k_size', type=int, default=15, help='k-mer size, must be odd (default 15)')
-    parser.add_argument('-long_k_size', type=int, default=29, help='k-mer size, must be odd (default 29)')
+    parser.add_argument('-k_size', type=int, default=15, help='k-mer size, must be odd, should not be less than 11 (default 15)')
+    parser.add_argument('-long_k_size', type=int, default=29, help='k-mer size, must be odd, should not be less than 21 (default 29)')
     parser.add_argument('-max_motifs', help='the maximum expected number of motifs extracted', default=20, type=int)
     parser.add_argument('-min_conf', help='the minimal confidence value (default is 100)', type=float, default=100)
     parser.add_argument('-target_chr', help='target chromosome name (by default all contigs/replicons are considered)', type=str, default='all')
     
 
 
     from snapper.src.motif_extraction import extract_motifs
@@ -34,18 +34,32 @@
     from snapper.src.methods import save_results, save_k_mers
     from snapper.src.statistics_methods import SAMPLESIZE, MINSAMPLESIZE
 
     if len(sys.argv)==1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
+
+    
+
     args = parser.parse_args()
 
     if args.k_size%2 == 0 or args.long_k_size%2 == 0:
         raise ValueError('Both -k_size and -long_k_size must be odd numbers')
+    
+    if args.k_size < 11:
+        raise ValueError('-k_size parameter should not be less than 11')
+
+    if args.long_k_size < 21:
+        raise ValueError('-long_k_size parameter should not be less than 21')
+    
+    if args.k_size >= args.long_k_size:
+        raise ValueError('K_SIZE should be less than LONG_K_SIZE')
+    
+
 
 
     if args.outdir == 'default':
         import datetime
         
         sp = str(datetime.datetime.now()
             ).replace(' ', '_').replace(':', '').replace('-', '_').split('.')[0]
```

### Comparing `snapper-ont-0.4.4/snapper/src/data_processing.py` & `snapper-ont-0.4.5/snapper/src/data_processing.py`

 * *Files identical despite different names*

### Comparing `snapper-ont-0.4.4/snapper/src/methods.py` & `snapper-ont-0.4.5/snapper/src/methods.py`

 * *Files identical despite different names*

### Comparing `snapper-ont-0.4.4/snapper/src/motif_extraction.py` & `snapper-ont-0.4.5/snapper/src/motif_extraction.py`

 * *Files identical despite different names*

### Comparing `snapper-ont-0.4.4/snapper/src/plotting.py` & `snapper-ont-0.4.5/snapper/src/plotting.py`

 * *Files identical despite different names*

### Comparing `snapper-ont-0.4.4/snapper/src/seq_processing.py` & `snapper-ont-0.4.5/snapper/src/seq_processing.py`

 * *Files identical despite different names*

### Comparing `snapper-ont-0.4.4/snapper/src/statistics_methods.py` & `snapper-ont-0.4.5/snapper/src/statistics_methods.py`

 * *Files identical despite different names*

### Comparing `snapper-ont-0.4.4/snapper/src/type_I_RM_system.py` & `snapper-ont-0.4.5/snapper/src/type_I_RM_system.py`

 * *Files identical despite different names*

