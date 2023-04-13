# Comparing `tmp/pymultilint-0.9.0.tar.gz` & `tmp/pymultilint-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultilint-0.9.0.tar", max compression
+gzip compressed data, was "pymultilint-1.0.0.tar", max compression
```

## Comparing `pymultilint-0.9.0.tar` & `pymultilint-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1070 2021-10-30 06:23:33.701064 pymultilint-0.9.0/LICENSE
--rw-r--r--   0        0        0     4515 2021-10-30 06:23:33.701252 pymultilint-0.9.0/README.md
--rwxr-xr-x   0        0        0    18674 2021-10-30 06:23:33.703816 pymultilint-0.9.0/multilint.py
--rw-r--r--   0        0        0     1347 2021-10-30 06:53:29.136423 pymultilint-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5540 2021-10-30 06:53:29.506826 pymultilint-0.9.0/setup.py
--rw-r--r--   0        0        0     5558 2021-10-30 06:53:29.507073 pymultilint-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 07:28:01.111554 pymultilint-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4518 2023-04-13 07:28:01.111554 pymultilint-1.0.0/README.md
+-rwxr-xr-x   0        0        0    18045 2023-04-13 07:28:01.111554 pymultilint-1.0.0/multilint.py
+-rw-r--r--   0        0        0     1281 2023-04-13 07:28:01.111554 pymultilint-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 pymultilint-1.0.0/PKG-INFO
```

### Comparing `pymultilint-0.9.0/LICENSE` & `pymultilint-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultilint-0.9.0/README.md` & `pymultilint-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Multilint (for Python)
 
