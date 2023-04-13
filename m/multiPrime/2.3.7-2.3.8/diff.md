# Comparing `tmp/multiPrime-2.3.7.tar.gz` & `tmp/multiPrime-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.3.7.tar", last modified: Wed Apr 12 10:01:32 2023, max compression
+gzip compressed data, was "multiPrime-2.3.8.tar", last modified: Thu Apr 13 01:46:23 2023, max compression
```

## Comparing `multiPrime-2.3.7.tar` & `multiPrime-2.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 10:01:32.145124 multiPrime-2.3.7/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.7/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 10:01:32.145124 multiPrime-2.3.7/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12802 2023-02-21 06:44:43.000000 multiPrime-2.3.7/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 10:01:32.144123 multiPrime-2.3.7/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-12 10:01:32.145124 multiPrime-2.3.7/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.7/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 10:01:32.144123 multiPrime-2.3.7/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.7/src/__init__.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-12 09:55:33.000000 multiPrime-2.3.7/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-12 10:01:12.000000 multiPrime-2.3.7/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    84362 2023-04-12 10:01:05.000000 multiPrime-2.3.7/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24853 2023-04-12 10:01:01.000000 multiPrime-2.3.7/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-13 01:46:23.810859 multiPrime-2.3.8/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.8/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-13 01:46:23.809859 multiPrime-2.3.8/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12802 2023-02-21 06:44:43.000000 multiPrime-2.3.8/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-13 01:46:23.796857 multiPrime-2.3.8/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-13 01:46:23.810859 multiPrime-2.3.8/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.8/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-13 01:46:23.809859 multiPrime-2.3.8/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.8/src/__init__.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-13 01:45:57.000000 multiPrime-2.3.8/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-13 01:45:21.000000 multiPrime-2.3.8/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    84525 2023-04-13 01:45:21.000000 multiPrime-2.3.8/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24918 2023-04-13 01:45:21.000000 multiPrime-2.3.8/src/utils.py
```

### Comparing `multiPrime-2.3.7/LICENSE` & `multiPrime-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.7/PKG-INFO` & `multiPrime-2.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.7
+Version: 2.3.8
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.3.7/README.md` & `multiPrime-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.7/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.3.8/multiPrime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.7
+Version: 2.3.8
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.3.7/setup.py` & `multiPrime-2.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.7/src/main.py` & `multiPrime-2.3.8/src/main.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.7/src/src.py` & `multiPrime-2.3.8/src/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -1430,26 +1430,29 @@
         with open(Output, "w") as fo:
             for seq in seq_ID.keys():
                 # print(">" + '_'.join(seq_ID[seq]))
                 # print(seq)
                 fo.write(">" + '_'.join(seq_ID[seq]) + "\n" + seq + "\n")
         return seq_ID
 
-    def Bowtie_index(self, Input):
+    def Bowtie_index(self, Input, method):
         Bowtie_file = Path(Input).parent.joinpath("Bowtie_DB")
         Bowtie_prefix = Path(Bowtie_file).joinpath(Path(Input).stem)
+        bowtie_cmd = method + "-build"
         if Bowtie_file.exists():
-            size = os.path.getsize(Bowtie_file)
+            size = os.listdir(Bowtie_file)
             if not size:
-                os.system("bowtie2-build {} {}".format(Input, Bowtie_prefix))
+                print("No bowtie index found, start building ...")
+                os.system("{} {} {}".format(bowtie_cmd, Input, Bowtie_prefix))
             else:
+                print("Bowtie index is OK.")
                 pass
         else:
             os.mkdir(Bowtie_file)
-            os.system("bowtie2-build {} {}".format(Input, Bowtie_prefix))
+            os.system("{} {} {}".format(bowtie_cmd, Input, Bowtie_prefix))
 
     def build_dict(self, Input):
         Input_dict = defaultdict(list)
         threshold = self.term_threshold
         with open(Input, "r") as f:
             position_pattern_1 = re.compile('MD:Z:(\w+)')
             position_pattern = re.compile("[A-Z]?(\d+)")
@@ -1475,22 +1478,22 @@
         out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".sam")
         for_out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".for.sam")
         rev_out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".rev.sam")
         nproc = self.nproc
         if for_out.exists() and rev_out.exists():
             pass
         else:
