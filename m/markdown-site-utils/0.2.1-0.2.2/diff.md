# Comparing `tmp/markdown_site_utils-0.2.1.tar.gz` & `tmp/markdown_site_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_site_utils-0.2.1.tar", max compression
+gzip compressed data, was "markdown_site_utils-0.2.2.tar", max compression
```

## Comparing `markdown_site_utils-0.2.1.tar` & `markdown_site_utils-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      550 2023-04-13 16:30:59.407240 markdown_site_utils-0.2.1/LICENSE
--rw-r--r--   0        0        0     1487 2023-04-13 16:45:57.957775 markdown_site_utils-0.2.1/README.md
--rw-r--r--   0        0        0       60 2023-04-13 16:04:59.007737 markdown_site_utils-0.2.1/mdsite/__init__.py
--rw-r--r--   0        0        0     5041 2023-04-13 16:28:04.313550 markdown_site_utils-0.2.1/mdsite/data.py
--rw-r--r--   0        0        0     2399 2023-04-13 16:28:08.209528 markdown_site_utils-0.2.1/mdsite/data_test.py
--rw-r--r--   0        0        0       22 2018-02-14 20:54:21.973447 markdown_site_utils-0.2.1/mdsite/testdata/config.toml
--rw-r--r--   0        0        0       14 2018-02-14 20:54:21.974283 markdown_site_utils-0.2.1/mdsite/testdata/conflict/index.md
--rw-r--r--   0        0        0        8 2018-02-14 20:54:21.973730 markdown_site_utils-0.2.1/mdsite/testdata/conflict.md
--rw-r--r--   0        0        0      160 2018-02-14 20:54:21.974602 markdown_site_utils-0.2.1/mdsite/testdata/json.md
--rw-r--r--   0        0        0       56 2023-04-13 15:56:34.040771 markdown_site_utils-0.2.1/mdsite/testdata/nohead.md
--rw-r--r--   0        0        0       29 2018-02-14 20:54:21.974977 markdown_site_utils-0.2.1/mdsite/testdata/nougat/config.json
--rw-r--r--   0        0        0      576 2020-01-26 16:09:19.091737 markdown_site_utils-0.2.1/mdsite/testdata/toml.md
--rw-r--r--   0        0        0      245 2018-02-14 20:54:21.975578 markdown_site_utils-0.2.1/mdsite/testdata/yaml.md
--rw-r--r--   0        0        0      709 2023-04-13 16:40:27.913220 markdown_site_utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 markdown_site_utils-0.2.1/setup.py
--rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 markdown_site_utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-04-13 16:48:59.731027 markdown_site_utils-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1487 2023-04-13 16:49:03.686324 markdown_site_utils-0.2.2/README.md
+-rw-r--r--   0        0        0       60 2023-04-13 17:49:28.439090 markdown_site_utils-0.2.2/mdsite/__init__.py
+-rw-r--r--   0        0        0     4897 2023-04-13 17:47:40.360731 markdown_site_utils-0.2.2/mdsite/data.py
+-rw-r--r--   0        0        0     2400 2023-04-13 17:47:57.272266 markdown_site_utils-0.2.2/mdsite/data_test.py
+-rw-r--r--   0        0        0       22 2018-02-14 20:54:21.973447 markdown_site_utils-0.2.2/mdsite/testdata/config.toml
+-rw-r--r--   0        0        0       14 2018-02-14 20:54:21.974283 markdown_site_utils-0.2.2/mdsite/testdata/conflict/index.md
+-rw-r--r--   0        0        0        8 2018-02-14 20:54:21.973730 markdown_site_utils-0.2.2/mdsite/testdata/conflict.md
+-rw-r--r--   0        0        0      160 2018-02-14 20:54:21.974602 markdown_site_utils-0.2.2/mdsite/testdata/json.md
+-rw-r--r--   0        0        0       60 2023-04-13 17:48:51.615654 markdown_site_utils-0.2.2/mdsite/testdata/nohead.md
+-rw-r--r--   0        0        0       29 2018-02-14 20:54:21.974977 markdown_site_utils-0.2.2/mdsite/testdata/nougat/config.json
+-rw-r--r--   0        0        0      576 2020-01-26 16:09:19.091737 markdown_site_utils-0.2.2/mdsite/testdata/toml.md
+-rw-r--r--   0        0        0      245 2018-02-14 20:54:21.975578 markdown_site_utils-0.2.2/mdsite/testdata/yaml.md
+-rw-r--r--   0        0        0      709 2023-04-13 17:49:41.088936 markdown_site_utils-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 markdown_site_utils-0.2.2/setup.py
+-rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 markdown_site_utils-0.2.2/PKG-INFO
```

### Comparing `markdown_site_utils-0.2.1/LICENSE` & `markdown_site_utils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_site_utils-0.2.1/README.md` & `markdown_site_utils-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_site_utils-0.2.1/mdsite/data.py` & `markdown_site_utils-0.2.2/mdsite/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,49 +28,44 @@
     files = [f[:-3] for f in files if f.endswith(".md")]
     return sorted(dirs), sorted(files)
 
 
 def parse_file(file_path):
     raw_data = []
     content = []
