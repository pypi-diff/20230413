# Comparing `tmp/tokenizer-viz-0.2.0.tar.gz` & `tmp/tokenizer-viz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizer-viz-0.2.0.tar", last modified: Thu Apr 13 12:57:49 2023, max compression
+gzip compressed data, was "tokenizer-viz-0.2.1.tar", last modified: Thu Apr 13 13:14:38 2023, max compression
```

## Comparing `tokenizer-viz-0.2.0.tar` & `tokenizer-viz-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 12:57:49.380427 tokenizer-viz-0.2.0/
--rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.2.0/LICENSE
--rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 12:57:49.380325 tokenizer-viz-0.2.0/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)     2148 2023-04-13 12:57:10.000000 tokenizer-viz-0.2.0/README.md
--rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-13 12:57:49.380464 tokenizer-viz-0.2.0/setup.cfg
--rw-r--r--   0 darienschettler   (501) staff       (20)      959 2023-04-13 12:40:42.000000 tokenizer-viz-0.2.0/setup.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 12:57:49.379491 tokenizer-viz-0.2.0/tokenizer_viz/
--rw-r--r--   0 darienschettler   (501) staff       (20)       46 2023-04-13 12:36:19.000000 tokenizer-viz-0.2.0/tokenizer_viz/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     7474 2023-04-13 12:56:37.000000 tokenizer-viz-0.2.0/tokenizer_viz/visualization.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 12:57:49.380165 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/
--rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      267 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/SOURCES.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/dependency_links.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/requires.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-13 12:57:49.000000 tokenizer-viz-0.2.0/tokenizer_viz.egg-info/top_level.txt
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 13:14:38.713411 tokenizer-viz-0.2.1/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.2.1/LICENSE
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 13:14:38.713305 tokenizer-viz-0.2.1/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2148 2023-04-13 12:57:10.000000 tokenizer-viz-0.2.1/README.md
+-rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-13 13:14:38.713452 tokenizer-viz-0.2.1/setup.cfg
+-rw-r--r--   0 darienschettler   (501) staff       (20)      959 2023-04-13 13:14:35.000000 tokenizer-viz-0.2.1/setup.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 13:14:38.712458 tokenizer-viz-0.2.1/tokenizer_viz/
+-rw-r--r--   0 darienschettler   (501) staff       (20)       46 2023-04-13 12:36:19.000000 tokenizer-viz-0.2.1/tokenizer_viz/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     8501 2023-04-13 13:14:15.000000 tokenizer-viz-0.2.1/tokenizer_viz/visualization.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-13 13:14:38.713128 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2803 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      267 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/requires.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-13 13:14:38.000000 tokenizer-viz-0.2.1/tokenizer_viz.egg-info/top_level.txt
```

### Comparing `tokenizer-viz-0.2.0/LICENSE` & `tokenizer-viz-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.2.0/PKG-INFO` & `tokenizer-viz-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package to visualize tokenization boundaries using HTML
 Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tokenizer-viz-0.2.0/README.md` & `tokenizer-viz-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.2.0/setup.py` & `tokenizer-viz-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tokenizer-viz",
-    version="0.2.0",
+    version="0.2.1",
     author="Darien Schettler",
     author_email="ds08tf@gmail.com",
     description="A package to visualize tokenization boundaries using HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ds08tf/tokenizer-viz",
     packages=find_packages(),
```

### Comparing `tokenizer-viz-0.2.0/tokenizer_viz/visualization.py` & `tokenizer-viz-0.2.1/tokenizer_viz/visualization.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,66 +90,81 @@
             str: A CSS style string for token elements.
         """
         style = f"<style>span.token {{font-family: {self.font_family}; font-size: {self.font_size}; " \
                 f"font-weight: {self.font_weight}; padding: {self.padding}; margin-right: {self.margin_right}; " \
                 f"border-color: rgba(0, 0, 0, 0.05); border-style: ridge; border-radius: {self.border_radius};}}</style>"
         return style
 
-    def generate_tokens(self, token_lines: List[List[str]]) -> str:
+    def generate_tokens(self, token_lines: List[List[str]], strip_padding: bool, pad_token: Union[int, str] = 0) -> str:
         """ Generates an HTML string containing the decoded token strings with their styles.
 
         Args:
             token_lines (List[List[str]]): A list of lists of tokens to generate HTML for.
