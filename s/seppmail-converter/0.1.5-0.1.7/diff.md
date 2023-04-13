# Comparing `tmp/seppmail-converter-0.1.5.tar.gz` & `tmp/seppmail_converter-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail-converter-0.1.5.tar", max compression
+gzip compressed data, was "seppmail_converter-0.1.7.tar", max compression
```

## Comparing `seppmail-converter-0.1.5.tar` & `seppmail_converter-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,7 @@
--rw-r--r--   0        0        0     1056 2022-11-30 17:34:50.297561 seppmail-converter-0.1.5/README.md
--rw-r--r--   0        0        0      591 2022-11-30 17:36:16.969291 seppmail-converter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2022-11-30 17:36:05.603826 seppmail-converter-0.1.5/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      178 2022-11-30 15:33:41.880575 seppmail-converter-0.1.5/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     2050 2022-11-30 17:35:44.602299 seppmail-converter-0.1.5/seppmail_converter/main.py
--rw-r--r--   0        0        0     3426 2022-11-30 17:05:43.679914 seppmail-converter-0.1.5/seppmail_converter/seppmail.py
--rw-r--r--   0        0        0     1476 2022-11-30 17:06:43.094125 seppmail-converter-0.1.5/seppmail_converter/server.py
--rw-r--r--   0        0        0     2394 2022-11-30 17:32:34.932187 seppmail-converter-0.1.5/seppmail_converter/templates/index.html
--rw-r--r--   0        0        0     2064 2022-11-30 17:36:44.505933 seppmail-converter-0.1.5/setup.py
--rw-r--r--   0        0        0     1752 2022-11-30 17:36:44.506085 seppmail-converter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      883 2023-04-13 20:56:58.210024 seppmail_converter-0.1.7/README.md
+-rw-r--r--   0        0        0      543 2023-04-13 20:55:01.641998 seppmail_converter-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-13 20:55:01.643417 seppmail_converter-0.1.7/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-13 20:35:22.726388 seppmail_converter-0.1.7/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     4113 2023-04-13 20:56:23.716858 seppmail_converter-0.1.7/seppmail_converter/main.py
+-rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 seppmail_converter-0.1.7/setup.py
+-rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 seppmail_converter-0.1.7/PKG-INFO
```

### Comparing `seppmail-converter-0.1.5/README.md` & `seppmail_converter-0.1.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,26 @@
 # SEPPMail Converter
 
 This python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.
 
 ## Usage
 
 ```
-Usage: main.py [OPTIONS] COMMAND [ARGS]...
+Usage: seppmail-converter [OPTIONS] INPUT_FILE
 
 Options:
-  --help  Show this message and exit.
-
-Commands:
-  convert*
-  serve 
-```
-
-### Convert
-
-Convert an encrypted email file to a `.eml` file.
-
-```
-Usage: main.py convert [OPTIONS] INPUT_FILE
-
-Options:
-  -o, --output PATH
   -u, --username TEXT
   -p, --password TEXT
+  -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
-  --help               Show this message and exit.
-```
-
-### Serve
-
-Start a web server to convert encrypted email files to `.eml` files via a web interface.
-
+  -o, --overwrite      Overwrite output file if it exists
+  -q, --quiet          Suppress all output except final path
+  --help               Show this message and exit. 
+ ```
 
 Relevant environment variables:
 
 | Name | Description |
 | ---- | ----------- |
 | `SEPPMAIL_USERNAME` | Email supplied during login |
 | `SEPPMAIL_PASSWORD` | Password supplied during login|
```

### Comparing `seppmail-converter-0.1.5/pyproject.toml` & `seppmail_converter-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [tool.poetry]
 name = "seppmail-converter"
