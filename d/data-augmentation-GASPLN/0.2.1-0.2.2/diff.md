# Comparing `tmp/data_augmentation_GASPLN-0.2.1.tar.gz` & `tmp/data_augmentation_GASPLN-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_augmentation_GASPLN-0.2.1.tar", last modified: Thu Apr 13 02:47:55 2023, max compression
+gzip compressed data, was "data_augmentation_GASPLN-0.2.2.tar", last modified: Thu Apr 13 02:49:45 2023, max compression
```

## Comparing `data_augmentation_GASPLN-0.2.1.tar` & `data_augmentation_GASPLN-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:47:55.361141 data_augmentation_GASPLN-0.2.1/
--rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      217 2023-04-13 02:47:55.361141 data_augmentation_GASPLN-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     9538 2023-04-13 02:47:23.000000 data_augmentation_GASPLN-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:47:55.346142 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN/
--rw-rw-rw-   0        0        0     9524 2023-04-13 02:46:48.000000 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:47:55.355142 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN/data/
--rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
-drwxrwxrwx   0        0        0        0 2023-04-13 02:47:55.354141 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN.egg-info/
--rw-rw-rw-   0        0        0      217 2023-04-13 02:47:55.000000 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-13 02:47:55.000000 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:47:55.000000 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-13 02:47:55.000000 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-13 02:47:55.000000 data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-13 02:47:55.362142 data_augmentation_GASPLN-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-13 02:47:30.000000 data_augmentation_GASPLN-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.683981 data_augmentation_GASPLN-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      217 2023-04-13 02:49:45.684499 data_augmentation_GASPLN-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9130 2023-04-13 02:49:17.000000 data_augmentation_GASPLN-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.643902 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/
+-rw-rw-rw-   0        0        0     9497 2023-04-13 02:48:58.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.676203 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/data/
+-rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
+drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.676203 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-13 02:49:45.686023 data_augmentation_GASPLN-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-13 02:49:34.000000 data_augmentation_GASPLN-0.2.2/setup.py
```

### Comparing `data_augmentation_GASPLN-0.2.1/LICENSE` & `data_augmentation_GASPLN-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.2.1/README.md` & `data_augmentation_GASPLN-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 
 This function is used to replace a percentage of words in a given text string with their synonyms. It takes three arguments: `text`, `synonyms_df`, and `percentage`.
 
 ### Arguments:
 
 * `text` (str): The input text to be processed. This can be any string, but should ideally be a full sentence or paragraph for best results.
 
-* `synonyms_df` (pd.DataFrame): A Pandas DataFrame containing word synonyms. This is already pre-loaded in the initialization, so there is no need to manually specify this parameter.
-
 * `percentage` (float, optional): The percentage of words in the input `text` that should be replaced with their synonyms. The default value is 0.25, which means that 25% of the words in the input text will be replaced.
 
 ### Example Usage:
 
 Here's an example of how to use the `synonyms_replacement` function:
 
 ```python
@@ -168,16 +166,14 @@
 
 ### Arguments:
 
 * `text` (str): The input text to be processed.
 
 * `use_synonyms` (bool, optional): Whether or not to use synonym replacement. Default is `True`.
 
-* `synonyms_df` (pd.DataFrame, optional): A Pandas DataFrame containing word synonyms. This is already pre-loaded in the initialization, so there is no need to manually specify this parameter. Default is `synonyms_df`.
-
 * `synonyms_percentage` (float, optional): The percentage of words in the input text that should be replaced with their synonyms. Default is 0.5.
 
 * `use_back_translation` (bool, optional): Whether or not to use back translation. Default is `False`.
 
 * `languages` (List[str], optional): A list of two-letter language codes representing the languages to translate the text to and back from. Default is `['en', 'es']`.
 
 * `translator` (str, optional): The name of the translator to use for back translation. Currently, the only supported value is `'google'`. Default is `'google'`.
```

### Comparing `data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN/__init__.py` & `data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         # Check that the word is still valid
         if len(words[i]) <= 1:
             continue
 
     return " ".join(words)
 
 def text_augmentation(text: str, 
-                      use_synonyms: bool = True, synonyms_df = synonyms_df, synonyms_percentage: float = 0.5,
+                      use_synonyms: bool = True, synonyms_percentage: float = 0.5,
                       use_back_translation: bool = False, languages: List[str] = ['en', 'es'], translator: str = 'google',
                       use_character_swap: bool = False, char_swap_prob: float = 0.25,
                       use_random_swap: bool = False, random_swap_percentage: float = None, num_words: int = None, random_swap_prob: float = 0.15,
                       use_add_noise: bool = True, word_noise_prob: float = 0.2, char_noise_prob: float = 0.2) -> str:
     """
     Apply multiple text augmentation techniques to the input text.
     """
```

### Comparing `data_augmentation_GASPLN-0.2.1/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet` & `data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.2.1/setup.py` & `data_augmentation_GASPLN-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='data_augmentation_GASPLN',
-    version='0.2.1',
+    version='0.2.2',
     author='Artur Melchiori Cerri',
     author_email='arturmelchiori@gmail.com',
     description='Data augmentation for Portuguese language',
     install_requires=[
         "spacy",
         "nltk",
         "pandas",
```

