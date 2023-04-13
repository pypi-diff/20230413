# Comparing `tmp/pathxf-0.0.1.tar.gz` & `tmp/pathxf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathxf-0.0.1.tar", max compression
+gzip compressed data, was "pathxf-0.0.2.tar", max compression
```

## Comparing `pathxf-0.0.1.tar` & `pathxf-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      756 2023-04-11 18:36:07.343580 pathxf-0.0.1/README.md
--rw-r--r--   0        0        0       22 2023-04-11 18:36:16.033650 pathxf-0.0.1/pathxf/__init__.py
--rw-r--r--   0        0        0     6338 2023-04-11 18:36:07.353580 pathxf-0.0.1/pathxf/app.py
--rw-r--r--   0        0        0     8169 2023-04-11 18:36:07.353580 pathxf-0.0.1/pathxf/bids.py
--rw-r--r--   0        0        0      557 2023-04-11 18:36:07.353580 pathxf-0.0.1/pathxf/spec.py
--rw-r--r--   0        0        0     6605 2023-04-11 18:36:07.353580 pathxf-0.0.1/pathxf/utils.py
--rw-r--r--   0        0        0      879 2023-04-11 18:36:16.033650 pathxf-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 pathxf-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      756 2023-04-11 18:36:07.343580 pathxf-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-13 20:37:29.064942 pathxf-0.0.2/pathxf/__init__.py
+-rw-r--r--   0        0        0     7281 2023-04-13 20:37:00.465169 pathxf-0.0.2/pathxf/app.py
+-rw-r--r--   0        0        0     8169 2023-04-11 18:36:07.353580 pathxf-0.0.2/pathxf/bids.py
+-rw-r--r--   0        0        0      557 2023-04-11 18:36:07.353580 pathxf-0.0.2/pathxf/spec.py
+-rw-r--r--   0        0        0     6934 2023-04-13 20:37:00.465169 pathxf-0.0.2/pathxf/utils.py
+-rw-r--r--   0        0        0      879 2023-04-13 20:37:29.064942 pathxf-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 pathxf-0.0.2/PKG-INFO
```

### Comparing `pathxf-0.0.1/README.md` & `pathxf-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pathxf-0.0.1/pathxf/app.py` & `pathxf-0.0.2/pathxf/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 from __future__ import annotations
 
 import copy
 import itertools as it
 import json
 import os
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Sequence
 
 import more_itertools as itx
 import typer
 import yaml
 from appdirs import user_cache_dir
 from typer import Option, Typer
 
 from pathxf.bids import bids
 from pathxf.spec import CompSpec, Spec
 from pathxf.utils import dict_merge, hash_container, listfiles, oswalk
 
 app = Typer()
 
-cache = Path(".cache")
-if cache.exists():
-    with cache.open() as f:
-        maps = json.load(f)
-
 
 def _merge_conditionals(compspec: CompSpec | list[CompSpec]) -> list[CompSpec]:
     if isinstance(compspec, list):
         return _merge_conditionals(CompSpec(conditions=compspec))
     if not "conditions" in compspec:
         return [compspec]
     mergables = copy.copy(compspec)
@@ -56,14 +51,19 @@
     def index(self, hash: str):
         return self.dir / "index" / hash
 
     def purge(self):
         for file in self.dir.joinpath("index").iterdir():
             os.remove(file)
 
+    def rm(self, spec: Spec):
+        name = hash_container(spec)
+        if self.contains(name):
+            os.remove(self.index(name))
+
     def __getitem__(self, spec: Spec):
         name = hash_container(spec)
         if self.contains(name):
             with open(self.index(name), "r") as f:
                 return json.load(f)["maps"]
         raise KeyError(name)
 
@@ -75,33 +75,37 @@
     def __contains__(self, __key: object) -> bool:
         if not isinstance(__key, dict):
             return False
         name = hash_container(__key)
         return self.contains(name)
 
 