-            if self.bowtie == 'bowtie2':
-                os.system("bowtie2 -p {} -f -N {} -L 8 -a -x {} -f -U {} -S {}".format(self.nproc, self.mismatch_num,
-                                                                                       ref_index, fa, out))
-            elif self.bowtie == 'bowtie':
+            if re.search('bowtie2', self.bowtie):
+                os.system("{} -p {} -N {} -L 8 -a -x {} -f -U {} -S {}".format(self.bowtie, self.nproc,
+                                                                               self.mismatch_num, ref_index, fa, out))
+            elif re.search('bowtie', self.bowtie):
                 os.system(
-                    "bowtie -p {} -f -n {} -l 8 -a -p {} --best --strata {} {} -S {}".format(self.nproc,
-                                                                                             self.mismatch_num,
-                                                                                             nproc, ref_index, fa, out))
+                    "{} -p {} -f -n {} -l 8 -a --best --strata {} {} -S {}".format(self.bowtie, self.nproc,
+                                                                                   self.mismatch_num, ref_index, fa,
+                                                                                   out))
             else:
                 print("mapping software must be bowtie or bowtie2 !")
                 sys.exit(1)
             os.system("samtools view -@ {} -F 16 {} > {}".format(nproc, out, for_out))
             os.system("samtools view -@ {} -f 16 {} > {}".format(nproc, out, rev_out))
 
     def build_dict_run(self):
@@ -1547,15 +1550,15 @@
                             # still stored in that process. In fact, this variable in the main process is equivalent
                             # to not being modified. In order to synchronize the changes of other processes to the
                             # main process, you need to create variables that can be shared among multiple processes.
         self.resQ.put(None)
 
     def run(self):
         self.get_term()
-        self.Bowtie_index(self.reference_file)
+        self.Bowtie_index(self.reference_file, self.bowtie)
         self.bowtie_map()
         target_gene, forward_dict, reverse_dict = self.build_dict_run()
         p = ProcessPoolExecutor(self.nproc)
         for gene in target_gene:
             p.submit(self.PCR_product(gene, forward_dict, reverse_dict))
         # This will submit all tasks to one place without blocking, and then each
         # thread in the thread pool will fetch tasks.
```

### Comparing `multiPrime-2.3.7/src/utils.py` & `multiPrime-2.3.8/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,23 +262,23 @@
         parser.print_help()
         print("No output file provided !!!")
         sys.exit(1)
     return parser.parse_args()
 
 
 def Errors_argsParse():
-    parser = OptionParser('Usage: %prog Errors -i [input] -r [bowtie index] -l [150,2000] -p [10]-o [output]')
+    parser = OptionParser('Usage: %prog Errors -i [input] -r [reference fasta] -l [150,2000] -p [10]-o [output]')
 
     parser.add_option('-i', '--input',
                       dest='input_file',
                       help='input file: primer.fa.')
 
     parser.add_option('-r', '--ref',
                       dest='ref',
-                      help='reference file: fasta file.')
+                      help='reference file: fasta format.')
 
     parser.add_option('-l', '--len',
                       dest='len',
                       default=18,
                       type="int",
                       help='Length of primer, which is used for mapping. Default: 18')
 
@@ -300,15 +300,16 @@
                       type="int",
                       help='Number of process. Default: 20')
 
     parser.add_option('-b', '--bowtie',
                       dest='bowtie',
                       default="bowtie2",
                       type="string",
-                      help='bowtie or bowtie2 was employed for mapping. Default: bowtie2')
+                      help='bowtie/ABS_path(bowtie) or bowtie2/ABS_path(bowtie2) was employed for mapping. '
+                           'Default: bowtie2 ')
 
     parser.add_option('-m', '--seedmms',
                       dest='seedmms',
                       default="1",
                       type="int",
                       help='Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).'
                            'Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1).')
@@ -323,15 +324,15 @@
         sys.exit(1)
     elif options.input_file is None:
         parser.print_help()
         print("Input file must be specified !!!")
         sys.exit(1)
     elif options.ref is None:
         parser.print_help()
-        print("reference index (bowtie) must be specified !!!")
+        print("reference (fasta) must be specified !!!")
         sys.exit(1)
     elif options.out is None:
         parser.print_help()
         print("No output file provided !!!")
         sys.exit(1)
     return parser.parse_args()
```

