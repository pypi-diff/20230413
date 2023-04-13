# Comparing `tmp/python_whiteprint-0.6.1.tar.gz` & `tmp/python_whiteprint-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_whiteprint-0.6.1.tar", max compression
+gzip compressed data, was "python_whiteprint-0.7.0.tar", max compression
```

## Comparing `python_whiteprint-0.6.1.tar` & `python_whiteprint-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0        0        0        0 2023-03-22 09:25:58.029072 python_whiteprint-0.6.1/LICENSES/
--rw-r--r--   0        0        0     2914 2023-03-22 09:25:58.029072 python_whiteprint-0.6.1/README.md
--rw-r--r--   0        0        0    29303 2023-03-22 09:26:25.225349 python_whiteprint-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      220 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/__init__.py
--rwxr-xr-x   0        0        0      200 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/__main__.py
--rw-r--r--   0        0        0     3350 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/cli.py
--rw-r--r--   0        0        0      318 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/console.py
--rw-r--r--   0        0        0      441 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/hello_world.py
--rw-r--r--   0        0        0      369 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/loc.py
--rw-r--r--   0        0        0      286 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/locale/base.pot
--rw-r--r--   0        0        0       97 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/locale/base.pot.license
--rw-r--r--   0        0        0      420 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       97 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po.license
--rw-r--r--   0        0        0      196 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/py.typed
--rw-r--r--   0        0        0      290 2023-03-22 09:25:58.033072 python_whiteprint-0.6.1/src/python_whiteprint/version.py
--rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 python_whiteprint-0.6.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-13 14:51:43.711629 python_whiteprint-0.7.0/LICENSES/
+-rw-r--r--   0        0        0     2917 2023-04-13 14:51:43.711629 python_whiteprint-0.7.0/README.md
+-rw-r--r--   0        0        0    30179 2023-04-13 14:52:09.680444 python_whiteprint-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/__init__.py
+-rwxr-xr-x   0        0        0      222 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/__main__.py
+-rw-r--r--   0        0        0      786 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/_callback.py
+-rw-r--r--   0        0        0      624 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/_click_app.py
+-rw-r--r--   0        0        0     1198 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/_logging.py
+-rw-r--r--   0        0        0     2130 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/entrypoint.py
+-rw-r--r--   0        0        0    16875 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/init.py
+-rw-r--r--   0        0        0      417 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/cli/type.py
+-rw-r--r--   0        0        0      322 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/console.py
+-rw-r--r--   0        0        0     2789 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/git.py
+-rw-r--r--   0        0        0      474 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/loc.py
+-rw-r--r--   0        0        0      286 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/base.pot
+-rw-r--r--   0        0        0      100 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/base.pot.license
+-rw-r--r--   0        0        0      420 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      100 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/locale/fr_FR/LC_MESSAGES/messages.po.license
+-rw-r--r--   0        0        0     3137 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/nox.py
+-rw-r--r--   0        0        0      882 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/poetry.py
+-rw-r--r--   0        0        0      199 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/py.typed
+-rw-r--r--   0        0        0      294 2023-04-13 14:51:43.715628 python_whiteprint-0.7.0/src/python_whiteprint/version.py
+-rw-r--r--   0        0        0     4709 1970-01-01 00:00:00.000000 python_whiteprint-0.7.0/PKG-INFO
```

### Comparing `python_whiteprint-0.6.1/README.md` & `python_whiteprint-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--
-SPDX-FileCopyrightText: 2023 Romain Brault <mail@romainbrault.com>
+SPDX-FileCopyrightText: © 2023 Romain Brault <mail@romainbrault.com>
 
 SPDX-License-Identifier: MIT
 -->
 
 # Python Whiteprint
 
 [![PyPI Version](https://img.shields.io/pypi/v/python-whiteprint.svg)](https://pypi.python.org/pypi/python-whiteprint)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python_whiteprint-0.6.1/pyproject.toml` & `python_whiteprint-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# SPDX-FileCopyrightText: 2023 Romain Brault <mail@romainbrault.com>
+# SPDX-FileCopyrightText: © 2023 Romain Brault <mail@romainbrault.com>
 #
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
 name = "python_whiteprint"
-version = "0.6.1"
+version = "0.7.0"
 description = "Generating Python projects using best practices"
 authors = [
     "Romain Brault <mail@romainbrault.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RomainBrault/python-whiteprint"
@@ -39,89 +39,97 @@
 [tool.poetry.dependencies]
 # Some packages, such as scipy, constrain their upper bound of Python versions
 # they support. Without also constraining the upper bound here, Poetry will not
 # select those versions and will result in an old version being
 # resolved/locked.
 python = ">=3.8, <3.12"
 rich = ">=12.5.0"
-typer = { version = ">=0.7.0", extras = ["all"] }
-beartype = ">=0.12.0"
-copier = ">=7.0.1"
+typer = ">=0.7.0"
+colorama = ">=0.4.3"
+shellingham = ">=1.3.0"
+beartype = ">=0.13.0"
+copier = ">=7.1.0"
 jinja2-time = ">=0.2.0"
+pygit2 = ">=1.11.1"
+python-slugify = ">=8.0.1"
+nox-poetry = ">=1.0.2"
+poetry = ">=1.4.2"
+virtualenv = "=20.16.5"
+typing-extensions = ">=4.5.0"
 
 [tool.poetry.group.localization.dependencies]
 Babel = ">=2.12.0"
 
 [tool.poetry.group.test.dependencies]
-xdoctest = "*"
-hypothesis = "*"
+xdoctest = ">=1.1.0"
+hypothesis = ">=6.71.0"
 pytest = ">=7.2.0"
-pytest-cov = "*"
-pytest-sugar = "*"
-pytest-randomly = "*"
-pytest-html = "*"
-pytest-xdist = "*"
+pytest-cov = ">=4.0.0"
+pytest-sugar = ">=0.9.7"
+pytest-randomly = ">=3.12.0"
+pytest-html = ">=3.2.0"
+pytest-xdist = ">=3.2.1"
 
 [tool.poetry.group.coverage.dependencies]
-pygments = "*"
-coverage = { version = "*", extras = ["toml"] }
+pygments = ">=2.15.0"
+coverage = { version = ">=7.2.3", extras = ["toml"] }
 
 [tool.poetry.group.profile.dependencies]
-scalene = "*"
+scalene = ">=1.5.19"
 
 [tool.poetry.group.complexity.dependencies]
-radon = "*"
-xenon = "*"
+radon = ">=5.1.0"
+xenon = ">=0.9.0"
 
 [tool.poetry.group.debug.dependencies]
-ipdb = "*"
-pdbpp = "*"
+ipdb = ">=0.13.13"
+pdbpp = ">=0.10.3"
 
 [tool.poetry.group.type_check.dependencies]
-mypy = "*"
+mypy = ">=1.2.0"
 # As of mypy 0.900, mypy no longer bundles the stubs for third-party libraries
 # that reside in the typeshed project. Add these "types-" packages here if you
 # depend on them in requirements.in (e.g. types-requests).
 # See: http://mypy-lang.blogspot.com/2021/06/mypy-0900-released.html
 #      https://github.com/python/typeshed/tree/master/stubs
+types-python-slugify = ">=8.0.0"
+types-PyYAML = ">=6.0.12"
 
 [tool.poetry.group.lint.dependencies]
-bandit = "*"
-pip-audit = "*"
-reuse = "*"
-tryceratops = "*"
-python-lsp-server = {extras = ["pylint"], version = "*"}
+bandit = ">=1.7.5"
+pip-audit = ">=2.5.4"
+reuse = ">=1.1.2"
+tryceratops = ">=1.1.0"
+python-lsp-server = {extras = ["pylint"], version = ">=1.7.2"}
 
 [tool.poetry.group.fmt.dependencies]
-black = "*"
-blacken-docs = "*"
-isort = "*"
-pyupgrade = "*"
-ruff = "*"
-python-lsp-ruff = "*"
+black = ">=23.3.0"
+blacken-docs = ">=1.13.0"
+ruff = ">=0.0.261"
+python-lsp-ruff = ">=1.4.0"
 
 [tool.poetry.group.pre-commit.dependencies]
-pre-commit = "*"
-pre-commit-hooks = "*"
+pre-commit = ">=3.2.2"
+pre-commit-hooks = ">=4.4.0"
 
 [tool.poetry.group.editors.dependencies]
-pynvim = "*"
+pynvim = ">=0.4.3"
 
 [tool.poetry.group.docs.dependencies]
-furo = "*"
-sphinx = "*"
-myst-parser = "*"
-sphinx-autobuild = "*"
-sphinx-autoapi = "*"
-sphinx-click = "*"
-sphinxcontrib-napoleon = "*"
-sphinxcontrib-spelling = "*"
+furo = ">=2023.3.27"
+sphinx = ">=6.1.3"
+myst-parser = ">=1.0.0"
+sphinx-autobuild = ">=2021.3.14"
+sphinx-autoapi = ">=2.1.0"
+sphinx-click = ">=4.4.0"
+sphinxcontrib-napoleon = ">=0.7"
+sphinxcontrib-spelling = ">=8.0.0"
 
 [tool.poetry.scripts]
-whiteprint = "python_whiteprint.cli:app"
+whiteprint = "python_whiteprint.cli.entrypoint:app"
 
 [build-system]
 requires = ["poetry-core", "Babel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit.assert_used]
 skips = ["*_test.py", "*/test_*.py"]
@@ -198,34 +206,32 @@
 xfail_strict = true
 filterwarnings = [
     # When running tests, treat warnings as errors (e.g. -Werror). See:
     # https://docs.pytest.org/en/latest/reference/reference.html#confval-filterwarnings
     "error",
     # Add additional warning supressions as needed here. For example, if a
     # third-party library is throwing a deprecation warning that needs to be
-    # fixed upstream: "ignore::DeprecationWarning:typer",
+    # fixed upstream:
+    "ignore:read_binary is deprecated:DeprecationWarning:",
+    # Concerns only python 3.11. Poetry need to update virtualenv dependency...
 ]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["python_whiteprint", "tests"]
-omit = ["**/__main__.py"]
+omit = ["**/__main__.py", "/tmp/**"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 100
 
-[tool.isort]
-profile = "black"
-lines_after_imports = 2
-
 [tool.ruff]
 select = [
     "F",      # pyflakes
     "E",      # pycodestyle
     "W",    # pycodestyle
     "C90",  # mccabe
     "I",    # isort
@@ -247,32 +253,40 @@
     "EXE",  # flake8-executable
     "ISC",  # flake8-implicit-str-concat
     "ICN",  # flake8-import-conventions
     "G",    # flake8-logging-format
     "INP",  # flake8-no-pep420
     "PIE",  # flake8-pie
     "T20",  # flake8-print
+    "PYI",  # flake8-pyi
     "PT",   # flake8-pytest-style
     "Q",    # flake8-quotes
     "RET",  # flake8-return
+    "SLF",  # flake8-self
     "SIM",  # flake8-simplify
     "TID",  # flake8-tidy-imports
     "TCH",  # flake8-type-checking
+    "INT",  # flake8-gettext
     "ARG",  # flake8-unused-arguments
     "PTH",  # flake8-use-pathlib
     "ERA",  # eradicate
     "PD",   # pandas-vet
     "PGH",  # pygrep-hooks
     "PL",   # pylint
+    "PLC",  # Convention
+    "PLE",  # Error
+    "PLR",  # Refactor
+    "PLW",  # Warning
     "TRY",  # tryceratops
     "RSE",  # flake8-raise
+    "NPY",  # Numpy
     "RUF",  # ruff-specific rules
 ]
 
-ignore = []
+ignore = ["ANN101"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = [
     "F",      # pyflakes
     "E",      # pycodestyle
     "W",    # pycodestyle
     "I",    # isort
@@ -283,24 +297,30 @@
     # "COM",  # flake8-commas
     "C4",   # flake8-comprehensions
     "DTZ",  # flake8-datetimez
     "EXE",  # flake8-executable
     "G",    # flake8-logging-format
     "PIE",  # flake8-pie
     # "T20",  # flake8-print
+    "PYI",  # flake8-pyi
     "PT",   # flake8-pytest-style
     "Q",    # flake8-quotes
     "RET",  # flake8-return
     "SIM",  # flake8-simplify
     "TID",  # flake8-tidy-imports
     "TCH",  # flake8-type-checking
     # "ERA",  # eradicate
     # "PD",   # pandas-vet
     "PL",   # pylint
+    "PLC",  # Convention
+    "PLE",  # Error
+    "PLR",  # Refactor
     "TRY",  # tryceratops
+    "RSE",  # flake8-raise
+    "NPY",  # Numpy
     "RUF",  # ruff-specific rules
 ]
 unfixable = []
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
@@ -368,15 +388,15 @@
 # run arbitrary code.
 # extension-pkg-allow-list =
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code. (This is an alternative name to extension-pkg-allow-list
 # for backward compatibility.)
-# extension-pkg-whitelist =
+extension-pkg-whitelist = ["pygit2"]
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 # fail-on =
 
 # Specify a score threshold under which the program will exit with error.
@@ -628,15 +648,15 @@
 overgeneral-exceptions = ["builtins.BaseException", "builtins.Exception"]
 
 [tool.pylint.format]
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 # expected-line-ending-format =
 
 # Regexp for a line that is allowed to be longer than the limit.
-ignore-long-lines = "^\\s*(# )?<?https?://\\S+>?$"
+ignore-long-lines = "^\\s*(#)?<?https?://\\S+>?$|^\\s*(\\w*\\s*=\\s*)?(\"|').*(\"|'),?\\s*$"
 
 # Number of spaces of indent required inside a hanging or continued line.
 indent-after-paren = 4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string = "    "
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python_whiteprint-0.6.1/PKG-INFO` & `python_whiteprint-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-whiteprint
-Version: 0.6.1
+Version: 0.7.0
 Summary: Generating Python projects using best practices
 Home-page: https://github.com/RomainBrault/python-whiteprint
 License: MIT
 Keywords: Python,Cookiecutter
 Author: Romain Brault
 Author-email: mail@romainbrault.com
 Requires-Python: >=3.8,<3.12
@@ -21,25 +21,33 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
-Requires-Dist: beartype (>=0.12.0)
-Requires-Dist: copier (>=7.0.1)
+Requires-Dist: beartype (>=0.13.0)
+Requires-Dist: colorama (>=0.4.3)
+Requires-Dist: copier (>=7.1.0)
 Requires-Dist: jinja2-time (>=0.2.0)
+Requires-Dist: nox-poetry (>=1.0.2)
+Requires-Dist: poetry (>=1.4.2)
+Requires-Dist: pygit2 (>=1.11.1)
+Requires-Dist: python-slugify (>=8.0.1)
 Requires-Dist: rich (>=12.5.0)
-Requires-Dist: typer[all] (>=0.7.0)
+Requires-Dist: shellingham (>=1.3.0)
+Requires-Dist: typer (>=0.7.0)
+Requires-Dist: typing-extensions (>=4.5.0)
+Requires-Dist: virtualenv (==20.16.5)
 Project-URL: Documentation, https://RomainBrault.github.io/python-whiteprint/
 Project-URL: Repository, https://github.com/RomainBrault/python-whiteprint.git
 Description-Content-Type: text/markdown
 
 <!--
-SPDX-FileCopyrightText: 2023 Romain Brault <mail@romainbrault.com>
+SPDX-FileCopyrightText: © 2023 Romain Brault <mail@romainbrault.com>
 
 SPDX-License-Identifier: MIT
 -->
 
 # Python Whiteprint
 
 [![PyPI Version](https://img.shields.io/pypi/v/python-whiteprint.svg)](https://pypi.python.org/pypi/python-whiteprint)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