-def index(config: Spec):
+def index(config: Spec, limit: Sequence[Path] | None = None):
     maps: dict[str, str] = {}
     for group in config["maps"]:
         if not "comps" in group:
-            for inp, wcards in listfiles(Path(config["input"], group["root"])):
+            for inp, wcards in listfiles(
+                Path(config["input"], group["root"]), dirs=limit
+            ):
                 wcards = dict(wcards.items())
                 try:
                     maps[group["out"].format(**wcards)] = inp
                 except KeyError:
                     raise Exception(
                         f"Not all wildcards found in input '{inp}'\n"
                         f"Found: {wcards}\n"
                     )
             continue
         for root, (path, _entityspecs) in it.product(
             itx.always_iterable(group["root"]), list(group["comps"].items())
         ):
             entityspecs = _merge_conditionals(_entityspecs)
-            for inp, wcards in listfiles(Path(config["input"], root + path)):
+            for inp, wcards in listfiles(
+                Path(config["input"], root + path), dirs=limit
+            ):
                 wcards = dict(wcards.items())
                 spec = None
                 for _spec in entityspecs:
                     good = True
                     if not "when" in _spec:
                         spec = _spec
                         break
@@ -133,55 +137,91 @@
                         f"Not all wildcards found in input '{inp}'\n"
                         f"Found: {wcards}\n"
                         f"Expected: {spec['bids']}"
                     )
     return maps
 
 
+def _normalize_limit(limits: Sequence[Path]):
+    viewed: set[Path] = set()
+    result: list[Path] = []
+    for limit in limits:
+        resolved = limit.resolve()
+        discard = False
+        for view in viewed:
+            if view in resolved.parents:
+                discard = True
+                break
+        if not discard:
+            result.append(limit)
+            viewed.add(resolved)
+    return result
+
+
 def main(
     config: Path,
-    input: Optional[Path] = Option(None, "-i", help="Override the input field in the config"),
-    output: Optional[Path] = Option(None, "-o", help="Override the ouptut field in the config"),
-    do_index: bool = Option(False, "--index", help="Force reindexing of the filesystem"),
+    input: Optional[Path] = Option(
+        None, "-i", help="Override the input field in the config"
+    ),
+    output: Optional[Path] = Option(
+        None, "-o", help="Override the ouptut field in the config"
+    ),
+    do_index: bool = Option(
+        False, "--index", help="Force reindexing of the filesystem"
+    ),
+    limit: Optional[list[Path]] = Option(
+        None, help="limit fs search to specific directories"
+    ),
     purge: bool = Option(False, help="Remove all cached indexes"),
-    _print: bool = Option(False, "--print", "-p", help="Print the file mapping as json, without doing any renaming"),
-    inverse: bool = Option(False, "-v", help="Print list of files in the input directory not indexed, formatted as json"),
+    _print: bool = Option(
+        False,
+        "--print",
+        "-p",
+        help="Print the file mapping as json, without doing any renaming",
+    ),
+    inverse: bool = Option(
+        False,
+        "-v",
+        help="Print list of files in the input directory not indexed, formatted as json",
+    ),
 ):
     cache = IndexCache()
     if purge:
         cache.purge()
         return
     with config.open() as f:
         config_obj: Spec = yaml.safe_load(f)
     if input is not None:
         config_obj["input"] = str(input)
     if output is not None:
         config_obj["output"] = str(output)
     if do_index or config_obj not in cache:
-        maps = index(config_obj)
+        maps = index(config_obj, limit=_normalize_limit(limit) if limit else None)
         cache[config_obj] = maps
     else:
         maps = cache[config_obj]
     if _print:
         print(json.dumps(maps))
         return
     if inverse:
         unused: list[str] = []
