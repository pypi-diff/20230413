# Comparing `tmp/relation_validator-0.2.0.tar.gz` & `tmp/relation_validator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relation_validator-0.2.0.tar", max compression
+gzip compressed data, was "relation_validator-0.2.1.tar", max compression
```

## Comparing `relation_validator-0.2.0.tar` & `relation_validator-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-25 20:00:56.444020 relation_validator-0.2.0/LICENSE
--rw-r--r--   0        0        0     2089 2023-04-10 20:51:03.249986 relation_validator-0.2.0/README.md
--rw-r--r--   0        0        0      594 2023-04-10 21:06:57.907532 relation_validator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-23 22:40:04.740921 relation_validator-0.2.0/src/relation_validator/__init__.py
--rw-r--r--   0        0        0     1457 2023-04-01 21:51:21.270341 relation_validator-0.2.0/src/relation_validator/__main__.py
--rw-r--r--   0        0        0        0 2023-03-26 11:57:02.725073 relation_validator-0.2.0/src/relation_validator/utils/__init__.py
--rw-r--r--   0        0        0     2403 2023-04-01 21:33:44.672394 relation_validator-0.2.0/src/relation_validator/utils/utils.py
--rw-r--r--   0        0        0      768 2023-04-01 21:39:21.268624 relation_validator-0.2.0/src/relation_validator/validator.py
--rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 relation_validator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 10:51:27.886165 relation_validator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2434 2023-04-13 10:51:27.886348 relation_validator-0.2.1/README.md
+-rw-r--r--   0        0        0      652 2023-04-13 10:59:36.877519 relation_validator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 10:51:27.888196 relation_validator-0.2.1/src/relation_validator/__init__.py
+-rw-r--r--   0        0        0     1457 2023-04-13 10:51:27.888327 relation_validator-0.2.1/src/relation_validator/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:51:27.888431 relation_validator-0.2.1/src/relation_validator/utils/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-13 10:51:27.888570 relation_validator-0.2.1/src/relation_validator/utils/utils.py
+-rw-r--r--   0        0        0      768 2023-04-13 10:51:27.888680 relation_validator-0.2.1/src/relation_validator/validator.py
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 relation_validator-0.2.1/PKG-INFO
```

### Comparing `relation_validator-0.2.0/LICENSE` & `relation_validator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relation_validator-0.2.0/README.md` & `relation_validator-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Relationship validator
 
-Validation process using [Ubergraph](https://zenodo.org/record/7249759#.ZDRuZOzML1c) as source of truth.
+Validate ontology relationships using [Ubergraph](https://zenodo.org/record/7249759#.ZDRuZOzML1c) as source of truth. Relationships in this context may be subClassOf axioms between names classes (e.g. 'lymphocyte' subClassOf 'cell') or existential restrictions, (e.g. 'enterocyte' part_of some ‘intestinal epithelium’).
 
-Ubergraph is an RDF triplestore with [39 OBO ontologies](https://github.com/INCATools/ubergraph#integrated-obo-ontology-triplestore) merged, precomputed OWL classification and materialized class relationship from existential properties restriction.
+Ubergraph is an RDF triplestore with [39 OBO ontologies](https://github.com/INCATools/ubergraph#integrated-obo-ontology-triplestore) merged, precomputed OWL classification and materialised class relationship from existential property restrictions.  Validation therefore works for any directly asserted or inferred/indirect subClassOf relationship or existential restriction.
 
 
 ## Install
 
 ```bash
 pip install relation-validator
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `relation_validator-0.2.0/pyproject.toml` & `relation_validator-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "relation-validator"
-version = "0.2.0"
+version = "0.2.1"
 description = "This package validates a list of relationships between two terms against the specified ontologies."
 authors = ["Anita Caron <anitac@ebi.ac.uk>"]
 readme = "README.md"
+packages = [{include = "relation_validator", from="src"}]
 repository = "https://github.com/anitacaron/relation-validator"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyaml = "^21.10.1"
 ruamel-yaml = "^0.17.21"
 pandas = "^1.5.3"
```

### Comparing `relation_validator-0.2.0/src/relation_validator/__main__.py` & `relation_validator-0.2.1/src/relation_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `relation_validator-0.2.0/src/relation_validator/utils/utils.py` & `relation_validator-0.2.1/src/relation_validator/utils/utils.py`

 * *Files identical despite different names*

### Comparing `relation_validator-0.2.0/src/relation_validator/validator.py` & `relation_validator-0.2.1/src/relation_validator/validator.py`

 * *Files identical despite different names*

### Comparing `relation_validator-0.2.0/PKG-INFO` & `relation_validator-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relation-validator
-Version: 0.2.0
+Version: 0.2.1
 Summary: This package validates a list of relationships between two terms against the specified ontologies.
 Home-page: https://github.com/anitacaron/relation-validator
 Author: Anita Caron
 Author-email: anitac@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,17 +15,17 @@
 Requires-Dist: pyaml (>=21.10.1,<22.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Project-URL: Repository, https://github.com/anitacaron/relation-validator
 Description-Content-Type: text/markdown
 
 # Relationship validator
 
-Validation process using [Ubergraph](https://zenodo.org/record/7249759#.ZDRuZOzML1c) as source of truth.
+Validate ontology relationships using [Ubergraph](https://zenodo.org/record/7249759#.ZDRuZOzML1c) as source of truth. Relationships in this context may be subClassOf axioms between names classes (e.g. 'lymphocyte' subClassOf 'cell') or existential restrictions, (e.g. 'enterocyte' part_of some ‘intestinal epithelium’).
 
-Ubergraph is an RDF triplestore with [39 OBO ontologies](https://github.com/INCATools/ubergraph#integrated-obo-ontology-triplestore) merged, precomputed OWL classification and materialized class relationship from existential properties restriction.
+Ubergraph is an RDF triplestore with [39 OBO ontologies](https://github.com/INCATools/ubergraph#integrated-obo-ontology-triplestore) merged, precomputed OWL classification and materialised class relationship from existential property restrictions.  Validation therefore works for any directly asserted or inferred/indirect subClassOf relationship or existential restriction.
 
 
 ## Install
 
 ```bash
 pip install relation-validator
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

