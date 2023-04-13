# Comparing `tmp/PyDesmos-0.1.0.tar.gz` & `tmp/PyDesmos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDesmos-0.1.0.tar", last modified: Thu Apr 13 09:36:35 2023, max compression
+gzip compressed data, was "PyDesmos-0.1.1.tar", last modified: Thu Apr 13 18:58:02 2023, max compression
```

## Comparing `PyDesmos-0.1.0.tar` & `PyDesmos-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:36:35.979521 PyDesmos-0.1.0/
--rw-rw-rw-   0        0        0      188 2023-04-13 09:35:45.000000 PyDesmos-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 09:32:41.000000 PyDesmos-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3530 2023-04-13 09:36:35.978523 PyDesmos-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 09:36:35.959574 PyDesmos-0.1.0/PyDesmos/
--rw-rw-rw-   0        0        0     9189 2023-04-13 09:33:06.000000 PyDesmos-0.1.0/PyDesmos/__init__.py
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.0/PyDesmos/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-13 09:36:35.977526 PyDesmos-0.1.0/PyDesmos.egg-info/
--rw-rw-rw-   0        0        0     3530 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2725 2023-04-13 09:34:37.000000 PyDesmos-0.1.0/README.md
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.0/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-13 09:36:35.979521 PyDesmos-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      869 2023-04-13 09:34:52.000000 PyDesmos-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:58:02.366411 PyDesmos-0.1.1/
+-rw-rw-rw-   0        0        0      306 2023-04-13 18:57:15.000000 PyDesmos-0.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-13 09:32:41.000000 PyDesmos-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3693 2023-04-13 18:58:02.366411 PyDesmos-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 18:58:02.345466 PyDesmos-0.1.1/PyDesmos/
+-rw-rw-rw-   0        0        0     9245 2023-04-13 18:57:37.000000 PyDesmos-0.1.1/PyDesmos/__init__.py
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.1/PyDesmos/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-13 18:58:02.364416 PyDesmos-0.1.1/PyDesmos.egg-info/
+-rw-rw-rw-   0        0        0     3693 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2770 2023-04-13 09:59:00.000000 PyDesmos-0.1.1/README.md
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.1/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:58:02.367408 PyDesmos-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      869 2023-04-13 18:55:12.000000 PyDesmos-0.1.1/setup.py
```

### Comparing `PyDesmos-0.1.0/LICENSE.txt` & `PyDesmos-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.0/PKG-INFO` & `PyDesmos-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy,api
 Classifier: Development Status :: 3 - Alpha
@@ -12,18 +12,18 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 We'll keep it simple. [Desmos](https://www.desmos.com/calculator) is one of the best online calculators.
-Python is one of the best programming language. So why no Python API? Who knows.
+Python is one of the best programming languages. So why no Python API? Who knows.
 What we do know is that PyDesmos is the next best thing.
 
-We've made it as easy as possible to interact with Desmos:
+We've made it as easy as possible to interact with Desmos from python:
 ```python
 from PyDesmos import Graph
 with Graph('my graph') as G:
     f, x = G.f, G.x
     f[x] = x ** 2
 ```
 With just these four lines: _an HTML file called "my graph.html" containing a Desmos graph with the expression "f(x)=x^2" already written, is compiled and then automatically opened in your favorite browser!_
@@ -46,18 +46,19 @@
 G.new_table({x: [0, 1, 2], y: [2, 3, 5]})  # where x, y = G.x, G.y, OR
 G(x=[0, 1, 2], y=[2, 3, 5])
 ```
 
 Plotting python functions:
 ```python
 f = lambda x: int(str(x)[::-1])
-G.plot_function(f, min=0, max=100)
+G.plot_function(f, 0, 100)  # OR
+G(f, min=0, max=100)
 ```
 
-Since Desmos uses latex to generate expressions, all latex-friendly [sympy](https://www.sympy.org/en/index.html) get automatically converted.
+Since Desmos uses latex to generate expressions, all latex-friendly [sympy](https://www.sympy.org/en/index.html) expressions get automatically converted.
 ```python
 import sympy as sp
 with Graph('my graph') as G:
     x, y = G.x, G.y
     G.le(sp.factorial(x + y), sp.sin(x - y))  # appends the expression "(x+y)! <= sin(x-y)"
 ```
 Sliders and greek letter support:
@@ -97,7 +98,12 @@
 - First Release
 
 0.1.0 (12/04/2023)
 -------------------
 - Entered Alpha
 - Major code revisions
 - improved README.md
+
+0.1.1 (13/04/2023)
+-------------------
+- Minor tweaks (mostly to README.md)
+- Fixed optional kwargs with tables
```

### Comparing `PyDesmos-0.1.0/PyDesmos/__init__.py` & `PyDesmos-0.1.1/PyDesmos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import types
 import webbrowser
 from sympy import *
