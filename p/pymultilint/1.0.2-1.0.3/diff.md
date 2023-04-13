# Comparing `tmp/pymultilint-1.0.2.tar.gz` & `tmp/pymultilint-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultilint-1.0.2.tar", max compression
+gzip compressed data, was "pymultilint-1.0.3.tar", max compression
```

## Comparing `pymultilint-1.0.2.tar` & `pymultilint-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-04-13 07:38:30.461308 pymultilint-1.0.2/LICENSE
--rw-r--r--   0        0        0     4518 2023-04-13 07:38:30.461308 pymultilint-1.0.2/README.md
--rwxr-xr-x   0        0        0    18098 2023-04-13 07:38:30.465308 pymultilint-1.0.2/multilint.py
--rw-r--r--   0        0        0     1281 2023-04-13 07:38:30.465308 pymultilint-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 pymultilint-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 18:51:24.661692 pymultilint-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4518 2023-04-13 18:51:24.661692 pymultilint-1.0.3/README.md
+-rwxr-xr-x   0        0        0    18125 2023-04-13 18:51:24.665693 pymultilint-1.0.3/multilint.py
+-rw-r--r--   0        0        0     1281 2023-04-13 18:51:24.665693 pymultilint-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 pymultilint-1.0.3/PKG-INFO
```

### Comparing `pymultilint-1.0.2/LICENSE` & `pymultilint-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultilint-1.0.2/README.md` & `pymultilint-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pymultilint-1.0.2/multilint.py` & `pymultilint-1.0.3/multilint.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,21 +445,20 @@
 
     with pyproject_toml.open("r") as file:
         return toml.load(file)
 
 
 def expand_src_paths(src_paths: Seq[Path]) -> list[Path]:
     """Expand source paths in case they are globs."""
-    return sum(
-        (
-            [Path(ge) for ge in glob(p.name)] if "*" in p.name else [p]
-            for p in src_paths
-        ),
-        [],
-    )
+    # fmt: off
+    return sum((
+        [Path(ge) for ge in glob(p.name)] if "*" in p.name else [p]
+        for p in src_paths
+    ), [])
+    # fmt: on
 
 
 TOOL_RUNNERS: Mapping[Tool, type[ToolRunner]] = {
     Tool.AUTOFLAKE: AutoflakeRunner,
     Tool.BLACK: BlackRunner,
     Tool.ISORT: ISortRunner,
     Tool.MYPY: MypyRunner,
@@ -518,24 +517,21 @@
 
         Runs a single specified linter or other code quality tool. Returns
         a ToolResult from the run.
         """
         LOGGER.info(f"Running {tool.value}...")
         tool_config: Mapping[str, Any] = self._get_tool_config(tool)
 
-        result: ToolResult = cast(
-            ToolRunner,
-            TOOL_RUNNERS[tool](
-                tool,
-                expand_src_paths(
-                    [Path(sp) for sp in tool_config.get("src_paths", self._src_paths)]
-                ),
-                tool_config,
-            ),
+        # fmt: off
+        result: ToolResult = cast(ToolRunner, TOOL_RUNNERS[tool](
+            tool, expand_src_paths(
+                [Path(sp) for sp in tool_config.get("src_paths", self._src_paths)]
+            ), tool_config),
         ).run()
+        # fmt: on
 
         LOGGER.info(f"{tool.value} exited with {result}")
 
         return result
 
     def run_all_tools(
         self: Multilint, order: Seq[Tool] = []
@@ -543,15 +539,16 @@
         """Run tools in specified order."""
         results: dict[Tool, ToolResult] = {}
 
         if not order:
             order = self._tool_order
 
         for tool in order:
-            results[tool] = self.run_tool(tool)
+            if tool.name not in self._multilint_config.get("disable", []):
+                results[tool] = self.run_tool(tool)
 
         return results
 
 
 def main(
     src_paths: Seq[Path] = [Path(p) for p in sys.argv[1:]],  # type: ignore[name-defined]
     do_exit: bool = True,
```

### Comparing `pymultilint-1.0.2/pyproject.toml` & `pymultilint-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pymultilint"
 packages = [{include = "multilint.py"}]
-version = "1.0.2"
+version = "1.0.3"
 description = "Utility tying multiple code quality tools together"
 authors = ["George Kontridze <george.kontridze@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gkze/multilint"
 repository = "https://github.com/gkze/multilint"
 documentation = "https://gkze.github.io/multilint/multilint.html"
```

### Comparing `pymultilint-1.0.2/PKG-INFO` & `pymultilint-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultilint
-Version: 1.0.2
+Version: 1.0.3
 Summary: Utility tying multiple code quality tools together
 Home-page: https://github.com/gkze/multilint
 License: MIT
 Keywords: lint,code-quality,tools
 Author: George Kontridze
 Author-email: george.kontridze@gmail.com
 Requires-Python: >=3.8,<4.0
```

