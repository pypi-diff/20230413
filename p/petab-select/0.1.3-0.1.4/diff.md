# Comparing `tmp/petab_select-0.1.3.tar.gz` & `tmp/petab_select-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab_select-0.1.3.tar", last modified: Fri Jan 20 03:49:10 2023, max compression
+gzip compressed data, was "petab_select-0.1.4.tar", last modified: Thu Apr 13 16:13:11 2023, max compression
```

## Comparing `petab_select-0.1.3.tar` & `petab_select-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-01-20 03:49:10.101174 petab_select-0.1.3/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.3/LICENSE
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-01-20 03:49:10.101174 petab_select-0.1.3/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-01-20 03:44:55.000000 petab_select-0.1.3/README.md
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-01-20 03:49:10.097174 petab_select-0.1.3/petab_select/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/__init__.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    51676 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/candidate_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/cli.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/constants.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/criteria.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.3/petab_select/descriptors.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/handlers.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/misc.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    25962 2022-10-04 16:18:55.000000 petab_select-0.1.3/petab_select/model.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/model_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/model_subspace.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/petab.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/problem.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    10044 2022-09-30 16:40:04.000000 petab_select-0.1.3/petab_select/ui.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.3/petab_select/validators.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-01-20 03:48:16.000000 petab_select-0.1.3/petab_select/version.py
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-01-20 03:49:10.101174 petab_select-0.1.3/petab_select.egg-info/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-01-20 03:49:10.000000 petab_select-0.1.3/petab_select.egg-info/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-01-20 03:49:10.000000 petab_select-0.1.3/petab_select.egg-info/SOURCES.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-01-20 03:49:10.000000 petab_select-0.1.3/petab_select.egg-info/dependency_links.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-01-20 03:49:10.000000 petab_select-0.1.3/petab_select.egg-info/entry_points.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-01-20 03:49:10.000000 petab_select-0.1.3/petab_select.egg-info/requires.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-01-20 03:49:10.000000 petab_select-0.1.3/petab_select.egg-info/top_level.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.3/pyproject.toml
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-01-20 03:49:10.101174 petab_select-0.1.3/setup.cfg
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2022-10-04 16:24:25.000000 petab_select-0.1.3/setup.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-13 16:13:11.128681 petab_select-0.1.4/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.4/LICENSE
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-04-13 16:13:11.128681 petab_select-0.1.4/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.4/README.md
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-13 16:13:11.124681 petab_select-0.1.4/petab_select/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.4/petab_select/__init__.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    51676 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/candidate_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/cli.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/constants.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/criteria.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.4/petab_select/descriptors.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/handlers.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/misc.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    25962 2023-04-13 16:12:57.000000 petab_select-0.1.4/petab_select/model.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/model_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/model_subspace.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/petab.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.4/petab_select/problem.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    10109 2023-04-13 16:12:57.000000 petab_select-0.1.4/petab_select/ui.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.4/petab_select/validators.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-04-13 16:12:57.000000 petab_select-0.1.4/petab_select/version.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-13 16:13:11.124681 petab_select-0.1.4/petab_select.egg-info/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/entry_points.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/requires.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/top_level.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.4/pyproject.toml
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-04-13 16:13:11.128681 petab_select-0.1.4/setup.cfg
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.4/setup.py
```

### Comparing `petab_select-0.1.3/LICENSE` & `petab_select-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/PKG-INFO` & `petab_select-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab_select
-Version: 0.1.3
+Version: 0.1.4
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -126,14 +126,14 @@
 | 0002<sup>[1](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0002)</sup>    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0003    | BIC       | all                | 1                 | Yes               |                   |                      |
 | 0004    | AICc      | backward           | 1                 |                   | 1                 |                      |
 | 0005    | AIC       | forward            | 1                 |                   |                   | 1                    |
 | 0006    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0007<sup>[2](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0007_and_0008)</sup>    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0008<sup>[2](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0007_and_0008)</sup>    | AICc       | backward            | 1                 |                   |                   |                      |
-| 0009<sup>[2](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0009)</sup>    | AICc       | FAMoS            | 1                 | Yes                  |                   | Yes                     |
+| 0009<sup>[3](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0009)</sup>    | AICc       | FAMoS            | 1                 | Yes                  |                   | Yes                     |
 
 <a name="test_case_0002">1</a>. Model `M1_0` differs from `M1_1` in three parameters, but only 1 additional estimated parameter. The effect of this on model selection criteria needs to be clarified. Test case 0006 is a duplicate of 0002 that doesn't have this issue.
 
 <a name="test_case_0007_and_0008">2</a>. Noise parameter is removed, noise is fixed to `1`.
 
 <a name="test_case_0009">3</a>. This is a computationally-expensive problem to solve. Developers can try a model selection initialized with the provided predecessor model, which is a model start that reproducibly finds the expected model. To solve the problem reproducibly <i>ab initio</i>, on the order of 100 random model starts are required. This test case reproduces the model selection problem presented in https://doi.org/10.1016/j.cels.2016.01.002 .
