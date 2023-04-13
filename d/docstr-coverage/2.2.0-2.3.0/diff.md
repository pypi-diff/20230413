# Comparing `tmp/docstr-coverage-2.2.0.tar.gz` & `tmp/docstr-coverage-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstr-coverage-2.2.0.tar", last modified: Thu Mar 17 22:27:08 2022, max compression
+gzip compressed data, was "docstr-coverage-2.3.0.tar", last modified: Thu Apr 13 21:19:54 2023, max compression
```

## Comparing `docstr-coverage-2.2.0.tar` & `docstr-coverage-2.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2022-03-17 22:27:08.397409 docstr-coverage-2.2.0/
--rw-r--r--   0 Hunter     (501) staff       (20)     1075 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/LICENSE.txt
--rw-r--r--   0 Hunter     (501) staff       (20)      127 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/MANIFEST.in
--rw-r--r--   0 Hunter     (501) staff       (20)    10631 2022-03-17 22:27:08.397475 docstr-coverage-2.2.0/PKG-INFO
--rw-r--r--   0 Hunter     (501) staff       (20)     9565 2022-03-17 22:18:54.000000 docstr-coverage-2.2.0/README.md
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2022-03-17 22:27:08.395868 docstr-coverage-2.2.0/docstr_coverage/
--rw-r--r--   0 Hunter     (501) staff       (20)      552 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/__init__.py
--rw-r--r--   0 Hunter     (501) staff       (20)     3005 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/badge.py
--rw-r--r--   0 Hunter     (501) staff       (20)    13323 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/cli.py
--rw-r--r--   0 Hunter     (501) staff       (20)     2841 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/config_file.py
--rw-r--r--   0 Hunter     (501) staff       (20)    10817 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/coverage.py
--rw-r--r--   0 Hunter     (501) staff       (20)     2854 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/ignore_config.py
--rw-r--r--   0 Hunter     (501) staff       (20)     5564 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/printers.py
--rw-r--r--   0 Hunter     (501) staff       (20)    12005 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/result_collection.py
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2022-03-17 22:27:08.396641 docstr-coverage-2.2.0/docstr_coverage/templates/
--rw-r--r--   0 Hunter     (501) staff       (20)     1108 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/templates/flat.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     4805 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/docstr_coverage/visitor.py
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2022-03-17 22:27:08.396546 docstr-coverage-2.2.0/docstr_coverage.egg-info/
--rw-r--r--   0 Hunter     (501) staff       (20)    10631 2022-03-17 22:27:08.000000 docstr-coverage-2.2.0/docstr_coverage.egg-info/PKG-INFO
--rw-r--r--   0 Hunter     (501) staff       (20)      867 2022-03-17 22:27:08.000000 docstr-coverage-2.2.0/docstr_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 Hunter     (501) staff       (20)        1 2022-03-17 22:27:08.000000 docstr-coverage-2.2.0/docstr_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 Hunter     (501) staff       (20)       65 2022-03-17 22:27:08.000000 docstr-coverage-2.2.0/docstr_coverage.egg-info/entry_points.txt
--rw-r--r--   0 Hunter     (501) staff       (20)        1 2021-11-07 22:18:00.000000 docstr-coverage-2.2.0/docstr_coverage.egg-info/not-zip-safe
--rw-r--r--   0 Hunter     (501) staff       (20)      103 2022-03-17 22:27:08.000000 docstr-coverage-2.2.0/docstr_coverage.egg-info/requires.txt
--rw-r--r--   0 Hunter     (501) staff       (20)       16 2022-03-17 22:27:08.000000 docstr-coverage-2.2.0/docstr_coverage.egg-info/top_level.txt
--rw-r--r--   0 Hunter     (501) staff       (20)      269 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/pyproject.toml
--rw-r--r--   0 Hunter     (501) staff       (20)      132 2022-03-17 22:27:08.397722 docstr-coverage-2.2.0/setup.cfg
--rw-r--r--   0 Hunter     (501) staff       (20)     1665 2022-03-17 22:17:46.000000 docstr-coverage-2.2.0/setup.py
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2022-03-17 22:27:08.394275 docstr-coverage-2.2.0/tests/
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2022-03-17 22:27:08.394314 docstr-coverage-2.2.0/tests/sample_files/
-drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2022-03-17 22:27:08.397318 docstr-coverage-2.2.0/tests/sample_files/badges/
--rw-r--r--   0 Hunter     (501) staff       (20)     1084 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/tests/sample_files/badges/0.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1085 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/tests/sample_files/badges/100.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/tests/sample_files/badges/12.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/tests/sample_files/badges/54.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/tests/sample_files/badges/71.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/tests/sample_files/badges/84.svg
--rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.2.0/tests/sample_files/badges/94.svg
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2023-04-13 21:19:54.884399 docstr-coverage-2.3.0/
+-rw-r--r--   0 Hunter     (501) staff       (20)     1075 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/LICENSE.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)      127 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/MANIFEST.in
+-rw-r--r--   0 Hunter     (501) staff       (20)    10546 2023-04-13 21:19:54.884482 docstr-coverage-2.3.0/PKG-INFO
+-rw-r--r--   0 Hunter     (501) staff       (20)     9228 2023-04-13 21:16:23.000000 docstr-coverage-2.3.0/README.md
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2023-04-13 21:19:54.881783 docstr-coverage-2.3.0/docstr_coverage/
+-rw-r--r--   0 Hunter     (501) staff       (20)      552 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/docstr_coverage/__init__.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     3005 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/docstr_coverage/badge.py
+-rw-r--r--   0 Hunter     (501) staff       (20)    14135 2023-04-13 20:04:25.000000 docstr-coverage-2.3.0/docstr_coverage/cli.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     2841 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/docstr_coverage/config_file.py
+-rw-r--r--   0 Hunter     (501) staff       (20)    11206 2023-04-13 20:04:25.000000 docstr-coverage-2.3.0/docstr_coverage/coverage.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     2854 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/docstr_coverage/ignore_config.py
+-rw-r--r--   0 Hunter     (501) staff       (20)     5564 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/docstr_coverage/printers.py
+-rw-r--r--   0 Hunter     (501) staff       (20)    12005 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/docstr_coverage/result_collection.py
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2023-04-13 21:19:54.883072 docstr-coverage-2.3.0/docstr_coverage/templates/
+-rw-r--r--   0 Hunter     (501) staff       (20)     1108 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/docstr_coverage/templates/flat.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     5032 2023-04-13 20:04:25.000000 docstr-coverage-2.3.0/docstr_coverage/visitor.py
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2023-04-13 21:19:54.882942 docstr-coverage-2.3.0/docstr_coverage.egg-info/
+-rw-r--r--   0 Hunter     (501) staff       (20)    10546 2023-04-13 21:19:54.000000 docstr-coverage-2.3.0/docstr_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 Hunter     (501) staff       (20)      867 2023-04-13 21:19:54.000000 docstr-coverage-2.3.0/docstr_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)        1 2023-04-13 21:19:54.000000 docstr-coverage-2.3.0/docstr_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)       65 2023-04-13 21:19:54.000000 docstr-coverage-2.3.0/docstr_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)        1 2021-11-07 22:18:00.000000 docstr-coverage-2.3.0/docstr_coverage.egg-info/not-zip-safe
+-rw-r--r--   0 Hunter     (501) staff       (20)      117 2023-04-13 21:19:54.000000 docstr-coverage-2.3.0/docstr_coverage.egg-info/requires.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)       16 2023-04-13 21:19:54.000000 docstr-coverage-2.3.0/docstr_coverage.egg-info/top_level.txt
+-rw-r--r--   0 Hunter     (501) staff       (20)      269 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/pyproject.toml
+-rw-r--r--   0 Hunter     (501) staff       (20)      132 2023-04-13 21:19:54.884757 docstr-coverage-2.3.0/setup.cfg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1929 2023-04-13 20:11:13.000000 docstr-coverage-2.3.0/setup.py
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2023-04-13 21:19:54.879573 docstr-coverage-2.3.0/tests/
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2023-04-13 21:19:54.879614 docstr-coverage-2.3.0/tests/sample_files/
+drwxr-xr-x   0 Hunter     (501) staff       (20)        0 2023-04-13 21:19:54.884270 docstr-coverage-2.3.0/tests/sample_files/badges/
+-rw-r--r--   0 Hunter     (501) staff       (20)     1084 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/tests/sample_files/badges/0.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1085 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/tests/sample_files/badges/100.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/tests/sample_files/badges/12.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/tests/sample_files/badges/54.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/tests/sample_files/badges/71.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/tests/sample_files/badges/84.svg
+-rw-r--r--   0 Hunter     (501) staff       (20)     1086 2021-11-05 17:40:10.000000 docstr-coverage-2.3.0/tests/sample_files/badges/94.svg
```

### Comparing `docstr-coverage-2.2.0/LICENSE.txt` & `docstr-coverage-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/PKG-INFO` & `docstr-coverage-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: docstr-coverage
-Version: 2.2.0
+Version: 2.3.0
 Summary: Utility for examining python source files to ensure proper documentation. Lists missing docstrings, and calculates overall docstring coverage percentage rating.
 Home-page: https://github.com/HunterMcGushion/docstr_coverage
 Author: Hunter McGushion
 Author-email: hunter@mcgushion.com
 License: MIT
 Keywords: docstring coverage documentation audit source code statistics report
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -113,35 +118,25 @@
 - _--verbose=\<level\>, -v \<level\>_ - Set verbosity level (0-3, default: 3)
   - 0 - Silence
   - 1 - Print overall statistics
   - 2 - Also print individual statistics for each file
   - 3 - Also print missing docstrings (function names, class names, etc.)
   - 4 - Also print information about present docstrings
 - _--fail-under=<int|float>, -F <int|float>_ - Fail if under a certain percentage of coverage (default: 100.0)
