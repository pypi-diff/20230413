# Comparing `tmp/idf-build-apps-0.5.2.tar.gz` & `tmp/idf-build-apps-0.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf-build-apps-0.5.2.tar", last modified: Fri Apr  7 02:55:57 2023, max compression
+gzip compressed data, was "idf-build-apps-0.6.0rc0.tar", last modified: Thu Apr 13 04:29:49 2023, max compression
```

## Comparing `idf-build-apps-0.5.2.tar` & `idf-build-apps-0.6.0rc0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0      351 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.editorconfig
--rw-r--r--   0        0        0      123 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.gitattributes
--rw-r--r--   0        0        0      253 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-04-07 02:55:53.554697 idf-build-apps-0.5.2/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3707 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/.gitignore
--rw-r--r--   0        0        0     1077 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/.readthedocs.yml
--rw-r--r--   0        0        0     2923 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     1834 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/LICENSE
--rw-r--r--   0        0        0     3843 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/README.md
--rw-r--r--   0        0        0       33 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/conf.py
--rw-r--r--   0        0        0    10368 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/find-build.md
--rw-r--r--   0        0        0      459 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/index.rst
--rw-r--r--   0        0        0     3651 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/docs/manifest.md
--rw-r--r--   0        0        0      483 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    21914 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/app.py
--rw-r--r--   0        0        0     2187 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6026 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/finder.py
--rw-r--r--   0        0        0     1359 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/log.py
--rw-r--r--   0        0        0    26258 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     5547 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5322 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     7459 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/license_header.txt
--rw-r--r--   0        0        0     1837 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0     2181 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/tests/test_build.py
--rw-r--r--   0        0        0     7948 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/tests/test_finder.py
--rw-r--r--   0        0        0      995 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/tests/test_manifest.py
--rw-r--r--   0        0        0     2394 2023-04-07 02:55:53.558697 idf-build-apps-0.5.2/tests/test_utils.py
--rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 idf-build-apps-0.5.2/setup.py
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 idf-build-apps-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.editorconfig
+-rw-r--r--   0        0        0      123 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.gitattributes
+-rw-r--r--   0        0        0      253 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3707 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.gitignore
+-rw-r--r--   0        0        0     1077 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.readthedocs.yml
+-rw-r--r--   0        0        0     3562 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     1834 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/LICENSE
+-rw-r--r--   0        0        0     3843 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/README.md
+-rw-r--r--   0        0        0       33 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/config_file.md
+-rw-r--r--   0        0        0    10368 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/docs/index.rst
+-rw-r--r--   0        0        0     3651 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/docs/manifest.md
+-rw-r--r--   0        0        0      487 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    21914 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2768 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2187 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6026 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     1359 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/log.py
+-rw-r--r--   0        0        0    28666 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     5547 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5322 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     7473 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/license_header.txt
+-rw-r--r--   0        0        0     1860 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0     2181 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_build.py
+-rw-r--r--   0        0        0     7948 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_finder.py
+-rw-r--r--   0        0        0      995 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_manifest.py
+-rw-r--r--   0        0        0     2394 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 idf-build-apps-0.6.0rc0/setup.py
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 idf-build-apps-0.6.0rc0/PKG-INFO
```

### Comparing `idf-build-apps-0.5.2/.github/workflows/issue_comment.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/.github/workflows/new_issues.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/.github/workflows/new_prs.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/.github/workflows/test-build-docs.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/.github/workflows/test-build-idf-apps.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/.gitignore` & `idf-build-apps-0.6.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/.pre-commit-config.yaml` & `idf-build-apps-0.6.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/CHANGELOG.md` & `idf-build-apps-0.6.0rc0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## Unreleased
+
+### Added
+
+- Support configuration file with
+  - `tool.idf-build-apps` section under `pyproject.toml` file
+  - `.idf_build_apps.toml` file
+- Improve help message, include default value, config name, and config type
+- Improve help message, add DeprecationWarning to change the CLI call method from "specify multiple times" to "space-separated list" for the following CLI options. (will be removed in 1.0.0)
+  - `--exclude`
+  - `--config`
+  - `--manifest-file`
+  - `--ignore-warning-str`
+
+### Fixed
+
+- Fix earlier python version pathlib does not support member function `expanduser` issue
+- Remove unused dependency `pyyaml`
+
 ## [0.5.2] (2023-04-07)
 
 ### Fixed
 
 - Remove empty expanded sdkconfig files folder after build
 - Split up expanded sdkconfig files folder for different build