-    raw_lines = []
     state = BEGIN_FILE
     end_sep = None
     data_parser = None
     seen_sep = False
     with open(file_path) as fp:
         for line in fp:
-            raw_lines.append(line)
             if state == BEGIN_FILE:
-                line = line.strip()
-                if not line:
-                    continue
-                if line in DATA_SEPS:
+                stripped = line.strip()
+                if stripped in DATA_SEPS:
                     seen_sep = True
                     state = IN_DATA
-                    end_sep, data_parser = DATA_SEPS[line]
-                    continue
+                    end_sep, data_parser = DATA_SEPS[stripped]
+                else:
+                    state = DATA_DONE
+                    content.append(line)
             elif state == IN_DATA:
                 if line.strip() == end_sep:
-                    state = DATA_DONE
+                    state = DATA_DONE        
                 else:
                     raw_data.append(line)
             elif state == DATA_DONE:
                 content.append(line)
             else:
                 raise AssertionError("Unreached")
     if raw_data:
         if not data_parser:
             raise ValueError("malformed input")
         data = data_parser("".join(raw_data))
     else:
         data = {}
-    if not seen_sep:
-        # no data header; backtrack to use all data without line stripping
-        content = raw_lines
     html = Markup(
         markdown2.markdown(
             "".join(content), extras=["markdown-in-html", "smarty-pants"]
         )
     )
     return data, html
```

### Comparing `markdown_site_utils-0.2.1/mdsite/data_test.py` & `markdown_site_utils-0.2.2/mdsite/data_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,9 +69,10 @@
 
     def testNoDataHeader(self):
         data = self.db.get_data("nohead")
         self.assertTrue(data.get("content", ""))
         self.assertIn("This markdown file", data.get("content", ""))
 
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `markdown_site_utils-0.2.1/mdsite/testdata/toml.md` & `markdown_site_utils-0.2.2/mdsite/testdata/toml.md`

 * *Files identical despite different names*

### Comparing `markdown_site_utils-0.2.1/pyproject.toml` & `markdown_site_utils-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markdown-site-utils"
-version = "0.2.1"
+version = "0.2.2"
 description = "Some utilities for managing Markdown files with metadata."
 authors = ["Jacob Smullyan <smulloni@smullyan.org>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/smulloni/markdown_site_utils"
 packages = [{include = "mdsite"}]
 include = [
```

### Comparing `markdown_site_utils-0.2.1/setup.py` & `markdown_site_utils-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ['MarkupSafe>=2.1.2,<3.0.0',
  'PyYAML>=6.0,<7.0',
  'markdown2>=2.4.8,<3.0.0',
  'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'markdown-site-utils',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Some utilities for managing Markdown files with metadata.',
     'long_description': '# Markdown Site Utils\n\nSome utilities for managing Markdown files with metadata.\n\nThe notion is that a content-oriented website may be written as a \nhierarchical series of Markdown files (with an ".md" extension) underneath\nsome data directory, e.g.:\n\n    DATA_DIR/\n      index.md\n      foo.md\n      bar.md\n      subdir/\n        index.md\n        foo.md\n        bar.md\n\nEach file may contain metadata, written in TOML in a section at\nthe top, bounded by \'+++\' lines:\n\n    +++\n    title = "My Page Title"\n    +++\n\n    # Some Markdown\n\nYAML and JSON may also be used. YAML blocks should start and end with lines\nconsisting of three dashes; JSON blocks should consist of a single JSON object\nwith opening and closing braces on lines by themselves. The data block is optional\nbut if present must begin on the first line of the file.\n\nTo use the library, you get create an `mdsite.DB` object with the path to your\ndata directory:\n\n    mydb = mdsite.DB("/path/to/data/dir")\n\nThen call `get_data(path)` for the path into the directory you want, leaving\nout the `.md` filename suffix, and, if you are looking for an index file, leaving\nout `index.md`:\n\n    data = mydb.get_data("/node/leaf")\n\nThe above gets data for `$DATA_DIR/node/leaf.md`, or for\n`$DATA_DIR/node/leaf/index.md`, if that file exists instead. \n\nThe library also supports hierarchical configuration, also written in TOML,\nYAML, or JSON, stored in files called `config.{toml,yaml,json}` depending on the\nconfig language employed.\n',
     'author': 'Jacob Smullyan',
     'author_email': 'smulloni@smullyan.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smulloni/markdown_site_utils',
```

### Comparing `markdown_site_utils-0.2.1/PKG-INFO` & `markdown_site_utils-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-site-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Some utilities for managing Markdown files with metadata.
 Home-page: https://github.com/smulloni/markdown_site_utils
 License: MIT
 Author: Jacob Smullyan
 Author-email: smulloni@smullyan.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

