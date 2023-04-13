# Comparing `tmp/watchtower_browser_testing-0.3.2.tar.gz` & `tmp/watchtower_browser_testing-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.2.tar", last modified: Thu Apr 13 18:07:52 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.3.tar", last modified: Thu Apr 13 18:29:17 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.2.tar` & `watchtower_browser_testing-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:07:52.274027 watchtower_browser_testing-0.3.2/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:07:52.258430 watchtower_browser_testing-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 18:07:52.274943 watchtower_browser_testing-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:07:52.258430 watchtower_browser_testing-0.3.2/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      677 2023-04-13 12:22:31.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1503 2023-04-13 18:01:14.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/helpers.py
--rw-rw-rw-   0        0        0    13936 2023-04-13 18:07:40.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 18:07:49.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:07:52.258430 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:29:17.249379 watchtower_browser_testing-0.3.3/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:29:17.233737 watchtower_browser_testing-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:29:17.249379 watchtower_browser_testing-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:29:17.233737 watchtower_browser_testing-0.3.3/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/helpers.py
+-rw-rw-rw-   0        0        0    14194 2023-04-13 18:29:02.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 18:29:02.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:29:17.233737 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.2/setup.py` & `watchtower_browser_testing-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.2/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.3.3/watchtower_browser_testing/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import json
 from marko.ext.gfm import gfm as markdown
 
+
 def trim(docstring):
     if not docstring:
         return ''
     # Convert tabs to spaces (following the normal Python rules)
     # and split into a list of lines:
     lines = docstring.expandtabs().splitlines()
     # Determine minimum indentation (first line doesn't count):
@@ -23,23 +24,25 @@
     while trimmed and not trimmed[-1]:
         trimmed.pop()
     while trimmed and not trimmed[0]:
         trimmed.pop(0)
     # Return a single string:
     return '\n'.join(trimmed)
 
+
 def build_html(structure):
 
     html = f'<div class="{structure["type"]}" id="{structure["id"]}">'
     html += markdown.render(structure.get('description') or '')
     if 'children' in structure and structure['children']:
         for child_structure in structure['children']:
             html += build_html(child_structure)
     html += '</div>'
     return html
 
+
 class ExtendedEncoder(json.JSONEncoder):
 
     def default(self, obj):
         if callable(obj):
             return obj.__name__
         return super().default(obj)
```

### Comparing `watchtower_browser_testing-0.3.2/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.3.3/watchtower_browser_testing/testsuite.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 import types
 import functools
 import json
 
 from playwright.sync_api import sync_playwright
 from marko.ext.gfm import gfm as markdown
+import jinja2
 
 from watchtower_browser_testing.tracking_validation import EventQueue, RequestValidator, Validator
 from watchtower_browser_testing import exceptions
 from watchtower_browser_testing import config
 from watchtower_browser_testing import helpers
 
 
@@ -383,14 +384,19 @@
 
         for test in tests:
             structure['children'].append(test['class'].md_description(parent=name))
 
 
         return structure
 
-    def html_description(self):
+    def html_report(self, title='Measurement Plan'):
+
+        jenv = jinja2.Environment(loader=jinja2.FileSystemLoader(config.TEMPLATES_PATH))
+        template = jenv.get_template('measurement_plan.html')
 
         structure = self.md_description()
-        return helpers.build_html(structure)
+        content = helpers.build_html(structure)
+
+        return template.render(title=title, content=content)
```

### Comparing `watchtower_browser_testing-0.3.2/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.3/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