```

### Comparing `petab_select-0.1.3/README.md` & `petab_select-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,14 @@
 | 0002<sup>[1](#test_case_0002)</sup>    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0003    | BIC       | all                | 1                 | Yes               |                   |                      |
 | 0004    | AICc      | backward           | 1                 |                   | 1                 |                      |
 | 0005    | AIC       | forward            | 1                 |                   |                   | 1                    |
 | 0006    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0007<sup>[2](#test_case_0007_and_0008)</sup>    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0008<sup>[2](#test_case_0007_and_0008)</sup>    | AICc       | backward            | 1                 |                   |                   |                      |
-| 0009<sup>[2](#test_case_0009)</sup>    | AICc       | FAMoS            | 1                 | Yes                  |                   | Yes                     |
+| 0009<sup>[3](#test_case_0009)</sup>    | AICc       | FAMoS            | 1                 | Yes                  |                   | Yes                     |
 
 <a name="test_case_0002">1</a>. Model `M1_0` differs from `M1_1` in three parameters, but only 1 additional estimated parameter. The effect of this on model selection criteria needs to be clarified. Test case 0006 is a duplicate of 0002 that doesn't have this issue.
 
 <a name="test_case_0007_and_0008">2</a>. Noise parameter is removed, noise is fixed to `1`.
 
 <a name="test_case_0009">3</a>. This is a computationally-expensive problem to solve. Developers can try a model selection initialized with the provided predecessor model, which is a model start that reproducibly finds the expected model. To solve the problem reproducibly <i>ab initio</i>, on the order of 100 random model starts are required. This test case reproduces the model selection problem presented in https://doi.org/10.1016/j.cels.2016.01.002 .
```

### Comparing `petab_select-0.1.3/petab_select/candidate_space.py` & `petab_select-0.1.4/petab_select/candidate_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/cli.py` & `petab_select-0.1.4/petab_select/cli.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/constants.py` & `petab_select-0.1.4/petab_select/constants.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/criteria.py` & `petab_select-0.1.4/petab_select/criteria.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/descriptors.py` & `petab_select-0.1.4/petab_select/descriptors.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/handlers.py` & `petab_select-0.1.4/petab_select/handlers.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/misc.py` & `petab_select-0.1.4/petab_select/misc.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/model.py` & `petab_select-0.1.4/petab_select/model.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/model_space.py` & `petab_select-0.1.4/petab_select/model_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/model_subspace.py` & `petab_select-0.1.4/petab_select/model_subspace.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/petab.py` & `petab_select-0.1.4/petab_select/petab.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/problem.py` & `petab_select-0.1.4/petab_select/problem.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/petab_select/ui.py` & `petab_select-0.1.4/petab_select/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,15 @@
             )
         )
 
     # FIXME remove once MostDistantCandidateSpace exists...
     method = candidate_space.method
     if (
         candidate_space.governing_method == Method.FAMOS
+        and isinstance(candidate_space.predecessor_model, Model)
         and candidate_space.predecessor_model.predecessor_model_hash is None
     ):
         with open(candidate_space.summary_tsv, 'r') as f:
             if sum(1 for _ in f) > 1:
                 method = Method.MOST_DISTANT
 
     candidate_space.write_summary_tsv(
```

### Comparing `petab_select-0.1.3/petab_select.egg-info/PKG-INFO` & `petab_select-0.1.4/petab_select.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab-select
-Version: 0.1.3
+Version: 0.1.4
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -126,14 +126,14 @@
 | 0002<sup>[1](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0002)</sup>    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0003    | BIC       | all                | 1                 | Yes               |                   |                      |
 | 0004    | AICc      | backward           | 1                 |                   | 1                 |                      |
 | 0005    | AIC       | forward            | 1                 |                   |                   | 1                    |
 | 0006    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0007<sup>[2](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0007_and_0008)</sup>    | AIC       | forward            | 1                 |                   |                   |                      |
 | 0008<sup>[2](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0007_and_0008)</sup>    | AICc       | backward            | 1                 |                   |                   |                      |
-| 0009<sup>[2](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0009)</sup>    | AICc       | FAMoS            | 1                 | Yes                  |                   | Yes                     |
+| 0009<sup>[3](https://github.com/PEtab-dev/petab_select/tree/main/#test_case_0009)</sup>    | AICc       | FAMoS            | 1                 | Yes                  |                   | Yes                     |
 
 <a name="test_case_0002">1</a>. Model `M1_0` differs from `M1_1` in three parameters, but only 1 additional estimated parameter. The effect of this on model selection criteria needs to be clarified. Test case 0006 is a duplicate of 0002 that doesn't have this issue.
 
 <a name="test_case_0007_and_0008">2</a>. Noise parameter is removed, noise is fixed to `1`.
 
 <a name="test_case_0009">3</a>. This is a computationally-expensive problem to solve. Developers can try a model selection initialized with the provided predecessor model, which is a model start that reproducibly finds the expected model. To solve the problem reproducibly <i>ab initio</i>, on the order of 100 random model starts are required. This test case reproduces the model selection problem presented in https://doi.org/10.1016/j.cels.2016.01.002 .
```

### Comparing `petab_select-0.1.3/petab_select.egg-info/SOURCES.txt` & `petab_select-0.1.4/petab_select.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.3/setup.py` & `petab_select-0.1.4/setup.py`

 * *Files identical despite different names*

