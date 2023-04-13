# Comparing `tmp/tokenizer-viz-0.2.1.tar.gz` & `tmp/tokenizer-viz-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizer-viz-0.2.1.tar", last modified: Thu Apr 13 13:14:38 2023, max compression
+gzip compressed data, was "tokenizer-viz-0.2.2.tar", last modified: Thu Apr 13 17:34:40 2023, max compression
```

## Comparing `tokenizer-viz-0.2.1.tar` & `tokenizer-viz-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 13:14:38.713411 tokenizer-viz-0.2.1/
--rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.2.1/LICENSE
--rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 13:14:38.713305 tokenizer-viz-0.2.1/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)     2148 2023-04-13 12:57:10.000000 tokenizer-viz-0.2.1/README.md
--rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-13 13:14:38.713452 tokenizer-viz-0.2.1/setup.cfg
--rw-r--r--   0 darienschettler   (501) staff       (20)      959 2023-04-13 13:14:35.000000 tokenizer-viz-0.2.1/setup.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 13:14:38.712458 tokenizer-viz-0.2.1/tokenizer_viz/
--rw-r--r--   0 darienschettler   (501) staff       (20)       46 2023-04-13 12:36:19.000000 tokenizer-viz-0.2.1/tokenizer_viz/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     8501 2023-04-13 13:14:15.000000 tokenizer-viz-0.2.1/tokenizer_viz/visualization.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 13:14:38.713128 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/
--rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      267 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/SOURCES.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/dependency_links.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/requires.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/top_level.txt
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 17:34:40.596416 tokenizer-viz-0.2.2/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.2.2/LICENSE
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 17:34:40.596293 tokenizer-viz-0.2.2/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2148 2023-04-13 12:57:10.000000 tokenizer-viz-0.2.2/README.md
+-rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-13 17:34:40.596462 tokenizer-viz-0.2.2/setup.cfg
+-rw-r--r--   0 darienschettler   (501) staff       (20)      959 2023-04-13 17:34:25.000000 tokenizer-viz-0.2.2/setup.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 17:34:40.595342 tokenizer-viz-0.2.2/tokenizer_viz/
+-rw-r--r--   0 darienschettler   (501) staff       (20)       46 2023-04-13 12:36:19.000000 tokenizer-viz-0.2.2/tokenizer_viz/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)    10016 2023-04-13 17:31:25.000000 tokenizer-viz-0.2.2/tokenizer_viz/visualization.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 17:34:40.596113 tokenizer-viz-0.2.2/tokenizer_viz.egg-info/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 17:34:40.000000 tokenizer-viz-0.2.2/tokenizer_viz.egg-info/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      267 2023-04-13 17:34:40.000000 tokenizer-viz-0.2.2/tokenizer_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-13 17:34:40.000000 tokenizer-viz-0.2.2/tokenizer_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-13 17:34:40.000000 tokenizer-viz-0.2.2/tokenizer_viz.egg-info/requires.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-13 17:34:40.000000 tokenizer-viz-0.2.2/tokenizer_viz.egg-info/top_level.txt
```

### Comparing `tokenizer-viz-0.2.1/LICENSE` & `tokenizer-viz-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.2.1/PKG-INFO` & `tokenizer-viz-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package to visualize tokenization boundaries using HTML
 Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tokenizer-viz-0.2.1/README.md` & `tokenizer-viz-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.2.1/setup.py` & `tokenizer-viz-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tokenizer-viz",
-    version="0.2.1",
+    version="0.2.2",
     author="Darien Schettler",
     author_email="ds08tf@gmail.com",
     description="A package to visualize tokenization boundaries using HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ds08tf/tokenizer-viz",
     packages=find_packages(),
```

### Comparing `tokenizer-viz-0.2.1/tokenizer_viz/visualization.py` & `tokenizer-viz-0.2.2/tokenizer_viz/visualization.py`

 * *Files 13% similar despite different names*

```diff
@@ -137,34 +137,57 @@
         container_html = f"<div style='background-color: {self.background_color}; line-height: 175%; padding: 25px; " \
                          f"border-radius: 8px; margin-left: 10px; margin-right: 10px; margin-top: 20px; " \
                          f"margin-bottom: 20px; overflow-x: auto; white-space: nowrap;'>"
         container_html += self.generate_tokens(token_lines, strip_padding, pad_token)
         container_html += "</div>"
         return container_html
 
-    def visualize(self, text: str, split_on: str = "\n", display_inline: bool = False,
+    def visualize(self, text: Union[str, list], split_on: str = "\n", display_inline: bool = False,
                   encoder: Optional[Callable] = None, decoder: Optional[Callable] = None,
                   strip_padding: bool = True, pad_token: Union[int, str] = 0) -> str:
         """ Visualizes the given text by generating an HTML string with styled tokens.
 
         Args:
-            text (str): The text to visualize.
+            text (str, list): The text to visualize. (can be a list of tokens or a string)
             split_on (str): The delimiter used to split the text into separate lines (default: newline character).
             display_inline (bool): Whether to display the generated HTML inline using IPython display (default: False).
             encoder (Optional[Callable]): An optional encoder function to override the default encoder (default: None).
             decoder (Optional[Callable]): An optional decoder function to override the default decoder (default: None).
             strip_padding (bool, optional): If True, remove padding tokens from the visualization (default: True).
             pad_token (Union[int, str], optional): The value of the padding token (default: 0).
 
         Returns:
             str: The generated HTML string containing the styled tokens and their container.
         """
 
         _encoder = self.encoder if encoder is None else encoder
         _decoder = self.decoder if decoder is None else decoder
-        token_lines = [_encoder(x + split_on) for x in text.split(split_on)]
+
+        if isinstance(text, str):
+            token_lines = [_encoder(x + split_on) for x in text.split(split_on)]
+        else:
+            token_lines = [_encoder(x + split_on) for x in _decoder(text).split(split_on)]
         html = self.generate_style() + self.generate_container(token_lines, strip_padding, pad_token)
 
         if display_inline:
             display(HTML(html))
 
         return html
+
+    def __call__(self, text: str, split_on: str = "\n", display_inline: bool = False,
+                 encoder: Optional[Callable] = None, decoder: Optional[Callable] = None,
+                 strip_padding: bool = True, pad_token: Union[int, str] = 0) -> str:
+        """ Makes the TokenVisualization instance callable like a function.
+
+        Args:
+            text (str): The text to visualize.
+            split_on (str): The delimiter used to split the text into separate lines (default: newline character).
+            display_inline (bool): Whether to display the generated HTML inline using IPython display (default: False).
+            encoder (Optional[Callable]): An optional encoder function to override the default encoder (default: None).
+            decoder (Optional[Callable]): An optional decoder function to override the default decoder (default: None).
+            strip_padding (bool, optional): If True, remove padding tokens from the visualization (default: True).
+            pad_token (Union[int, str], optional): The value of the padding token (default: 0).
+
+        Returns:
+            str: The generated HTML string containing the styled tokens and their container.
+        """
+        return self.visualize(text, split_on, display_inline, encoder, decoder, strip_padding, pad_token)
```

### Comparing `tokenizer-viz-0.2.1/tokenizer_viz.egg-info/PKG-INFO` & `tokenizer-viz-0.2.2/tokenizer_viz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package to visualize tokenization boundaries using HTML
 Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

