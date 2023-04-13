# Comparing `tmp/MarkerMAG-1.1.8.tar.gz` & `tmp/MarkerMAG-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarkerMAG-1.1.8.tar", last modified: Wed Feb  9 05:23:51 2022, max compression
+gzip compressed data, was "MarkerMAG-1.1.9.tar", last modified: Wed Feb  9 05:29:58 2022, max compression
```

## Comparing `MarkerMAG-1.1.8.tar` & `MarkerMAG-1.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:23:51.585583 MarkerMAG-1.1.8/
--rw-r--r--   0 songweizhi   (501) staff       (20)    32387 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/LICENSE.txt
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      162 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MANIFEST.in
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:23:51.584384 MarkerMAG-1.1.8/MarkerMAG/
--rw-r--r--   0 songweizhi   (501) staff       (20)      542 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/MarkerMAG_config.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  1859687 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/SILVA_16S_order.fasta
--rw-r--r--   0 songweizhi   (501) staff       (20)      159 2022-02-09 05:23:51.000000 MarkerMAG-1.1.8/MarkerMAG/VERSION
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7729 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/barrnap_16s.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5073 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/filter_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4122 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/gc_bias.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1502 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/get_16s_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)   135055 2022-02-09 05:23:51.000000 MarkerMAG-1.1.8/MarkerMAG/get_cp_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    16245 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/get_mag_depth.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)   276538 2021-11-24 12:38:09.000000 MarkerMAG-1.1.8/MarkerMAG/link_16s.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    21030 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/matam_16s.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2462 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/polish_16s.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7599 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/recovery_16s.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     4184 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/rename_reads.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2985 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/subsample_reads.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4950 2021-11-13 21:38:33.000000 MarkerMAG-1.1.8/MarkerMAG/uclust_16s.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:23:51.584912 MarkerMAG-1.1.8/MarkerMAG.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      510 2022-02-09 05:23:51.000000 MarkerMAG-1.1.8/MarkerMAG.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)      644 2022-02-09 05:23:51.000000 MarkerMAG-1.1.8/MarkerMAG.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2022-02-09 05:23:51.000000 MarkerMAG-1.1.8/MarkerMAG.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       49 2022-02-09 05:23:51.000000 MarkerMAG-1.1.8/MarkerMAG.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       10 2022-02-09 05:23:51.000000 MarkerMAG-1.1.8/MarkerMAG.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)      510 2022-02-09 05:23:51.585448 MarkerMAG-1.1.8/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     5803 2021-11-19 23:39:08.000000 MarkerMAG-1.1.8/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:23:51.584998 MarkerMAG-1.1.8/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    22410 2022-02-09 04:05:08.000000 MarkerMAG-1.1.8/bin/MarkerMAG
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2022-02-09 05:23:51.585627 MarkerMAG-1.1.8/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2021-11-18 03:22:15.000000 MarkerMAG-1.1.8/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:29:58.002015 MarkerMAG-1.1.9/
+-rw-r--r--   0 songweizhi   (501) staff       (20)    32387 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/LICENSE.txt
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      162 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MANIFEST.in
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:29:58.001150 MarkerMAG-1.1.9/MarkerMAG/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      542 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/MarkerMAG_config.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  1859687 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/SILVA_16S_order.fasta
+-rw-r--r--   0 songweizhi   (501) staff       (20)      159 2022-02-09 05:29:57.000000 MarkerMAG-1.1.9/MarkerMAG/VERSION
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7729 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/barrnap_16s.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5073 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/filter_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4122 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/gc_bias.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1502 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/get_16s_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)   135055 2022-02-09 05:23:51.000000 MarkerMAG-1.1.9/MarkerMAG/get_cp_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16245 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/get_mag_depth.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)   276538 2021-11-24 12:38:09.000000 MarkerMAG-1.1.9/MarkerMAG/link_16s.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    21030 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/matam_16s.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2462 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/polish_16s.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7599 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/recovery_16s.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     4184 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/rename_reads.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2985 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/subsample_reads.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4950 2021-11-13 21:38:33.000000 MarkerMAG-1.1.9/MarkerMAG/uclust_16s.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:29:58.001649 MarkerMAG-1.1.9/MarkerMAG.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      510 2022-02-09 05:29:57.000000 MarkerMAG-1.1.9/MarkerMAG.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)      644 2022-02-09 05:29:57.000000 MarkerMAG-1.1.9/MarkerMAG.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2022-02-09 05:29:57.000000 MarkerMAG-1.1.9/MarkerMAG.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       49 2022-02-09 05:29:57.000000 MarkerMAG-1.1.9/MarkerMAG.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       10 2022-02-09 05:29:57.000000 MarkerMAG-1.1.9/MarkerMAG.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)      510 2022-02-09 05:29:58.001894 MarkerMAG-1.1.9/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5803 2021-11-19 23:39:08.000000 MarkerMAG-1.1.9/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2022-02-09 05:29:58.001738 MarkerMAG-1.1.9/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    22498 2022-02-09 05:29:35.000000 MarkerMAG-1.1.9/bin/MarkerMAG
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2022-02-09 05:29:58.002054 MarkerMAG-1.1.9/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2021-11-18 03:22:15.000000 MarkerMAG-1.1.9/setup.py
```

### Comparing `MarkerMAG-1.1.8/LICENSE.txt` & `MarkerMAG-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/MarkerMAG_config.py` & `MarkerMAG-1.1.9/MarkerMAG/MarkerMAG_config.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/SILVA_16S_order.fasta` & `MarkerMAG-1.1.9/MarkerMAG/SILVA_16S_order.fasta`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/barrnap_16s.py` & `MarkerMAG-1.1.9/MarkerMAG/barrnap_16s.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/filter_sam.py` & `MarkerMAG-1.1.9/MarkerMAG/filter_sam.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/gc_bias.py` & `MarkerMAG-1.1.9/MarkerMAG/gc_bias.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/get_16s_depth.py` & `MarkerMAG-1.1.9/MarkerMAG/get_16s_depth.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/get_cp_num.py` & `MarkerMAG-1.1.9/MarkerMAG/get_cp_num.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/get_mag_depth.py` & `MarkerMAG-1.1.9/MarkerMAG/get_mag_depth.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/link_16s.py` & `MarkerMAG-1.1.9/MarkerMAG/link_16s.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/matam_16s.py` & `MarkerMAG-1.1.9/MarkerMAG/matam_16s.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/polish_16s.py` & `MarkerMAG-1.1.9/MarkerMAG/polish_16s.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/recovery_16s.py` & `MarkerMAG-1.1.9/MarkerMAG/recovery_16s.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/rename_reads.py` & `MarkerMAG-1.1.9/MarkerMAG/rename_reads.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/subsample_reads.py` & `MarkerMAG-1.1.9/MarkerMAG/subsample_reads.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG/uclust_16s.py` & `MarkerMAG-1.1.9/MarkerMAG/uclust_16s.py`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/MarkerMAG.egg-info/SOURCES.txt` & `MarkerMAG-1.1.9/MarkerMAG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/README.md` & `MarkerMAG-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `MarkerMAG-1.1.8/bin/MarkerMAG` & `MarkerMAG-1.1.9/bin/MarkerMAG`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,16 @@
         get_16s_copy_num_parser.add_argument('-t',                      required=False, type=int, default=1,                    help='number of threads')
         get_16s_copy_num_parser.add_argument('-force',                  required=False, action="store_true",                    help='Force overwrite existing results')
         get_16s_copy_num_parser.add_argument('-quiet',                  required=False, action="store_true",                    help='Not report progress')
         get_16s_copy_num_parser.add_argument('-silva_order_refs',       required=False,                                         help='subsampled SILVA 16S sequences (order level)')
         get_16s_copy_num_parser.add_argument('-hmm_bac',                required=False,                                         help='vxtractor hmm_bac folder')
         get_16s_copy_num_parser.add_argument('-hmm_arc',                required=False,                                         help='vxtractor hmm_arc folder')
         args = vars(parser.parse_args())
+        for each_key in config_dict:
+            args[each_key] = config_dict[each_key]
         get_cp_num.get_16s_copy_num(args)
 
     elif sys.argv[1] == 'rename_reads':
         from MarkerMAG import rename_reads
         rename_reads_parser = subparsers.add_parser('rename_reads', description='Rename reads', usage=rename_reads.rename_reads_usage)
         rename_reads_parser.add_argument('-r1',  required=True, type=str,               help='forward reads, fasta format')
         rename_reads_parser.add_argument('-r2',  required=True, type=str,               help='reverse reads, fasta format')
```

### Comparing `MarkerMAG-1.1.8/setup.py` & `MarkerMAG-1.1.9/setup.py`

 * *Files identical despite different names*

