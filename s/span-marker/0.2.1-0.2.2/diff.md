# Comparing `tmp/span_marker-0.2.1.tar.gz` & `tmp/span_marker-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-0.2.1.tar", last modified: Fri Apr  7 14:01:25 2023, max compression
+gzip compressed data, was "span_marker-0.2.2.tar", last modified: Thu Apr 13 14:12:02 2023, max compression
```

## Comparing `span_marker-0.2.1.tar` & `span_marker-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 14:01:25.193067 span_marker-0.2.1/
--rw-rw-rw-   0        0        0     1088 2023-03-28 09:30:50.000000 span_marker-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4407 2023-04-07 14:01:25.193067 span_marker-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3830 2023-04-07 10:47:40.000000 span_marker-0.2.1/README.md
--rw-rw-rw-   0        0        0     2305 2023-04-06 15:01:25.000000 span_marker-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 14:01:25.193067 span_marker-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 14:01:25.178905 span_marker-0.2.1/span_marker/
--rw-rw-rw-   0        0        0      352 2023-04-07 13:58:03.000000 span_marker-0.2.1/span_marker/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-04-07 13:40:17.000000 span_marker-0.2.1/span_marker/configuration.py
--rw-rw-rw-   0        0        0     5389 2023-04-06 13:34:33.000000 span_marker-0.2.1/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     4295 2023-04-06 07:35:29.000000 span_marker-0.2.1/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     4831 2023-04-06 07:35:29.000000 span_marker-0.2.1/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     1086 2023-04-07 13:56:16.000000 span_marker-0.2.1/span_marker/model_card.py
--rw-rw-rw-   0        0        0    20210 2023-04-07 13:56:16.000000 span_marker-0.2.1/span_marker/modeling.py
--rw-rw-rw-   0        0        0     1686 2023-04-06 14:00:45.000000 span_marker-0.2.1/span_marker/output.py
--rw-rw-rw-   0        0        0     6313 2023-04-07 12:12:36.000000 span_marker-0.2.1/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    11036 2023-04-06 14:00:45.000000 span_marker-0.2.1/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 14:01:25.191066 span_marker-0.2.1/span_marker.egg-info/
--rw-rw-rw-   0        0        0     4407 2023-04-07 14:01:25.000000 span_marker-0.2.1/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-04-07 14:01:25.000000 span_marker-0.2.1/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 14:01:25.000000 span_marker-0.2.1/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2023-04-07 14:01:25.000000 span_marker-0.2.1/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-07 14:01:25.000000 span_marker-0.2.1/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-07 14:01:25.192067 span_marker-0.2.1/tests/
--rw-rw-rw-   0        0        0      961 2023-04-06 07:35:29.000000 span_marker-0.2.1/tests/test_configuration.py
--rw-rw-rw-   0        0        0     3534 2023-04-06 07:35:29.000000 span_marker-0.2.1/tests/test_modeling.py
--rw-rw-rw-   0        0        0     3992 2023-04-06 07:35:29.000000 span_marker-0.2.1/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.552919 span_marker-0.2.2/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 09:30:50.000000 span_marker-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4407 2023-04-13 14:12:02.552919 span_marker-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3830 2023-04-07 10:47:40.000000 span_marker-0.2.2/README.md
+-rw-rw-rw-   0        0        0     2349 2023-04-13 12:27:58.000000 span_marker-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:12:02.552919 span_marker-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.534551 span_marker-0.2.2/span_marker/
+-rw-rw-rw-   0        0        0      352 2023-04-13 14:11:49.000000 span_marker-0.2.2/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     6408 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     5389 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     4295 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     4831 2023-04-06 07:35:29.000000 span_marker-0.2.2/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     1089 2023-04-07 14:45:51.000000 span_marker-0.2.2/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    21801 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     1686 2023-04-06 14:00:45.000000 span_marker-0.2.2/span_marker/output.py
+-rw-rw-rw-   0        0        0     6313 2023-04-13 14:08:07.000000 span_marker-0.2.2/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    11036 2023-04-11 11:25:40.000000 span_marker-0.2.2/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.549567 span_marker-0.2.2/span_marker.egg-info/
+-rw-rw-rw-   0        0        0     4407 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 14:12:02.000000 span_marker-0.2.2/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 14:12:02.551916 span_marker-0.2.2/tests/
+-rw-rw-rw-   0        0        0      961 2023-04-06 07:35:29.000000 span_marker-0.2.2/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     3534 2023-04-06 07:35:29.000000 span_marker-0.2.2/tests/test_modeling.py
+-rw-rw-rw-   0        0        0     3992 2023-04-06 07:35:29.000000 span_marker-0.2.2/tests/test_trainer.py
```

### Comparing `span_marker-0.2.1/LICENSE` & `span_marker-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/PKG-INFO` & `span_marker-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span_marker
-Version: 0.2.1
+Version: 0.2.2
 Summary: Few-Shot Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
