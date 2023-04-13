# Comparing `tmp/schnitsum-0.4.3.tar.gz` & `tmp/schnitsum-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schnitsum-0.4.3.tar", max compression
+gzip compressed data, was "schnitsum-0.4.4.tar", max compression
```

## Comparing `schnitsum-0.4.3.tar` & `schnitsum-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2022-09-29 19:29:08.745912 schnitsum-0.4.3/LICENSE
--rw-r--r--   0        0        0     2117 2022-10-02 07:50:48.157911 schnitsum-0.4.3/README.md
--rw-r--r--   0        0        0      546 2022-11-21 10:04:59.651902 schnitsum-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       37 2022-09-30 14:59:31.703238 schnitsum-0.4.3/schnitsum/__init__.py
--rw-r--r--   0        0        0      693 2022-10-01 09:02:23.109770 schnitsum-0.4.3/schnitsum/bin/summarize.py
--rw-r--r--   0        0        0     1974 2022-10-01 09:04:04.247081 schnitsum-0.4.3/schnitsum/main.py
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 schnitsum-0.4.3/setup.py
--rw-r--r--   0        0        0     2661 1970-01-01 00:00:00.000000 schnitsum-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-29 19:29:08.745912 schnitsum-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2117 2022-10-02 07:50:48.157911 schnitsum-0.4.4/README.md
+-rw-r--r--   0        0        0      547 2023-04-13 09:10:55.016639 schnitsum-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1974 2023-04-13 09:04:35.960134 schnitsum-0.4.4/schnitsum/.null-ls_956519_main.py
+-rw-r--r--   0        0        0       37 2022-09-30 14:59:31.703238 schnitsum-0.4.4/schnitsum/__init__.py
+-rw-r--r--   0        0        0      693 2022-10-01 09:02:23.109770 schnitsum-0.4.4/schnitsum/bin/summarize.py
+-rw-r--r--   0        0        0     2112 2023-04-13 09:09:35.300804 schnitsum-0.4.4/schnitsum/main.py
+-rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 schnitsum-0.4.4/setup.py
+-rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 schnitsum-0.4.4/PKG-INFO
```

### Comparing `schnitsum-0.4.3/LICENSE` & `schnitsum-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `schnitsum-0.4.3/README.md` & `schnitsum-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `schnitsum-0.4.3/schnitsum/bin/summarize.py` & `schnitsum-0.4.4/schnitsum/bin/summarize.py`

 * *Files identical despite different names*

### Comparing `schnitsum-0.4.3/schnitsum/main.py` & `schnitsum-0.4.4/schnitsum/.null-ls_956519_main.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from tqdm import tqdm
 
+from tqdm import tqdm
 from transformers import AutoModelForSeq2SeqLM, AutoTokenizer
 
 MODEL_NAMES = [
     "sobamchan/bart-large-scitldr",
     "sobamchan/bart-large-scitldr-distilled-3-3",
     "sobamchan/bart-large-scitldr-distilled-12-3",
 ]
```

### Comparing `schnitsum-0.4.3/setup.py` & `schnitsum-0.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['fire>=0.4.0,<0.5.0',
  'sienna>=0.1.5,<0.2.0',
- 'torch==1.12.1',
+ 'torch>=2.0.0',
  'transformers==4.22.2']
 
 entry_points = \
 {'console_scripts': ['schnitsum = schnitsum.bin.summarize:cli']}
 
 setup_kwargs = {
     'name': 'schnitsum',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': '',
     'long_description': '# Schnitsum: Easy to use neural network based summarization models\n\nThis package enables to generate summaries of you documents of interests.\n\nCurrently, we support following models,\n\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)).\n  - Model name: `sobamchan/bart-large-scitldr`\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 65% parameters less.\n  - Model name: `sobamchan/bart-large-scitldr-distilled-3-3`\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 37% parameters less.\n  - Model name: `sobamchan/bart-large-scitldr-distilled-12-3`\n\nwe are planning to expand coverage soon to other sizes, domains, languages, models soon.\n\n\n# Installation\n\n```bash\npip install schnitsum  # or poetry add schnitsum\n```\n\nThis will let you generate summaries with CPUs only, if you want to utilize your GPUs, please follow the instruction by PyTorch, [here](https://pytorch.org/get-started/locally/).\n\n\n# Usage\n\n## From Command Line\nPass document as an argument and print the summary\n```sh\n> schnitsum --model-name sobamchan/bart-large-scitldr-distilled-3-3 --text "Text to summarize"\n```\n\nPass documents as a file and save summaries in a file.\nInput file needs to contain documents line by line. [example](https://github.com/sobamchan/schnitsum/blob/main/examples/docs.txt)\n```sh\n> schnitsum --model-name sobamchan/bart-large-scitldr-distilled-3-3 --file docs.txt --opath sums.txt\n```\n\n## From Python\n```py3\nfrom schnitsum import SchnitSum\n\nmodel = SchnitSum("sobamchan/bart-large-scitldr-distilled-3-3")\ndocs = [\n    "Document you want to summarize."\n]\nsummaries = model(docs)\nprint(summaries)\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `schnitsum-0.4.3/PKG-INFO` & `schnitsum-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: schnitsum
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: sienna (>=0.1.5,<0.2.0)
-Requires-Dist: torch (==1.12.1)
+Requires-Dist: torch (>=2.0.0)
 Requires-Dist: transformers (==4.22.2)
 Description-Content-Type: text/markdown
 
 # Schnitsum: Easy to use neural network based summarization models
 
 This package enables to generate summaries of you documents of interests.
```

