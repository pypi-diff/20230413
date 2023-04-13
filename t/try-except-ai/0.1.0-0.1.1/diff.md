# Comparing `tmp/try-except-ai-0.1.0.tar.gz` & `tmp/try-except-ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "try-except-ai-0.1.0.tar", max compression
+gzip compressed data, was "try-except-ai-0.1.1.tar", max compression
```

## Comparing `try-except-ai-0.1.0.tar` & `try-except-ai-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      607 2023-04-13 19:45:09.178985 try-except-ai-0.1.0/README.md
--rw-r--r--   0        0        0      978 2023-04-13 19:56:53.829570 try-except-ai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 19:49:16.537862 try-except-ai-0.1.0/try_except_ai/__init__.py
--rw-r--r--   0        0        0     2153 2023-04-13 19:39:07.828199 try-except-ai-0.1.0/try_except_ai/try_except_ai.py
--rw-r--r--   0        0        0     1350 2023-04-13 19:57:04.253835 try-except-ai-0.1.0/setup.py
--rw-r--r--   0        0        0     1518 2023-04-13 19:57:04.253973 try-except-ai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-04-13 20:00:37.752325 try-except-ai-0.1.1/README.md
+-rw-r--r--   0        0        0      978 2023-04-13 20:04:34.839289 try-except-ai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-04-13 20:03:54.418576 try-except-ai-0.1.1/try_except_ai/__init__.py
+-rw-r--r--   0        0        0     2153 2023-04-13 19:39:07.828199 try-except-ai-0.1.1/try_except_ai/try_except_ai.py
+-rw-r--r--   0        0        0     1481 2023-04-13 20:07:04.327182 try-except-ai-0.1.1/setup.py
+-rw-r--r--   0        0        0     1645 2023-04-13 20:07:04.327317 try-except-ai-0.1.1/PKG-INFO
```

### Comparing `try-except-ai-0.1.0/pyproject.toml` & `try-except-ai-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "try-except-ai"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package to handle exceptions and suggest resolutions using OpenAI"
 authors = ["Federico Ulfo <federicoulfo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/etnalab/try-except-ai"
 repository = "https://github.com/etnalab/try-except-ai"
 documentation = ""
```

### Comparing `try-except-ai-0.1.0/try_except_ai/try_except_ai.py` & `try-except-ai-0.1.1/try_except_ai/try_except_ai.py`

 * *Files identical despite different names*

### Comparing `try-except-ai-0.1.0/setup.py` & `try-except-ai-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.4,<0.28.0']
 
 setup_kwargs = {
     'name': 'try-except-ai',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A Python package to handle exceptions and suggest resolutions using OpenAI',
-    'long_description': '# TryExceptAI\n\nA Python package to handle exceptions and suggest resolutions using OpenAI.\n\n## Installation\n\nInstall the package using [Poetry](https://python-poetry.org/):\n\n```bash\npoetry add try-except-ai\n```\n\n## Usage\n```python\nfrom try_except_ai import TryExceptAI\n\ndef test_function():\n    try:\n        # Code that might raise an exception\n        result = 1 / 0\n        print(result)\n    except Exception as e:\n        TryExceptAI().handle_exception(e)\n\nif __name__ == "__main__":\n    test_function()\n\n```\n\n## License\nThis project is licensed under the MIT License. See the LICENSE file for details.\n\n',
+    'long_description': '# TryExceptAI\n\nA Python package to handle exceptions and suggest resolutions using OpenAI.\n\n## Installation\n\nInstall the package using [Poetry](https://python-poetry.org/):\n\n```bash\npoetry add try-except-ai\n```\n\n## Usage\nAdd `export OPENAI_API_KEY={your openai api key here}` to your .zshrc or .bash_profile file.\n\nThen test it with the following\n\n```python\nfrom try_except_ai import TryExceptAI\n\ndef test_function():\n    try:\n        # Code that might raise an exception\n        result = 1 / 0\n        print(result)\n    except Exception as e:\n        TryExceptAI().handle_exception(e)\n\nif __name__ == "__main__":\n    test_function()\n\n```\n\n## License\nThis project is licensed under the MIT License. See the LICENSE file for details.\n\n',
     'author': 'Federico Ulfo',
     'author_email': 'federicoulfo@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/etnalab/try-except-ai',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `try-except-ai-0.1.0/PKG-INFO` & `try-except-ai-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: try-except-ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to handle exceptions and suggest resolutions using OpenAI
 Home-page: https://github.com/etnalab/try-except-ai
 License: MIT
 Keywords: openai,exceptions,ai
 Author: Federico Ulfo
 Author-email: federicoulfo@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -30,14 +30,18 @@
 Install the package using [Poetry](https://python-poetry.org/):
 
 ```bash
 poetry add try-except-ai
 ```
 
 ## Usage
+Add `export OPENAI_API_KEY={your openai api key here}` to your .zshrc or .bash_profile file.
+
+Then test it with the following
+
 ```python
 from try_except_ai import TryExceptAI
 
 def test_function():
     try:
         # Code that might raise an exception
         result = 1 / 0
```