```

### Comparing `span_marker-0.2.1/README.md` & `span_marker-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/pyproject.toml` & `span_marker-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     {name = "Tom Aarsen"}
 ]
 maintainers = [
     {name = "Tom Aarsen"}
 ]
 dependencies = [
     "torch",
-    "transformers",
+    "transformers>4.19.0", # required for EvalPrediction.inputs
     "datasets",
     "evaluate",
     "seqeval"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
```

### Comparing `span_marker-0.2.1/span_marker/data_collator.py` & `span_marker-0.2.2/span_marker/data_collator.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/span_marker/evaluation.py` & `span_marker-0.2.2/span_marker/evaluation.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/span_marker/label_normalizer.py` & `span_marker-0.2.2/span_marker/label_normalizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/span_marker/model_card.py` & `span_marker-0.2.2/span_marker/model_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 
 ```python
 from span_marker import SpanMarkerModel
 
 # Download from Hub and run inference
 model = SpanMarkerModel.from_pretrained("span_marker_model_name")
 # Run inference
-preds = model.predict("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
+entities = model.predict("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
 ```
 
 See the [SpanMarker](https://github.com/tomaarsen/SpanMarkerNER) repository for documentation and additional information on this model framework.
 """
```

### Comparing `span_marker-0.2.1/span_marker/modeling.py` & `span_marker-0.2.2/span_marker/modeling.py`

 * *Files 6% similar despite different names*

```diff
@@ -215,15 +215,17 @@
                     f'...     "{pretrained_model_name_or_path}",\n'
                     '...     labels=["O", "PER", "ORG", "LOC", "MISC"]\n'
                     "... )"
                 )
             config.id2label = dict(enumerate(labels))
             config.label2id = {v: k for k, v in config.id2label.items()}
             # Set the span_marker version for freshly initialized models
-            config = cls.config_class(encoder_config=config.to_dict(), span_marker_version=span_marker_version)
+            config = cls.config_class(
+                encoder_config=config.to_dict(), span_marker_version=span_marker_version, **kwargs
+            )
             model = cls(config, encoder, *model_args, **kwargs)
 
         # Pass the tokenizer directly to the model for convenience, this way the user doesn't have to
         # make it themselves.
         tokenizer = SpanMarkerTokenizer.from_pretrained(
             config.encoder.get("_name_or_path", pretrained_model_name_or_path), config=config, **kwargs
         )
@@ -233,14 +235,28 @@
         return model
 
     def predict(
         self, inputs: Union[str, List[str], List[List[str]]], allow_overlapping: bool = False
     ) -> Union[List[Dict[str, Union[str, int, float]]], List[List[Dict[str, Union[str, int, float]]]]]:
         """Predict named entities from input texts.
 
+        Example:
+
+            >>> model = SpanMarkerModel.from_pretrained(...)
+            >>> model.predict("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
+            [{'span': 'Amelia Earhart', 'label': 'person-other', 'score': 0.7629689574241638, 'char_start_index': 0, 'char_end_index': 14},
+             {'span': 'Lockheed Vega 5B', 'label': 'product-airplane', 'score': 0.9833564758300781, 'char_start_index': 38, 'char_end_index': 54},
+             {'span': 'Atlantic', 'label': 'location-bodiesofwater', 'score': 0.7621214389801025, 'char_start_index': 66, 'char_end_index': 74},
+             {'span': 'Paris', 'label': 'location-GPE', 'score': 0.9807717204093933, 'char_start_index': 78, 'char_end_index': 83}]
+            >>> model.predict(['Caesar', 'led', 'the', 'Roman', 'armies', 'in', 'the', 'Gallic', 'Wars', 'before', 'defeating', 'his', 'political', 'rival', 'Pompey', 'in', 'a', 'civil', 'war'])
+            [{'span': ['Caesar'], 'label': 'person-politician', 'score': 0.683479905128479, 'word_start_index': 0, 'word_end_index': 1},
+             {'span': ['Roman'], 'label': 'location-GPE', 'score': 0.7114525437355042, 'word_start_index': 3, 'word_end_index': 4},
+             {'span': ['Gallic', 'Wars'], 'label': 'event-attack/battle/war/militaryconflict', 'score': 0.9015670418739319, 'word_start_index': 7, 'word_end_index': 9},
+             {'span': ['Pompey'], 'label': 'person-politician', 'score': 0.9601260423660278, 'word_start_index': 14, 'word_end_index': 15}]
+
         Args:
             inputs (Union[str, List[str], List[List[str]]]): Input sentences from which to extract entities.
                 Valid datastructures are:
 
                 * str: a string sentence.
                 * List[str]: a pre-tokenized string sentence, i.e. a list of words.
                 * List[str]: a list of multiple string sentences.
```

### Comparing `span_marker-0.2.1/span_marker/output.py` & `span_marker-0.2.2/span_marker/output.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/span_marker/tokenizer.py` & `span_marker-0.2.2/span_marker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/span_marker/trainer.py` & `span_marker-0.2.2/span_marker/trainer.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/span_marker.egg-info/PKG-INFO` & `span_marker-0.2.2/span_marker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span-marker
-Version: 0.2.1
+Version: 0.2.2
 Summary: Few-Shot Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
```

### Comparing `span_marker-0.2.1/span_marker.egg-info/SOURCES.txt` & `span_marker-0.2.2/span_marker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/tests/test_configuration.py` & `span_marker-0.2.2/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/tests/test_modeling.py` & `span_marker-0.2.2/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `span_marker-0.2.1/tests/test_trainer.py` & `span_marker-0.2.2/tests/test_trainer.py`

 * *Files identical despite different names*