```

### Comparing `idf-build-apps-0.5.2/CONTRIBUTING.md` & `idf-build-apps-0.6.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/LICENSE` & `idf-build-apps-0.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/README.md` & `idf-build-apps-0.6.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/docs/Makefile` & `idf-build-apps-0.6.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/docs/_static/espressif-logo.svg` & `idf-build-apps-0.6.0rc0/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/docs/_static/theme_overrides.css` & `idf-build-apps-0.6.0rc0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/docs/conf.py` & `idf-build-apps-0.6.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/docs/find-build.md` & `idf-build-apps-0.6.0rc0/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/docs/manifest.md` & `idf-build-apps-0.6.0rc0/docs/manifest.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/app.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/app.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/constants.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/finder.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/log.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/main.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+
 import argparse
 import os
 import re
 import shutil
 import sys
+import textwrap
 from pathlib import (
     Path,
 )
 
 from . import (
     LOGGER,
 )
 from .app import (
     App,
 )
+from .config import (
+    get_valid_config,
+)
 from .constants import (
     ALL_TARGETS,
 )
 from .finder import (
     _find_apps,
 )
 from .manifest.manifest import (
@@ -349,107 +354,162 @@
 
     if depends_on_components is not None:
         return exit_code, actual_built_apps
     else:
         return exit_code
 
 
+class IdfBuildAppsCliFormatter(argparse.HelpFormatter):
+    LINE_SEP = '$LINE_SEP$'
+
+    def _split_lines(self, text, width):
+        parts = text.split(self.LINE_SEP)
+
+        text = self._whitespace_matcher.sub(' ', parts[0]).strip()
+        return textwrap.wrap(text, width) + parts[1:]
+
+    def _get_help_string(self, action):
+        """
+        Add the default value to the option help message.
+
+        ArgumentDefaultsHelpFormatter and BooleanOptionalAction when it isn't
+        already present. This code will do that, detecting cornercases to
+        prevent duplicates or cases where it wouldn't make sense to the end
+        user.
+        """
+        _help = action.help
+        if _help is None:
+            _help = ''
+
+        if action.dest == 'config_file':
+            return _help
+
+        if action.default is not argparse.SUPPRESS:
+            if action.default is None:
+                default_type = str
+            else:
+                default_type = type(action.default)
+
+            if isinstance(action, argparse._AppendAction):  # noqa
+                _help += (
+                    '. Could be specified for multiple times'
+                    '{} ! DeprecationWarning: will change to space-separated list in idf-build-apps 1.0.0 version'.format(
+                        self.LINE_SEP
+                    )
+                )
+                _type = 'list[{}]'.format(default_type.__name__)
+            elif action.nargs in [argparse.ZERO_OR_MORE, argparse.ONE_OR_MORE]:
+                _type = 'list[{}]'.format(default_type.__name__)
+            else:
+                _type = default_type.__name__
+
+            defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
+            if action.option_strings or action.nargs in defaulting_nargs:
+                _help += '{} - default: %(default)s'.format(self.LINE_SEP)
+
+            _help += '{} - config name: {}'.format(self.LINE_SEP, action.dest)
+            _help += '{} - config type: {}'.format(self.LINE_SEP, _type)
+
+        return _help
+
+
 def main():
     parser = argparse.ArgumentParser(
         description='Tools for building ESP-IDF related apps.'
         'Some CLI options can be expanded by the following placeholders, like "--work-dir", "--build-dir", etc.:\n'
         '- @t: would be replaced by the target chip type\n'
         '- @w: would be replaced by the wildcard, usually the sdkconfig\n'
         '- @n: would be replaced by the app name\n'
         '- @f: would be replaced by the escaped app path (replaced "/" to "_")\n'
         '- @i: would be replaced by the build index',
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     actions = parser.add_subparsers(dest='action')
 
     common_args = argparse.ArgumentParser(add_help=False)
-    common_args.add_argument('-p', '--paths', nargs='+', help='One or more paths to look for apps.')
-    common_args.add_argument('-t', '--target', help='filter apps by given target.')
     common_args.add_argument(
-        '--build-system',
-        default='cmake',
-        choices=['cmake'],
-        help='build with given build system',
+        '-c',
+        '--config-file',
+        help='Path to the default configuration file, toml file',
+    )
+
+    common_args.add_argument('-p', '--paths', nargs='+', help='One or more paths to look for apps')
+    common_args.add_argument('-t', '--target', help='filter apps by given target')
+    common_args.add_argument(
+        '--build-system', default='cmake', choices=['cmake'], help='filter apps by given build system'
     )
     common_args.add_argument(
         '--recursive',
         action='store_true',
-        help='Look for apps in the specified directories recursively.',
+        help='Look for apps in the specified paths recursively',
     )
     common_args.add_argument(
         '--exclude',
         action='append',
-        help='Ignore specified directory (if --recursive is given). Can be used multiple times.',
+        help='Ignore specified directory (if --recursive is given)',
     )
     common_args.add_argument(
         '--work-dir',
         help='If set, the app is first copied into the specified directory, and then built. '
-        'If not set, the work directory is the directory of the app. Can expand placeholders.',
+        'If not set, the work directory is the directory of the app. Can expand placeholders',
     )
     common_args.add_argument(
         '--build-dir',
-        help='If set, specifies the build directory name. Can expand placeholders. Can be either a '
-        'name relative to the work directory, or an absolute path.',
+        default='build',
+        help='If set, specifies the build directory name. Can be either a name relative to the work directory, '
+        'or an absolute path. Can expand placeholders',
     )
     common_args.add_argument(
         '--build-log',
-        help='Relative to build dir. The build log will be written to this file instead of sys.stdout if specified.'
-        'Can expand placeholders.',
+        help='Relative to build dir. The build log will be written to this file instead of sys.stdout if specified. Can expand placeholders',
     )
     common_args.add_argument(
         '--size-file',
-        help='Relative to build dir. The size json will be written to this file if specified. Can expand placeholders.',
+        help='Relative to build dir. The size json will be written to this file if specified. Can expand placeholders',
     )
     common_args.add_argument(
         '--config',
         action='append',
-        help='Adds configurations (sdkconfig file names) to build. Could be specified for multiple times.'
-        'This can either be '
-        'FILENAME[=NAME] or FILEPATTERN. FILENAME is the name of the sdkconfig file, '
+        help='Adds configurations (sdkconfig file names) to build. '
+        'This can either be FILENAME[=NAME] or FILEPATTERN. FILENAME is the name of the sdkconfig file, '
         'relative to the project directory, to be used. Optional NAME can be specified, '
         'which can be used as a name of this configuration. FILEPATTERN is the name of '
         'the sdkconfig file, relative to the project directory, with at most one wildcard. '
-        'The part captured by the wildcard is used as the name of the configuration.',
+        'The part captured by the wildcard is used as the name of the configuration',
     )
     common_args.add_argument(
         '--sdkconfig-defaults',
         help='semicolon-separated string, pass to idf.py -DSDKCONFIG_DEFAULTS if specified, also could be set via '
         'environment variables "SDKCONFIG_DEFAULTS"',
     )
     common_args.add_argument(
         '-v',
         '--verbose',
         default=0,
         action='count',
-        help='Increase the logging level of the whole process. Can be specified multiple times.',
+        help='Increase the logging level of the whole process. Can be specified multiple times. '
+        'By default set to WARNING level. Specify once to set to INFO level. Specify twice or more to set to DEBUG level',
     )
     common_args.add_argument(
         '--log-file',
         type=argparse.FileType('w'),
-        help='Write the script log to the specified file, instead of stderr',
+        help='Write the log to the specified file, instead of stderr',
     )
     common_args.add_argument(
-        '--check-warnings',
-        action='store_true',
-        help='Check for warnings in the build output.',
+        '--check-warnings', action='store_true', help='If set, fail the build if warnings are found'
     )
     common_args.add_argument(
         '--manifest-file',
         action='append',
-        help='manifest file to specify the build test rules of the apps, could be specified multiple times.',
+        help='Manifest files which specify the build test rules of the apps',
     )
     common_args.add_argument(
         '--manifest-rootpath',
         help='Root directory for calculating the realpath of the relative path defined in the manifest files. '
-        'Would use the current directory if not set.',
+        'Would use the current directory if not set',
     )
     common_args.add_argument(
         '--default-build-targets',
         help='comma-separated list of supported targets. Targets supported in current ESP-IDF branch '
         '(except preview ones) would be used if this option is not set',
     )
     common_args.add_argument(
@@ -477,90 +537,91 @@
     )
     common_args.add_argument(
         '--no-color',
         action='store_true',
         help='enable colored output by default on UNIX-like systems. enable this flag to make the logs uncolored.',
     )
 
-    find_parser = actions.add_parser('find', parents=[common_args])
-    find_parser.add_argument(
-        '-o',
-        '--output',
-        help='Output the found apps to the specified file instead of sys.stdout.',
-    )
+    find_parser = actions.add_parser('find', parents=[common_args], formatter_class=IdfBuildAppsCliFormatter)
+    find_parser.add_argument('-o', '--output', help='Print the found apps to the specified file instead of stdout')
 
-    build_parser = actions.add_parser('build', parents=[common_args])
+    build_parser = actions.add_parser('build', parents=[common_args], formatter_class=IdfBuildAppsCliFormatter)
     build_parser.add_argument(
         '--build-verbose',
         action='store_true',
-        help='Enable verbose output from build system.',
+        help='Enable verbose output of the build system',
     )
     build_parser.add_argument(
         '--parallel-count',
         default=1,
         type=int,
-        help="Number of parallel build jobs. Note that this script doesn't start the jobs, "
-        + 'it needs to be executed multiple times with same value of --parallel-count and '
-        + 'different values of --parallel-index.',
+        help="Number of parallel build jobs. Note that this script doesn't start all jobs simultaneously. "
+        'It needs to be executed multiple times with same value of --parallel-count and '
+        'different values of --parallel-index',
     )
     build_parser.add_argument(
         '--parallel-index',
         default=1,
         type=int,
-        help='Index (1-based) of the job, out of the number specified by --parallel-count.',
+        help='Index (1-based) of the job, out of the number specified by --parallel-count',
     )
     build_parser.add_argument(
         '--dry-run',
         action='store_true',
         help="Don't actually build, only print the build commands",
     )
     build_parser.add_argument(
         '--keep-going',
         action='store_true',
-        help="Don't exit immediately when a build fails.",
+        help="Don't exit immediately when a build fails",
     )
     build_parser.add_argument(
         '--no-preserve',
         action='store_true',
-        help="Don't preserve the build directory after a successful build.",
+        help="Don't preserve the build directory after a successful build",
     )
     build_parser.add_argument(
         '--collect-size-info',
         type=argparse.FileType('w'),
-        help='write size info json file while building into the specified file. each line is a json object.',
+        help='write size info json file while building into the specified file. each line is a json object',
     )
     build_parser.add_argument(
         '--collect-app-info',
         type=argparse.FileType('w'),
-        help='write app info json file while building into the specified file. each line is a json object.',
+        help='write app info json file while building into the specified file. each line is a json object',
     )
     build_parser.add_argument(
         '--ignore-warning-str',
         action='append',
-        help='Ignore the warning string that match the specified regex in the build output. '
-        'Can be specified multiple times.',
+        help='Ignore the warning string that match the specified regex in the build output',
     )
     build_parser.add_argument(
         '--ignore-warning-file',
         type=argparse.FileType('r'),
-        help='Ignore the warning strings in the specified file. Each line should be a regex string.',
+        help='Ignore the warning strings in the specified file. Each line should be a regex string',
     )
     build_parser.add_argument(
         '--copy-sdkconfig',
         action='store_true',
-        help='Copy the sdkconfig file to the build directory.',
+        help='Copy the sdkconfig file to the build directory',
     )
 
     args = parser.parse_args()
 
-    # validate cli options
+    # validate cli subcommands
     if args.action not in ['find', 'build']:
         parser.print_help()
         raise InvalidCommand('subcommand is required. {find, build}')
 
+    # support toml config file
+    config_dict = get_valid_config(custom_path=args.config_file)
+    if config_dict:
+        for k, v in config_dict.items():
+            setattr(args, k, v)
+
     if not args.paths:
         raise InvalidCommand(
             'Must specify at least one path to search for the apps ' 'with CLI option "-p <path>" or "--path <path>"'
         )
 
     if not args.target:
         raise InvalidCommand(
```

### Comparing `idf-build-apps-0.5.2/idf_build_apps/manifest/if_parser.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/manifest/manifest.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/manifest/soc_header.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/idf_build_apps/utils.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,17 +231,17 @@
     elif isinstance(s, list):
         return s
     else:
         return [s]
 
 
 def to_absolute_path(s, rootpath=None):  # type: (str, str | None) -> Path
-    rp = Path(rootpath or '.').expanduser().resolve()
+    rp = Path(os.path.expanduser(rootpath or '.')).resolve()
 
-    sp = Path(s).expanduser()
+    sp = Path(os.path.expanduser(s))
     if sp.is_absolute():
         return sp.resolve()
     else:
         return (rp / sp).resolve()
 
 
 def files_matches_patterns(
```

### Comparing `idf-build-apps-0.5.2/pyproject.toml` & `idf-build-apps-0.6.0rc0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 ]
 dynamic = ["version", "description"]
 requires-python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 
 dependencies = [
     "pathlib; python_version < '3.4'",
     "pyparsing",
-    "pyyaml",
     "packaging",
+    "toml; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
 ]
```

### Comparing `idf-build-apps-0.5.2/tests/conftest.py` & `idf-build-apps-0.6.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/tests/test_build.py` & `idf-build-apps-0.6.0rc0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/tests/test_finder.py` & `idf-build-apps-0.6.0rc0/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/tests/test_manifest.py` & `idf-build-apps-0.6.0rc0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/tests/test_utils.py` & `idf-build-apps-0.6.0rc0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.5.2/setup.py` & `idf-build-apps-0.6.0rc0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 packages = \
 ['idf_build_apps', 'idf_build_apps.manifest']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyparsing', 'pyyaml', 'packaging']
+['pyparsing', 'packaging']
 
 extras_require = \
-{":python_version < '3.4'": ['pathlib'],
+{":python_version < '3.11'": ['toml'],
+ ":python_version < '3.4'": ['pathlib'],
  'doc': ['sphinx',
          'sphinx-rtd-theme',
          'sphinx_copybutton',
          'myst-parser',
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='0.5.2',
+      version='0.6.0rc0',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf-build-apps-0.5.2/PKG-INFO` & `idf-build-apps-0.6.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 0.5.2
+Version: 0.6.0rc0
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pathlib; python_version < '3.4'
 Requires-Dist: pyparsing
-Requires-Dist: pyyaml
 Requires-Dist: packaging
+Requires-Dist: toml; python_version < '3.11'
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme ; extra == "doc"
 Requires-Dist: sphinx_copybutton ; extra == "doc"
 Requires-Dist: myst-parser ; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
```