-        for f in oswalk(config_obj["input"]):
-            if Path(f).is_dir():
-                continue
-            if f in maps:
-                continue
-            unused.append(f)
+        for d in limit or [config_obj["input"]]:
+            for f in oswalk(d):
+                if Path(f).is_dir():
+                    continue
+                if f in maps:
+                    continue
+                unused.append(f)
         print(json.dumps(unused))
         return
 
     for src, dest in maps.items():
         if Path(src).exists() and not Path(dest).exists():
             Path(dest).parent.mkdir(parents=True, exist_ok=True)
             os.symlink(
                 os.path.relpath(Path(src).resolve(), Path(dest).resolve().parent), dest
             )
+    cache.rm(config_obj)
 
 
 def run():
     typer.run(main)
```

### Comparing `pathxf-0.0.1/pathxf/bids.py` & `pathxf-0.0.2/pathxf/bids.py`

 * *Files identical despite different names*

### Comparing `pathxf-0.0.1/pathxf/spec.py` & `pathxf-0.0.2/pathxf/spec.py`

 * *Files identical despite different names*

### Comparing `pathxf-0.0.1/pathxf/utils.py` & `pathxf-0.0.2/pathxf/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
 WalkTuple: TypeAlias = "tuple[AnyStr, list[AnyStr], list[AnyStr]]"
 
 
 class oswalk:
     cache: dict[str, tuple[str]] = {}
 
-    def __init__(self, dirname: str):
-        self.dirname = dirname
+    def __init__(self, dirname: str | Path):
+        self.dirname = str(dirname)
         if str(self.dirname) in self.cache:
             self.iter = iter(self.cache[str(self.dirname)])
             return
         paths: list[str] = []
         for root, dirs, files in os.walk(self.dirname):
             for file in it.chain(files, dirs):
                 paths.append(str(os.path.join(root, file)))
@@ -83,23 +83,25 @@
         return next(self.iter)
 
 
 def listfiles(
     pattern: str | Path,
     restriction: dict[str, Sequence[str]] | None = None,
     omit_value: str | None = None,
+    dirs: Sequence[str | Path] | None = None,
 ) -> Iterable[tuple[str, dict[str, str]]]:
     """Yield a tuple of existing filepaths for the given pattern.
 
     Wildcard values are yielded as the second tuple item.
 
     Args:
         pattern (str):       a filepattern. Wildcards are specified in snakemake syntax, e.g. "{id}.txt"
         restriction (dict):  restrict to wildcard values given in this dictionary
         omit_value (str):    wildcard value to omit
+        dirs:                Specified directories to search
 
     Yields:
         tuple: The next file matching the pattern, and the corresponding wildcards object
     """
     pattern = os.path.normpath(pattern)
     first_wildcard = re.search("{[^{]", pattern)
     if first_wildcard:
@@ -112,18 +114,24 @@
     re_patterns: dict[str, str] = {}
     for wildcard, restrictions in (restriction or {}).items():
         re_patterns[wildcard] = (
             "(" + "|".join(re.escape(restr) for restr in restrictions) + ")"
         )
     pattern_regex = re.compile(regex(pattern, re_patterns), re.VERBOSE)
 
-    for path in oswalk(dirname):
-        match = re.match(pattern_regex, path)
-        if match:
-            yield path, dict(match.groupdict())
+    for dir in dirs or [dirname]:
+        if (
+            Path(dir).resolve() != Path(dirname).resolve()
+            and Path(dirname) not in Path(dir).parents
+        ):
+            continue
+        for path in oswalk(str(dir)):
+            match = re.match(pattern_regex, path)
+            if match:
+                yield path, dict(match.groupdict())
 
 
 class MissingDict(dict):
     def __missing__(self, key):
         try:
             return self[key[: key.index(",")]]
         except (KeyError, ValueError):
```

### Comparing `pathxf-0.0.1/pyproject.toml` & `pathxf-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pathxf"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Peter Van Dyken <pvandyk2@uwo.ca>"]
 readme = "README.md"
 packages = [{include = "pathxf"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `pathxf-0.0.1/PKG-INFO` & `pathxf-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathxf
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Peter Van Dyken
 Author-email: pvandyk2@uwo.ca
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

