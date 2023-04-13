# Comparing `tmp/dw_content_tools-0.5.0.tar.gz` & `tmp/dw_content_tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dw_content_tools-0.5.0.tar", max compression
+gzip compressed data, was "dw_content_tools-0.6.0.tar", max compression
```

## Comparing `dw_content_tools-0.5.0.tar` & `dw_content_tools-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1086 2023-01-03 19:36:31.240150 dw_content_tools-0.5.0/README.md
--rw-r--r--   0        0        0        0 2022-12-30 17:50:27.896885 dw_content_tools-0.5.0/content_tools/__init__.py
--rw-r--r--   0        0        0     6860 2023-01-25 17:02:11.842604 dw_content_tools-0.5.0/content_tools/__main__.py
--rw-r--r--   0        0        0     1475 2023-01-20 14:20:56.213727 dw_content_tools-0.5.0/content_tools/json_schemas.py
--rw-r--r--   0        0        0      572 2023-01-25 17:02:19.015644 dw_content_tools-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 dw_content_tools-0.5.0/setup.py
--rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 dw_content_tools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-01-03 19:36:31.240150 dw_content_tools-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-30 17:50:27.896885 dw_content_tools-0.6.0/content_tools/__init__.py
+-rw-r--r--   0        0        0     6860 2023-04-13 15:01:53.747805 dw_content_tools-0.6.0/content_tools/__main__.py
+-rw-r--r--   0        0        0     1545 2023-04-13 15:01:00.327531 dw_content_tools-0.6.0/content_tools/json_schemas.py
+-rw-r--r--   0        0        0      572 2023-04-13 15:02:02.416711 dw_content_tools-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 dw_content_tools-0.6.0/setup.py
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 dw_content_tools-0.6.0/PKG-INFO
```

### Comparing `dw_content_tools-0.5.0/README.md` & `dw_content_tools-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dw_content_tools-0.5.0/content_tools/__main__.py` & `dw_content_tools-0.6.0/content_tools/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         "english.md": __validate_english_md,
     }
     validator_callable = mapping[file]
     validator_callable(path, file)
 
 
 @click.group()
-@click.version_option("0.5.0")
+@click.version_option("0.6.0")
 def content_tools():
     pass
 
 
 @content_tools.command()
 @click.argument(
     "path",
```

### Comparing `dw_content_tools-0.5.0/content_tools/json_schemas.py` & `dw_content_tools-0.6.0/content_tools/json_schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         },
         "environment": {
             "type": "array",
             "minItems": 0,
             "items": {"type": "string"},
         },
         "command": {"type": "string"},
+        "cpu": {"type": "number"},
+        "ram": {"type": "string"},
         "x-views": {
             "type": "array",
             "items": {
                 "type": "object",
                 "additionalProperties": False,
                 "required": ["name", "url", "port"],
                 "properties": {
```

### Comparing `dw_content_tools-0.5.0/pyproject.toml` & `dw_content_tools-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dw-content-tools"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Martin Zugnoni <mzugnoni@datawars.io>"]
 readme = "README.md"
 packages = [{include = "content_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dw_content_tools-0.5.0/setup.py` & `dw_content_tools-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pyyaml>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['content_tools = content_tools.__main__:content_tools']}
 
 setup_kwargs = {
     'name': 'dw-content-tools',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': '',
     'long_description': '# Content CLI Tools\n\n## Installation\n\n```\n$ pip3 install dw-content-tools\n```\n\n## Module Repository Validator\n\n```\nValidates that a module repo structure and content is valid, based\non the following rules:\n\n* metadata.yml exists\n* metadata.yml is valid\n    * validate JSON schema\n* docker-compose.yml exists\n* docker-compose.yml is valid\n    * validate JSON schema\n* english.md exists\n* validating english.md:\n    * pages:\n        * unique IDs\n        * all pages contain a valid ID\n        * all pages have a name\n    * all images referenced in md exist as static files\n    * activities:\n        * all activities have an unique `id`\n        * all activities have `type` defined\n        * input:\n            * has required `correct-answer` tag\n        * multiple-choice:\n            * has required `answer` (many) tags\n            * at least one answer is marked as `is-correct`\n            * when more than one answer is correct, `widget` has to be `checkbox`\n        * code:\n            * `template` and `device` attrs are defined\n            * has required `validation-code` tag\n```\n',
     'author': 'Martin Zugnoni',
     'author_email': 'mzugnoni@datawars.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dw_content_tools-0.5.0/PKG-INFO` & `dw_content_tools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dw-content-tools
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Martin Zugnoni
 Author-email: mzugnoni@datawars.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