+            strip_padding (bool): If True, remove padding tokens from the visualization.
+            pad_token (Union[int, str], optional): The value of the padding token (default: 0).
 
         Returns:
             str: An HTML string containing the styled tokens.
         """
         tokens_html = ""
         for token_line in token_lines:
             for i, token in enumerate(token_line):
+                if strip_padding and token == pad_token:
+                    continue
+
                 color = self.get_color(i)
                 try:
                     tokens_html += f"<span class='token' style='{color}'>{self.decoder(token).replace(' ', '&nbsp;')}</span>".replace(
                         '\t', '\\t').replace('\n', '\\n').replace('\r', '\\r').replace('\f', '\\f').replace('\v', '\\v')
                 except TypeError:
                     tokens_html += f"<span class='token' style='{color}'>{self.unk_token}</span>"
             tokens_html = self.replace_rightmost_newline(tokens_html)
         return tokens_html
 
-    def generate_container(self, token_lines: List[List[str]]) -> str:
+    def generate_container(self,
+                           token_lines: List[List[str]],
+                           strip_padding: bool,
+                           pad_token: Union[int, str] = 0) -> str:
         """ Generates an HTML container string with the specified token_lines.
 
         Args:
             token_lines (List[List[str]]): A list of lists of tokens to generate the container for.
+            strip_padding (bool): If True, remove padding tokens from the visualization.
+            pad_token (Union[int, str], optional): The value of the padding token (default: 0).
 
         Returns:
             str: An HTML container string containing the token_lines.
         """
-        container_html = f"<div style='background-color: {self.background_color}; line-height: 175%; padding: 25px; border-radius: 8px; margin-left: 10px; margin-right: 10px; margin-top: 20px; margin-bottom: 20px; overflow-x: auto; white-space: nowrap;'>"
-        container_html += self.generate_tokens(token_lines)
+        container_html = f"<div style='background-color: {self.background_color}; line-height: 175%; padding: 25px; " \
+                         f"border-radius: 8px; margin-left: 10px; margin-right: 10px; margin-top: 20px; " \
+                         f"margin-bottom: 20px; overflow-x: auto; white-space: nowrap;'>"
+        container_html += self.generate_tokens(token_lines, strip_padding, pad_token)
         container_html += "</div>"
         return container_html
 
     def visualize(self, text: str, split_on: str = "\n", display_inline: bool = False,
-                  encoder: Optional[Callable] = None, decoder: Optional[Callable] = None) -> str:
+                  encoder: Optional[Callable] = None, decoder: Optional[Callable] = None,
+                  strip_padding: bool = True, pad_token: Union[int, str] = 0) -> str:
         """ Visualizes the given text by generating an HTML string with styled tokens.
 
         Args:
             text (str): The text to visualize.
-            split_on (str, optional): The delimiter used to split the text into separate lines (default: newline character).
-            display_inline (bool, optional): Whether to display the generated HTML inline using IPython display (default: False).
+            split_on (str): The delimiter used to split the text into separate lines (default: newline character).
+            display_inline (bool): Whether to display the generated HTML inline using IPython display (default: False).
             encoder (Optional[Callable]): An optional encoder function to override the default encoder (default: None).
             decoder (Optional[Callable]): An optional decoder function to override the default decoder (default: None).
+            strip_padding (bool, optional): If True, remove padding tokens from the visualization (default: True).
+            pad_token (Union[int, str], optional): The value of the padding token (default: 0).
 
         Returns:
             str: The generated HTML string containing the styled tokens and their container.
         """
 
         _encoder = self.encoder if encoder is None else encoder
         _decoder = self.decoder if decoder is None else decoder
         token_lines = [_encoder(x + split_on) for x in text.split(split_on)]
-        html = self.generate_style() + self.generate_container(token_lines)
+        html = self.generate_style() + self.generate_container(token_lines, strip_padding, pad_token)
 
         if display_inline:
             display(HTML(html))
 
         return html
```

### Comparing `tokenizer-viz-0.2.0/tokenizer_viz.egg-info/PKG-INFO` & `tokenizer-viz-0.2.1/tokenizer_viz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package to visualize tokenization boundaries using HTML
 Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