-[![Actions Test Workflow Widget](https://github.com/gkze/multilint/workflows/ci/badge.svg)](https://github.com/gkze/multilint/actions?query=workflow%3Aci)
+[![Actions Test Workflow Widget](https://github.com/gkze/multilint/workflows/CI/badge.svg)](https://github.com/gkze/multilint/actions?query=workflow%3ACI)
 [![PyPI Version](https://img.shields.io/pypi/v/pymultilint)](https://pypi.org/project/pymultilint/)
 [![Pdoc Documentation](https://img.shields.io/badge/pdoc-docs-green)](https://gkze.github.io/multilint/multilint.html)
 
 A utility tying together multiple linting and other code quality tools
 
 ## Intro
 
@@ -15,15 +15,15 @@
 ## Installation
 
 Since there is an existing project called
 [`multilint`](https://pypi.org/project/multilint/), this Multilint can be
 installed as `pymultilint`:
 
 ```bash
-$ pip3 install multilint
+$ pip3 install pymultilint
 ```
 
 ## Usage
 
 Multilint exposes a CLI entry point:
 
 ```bash
@@ -31,16 +31,16 @@
 ```
 
 It can optionally take a set of starting paths. There are no CLI options,
 as Multilint strives to have all of its configuration codified (see
 [Configurability](#configurability)).
 
 Alternatively, Multilint is also usable via its API - either the
-[`main`](multilint.py#L526) method, or the
-[`Multilint`](multilint.py#L447) class
+[`main`](multilint.py#L570) method, or the
+[`Multilint`](multilint.py#L488) class.
 
 ## Supported Tools
 
 Currently, Multilint integrates the following code quality tools:
 
 * [Autoflake](https://github.com/myint/autoflake) - removes unused imports and
   unused variables as identified by [Pyflakes](https://github.com/PyCQA/pyflakes)
@@ -108,22 +108,22 @@
 Each integrated tool additionally supports `src_dirs` as an override, in case
 it is desired to target a specific tool at a different set of files
 / directories.
 
 ## Extending Multilint
 
 Support for more tools may be added by subclassing the
-[`ToolRunner`](multilint.py#L127) class and overriding the
-[`.run(...)`](multilint.py#L159) method.
+[`ToolRunner`](multilint.py#L128) class and overriding the
+[`.run(...)`](multilint.py#L160) method.
 
 There are some utilities provided, such as:
 
 * A logger that masquerades as a TextIO object to allow capturing tool output
   from within and wrapping it with preferred logging
 * A dictionary for tool configuration that is automatically available in the
   `ToolRunner` class, as long as the tool is registered in
-  * The [`Tool`](multilint.py#L47) enum,
-  * The [`TOOL_RUNNERS`](multilint.py#L446) mapping, and declared
-  * The [`DEFAULT_TOOL_ORDER`](multilint.py#L465) class variable of `Multilint`.
+  * The [`Tool`](multilint.py#L48) enum,
+  * The [`TOOL_RUNNERS`](multilint.py#L480) mapping, and declared
+  * The [`DEFAULT_TOOL_ORDER`](multilint.py#L500) class variable of `Multilint`.
 
 Documentation about adding support for more tools to Multilint may be added in
 the future.
```

### Comparing `pymultilint-0.9.0/multilint.py` & `pymultilint-1.0.0/multilint.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 """
 from __future__ import annotations
 
 import logging
 import re
 import sys
 from argparse import Namespace
+from collections.abc import Iterable, Mapping
+from collections.abc import Sequence as Seq
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from glob import glob
 from io import TextIOBase
 from logging import Formatter, Logger, StreamHandler
 from pathlib import Path
-from typing import Any, Iterable, Mapping
-from typing import Sequence as Seq
-from typing import TextIO, TypeVar, cast
+from typing import Any, TextIO, TypeVar, cast
 from unittest.mock import patch
 
-import pydocstyle  # type: ignore
+import pydocstyle  # type: ignore[import]
 import toml
-from autoflake import _main as autoflake_main  # type: ignore
+from autoflake import _main as autoflake_main  # type: ignore[attr-defined,import]
 from black import main as black_main
 from isort import files as isort_files
 from isort.api import sort_file as isort_file
 from isort.settings import DEFAULT_CONFIG
 from mypy.main import main as mypy_main  # pylint: disable=no-name-in-module
-from pylint.lint import Run as PylintRun  # type: ignore
-from pyupgrade._main import _fix_file as pyupgrade_fix_file  # type: ignore
+from pylint.lint import Run as PylintRun  # type: ignore[import]
+from pyupgrade._main import _fix_file as pyupgrade_fix_file  # type: ignore[import]
 
 FILE_DIR: Path = Path(__file__).resolve().parent
 ROOT_DIR: Path = FILE_DIR
 PYPROJECT_TOML_FILENAME: str = "pyproject.toml"
 
 LogLevel = TypeVar("LogLevel", bound=int)
 
@@ -44,30 +44,30 @@
 logging.basicConfig(level=logging.INFO, format=LOG_FMT)
 LOGGER: Logger = logging.getLogger("multilint")
 
 
 class Tool(Enum):
     """Encapsulates all supported linters, including Multilint itself."""
 
-    AUTOFLAKE: str = "autoflake"
-    BLACK: str = "black"
-    ISORT: str = "isort"
-    MULTILINT: str = "multilint"
-    MYPY: str = "mypy"
-    PYDOCSTYLE: str = "pydocstyle"
-    PYLINT: str = "pylint"
-    PYUPGRADE: str = "pyupgrade"
+    AUTOFLAKE = "autoflake"
+    BLACK = "black"
+    ISORT = "isort"
+    MULTILINT = "multilint"
+    MYPY = "mypy"
+    PYDOCSTYLE = "pydocstyle"
+    PYLINT = "pylint"
+    PYUPGRADE = "pyupgrade"
 
 
 class ToolResult(Enum):
     """ToolResult describes a generic run result from a code quality tool."""
 
-    SUCCESS: int = auto()
-    SUCCESS_PARTIAL: int = auto()
-    FAILURE: int = auto()
+    SUCCESS = auto()
+    SUCCESS_PARTIAL = auto()
+    FAILURE = auto()
 
 
 class ToolLogger(Logger):
     """ToolLogger allows setting format on itself during instantiation."""
 
     def __init__(
         self: ToolLogger, name: str, level: LogLevel, logfmt: str = LOG_FMT
@@ -167,48 +167,26 @@
 
     Autoflake removes unused imports and variables among other
     things. Reads autoflake arguments from pyproject.toml. Arguments are
     specified by their full name, with underscores or dashes - either style is
     accepted.
     """
 
-    def _make_autoflake_args(self: AutoflakeRunner) -> list[str]:
-        args: list[str] = []
-
-        for key, val in self.config.items():
-            if key == "src_paths":
-                for src in val:
-                    args.append(src)
-
-                continue
-
-            opt: str = f"--{key.replace('_', '-')}"
-
-            if isinstance(val, bool):
-                args.append(opt)
-
-                continue
-
-            args.append(f"{opt}={val}")
-
-        return args
-
     def run(self: AutoflakeRunner) -> ToolResult:
         """Run autoflake."""
         logger: Logger = self.make_logger(TextIOLogger, logging.INFO)
-        autoflake_args: list[str] = self._make_autoflake_args()
-        if all(cfgval.startswith("--") for cfgval in autoflake_args):
-            autoflake_args.extend([str(p) for p in self.src_paths])
-
-        retcode: int = autoflake_main(
-            [self._tool.value, *autoflake_args], logger, logger
+        return (
+            ToolResult.SUCCESS
+            if autoflake_main(
+                ["autoflake", *[p.name for p in self.src_paths]], logger, logger, None
+            )
+            == 0
+            else ToolResult.FAILURE
         )
 
-        return ToolResult.SUCCESS if retcode == 0 else ToolResult.FAILURE
-
 
 @dataclass
 class ISortResult:
     """Isort run result.
 
     Encapsulates a result from an isort run: the Python file, the ToolResult,
     and an error message (if and when applicable).
@@ -226,42 +204,44 @@
 class ISortRunner(ToolRunner):
     """Runs isort.
 
     Isort is able to sort imports in a Python source file according to a defined
     rule set (with sensible defaults).
     """
 
-    # pylint: disable=too-many-branches
     def run(self: ISortRunner) -> ToolResult:
         """Run isort."""
         logger: Logger = self.make_logger(ToolLogger, logging.INFO)
         results: set[ISortResult] = set()
 
         isort_logger: TextIOLogger = cast(
             TextIOLogger, self.make_logger(TextIOLogger, logging.INFO)
         )
 
-        # fmt: off
         for file in isort_files.find(
             [str(p) for p in self.src_paths]
             or cast(Iterable[str], DEFAULT_CONFIG.src_paths),
-            DEFAULT_CONFIG, [], [],
+            DEFAULT_CONFIG,
+            [],
+            [],
         ):
             try:
                 with patch("sys.stdout", isort_logger):
                     isort_file(file)
 
                 results.add(ISortResult(Path(file), ToolResult.SUCCESS))
-            # pylint: disable=broad-except
-            except Exception as ex:
-                results.add(ISortResult(
-                    Path(file), ToolResult.FAILURE,
-                    getattr(ex, "message") if hasattr(ex, "message") else "",
-                ))
-        # fmt: on
+
+            except Exception as ex:  # pylint: disable=broad-exception-caught
+                results.add(
+                    ISortResult(
+                        Path(file),
+                        ToolResult.FAILURE,
+                        getattr(ex, "message") if hasattr(ex, "message") else "",
+                    )
+                )
 
         failed: set[ISortResult] = set()
         for isort_result in results:
             if isort_result.result == ToolResult.FAILURE:
                 failed.add(isort_result)
 
         if len(failed) > 0:
@@ -290,24 +270,25 @@
         iologger: Logger = self.make_logger(TextIOLogger, logging.INFO)
         sys_stdout_orig = sys.stdout
         sys_stderr_orig = sys.stderr
 
         try:
             sys.stdout = cast(TextIO, iologger)
             sys.stderr = cast(TextIO, iologger)
+
             # pylint: disable=no-value-for-parameter
             black_main([str(p) for p in self.src_paths])
 
             return ToolResult.SUCCESS
 
         except SystemExit as sysexit:
             return ToolResult.SUCCESS if sysexit.code == 0 else ToolResult.FAILURE
 
         finally:
-            sys.stdout = sys_stdout_orig  # type: ignore
+            sys.stdout = sys_stdout_orig
             sys.stderr = sys_stderr_orig
 
 
 class MypyRunner(ToolRunner):
     """Runs Mypy.
 
     Mypy is a static type checker for Python.
@@ -319,18 +300,18 @@
             TextIOLogger, self.make_logger(TextIOLogger, logging.INFO)
         )
 
         logger_as_textio: TextIO = cast(TextIO, logger)
 
         try:
             mypy_main(
-                None,
-                logger_as_textio,
-                logger_as_textio,
-                [str(p) for p in self.src_paths],
+                args=[p.name for p in self.src_paths],
+                stdout=logger_as_textio,
+                stderr=logger_as_textio,
+                clean_exit=True,
             )
 
             return ToolResult.SUCCESS
 
         except SystemExit as sysexit:
             return ToolResult.SUCCESS if sysexit.code == 0 else ToolResult.FAILURE
 
@@ -371,23 +352,20 @@
                 self.level = logging.INFO
 
         info_logger: InfoToolLogger = InfoToolLogger(self._tool.value, logging.INFO)
         pydocstyle_log_orig: Logger = pydocstyle.utils.log
         try:
             pydocstyle.utils.log = info_logger
             pydocstyle.checker.log = info_logger
+
             # pylint: disable=import-outside-toplevel
-            from pydocstyle.cli import run_pydocstyle as pydocstyle_main  # type: ignore
+            from pydocstyle.cli import run_pydocstyle  # type: ignore[import]
 
             with patch("sys.stdout", self.make_logger(TextIOLogger, logging.INFO)):
-                return [
-                    ToolResult.SUCCESS,
-                    ToolResult.SUCCESS_PARTIAL,
-                    ToolResult.FAILURE,
-                ][pydocstyle_main()]
+                return list(ToolResult)[run_pydocstyle()]
 
         finally:
             pydocstyle.utils.log = pydocstyle_log_orig
             pydocstyle.checker.log = pydocstyle_log_orig
 
 
 class PyupgradeRunner(ToolRunner):
@@ -407,17 +385,17 @@
         """Run Pyupgrade."""
         self._validate_config()
 
         logger: ToolLogger = self.make_logger(TextIOLogger, logging.INFO)
 
         with patch("sys.stdout", logger), patch("sys.stderr", logger):
             retcode: int = 0
-            for src_path in self.src_paths:
+            for src_path in [p for p in self.src_paths if p.is_file()]:
                 retcode |= pyupgrade_fix_file(
-                    src_path,
+                    src_path.resolve().name,
                     Namespace(
                         exit_zero_even_if_changed=self.config.get(
                             "exit_zero_even_if_changed", None
                         ),
                         keep_mock=self.config.get("keep_mock", None),
                         keep_percent_format=self.config.get(
                             "keep_percent_format", None
@@ -539,45 +517,47 @@
 
         Runs a single specified linter or other code quality tool. Returns
         a ToolResult from the run.
         """
         LOGGER.info(f"Running {tool.value}...")
         tool_config: Mapping[str, Any] = self._get_tool_config(tool)
 
-        # fmt: off
-        result: ToolResult = cast(ToolRunner, TOOL_RUNNERS[tool](
-            tool,
-            expand_src_paths(
-                [Path(sp) for sp in tool_config.get("src_paths", self._src_paths)]
+        result: ToolResult = cast(
+            ToolRunner,
+            TOOL_RUNNERS[tool](
+                tool,
+                expand_src_paths(
+                    [Path(sp) for sp in tool_config.get("src_paths", self._src_paths)]
+                ),
+                tool_config,
             ),
-            tool_config,
-        )).run()
-        # fmt: on
+        ).run()
 
         LOGGER.info(f"{tool.value} exited with {result}")
 
         return result
 
     def run_all_tools(
-        self: Multilint, order: Seq[Tool] = None
+        self: Multilint, order: Seq[Tool] = []
     ) -> Mapping[Tool, ToolResult]:
         """Run tools in specified order."""
         results: dict[Tool, ToolResult] = {}
 
-        if order is None:
+        if not order:
             order = self._tool_order
 
         for tool in order:
             results[tool] = self.run_tool(tool)
 
         return results
 
 
 def main(
-    src_paths: Seq[Path] = list(map(Path, sys.argv[1:])), do_exit: bool = True
+    src_paths: Seq[Path] = [Path(p) for p in sys.argv[1:]],  # type: ignore[name-defined]
+    do_exit: bool = True,
 ) -> int | None:
     """Acts as the default entry point for Multilint.
 
     The main / default entry point to multilint. Runs all tools and logs
     their results.
     """
     results: Mapping[Tool, ToolResult] = Multilint(src_paths).run_all_tools()
@@ -591,8 +571,8 @@
     if do_exit:
         sys.exit(retcode)
 
     return retcode
 
 
 if __name__ == "__main__":
-    sys.exit(main(list(map(Path, sys.argv[1:]))))
+    sys.exit(main([Path(arg) for arg in sys.argv[1:]]))
```

### Comparing `pymultilint-0.9.0/pyproject.toml` & `pymultilint-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 [tool.poetry]
 name = "pymultilint"
 packages = [{include = "multilint.py"}]
-version = "0.9.0"
+version = "1.0.0"
 description = "Utility tying multiple code quality tools together"
 authors = ["George Kontridze <george.kontridze@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gkze/multilint"
 repository = "https://github.com/gkze/multilint"
 documentation = "https://gkze.github.io/multilint/multilint.html"
 keywords = ["lint", "code-quality", "tools"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydocstyle = "^6.0.0"
-autoflake = "^1.4"
-isort = "^5.8.0"
-pylint = "^2.8.2"
-toml = "^0.10.2"
-black = "^21.5b0"
-mypy = "^0.812"
-pyupgrade = "^2.14.0"
-
-[tool.poetry.dev-dependencies]
-ipython = "^7.19.0"
-jedi = "0.17.2"
-parso = "0.7.1"
-sphinx-rtd-theme = "^0.5.1"
-pdoc = "^4.0.0"
+autoflake = "^2.0"
+black = "^23.3"
+isort = "^5.12"
+mypy = "^1.2"
+pydocstyle = "^6.3"
+pylint = "^2.17"
+pyupgrade = "^3.3"
+toml = "^0.10"
 
 [tool.poetry.scripts]
 multilint = "multilint:main"
 
+[tool.poetry.group.dev.dependencies]
+ipython = "^8.12"
+jedi = "^0.18"
+parso = "^0.8"
+pdoc = "^13.1"
+sphinx-rtd-theme = "^1.2"
+types-pyflakes = "^3.0.0.3"
+types-toml = "^0.10"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.multilint]
-src_paths = ["*.py", "docs"]
+src_paths = ["*.py"]
 
 [tool.autoflake]
-recursive = true
-in_place = true
-ignore_init_module_imports = true
-remove_all_unused_imports = true
-remove_unused_variables = true
-verbose = true
+in-place = true
+remove-unused-variables = true
+remove-rhs-for-unused-variables = true
 
 [tool.mypy]
-src_paths = ["*.py"]
+mypy_path = "stubs"
 
 [tool.pyupgrade]
-src_paths = ["*.py", "**/*.py"]
-min_version = "3.9"
+min_version = "3.8"
 
 [tool.pylint.messages_control]
 disable = ["logging-fstring-interpolation", "dangerous-default-value"]
```

### Comparing `pymultilint-0.9.0/setup.py` & `pymultilint-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,158 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pymultilint
+Version: 1.0.0
+Summary: Utility tying multiple code quality tools together
+Home-page: https://github.com/gkze/multilint
+License: MIT
+Keywords: lint,code-quality,tools
+Author: George Kontridze
+Author-email: george.kontridze@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: autoflake (>=2.0,<3.0)
+Requires-Dist: black (>=23.3,<24.0)
+Requires-Dist: isort (>=5.12,<6.0)
+Requires-Dist: mypy (>=1.2,<2.0)
+Requires-Dist: pydocstyle (>=6.3,<7.0)
+Requires-Dist: pylint (>=2.17,<3.0)
+Requires-Dist: pyupgrade (>=3.3,<4.0)
+Requires-Dist: toml (>=0.10,<0.11)
+Project-URL: Documentation, https://gkze.github.io/multilint/multilint.html
+Project-URL: Repository, https://github.com/gkze/multilint
+Description-Content-Type: text/markdown
 
-modules = \
-['multilint']
-install_requires = \
-['autoflake>=1.4,<2.0',
- 'black>=21.5b0,<22.0',
- 'isort>=5.8.0,<6.0.0',
- 'mypy>=0.812,<0.813',
- 'pydocstyle>=6.0.0,<7.0.0',
- 'pylint>=2.8.2,<3.0.0',
- 'pyupgrade>=2.14.0,<3.0.0',
- 'toml>=0.10.2,<0.11.0']
-
-entry_points = \
-{'console_scripts': ['multilint = multilint:main']}
-
-setup_kwargs = {
-    'name': 'pymultilint',
-    'version': '0.9.0',
-    'description': 'Utility tying multiple code quality tools together',
-    'long_description': '# Multilint (for Python)\n\n[![Actions Test Workflow Widget](https://github.com/gkze/multilint/workflows/ci/badge.svg)](https://github.com/gkze/multilint/actions?query=workflow%3Aci)\n[![PyPI Version](https://img.shields.io/pypi/v/pymultilint)](https://pypi.org/project/pymultilint/)\n[![Pdoc Documentation](https://img.shields.io/badge/pdoc-docs-green)](https://gkze.github.io/multilint/multilint.html)\n\nA utility tying together multiple linting and other code quality tools\n\n## Intro\n\nMultilint allows running several code quality tools under the same interface.\nThis is convenient as it saves time on writing multiple linter / formatter /\nchecker invocations every time in a project.\n\n## Installation\n\nSince there is an existing project called\n[`multilint`](https://pypi.org/project/multilint/), this Multilint can be\ninstalled as `pymultilint`:\n\n```bash\n$ pip3 install multilint\n```\n\n## Usage\n\nMultilint exposes a CLI entry point:\n\n```bash\n$ multilint [paths ...]\n```\n\nIt can optionally take a set of starting paths. There are no CLI options,\nas Multilint strives to have all of its configuration codified (see\n[Configurability](#configurability)).\n\nAlternatively, Multilint is also usable via its API - either the\n[`main`](multilint.py#L526) method, or the\n[`Multilint`](multilint.py#L447) class\n\n## Supported Tools\n\nCurrently, Multilint integrates the following code quality tools:\n\n* [Autoflake](https://github.com/myint/autoflake) - removes unused imports and\n  unused variables as identified by [Pyflakes](https://github.com/PyCQA/pyflakes)\n* [Isort](https://pycqa.github.io/isort/) - sorts imports according to specified\n  orders\n* [Black](https://black.readthedocs.io/en/stable/) - the self-proclaimed\n  "uncompromising code formatter" - formats Python source with an opinionated\n  style\n* [Mypy](http://mypy-lang.org) - static type checker for Python\n* [Pylint](https://www.pylint.org) - general best practices linter\n* [Pydocstyle](http://www.pydocstyle.org/en/stable/) - in-source documentation\n  best practices linter\n* [Pyupgrade](https://github.com/asottile/pyupgrade) - upgrades Python syntax to\n  the latest for the specified version\n\n## Configurability\n\nAdditionally, for tools that do not currently support configuration via\n`pyproject.toml`([PEP-621](https://www.python.org/dev/peps/pep-0621/)),\nMultilint exposes a configuration interface for them. This allows for\ncentralized codification of configuration of all code quality tools being used\nin a project.\n\nExample relevant sections from a `pyproject.toml`:\n\n```toml\n[tool.autoflake]\nrecursive = true\nin_place = true\nignore_init_module_imports = true\nremove_all_unused_imports = true\nremove_unused_variables = true\nverbose = true\nsrcs_paths = ["somepackage"]\n\n[tool.mypy]\nsrc_paths = ["someotherpackage"]\n\n[tool.multilint]\ntool_order = [\n  "autoflake",\n  "isort",\n  "pyupgrade",\n  "black",\n  "mypy",\n  "pylint",\n  "pydocstyle"\n]\nsrc_paths = ["."]\n```\n\nAt the time of writing of this README (2020-01-31), neither\n[Autoflake](https://github.com/myint/autoflake/issues/59) nor\n[Mypy](https://github.com/python/mypy/issues/5205https://github.com/python/mypy/issues/5205)\nsupport configuration via `pyproject.toml`. While support for each may or may\nnot be added at some point in the future, with multilint configuring these tools\nis possible **today**.\n\nCurrently, the only two supported configuration option for Multilint are:\n\n* `tool_order`, which defines the execution order of supported tools, and\n* `src_paths`, which specifies the source paths (can be files and directories)\n  for Multilint to operate on.\n\nEach integrated tool additionally supports `src_dirs` as an override, in case\nit is desired to target a specific tool at a different set of files\n/ directories.\n\n## Extending Multilint\n\nSupport for more tools may be added by subclassing the\n[`ToolRunner`](multilint.py#L127) class and overriding the\n[`.run(...)`](multilint.py#L159) method.\n\nThere are some utilities provided, such as:\n\n* A logger that masquerades as a TextIO object to allow capturing tool output\n  from within and wrapping it with preferred logging\n* A dictionary for tool configuration that is automatically available in the\n  `ToolRunner` class, as long as the tool is registered in\n  * The [`Tool`](multilint.py#L47) enum,\n  * The [`TOOL_RUNNERS`](multilint.py#L446) mapping, and declared\n  * The [`DEFAULT_TOOL_ORDER`](multilint.py#L465) class variable of `Multilint`.\n\nDocumentation about adding support for more tools to Multilint may be added in\nthe future.\n',
-    'author': 'George Kontridze',
-    'author_email': 'george.kontridze@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/gkze/multilint',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+# Multilint (for Python)
 
+[![Actions Test Workflow Widget](https://github.com/gkze/multilint/workflows/CI/badge.svg)](https://github.com/gkze/multilint/actions?query=workflow%3ACI)
+[![PyPI Version](https://img.shields.io/pypi/v/pymultilint)](https://pypi.org/project/pymultilint/)
+[![Pdoc Documentation](https://img.shields.io/badge/pdoc-docs-green)](https://gkze.github.io/multilint/multilint.html)
+
+A utility tying together multiple linting and other code quality tools
+
+## Intro
+
+Multilint allows running several code quality tools under the same interface.
+This is convenient as it saves time on writing multiple linter / formatter /
+checker invocations every time in a project.
+
+## Installation
+
+Since there is an existing project called
+[`multilint`](https://pypi.org/project/multilint/), this Multilint can be
+installed as `pymultilint`:
+
+```bash
+$ pip3 install pymultilint
+```
+
+## Usage
+
+Multilint exposes a CLI entry point:
+
+```bash
+$ multilint [paths ...]
+```
+
+It can optionally take a set of starting paths. There are no CLI options,
+as Multilint strives to have all of its configuration codified (see
+[Configurability](#configurability)).
+
+Alternatively, Multilint is also usable via its API - either the
+[`main`](multilint.py#L570) method, or the
+[`Multilint`](multilint.py#L488) class.
+
+## Supported Tools
+
+Currently, Multilint integrates the following code quality tools:
+
+* [Autoflake](https://github.com/myint/autoflake) - removes unused imports and
+  unused variables as identified by [Pyflakes](https://github.com/PyCQA/pyflakes)
+* [Isort](https://pycqa.github.io/isort/) - sorts imports according to specified
+  orders
+* [Black](https://black.readthedocs.io/en/stable/) - the self-proclaimed
+  "uncompromising code formatter" - formats Python source with an opinionated
+  style
+* [Mypy](http://mypy-lang.org) - static type checker for Python
+* [Pylint](https://www.pylint.org) - general best practices linter
+* [Pydocstyle](http://www.pydocstyle.org/en/stable/) - in-source documentation
+  best practices linter
+* [Pyupgrade](https://github.com/asottile/pyupgrade) - upgrades Python syntax to
+  the latest for the specified version
+
+## Configurability
+
+Additionally, for tools that do not currently support configuration via
+`pyproject.toml`([PEP-621](https://www.python.org/dev/peps/pep-0621/)),
+Multilint exposes a configuration interface for them. This allows for
+centralized codification of configuration of all code quality tools being used
+in a project.
+
+Example relevant sections from a `pyproject.toml`:
+
+```toml
+[tool.autoflake]
+recursive = true
+in_place = true
+ignore_init_module_imports = true
+remove_all_unused_imports = true
+remove_unused_variables = true
+verbose = true
+srcs_paths = ["somepackage"]
+
+[tool.mypy]
+src_paths = ["someotherpackage"]
+
+[tool.multilint]
+tool_order = [
+  "autoflake",
+  "isort",
+  "pyupgrade",
+  "black",
+  "mypy",
+  "pylint",
+  "pydocstyle"
+]
+src_paths = ["."]
+```
+
+At the time of writing of this README (2020-01-31), neither
+[Autoflake](https://github.com/myint/autoflake/issues/59) nor
+[Mypy](https://github.com/python/mypy/issues/5205https://github.com/python/mypy/issues/5205)
+support configuration via `pyproject.toml`. While support for each may or may
+not be added at some point in the future, with multilint configuring these tools
+is possible **today**.
+
+Currently, the only two supported configuration option for Multilint are:
+
+* `tool_order`, which defines the execution order of supported tools, and
+* `src_paths`, which specifies the source paths (can be files and directories)
+  for Multilint to operate on.
+
+Each integrated tool additionally supports `src_dirs` as an override, in case
+it is desired to target a specific tool at a different set of files
+/ directories.
+
+## Extending Multilint
+
+Support for more tools may be added by subclassing the
+[`ToolRunner`](multilint.py#L128) class and overriding the
+[`.run(...)`](multilint.py#L160) method.
+
+There are some utilities provided, such as:
+
+* A logger that masquerades as a TextIO object to allow capturing tool output
+  from within and wrapping it with preferred logging
+* A dictionary for tool configuration that is automatically available in the
+  `ToolRunner` class, as long as the tool is registered in
+  * The [`Tool`](multilint.py#L48) enum,
+  * The [`TOOL_RUNNERS`](multilint.py#L480) mapping, and declared
+  * The [`DEFAULT_TOOL_ORDER`](multilint.py#L500) class variable of `Multilint`.
+
+Documentation about adding support for more tools to Multilint may be added in
+the future.
 
-setup(**setup_kwargs)
```

