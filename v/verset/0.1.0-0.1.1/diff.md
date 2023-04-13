# Comparing `tmp/verset-0.1.0.tar.gz` & `tmp/verset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verset-0.1.0.tar", max compression
+gzip compressed data, was "verset-0.1.1.tar", max compression
```

## Comparing `verset-0.1.0.tar` & `verset-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2291 2023-04-13 18:52:13.604938 verset-0.1.0/README.md
--rw-r--r--   0        0        0      604 2023-04-13 18:57:05.092975 verset-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2795 2023-04-13 18:48:55.034029 verset-0.1.0/src/verset/__init__.py
--rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 verset-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2288 2023-04-13 20:12:13.799224 verset-0.1.1/README.md
+-rw-r--r--   0        0        0      604 2023-04-13 20:13:56.066612 verset-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2875 2023-04-13 20:10:35.084810 verset-0.1.1/src/verset/__init__.py
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 verset-0.1.1/PKG-INFO
```

### Comparing `verset-0.1.0/README.md` & `verset-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,33 +46,34 @@
 docutils = "~0.19" # >= 0.12
 python = "~3.10.10" # >=3.8
 
 python-dateutil = {version="~2.8.2", optional=true} # ^2.8.2
 jira = {version="^3.1.1", optional=true} # Not found
 six = {version="~1.16.0", optional=true} # ^1.16
 pygments = {version="~2.14.0", optional=true} # ^2.12.0
+
 ```
 and if you run it again, you are back to the original version (as tilde):
 
 ```toml
 [tool.poetry.dependencies]
-docutils = "~0.19" # >= 0.12
+docutils = "~0.12" # ~0.19
 python = "~3.8" # ~3.10.10
 
 python-dateutil = {version="~2.8.2", optional=true} # ~2.8.2
 jira = {version="^3.1.1", optional=true} # Not found
 six = {version="~1.16", optional=true} # ~1.16.0
 pygments = {version="~2.12.0", optional=true} # ~2.14.0
 ```
 
 if you would like the more inclusive carret versions, just use `veset relax`:
 
 ```toml
 [tool.poetry.dependencies]
-docutils = "~0.19" # >= 0.12
+docutils = "^0.19" # ~0.12
 python = "^3.10.10" # ~3.8
 
 python-dateutil = {version="^2.8.2", optional=true} # ~2.8.2
 jira = {version="^3.1.1", optional=true} # Not found
 six = {version="^1.16.0", optional=true} # ~1.16
 pygments = {version="^2.14.0", optional=true} # ~2.12.0
 ```
```

### Comparing `verset-0.1.0/pyproject.toml` & `verset-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "verset"
-version = "0.1.0"
+version = "0.1.1"
 description = "pyprojects.toml dependencies version manager"
 authors = ["fdev31 <fdev31@gmail.com>"]
 homepage = "https://github.com/fdev31/verset"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `verset-0.1.0/src/verset/__init__.py` & `verset-0.1.1/src/verset/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,28 @@
 def clear(deps):
     for dep in deps:
         deps[dep]._trivia.comment = ''
 
 def extract_version(txt):
     i = 0
     for i, c in enumerate(txt):
-        if c not in '^~>=<':
+        if c not in '^~>=< ':
             break
     v = txt[i:]
-    print(v)
     if v[0].isdigit():
         return v
     
 
 def _apply(deps, prefix):
     for dep in deps:
+        _comment = deps[dep]._trivia.comment
+        if not _comment:
+            continue
         version = extract_version(deps[dep]._trivia.comment.split('#', 1)[1].strip())
+
         if version:
             d = deps[dep]
             if isinstance(d, tomlkit.items.InlineTable):
                 old_version = str(deps[dep]['version'])
                 deps[dep]['version'] = prefix + version
             else:
                 old_version = str(deps[dep])
```

### Comparing `verset-0.1.0/PKG-INFO` & `verset-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verset
-Version: 0.1.0
+Version: 0.1.1
 Summary: pyprojects.toml dependencies version manager
 Home-page: https://github.com/fdev31/verset
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -62,33 +62,34 @@
 docutils = "~0.19" # >= 0.12
 python = "~3.10.10" # >=3.8
 
 python-dateutil = {version="~2.8.2", optional=true} # ^2.8.2
 jira = {version="^3.1.1", optional=true} # Not found
 six = {version="~1.16.0", optional=true} # ^1.16
 pygments = {version="~2.14.0", optional=true} # ^2.12.0
+
 ```
 and if you run it again, you are back to the original version (as tilde):
 
 ```toml
 [tool.poetry.dependencies]
-docutils = "~0.19" # >= 0.12
+docutils = "~0.12" # ~0.19
 python = "~3.8" # ~3.10.10
 
 python-dateutil = {version="~2.8.2", optional=true} # ~2.8.2
 jira = {version="^3.1.1", optional=true} # Not found
 six = {version="~1.16", optional=true} # ~1.16.0
 pygments = {version="~2.12.0", optional=true} # ~2.14.0
 ```
 
 if you would like the more inclusive carret versions, just use `veset relax`:
 
 ```toml
 [tool.poetry.dependencies]
-docutils = "~0.19" # >= 0.12
+docutils = "^0.19" # ~0.12
 python = "^3.10.10" # ~3.8
 
 python-dateutil = {version="^2.8.2", optional=true} # ~2.8.2
 jira = {version="^3.1.1", optional=true} # Not found
 six = {version="^1.16.0", optional=true} # ~1.16
 pygments = {version="^2.14.0", optional=true} # ~2.12.0
 ```
```