-- _--docstr-ignore-file=\<filepath\>, -d \<filepath\>_ - Filepath containing list of patterns to ignore. Patterns are (file-pattern, name-pattern) pairs
-  - File content example:
-
-  ```
-  SomeFile method_to_ignore1 method_to_ignore2 method_to_ignore3
-  FileWhereWeWantToIgnoreAllSpecialMethods __.+__
-  .* method_to_ignore_in_all_files
-  a_very_important_view_file ^get$ ^set$ ^post$
-  detect_.* get_val.*
-  ```
 - _--badge=\<filepath\>, -b \<filepath\>_ - Generate a docstring coverage percent badge as an SVG saved to a given filepath
   - Include the badge in a repo's README using 
   ```[![docstr_coverage](<filepath/of/your/saved/badge.svg>)](https://github.com/HunterMcGushion/docstr_coverage)```,
   where `<filepath/of/your/saved/badge.svg>` is the path provided to the `--badge` option
 - _--follow-links, -l_ - Follow symlinks
 - _--percentage-only, -p_ - Output only the overall coverage percentage as a float, silencing all other logging
 - _--help, -h_ - Display CLI options
 
 #### Config File
 All options can be saved in a config file. A file named `.docstr.yaml` in the folder in which `docstr-coverage` is executed is picked up automatically. 