-version = "0.1.5"
+version = "0.1.7"
 description = "Decode SEPPMail emails into EML files"
 license = "MIT"
 authors = ["Daniel Malik <daniel.malik@mhsp.solutions>"]
 readme = "README.md"
 classifiers = ["Environment :: Console"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.1"
 click = "^8.1.3"
 beautifulsoup4 = "^4.11.1"
 lxml = "^4.9.1"
-Flask = "^2.2.2"
-click-default-group = "^1.2.2"
 
 [tool.poetry.scripts]
 seppmail-converter = 'seppmail_converter.main:entry'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seppmail-converter-0.1.5/setup.py` & `seppmail_converter-0.1.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['seppmail_converter']
 
 package_data = \
-{'': ['*'], 'seppmail_converter': ['templates/*']}
+{'': ['*']}
 
 install_requires = \
-['Flask>=2.2.2,<3.0.0',
- 'beautifulsoup4>=4.11.1,<5.0.0',
- 'click-default-group>=1.2.2,<2.0.0',
+['beautifulsoup4>=4.11.1,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'lxml>=4.9.1,<5.0.0',
  'requests>=2.28.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['seppmail-converter = seppmail_converter.main:entry']}
 
 setup_kwargs = {
     'name': 'seppmail-converter',
-    'version': '0.1.5',
+    'version': '0.1.7',
     'description': 'Decode SEPPMail emails into EML files',
-    'long_description': '# SEPPMail Converter\n\nThis python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.\n\n## Usage\n\n```\nUsage: main.py [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  convert*\n  serve \n```\n\n### Convert\n\nConvert an encrypted email file to a `.eml` file.\n\n```\nUsage: main.py convert [OPTIONS] INPUT_FILE\n\nOptions:\n  -o, --output PATH\n  -u, --username TEXT\n  -p, --password TEXT\n  -f, --force          Skip SEPPMail input file validation\n  -d, --delete         Delete input file after conversion\n  --help               Show this message and exit.\n```\n\n### Serve\n\nStart a web server to convert encrypted email files to `.eml` files via a web interface.\n\n\nRelevant environment variables:\n\n| Name | Description |\n| ---- | ----------- |\n| `SEPPMAIL_USERNAME` | Email supplied during login |\n| `SEPPMAIL_PASSWORD` | Password supplied during login|\n\nUnless specified, the script will place the output file next to the input file and name it after the original file.\n',
+    'long_description': '# SEPPMail Converter\n\nThis python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.\n\n## Usage\n\n```\nUsage: seppmail-converter [OPTIONS] INPUT_FILE\n\nOptions:\n  -u, --username TEXT\n  -p, --password TEXT\n  -o, --output PATH\n  -f, --force          Skip SEPPMail input file validation\n  -d, --delete         Delete input file after conversion\n  -o, --overwrite      Overwrite output file if it exists\n  -q, --quiet          Suppress all output except final path\n  --help               Show this message and exit. \n ```\n\nRelevant environment variables:\n\n| Name | Description |\n| ---- | ----------- |\n| `SEPPMAIL_USERNAME` | Email supplied during login |\n| `SEPPMAIL_PASSWORD` | Password supplied during login|\n\nUnless specified, the script will place the output file next to the input file and name it after the original file.\n',
     'author': 'Daniel Malik',
     'author_email': 'daniel.malik@mhsp.solutions',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `seppmail-converter-0.1.5/PKG-INFO` & `seppmail_converter-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,45 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 0.1.5
+Version: 0.1.7
 Summary: Decode SEPPMail emails into EML files
 License: MIT
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Flask (>=2.2.2,<3.0.0)
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # SEPPMail Converter
 
 This python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.
 
 ## Usage
 
 ```
-Usage: main.py [OPTIONS] COMMAND [ARGS]...
+Usage: seppmail-converter [OPTIONS] INPUT_FILE
 
 Options:
-  --help  Show this message and exit.
-
-Commands:
-  convert*
-  serve 
-```
-
-### Convert
-
-Convert an encrypted email file to a `.eml` file.
-
-```
-Usage: main.py convert [OPTIONS] INPUT_FILE
-
-Options:
-  -o, --output PATH
   -u, --username TEXT
   -p, --password TEXT
+  -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
-  --help               Show this message and exit.
-```
-
-### Serve
-
-Start a web server to convert encrypted email files to `.eml` files via a web interface.
-
+  -o, --overwrite      Overwrite output file if it exists
+  -q, --quiet          Suppress all output except final path
+  --help               Show this message and exit. 
+ ```
 
 Relevant environment variables:
 
 | Name | Description |
 | ---- | ----------- |
 | `SEPPMAIL_USERNAME` | Email supplied during login |
 | `SEPPMAIL_PASSWORD` | Password supplied during login|
```