-import itertools as it
 import math
 
 
 desmos_symbols = {chr(i): chr(i) for i in range(65, 91)}
 desmos_symbols.update({chr(i): chr(i) for i in range(97, 123)})
 desmos_symbols.update({
     'alpha': r'\alpha',
@@ -142,19 +141,22 @@
         self.define(lhs, rhs, r'\ge ', **kwargs)
 
     def new_slider(self, symbol, initial_value=1, min=-10, max=10, step='""', **kwargs):
         kwargs.update({'sliderBounds': {'min': to_latex(min), 'max': to_latex(max), 'step': to_latex(step)}})
         self.define(symbol, initial_value, **kwargs)
 
     def new_table(self, columns, **kwargs):
-        kwargs.update({'type': 'table', 'columns': [
-            {'latex': to_latex(latex), 'values': [to_latex(x) for x in values]} if values else
-            {'latex': to_latex(latex)} for latex, values in columns.items()
-        ]})
-        self.set_expression(**kwargs)
+        new_columns = []
+        for latex, values in columns.items():
+            column = {'latex': to_latex(latex)}
+            if values:
+                column['values'] = [to_latex(x) for x in values]
+            column.update(kwargs)
+            new_columns.append(column)
+        self.set_expression(**{'type': 'table', 'columns': new_columns})
 
     def save(self):
         with open(self.file_name, 'w') as html_file:
             html_file.write(self.html + '</script>')
 
     def open(self):
         self.save()
@@ -198,8 +200,8 @@
     def plot_function(self, function, min, max, step=1, independent_variable='x', dependent_variable='y', **kwargs):
         N = math.ceil((max - min) / step)
         X = [min + step * n for n in range(int(N))]
         Y = [function(x) for x in X]
         self.new_table({independent_variable: X, dependent_variable: Y}, **kwargs)
 
     def __or__(self, other):
-        self.__call__(other)
+        self.__call__(other)
```

### Comparing `PyDesmos-0.1.0/PyDesmos/logo.png` & `PyDesmos-0.1.1/PyDesmos/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.0/PyDesmos.egg-info/PKG-INFO` & `PyDesmos-0.1.1/PyDesmos.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy,api
 Classifier: Development Status :: 3 - Alpha
@@ -12,18 +12,18 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 We'll keep it simple. [Desmos](https://www.desmos.com/calculator) is one of the best online calculators.
-Python is one of the best programming language. So why no Python API? Who knows.
+Python is one of the best programming languages. So why no Python API? Who knows.
 What we do know is that PyDesmos is the next best thing.
 
-We've made it as easy as possible to interact with Desmos:
+We've made it as easy as possible to interact with Desmos from python:
 ```python
 from PyDesmos import Graph
 with Graph('my graph') as G:
     f, x = G.f, G.x
     f[x] = x ** 2
 ```
 With just these four lines: _an HTML file called "my graph.html" containing a Desmos graph with the expression "f(x)=x^2" already written, is compiled and then automatically opened in your favorite browser!_
@@ -46,18 +46,19 @@
 G.new_table({x: [0, 1, 2], y: [2, 3, 5]})  # where x, y = G.x, G.y, OR
 G(x=[0, 1, 2], y=[2, 3, 5])
 ```
 
 Plotting python functions:
 ```python
 f = lambda x: int(str(x)[::-1])
-G.plot_function(f, min=0, max=100)
+G.plot_function(f, 0, 100)  # OR
+G(f, min=0, max=100)
 ```
 
-Since Desmos uses latex to generate expressions, all latex-friendly [sympy](https://www.sympy.org/en/index.html) get automatically converted.
+Since Desmos uses latex to generate expressions, all latex-friendly [sympy](https://www.sympy.org/en/index.html) expressions get automatically converted.
 ```python
 import sympy as sp
 with Graph('my graph') as G:
     x, y = G.x, G.y
     G.le(sp.factorial(x + y), sp.sin(x - y))  # appends the expression "(x+y)! <= sin(x-y)"
 ```
 Sliders and greek letter support:
@@ -97,7 +98,12 @@
 - First Release
 
 0.1.0 (12/04/2023)
 -------------------
 - Entered Alpha
 - Major code revisions
 - improved README.md
+
+0.1.1 (13/04/2023)
+-------------------
+- Minor tweaks (mostly to README.md)
+- Fixed optional kwargs with tables
```

### Comparing `PyDesmos-0.1.0/README.md` & `PyDesmos-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 We'll keep it simple. [Desmos](https://www.desmos.com/calculator) is one of the best online calculators.
-Python is one of the best programming language. So why no Python API? Who knows.
+Python is one of the best programming languages. So why no Python API? Who knows.
 What we do know is that PyDesmos is the next best thing.
 
-We've made it as easy as possible to interact with Desmos:
+We've made it as easy as possible to interact with Desmos from python:
 ```python
 from PyDesmos import Graph
 with Graph('my graph') as G:
     f, x = G.f, G.x
     f[x] = x ** 2
 ```
 With just these four lines: _an HTML file called "my graph.html" containing a Desmos graph with the expression "f(x)=x^2" already written, is compiled and then automatically opened in your favorite browser!_
@@ -29,18 +29,19 @@
 G.new_table({x: [0, 1, 2], y: [2, 3, 5]})  # where x, y = G.x, G.y, OR
 G(x=[0, 1, 2], y=[2, 3, 5])
 ```
 
 Plotting python functions:
 ```python
 f = lambda x: int(str(x)[::-1])
-G.plot_function(f, min=0, max=100)
+G.plot_function(f, 0, 100)  # OR
+G(f, min=0, max=100)
 ```
 
-Since Desmos uses latex to generate expressions, all latex-friendly [sympy](https://www.sympy.org/en/index.html) get automatically converted.
+Since Desmos uses latex to generate expressions, all latex-friendly [sympy](https://www.sympy.org/en/index.html) expressions get automatically converted.
 ```python
 import sympy as sp
 with Graph('my graph') as G:
     x, y = G.x, G.y
     G.le(sp.factorial(x + y), sp.sin(x - y))  # appends the expression "(x+y)! <= sin(x-y)"
 ```
 Sliders and greek letter support:
```

### Comparing `PyDesmos-0.1.0/logo.png` & `PyDesmos-0.1.1/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.0/setup.py` & `PyDesmos-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='PyDesmos',
-    version='0.1.0',
+    version='0.1.1',
     description='An easy-to-use Python to Desmos graph HTML compiler via the Desmos API.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
```