-Other locations can be passed using `docstr-coverage -C path/to/config.json` or the long version `--config`.
+Other locations can be passed using `docstr-coverage -C path/to/config.yml` or the long version `--config`.
 
 Example:
 ```yaml
 paths: # list or string
   - docstr_coverage
 badge: docs # Path
 exclude: .*/test # regex
@@ -173,16 +168,18 @@
 equivalent to
 ```
 docstr-coverage docstr_coverage -e ".*/test" --skip-magic --skip-init --badge="docs" --skip-class-def etc...
 ```
 
 Note that options passed as command line arguments have precedence over options 
 configured in a config file.
-Exception: If a `--docstr-ignore-file` is present and the yml config contains `ignore_patterns`,
-a `ValueError` is raised.
+
+#### Ignoring by Regex
+In your config files, using `ignore_patterns`, you can specify regex patterns for files names and nodes (methods, ...)
+which should be ignored. See config file example above.
 
 #### Overriding by Comments
 Note that `docstr-coverage` can not parse 
 dynamically added documentation (e.g. through class extension).
 Thus, some of your code which deliberately has no docstring might be counted as uncovered.
 
 You can override this by adding either ```# docstr-coverage:inherited``` 
@@ -207,15 +204,15 @@
 and configuring the `paths` section of the [`.docstr.yaml` config](#config-file). 
  This is preferrable over [pre-commit args](https://pre-commit.com/#config-args), 
  as it facilitates the use of the same config in CI, pre-commit and manual runs.
 
 ```yaml
 repos:
   - repo: https://github.com/HunterMcGushion/docstr_coverage
-    rev: v2.2.0 # most recent docstr-coverage release or commit sha
+    rev: v2.3.0 # most recent docstr-coverage release or commit sha
     hooks:
       - id: docstr-coverage
         args: ["--verbose", "2"] # override the .docstr.yaml to see less output
 ```
 
 #### Package in Your Project
```

### Comparing `docstr-coverage-2.2.0/README.md` & `docstr-coverage-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -88,35 +88,25 @@
 - _--verbose=\<level\>, -v \<level\>_ - Set verbosity level (0-3, default: 3)
   - 0 - Silence
   - 1 - Print overall statistics
   - 2 - Also print individual statistics for each file
   - 3 - Also print missing docstrings (function names, class names, etc.)
   - 4 - Also print information about present docstrings
 - _--fail-under=<int|float>, -F <int|float>_ - Fail if under a certain percentage of coverage (default: 100.0)
-- _--docstr-ignore-file=\<filepath\>, -d \<filepath\>_ - Filepath containing list of patterns to ignore. Patterns are (file-pattern, name-pattern) pairs
-  - File content example:
-
-  ```
-  SomeFile method_to_ignore1 method_to_ignore2 method_to_ignore3
-  FileWhereWeWantToIgnoreAllSpecialMethods __.+__
-  .* method_to_ignore_in_all_files
-  a_very_important_view_file ^get$ ^set$ ^post$
-  detect_.* get_val.*
-  ```
 - _--badge=\<filepath\>, -b \<filepath\>_ - Generate a docstring coverage percent badge as an SVG saved to a given filepath
   - Include the badge in a repo's README using 
   ```[![docstr_coverage](<filepath/of/your/saved/badge.svg>)](https://github.com/HunterMcGushion/docstr_coverage)```,
   where `<filepath/of/your/saved/badge.svg>` is the path provided to the `--badge` option
 - _--follow-links, -l_ - Follow symlinks
 - _--percentage-only, -p_ - Output only the overall coverage percentage as a float, silencing all other logging
 - _--help, -h_ - Display CLI options
 
 #### Config File
 All options can be saved in a config file. A file named `.docstr.yaml` in the folder in which `docstr-coverage` is executed is picked up automatically. 
-Other locations can be passed using `docstr-coverage -C path/to/config.json` or the long version `--config`.
+Other locations can be passed using `docstr-coverage -C path/to/config.yml` or the long version `--config`.
 
 Example:
 ```yaml
 paths: # list or string
   - docstr_coverage
 badge: docs # Path
 exclude: .*/test # regex
@@ -148,16 +138,18 @@
 equivalent to
 ```
 docstr-coverage docstr_coverage -e ".*/test" --skip-magic --skip-init --badge="docs" --skip-class-def etc...
 ```
 
 Note that options passed as command line arguments have precedence over options 
 configured in a config file.
-Exception: If a `--docstr-ignore-file` is present and the yml config contains `ignore_patterns`,
-a `ValueError` is raised.
+
+#### Ignoring by Regex
+In your config files, using `ignore_patterns`, you can specify regex patterns for files names and nodes (methods, ...)
+which should be ignored. See config file example above.
 
 #### Overriding by Comments
 Note that `docstr-coverage` can not parse 
 dynamically added documentation (e.g. through class extension).
 Thus, some of your code which deliberately has no docstring might be counted as uncovered.
 
 You can override this by adding either ```# docstr-coverage:inherited``` 
@@ -182,15 +174,15 @@
 and configuring the `paths` section of the [`.docstr.yaml` config](#config-file). 
  This is preferrable over [pre-commit args](https://pre-commit.com/#config-args), 
  as it facilitates the use of the same config in CI, pre-commit and manual runs.
 
 ```yaml
 repos:
   - repo: https://github.com/HunterMcGushion/docstr_coverage
-    rev: v2.2.0 # most recent docstr-coverage release or commit sha
+    rev: v2.3.0 # most recent docstr-coverage release or commit sha
     hooks:
       - id: docstr-coverage
         args: ["--verbose", "2"] # override the .docstr.yaml to see less output
 ```
 
 #### Package in Your Project
```

### Comparing `docstr-coverage-2.2.0/docstr_coverage/__init__.py` & `docstr-coverage-2.3.0/docstr_coverage/__init__.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/docstr_coverage/badge.py` & `docstr-coverage-2.3.0/docstr_coverage/badge.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/docstr_coverage/cli.py` & `docstr-coverage-2.3.0/docstr_coverage/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,23 +199,14 @@
     "-P",
     "--skip-private",
     is_flag=True,
     help="Ignore docstrings of functions starting with a single underscore",
 )
 @click.option("-l", "--follow-links", is_flag=True, help="Follow symlinks")
 @click.option(
-    "-d",
-    "--docstr-ignore-file",
-    "ignore_names_file",  # TODO: Remove after deprecating in favor of pyproject.toml `blacklist`
-    type=click.Path(exists=False, resolve_path=True),
-    default=".docstr_coverage",
-    help="Filepath containing list of regex (file-pattern, name-pattern) pairs",
-    show_default=True,
-)
-@click.option(
     "-F",
     "--fail-under",
     type=float,
     default=100.0,
     help="Fail when coverage % is less than a given amount",
     show_default=True,
     metavar="NUMBER",
@@ -258,33 +249,26 @@
 )
 @click.option("--skipmagic", is_flag=True, help="Deprecated. Use --skip-magic")
 @click.option("--skipfiledoc", is_flag=True, help="Deprecated. Use --skip-file-doc")
 @click.option("--skipinit", is_flag=True, help="Deprecated. Use --skip-init")
 @click.option("--skipclassdef", is_flag=True, help="Deprecated. Use --skip-class-def")
 @click.option("--followlinks", is_flag=True, help="Deprecated. Use --follow-links")
 @click.option("--failunder", type=float, help="Deprecated. Use --fail-under")
+@click.option(
+    "-d",
+    "--docstr-ignore-file",
+    "ignore_names_file",
+    type=click.Path(exists=False, resolve_path=True),
+    default=".docstr_coverage",
+    help="Deprecated. Use json config (--config / -C) instead",
+)
 def execute(paths, **kwargs):
     """Measure docstring coverage for `PATHS`"""
-    for deprecated_name, name in [
-        ("skipmagic", "skip_magic"),
-        ("skipfiledoc", "skip_file_doc"),
-        ("skipinit", "skip_init"),
-        ("skipclassdef", "skip_class_def"),
-        ("followlinks", "follow_links"),
-    ]:
-        if kwargs.get(deprecated_name):
-            new_flag = name.replace("_", "-")
-            if kwargs.get(name):
-                raise ValueError(
-                    "Should not set deprecated --{} and new --{}".format(deprecated_name, new_flag)
-                )
-            click.secho(
-                "Using deprecated --{}, should use --{}".format(deprecated_name, new_flag), fg="red"
-            )
-            kwargs[name] = kwargs.pop(deprecated_name)
+
+    _deprecation_alerts(kwargs)
 
     # handle fail under
     if kwargs.get("failunder") is not None:
         if kwargs.get("fail_under") != 100.0:
             raise ValueError("Should not set deprecated --failunder and --fail-under")
         click.secho("Using deprecated --failunder, should use --fail-under", fg="red")
         kwargs["fail_under"] = kwargs.pop("failunder")
@@ -313,15 +297,15 @@
 
     # Parse ignore names file
     has_ignore_patterns_in_config = "ignore_patterns" in kwargs
     if os.path.isfile(kwargs["ignore_names_file"]) and has_ignore_patterns_in_config:
         raise ValueError(
             (
                 "The docstr-coverage configuration file {} contains ignore_patterns,"
-                " and at the same time an ignore file {} was found."
+                " and at the same time a (deprecated) ignore file {} was found."
                 " Ignore patterns must be specified in only one location at a time."
             ).format(kwargs["config_file"], kwargs["ignore_names_file"])
         )
     elif os.path.isfile(kwargs["ignore_names_file"]):
         ignore_names = parse_ignore_names_file(kwargs["ignore_names_file"])
     elif has_ignore_patterns_in_config:
         ignore_names = parse_ignore_patterns_from_dict(kwargs["ignore_patterns"])
@@ -337,15 +321,16 @@
         skip_property=kwargs["skip_property"],
         skip_setter=not kwargs["include_setter"],
         skip_deleter=not kwargs["include_deleter"],
         ignore_names=ignore_names,
     )
 
     # Calculate docstring coverage
-    results = analyze(all_paths, ignore_config=ignore_config)
+    show_progress = not kwargs["percentage_only"]
+    results = analyze(all_paths, ignore_config=ignore_config, show_progress=show_progress)
 
     LegacyPrinter(verbosity=kwargs["verbose"], ignore_config=ignore_config).print(results)
 
     file_results, total_results = results.to_legacy()
 
     # Save badge
     if kwargs["badge"]:
@@ -361,9 +346,49 @@
     # Exit
     if total_results["coverage"] < kwargs["fail_under"]:
         raise SystemExit(1)
 
     raise SystemExit(0)
 
 
+def _deprecation_alerts(kwargs):
+    """Warns users if they are using deprecated flags"""
+    for deprecated_name, name in [
+        ("skipmagic", "skip_magic"),
+        ("skipfiledoc", "skip_file_doc"),
+        ("skipinit", "skip_init"),
+        ("skipclassdef", "skip_class_def"),
+        ("followlinks", "follow_links"),
+    ]:
+        if kwargs.get(deprecated_name):
+            new_flag = name.replace("_", "-")
+            if kwargs.get(name):
+                raise ValueError(
+                    "Should not set deprecated --{} and new --{}".format(deprecated_name, new_flag)
+                )
+            click.secho(
+                "Using deprecated --{}, should use --{}".format(deprecated_name, new_flag), fg="red"
+            )
+            kwargs[name] = kwargs.pop(deprecated_name)
+
+    # Deprecated old ignore files
+    ignore_file_old_casing = kwargs.get("docstr-ignore-file")
+    ignore_file_new_casing = kwargs.get("ignore_names_file")
+
+    def _nondefault_or_existing_file(path):
+        if path is None:
+            return False
+        return os.path.split(path)[-1] != ".docstr_coverage" or os.path.isfile(path)
+
+    if _nondefault_or_existing_file(ignore_file_old_casing) or _nondefault_or_existing_file(
+        ignore_file_new_casing
+    ):
+        click.secho(
+            "Using deprecated ignore files."
+            "We'll keep them supported for a while, "
+            "but we recommend switching to a proper config file "
+            "(see commands -C / --config)"
+        )
+
+
 if __name__ == "__main__":
     execute()
```

### Comparing `docstr-coverage-2.2.0/docstr_coverage/config_file.py` & `docstr-coverage-2.3.0/docstr_coverage/config_file.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/docstr_coverage/coverage.py` & `docstr-coverage-2.3.0/docstr_coverage/coverage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """The central module for coverage collection and file-walking"""
 
 import os
 import re
 from ast import parse
 from typing import Dict, List, Optional, Tuple
 
+from tqdm import tqdm
+
 from docstr_coverage.ignore_config import IgnoreConfig
 from docstr_coverage.printers import LegacyPrinter
 from docstr_coverage.result_collection import File, FileStatus, ResultCollection
 from docstr_coverage.visitor import DocStringCoverageVisitor
 
 
 def _do_ignore_node(filename: str, base_name: str, node_name: str, ignore_names: tuple) -> bool:
@@ -211,15 +213,17 @@
         ignore_names=ignore_names,
     )
     results = analyze(filenames, ignore_config)
     LegacyPrinter(verbosity=verbose, ignore_config=ignore_config).print(results)
     return results.to_legacy()
 
 
-def analyze(filenames: list, ignore_config: IgnoreConfig = IgnoreConfig()) -> ResultCollection:
+def analyze(
+    filenames: list, ignore_config: IgnoreConfig = IgnoreConfig(), show_progress=True
+) -> ResultCollection:
     """EXPERIMENTAL: More expressive alternative to `get_docstring_coverage`.
 
         Checks contents of `filenames` for missing docstrings, and produces a report detailing
     docstring status
 
     Note that this method, as well as its parameters and return types
         are still experimental and may change in future versions.
@@ -228,21 +232,34 @@
         ----------
         filenames: List
             List of filename strings that are absolute or relative paths
 
         ignore_config: IgnoreConfig
             Information about which docstrings are to be ignored
 
+        show_progress: Boolean, default=True
+            If True, prints a progress bar to stdout
+
     Returns
     -------
     ResultCollection
         The collected information about docstring presence"""
     results = ResultCollection()
 
-    for filename in filenames:
+    iterator = iter(filenames)
+    if show_progress:
+        iterator = tqdm(
+            iterator,
+            desc="Checking python files",
+            unit="files",
+            unit_scale=True,
+            total=len(filenames),
+        )
+
+    for filename in iterator:
         file_result = results.get_file(file_path=filename)
 
         ##################################################
         # Read and Parse Source
         ##################################################
         with open(filename, "r", encoding="utf-8") as f:
             source_tree = f.read()
```

### Comparing `docstr-coverage-2.2.0/docstr_coverage/ignore_config.py` & `docstr-coverage-2.3.0/docstr_coverage/ignore_config.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/docstr_coverage/printers.py` & `docstr-coverage-2.3.0/docstr_coverage/printers.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/docstr_coverage/result_collection.py` & `docstr-coverage-2.3.0/docstr_coverage/result_collection.py`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/docstr_coverage/templates/flat.svg` & `docstr-coverage-2.3.0/docstr_coverage/templates/flat.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/docstr_coverage/visitor.py` & `docstr-coverage-2.3.0/docstr_coverage/visitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 """This module handles traversing abstract syntax trees to check for docstrings"""
 import re
 import tokenize
-from ast import ClassDef, FunctionDef, Module, NodeVisitor, get_docstring
+from ast import (
+    AsyncFunctionDef,
+    ClassDef,
+    FunctionDef,
+    Module,
+    NodeVisitor,
+    get_docstring,
+)
 from typing import Optional
 
 ACCEPTED_EXCUSE_PATTERNS = (
     re.compile(r"#\s*docstr-coverage\s*:\s*inherit(ed)?\s*"),
     re.compile(r"#\s*docstr-coverage\s*:\s*excuse(d)?\s* `.*`\s*"),
 )
 
@@ -33,14 +40,18 @@
         """Collect information regarding class declaration nodes"""
         self._visit_helper(node)
 
     def visit_FunctionDef(self, node: FunctionDef):
         """Collect information regarding function/method declaration nodes"""
         self._visit_helper(node)
 
+    def visit_AsyncFunctionDef(self, node: AsyncFunctionDef):
+        """Collect information regarding async function/method declaration nodes"""
+        self._visit_helper(node)
+
     def _visit_helper(self, node):
         """Helper method to update :attr:`DocStringCoverageVisitor.tree` with pertinent
         documentation information for `node`, then ensure all child nodes are
         also visited"""
         self.symbol_count += 1
         has_doc = self._has_doc_or_excuse(node)
         relevant_decorator = self._relevant_decorator(node)
```

### Comparing `docstr-coverage-2.2.0/docstr_coverage.egg-info/PKG-INFO` & `docstr-coverage-2.3.0/docstr_coverage.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: docstr-coverage
-Version: 2.2.0
+Version: 2.3.0
 Summary: Utility for examining python source files to ensure proper documentation. Lists missing docstrings, and calculates overall docstring coverage percentage rating.
 Home-page: https://github.com/HunterMcGushion/docstr_coverage
 Author: Hunter McGushion
 Author-email: hunter@mcgushion.com
 License: MIT
 Keywords: docstring coverage documentation audit source code statistics report
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -113,35 +118,25 @@
 - _--verbose=\<level\>, -v \<level\>_ - Set verbosity level (0-3, default: 3)
   - 0 - Silence
   - 1 - Print overall statistics
   - 2 - Also print individual statistics for each file
   - 3 - Also print missing docstrings (function names, class names, etc.)
   - 4 - Also print information about present docstrings
 - _--fail-under=<int|float>, -F <int|float>_ - Fail if under a certain percentage of coverage (default: 100.0)
-- _--docstr-ignore-file=\<filepath\>, -d \<filepath\>_ - Filepath containing list of patterns to ignore. Patterns are (file-pattern, name-pattern) pairs
-  - File content example:
-
-  ```
-  SomeFile method_to_ignore1 method_to_ignore2 method_to_ignore3
-  FileWhereWeWantToIgnoreAllSpecialMethods __.+__
-  .* method_to_ignore_in_all_files
-  a_very_important_view_file ^get$ ^set$ ^post$
-  detect_.* get_val.*
-  ```
 - _--badge=\<filepath\>, -b \<filepath\>_ - Generate a docstring coverage percent badge as an SVG saved to a given filepath
   - Include the badge in a repo's README using 
   ```[![docstr_coverage](<filepath/of/your/saved/badge.svg>)](https://github.com/HunterMcGushion/docstr_coverage)```,
   where `<filepath/of/your/saved/badge.svg>` is the path provided to the `--badge` option
 - _--follow-links, -l_ - Follow symlinks
 - _--percentage-only, -p_ - Output only the overall coverage percentage as a float, silencing all other logging
 - _--help, -h_ - Display CLI options
 
 #### Config File
 All options can be saved in a config file. A file named `.docstr.yaml` in the folder in which `docstr-coverage` is executed is picked up automatically. 
-Other locations can be passed using `docstr-coverage -C path/to/config.json` or the long version `--config`.
+Other locations can be passed using `docstr-coverage -C path/to/config.yml` or the long version `--config`.
 
 Example:
 ```yaml
 paths: # list or string
   - docstr_coverage
 badge: docs # Path
 exclude: .*/test # regex
@@ -173,16 +168,18 @@
 equivalent to
 ```
 docstr-coverage docstr_coverage -e ".*/test" --skip-magic --skip-init --badge="docs" --skip-class-def etc...
 ```
 
 Note that options passed as command line arguments have precedence over options 
 configured in a config file.
-Exception: If a `--docstr-ignore-file` is present and the yml config contains `ignore_patterns`,
-a `ValueError` is raised.
+
+#### Ignoring by Regex
+In your config files, using `ignore_patterns`, you can specify regex patterns for files names and nodes (methods, ...)
+which should be ignored. See config file example above.
 
 #### Overriding by Comments
 Note that `docstr-coverage` can not parse 
 dynamically added documentation (e.g. through class extension).
 Thus, some of your code which deliberately has no docstring might be counted as uncovered.
 
 You can override this by adding either ```# docstr-coverage:inherited``` 
@@ -207,15 +204,15 @@
 and configuring the `paths` section of the [`.docstr.yaml` config](#config-file). 
  This is preferrable over [pre-commit args](https://pre-commit.com/#config-args), 
  as it facilitates the use of the same config in CI, pre-commit and manual runs.
 
 ```yaml
 repos:
   - repo: https://github.com/HunterMcGushion/docstr_coverage
-    rev: v2.2.0 # most recent docstr-coverage release or commit sha
+    rev: v2.3.0 # most recent docstr-coverage release or commit sha
     hooks:
       - id: docstr-coverage
         args: ["--verbose", "2"] # override the .docstr.yaml to see less output
 ```
 
 #### Package in Your Project
```

### Comparing `docstr-coverage-2.2.0/docstr_coverage.egg-info/SOURCES.txt` & `docstr-coverage-2.3.0/docstr_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/setup.py` & `docstr-coverage-2.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
-MAJOR, MINOR, MICRO = 2, 2, 0
+MAJOR, MINOR, MICRO = 2, 3, 0
 __VERSION__ = "{}.{}.{}".format(MAJOR, MINOR, MICRO)
 
 setup(
     name="docstr-coverage",
     version=__VERSION__,
     description=(
         "Utility for examining python source files to ensure proper documentation. "
@@ -21,24 +21,29 @@
     long_description=readme(),
     keywords="docstring coverage documentation audit source code statistics report",
     url="https://github.com/HunterMcGushion/docstr_coverage",
     author="Hunter McGushion",
     author_email="hunter@mcgushion.com",
     license="MIT",
     packages=["docstr_coverage"],
-    install_requires=["click", "PyYAML"],
+    install_requires=["click", "PyYAML", "tqdm==4.63.1"],
     extras_require={
-        "lint": ["flake8==3.9.2", "black==21.5b2", "isort==5.9.0"],
+        "lint": ["flake8==4.0.1", "black==22.3.0", "isort==5.10.1"],
         "test": ["pytest==6.2.5", "pytest-mock==3.4.0"],
     },
     include_package_data=True,
     zip_safe=False,
     entry_points=dict(console_scripts=["docstr-coverage=docstr_coverage.cli:execute"]),
     classifiers=[
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Documentation",
         "Topic :: Documentation :: Sphinx",
         "Topic :: Software Development",
         "Topic :: Software Development :: Documentation",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `docstr-coverage-2.2.0/tests/sample_files/badges/0.svg` & `docstr-coverage-2.3.0/tests/sample_files/badges/0.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/tests/sample_files/badges/100.svg` & `docstr-coverage-2.3.0/tests/sample_files/badges/100.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/tests/sample_files/badges/12.svg` & `docstr-coverage-2.3.0/tests/sample_files/badges/12.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/tests/sample_files/badges/54.svg` & `docstr-coverage-2.3.0/tests/sample_files/badges/54.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/tests/sample_files/badges/71.svg` & `docstr-coverage-2.3.0/tests/sample_files/badges/71.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/tests/sample_files/badges/84.svg` & `docstr-coverage-2.3.0/tests/sample_files/badges/84.svg`

 * *Files identical despite different names*

### Comparing `docstr-coverage-2.2.0/tests/sample_files/badges/94.svg` & `docstr-coverage-2.3.0/tests/sample_files/badges/94.svg`

 * *Files identical despite different names*

