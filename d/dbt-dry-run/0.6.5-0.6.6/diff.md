# Comparing `tmp/dbt_dry_run-0.6.5.tar.gz` & `tmp/dbt_dry_run-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_dry_run-0.6.5.tar", max compression
+gzip compressed data, was "dbt_dry_run-0.6.6.tar", max compression
```

## Comparing `dbt_dry_run-0.6.5.tar` & `dbt_dry_run-0.6.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    11356 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/LICENSE
--rw-r--r--   0        0        0    11670 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/README.md
--rw-r--r--   0        0        0        0 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/__init__.py
--rw-r--r--   0        0        0      110 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/__main__.py
--rw-r--r--   0        0        0        0 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/adapter/__init__.py
--rw-r--r--   0        0        0     1597 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/adapter/service.py
--rw-r--r--   0        0        0     2587 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/cli.py
--rw-r--r--   0        0        0     3691 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/columns_metadata.py
--rw-r--r--   0        0        0     1327 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/exception.py
--rw-r--r--   0        0        0     4543 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/execution.py
--rw-r--r--   0        0        0      331 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/flags.py
--rw-r--r--   0        0        0        0 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/linting/__init__.py
--rw-r--r--   0        0        0     1783 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/linting/column_linting.py
--rw-r--r--   0        0        0     4967 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/literals.py
--rw-r--r--   0        0        0      264 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/models/__init__.py
--rw-r--r--   0        0        0     4226 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/models/manifest.py
--rw-r--r--   0        0        0     2491 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/models/profile.py
--rw-r--r--   0        0        0      692 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/models/report.py
--rw-r--r--   0        0        0     2176 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/models/table.py
--rw-r--r--   0        0        0     1757 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/node_runner/__init__.py
--rw-r--r--   0        0        0     4671 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/node_runner/model_runner.py
--rw-r--r--   0        0        0      759 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/node_runner/node_test_runner.py
--rw-r--r--   0        0        0     1564 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/node_runner/seed_runner.py
--rw-r--r--   0        0        0     3861 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/node_runner/snapshot_runner.py
--rw-r--r--   0        0        0     1521 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/node_runner/source_runner.py
--rw-r--r--   0        0        0     4679 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/result_reporter.py
--rw-r--r--   0        0        0     2468 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/results.py
--rw-r--r--   0        0        0     4899 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/scheduler.py
--rw-r--r--   0        0        0      620 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/sql_runner/__init__.py
--rw-r--r--   0        0        0     3487 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/sql_runner/big_query_sql_runner.py
--rw-r--r--   0        0        0        0 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/__init__.py
--rw-r--r--   0        0        0      231 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/conftest.py
--rw-r--r--   0        0        0        0 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/linting/__init__.py
--rw-r--r--   0        0        0     1846 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/linting/test_column_linting.py
--rw-r--r--   0        0        0     1462 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/models/test_manifest.py
--rw-r--r--   0        0        0     2761 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/models/test_profile.py
--rw-r--r--   0        0        0        0 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/__init__.py
--rw-r--r--   0        0        0    15828 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_model_runner.py
--rw-r--r--   0        0        0     1019 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_node_runner.py
--rw-r--r--   0        0        0     2482 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_seed_runner.py
--rw-r--r--   0        0        0     9693 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_snapshot_runner.py
--rw-r--r--   0        0        0     2938 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_test_runner.py
--rw-r--r--   0        0        0        0 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/sql_runner/__init__.py
--rw-r--r--   0        0        0     4436 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
--rw-r--r--   0        0        0     5503 2023-02-09 10:36:56.709848 dbt_dry_run-0.6.5/dbt_dry_run/test/test_columns_metadata.py
--rw-r--r--   0        0        0     8855 2023-02-09 10:36:56.713848 dbt_dry_run-0.6.5/dbt_dry_run/test/test_literals.py
--rw-r--r--   0        0        0     2337 2023-02-09 10:36:56.713848 dbt_dry_run-0.6.5/dbt_dry_run/test/test_result_reporter.py
--rw-r--r--   0        0        0     3831 2023-02-09 10:36:56.713848 dbt_dry_run-0.6.5/dbt_dry_run/test/test_scheduler.py
--rw-r--r--   0        0        0     1879 2023-02-09 10:36:56.713848 dbt_dry_run-0.6.5/dbt_dry_run/test/utils.py
--rw-r--r--   0        0        0      184 2023-02-09 10:36:56.713848 dbt_dry_run-0.6.5/dbt_dry_run/version.py
--rw-r--r--   0        0        0     1856 2023-02-09 10:36:56.717848 dbt_dry_run-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    13186 1970-01-01 00:00:00.000000 dbt_dry_run-0.6.5/setup.py
--rw-r--r--   0        0        0    12518 1970-01-01 00:00:00.000000 dbt_dry_run-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/LICENSE
+-rw-r--r--   0        0        0    12394 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/adapter/__init__.py
+-rw-r--r--   0        0        0     1597 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/adapter/service.py
+-rw-r--r--   0        0        0     3626 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/cli.py
+-rw-r--r--   0        0        0     3691 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/columns_metadata.py
+-rw-r--r--   0        0        0     1327 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/exception.py
+-rw-r--r--   0        0        0     5035 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/execution.py
+-rw-r--r--   0        0        0      595 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/flags.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/linting/__init__.py
+-rw-r--r--   0        0        0     1783 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/linting/column_linting.py
+-rw-r--r--   0        0        0     4967 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/literals.py
+-rw-r--r--   0        0        0      264 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/__init__.py
+-rw-r--r--   0        0        0     4471 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/manifest.py
+-rw-r--r--   0        0        0     2491 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/profile.py
+-rw-r--r--   0        0        0      692 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/report.py
+-rw-r--r--   0        0        0     2176 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/table.py
+-rw-r--r--   0        0        0     1757 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/__init__.py
+-rw-r--r--   0        0        0     4671 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/model_runner.py
+-rw-r--r--   0        0        0      759 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/node_test_runner.py
+-rw-r--r--   0        0        0     1564 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/seed_runner.py
+-rw-r--r--   0        0        0     3861 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/snapshot_runner.py
+-rw-r--r--   0        0        0     1521 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/source_runner.py
+-rw-r--r--   0        0        0     4679 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/result_reporter.py
+-rw-r--r--   0        0        0     2468 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/results.py
+-rw-r--r--   0        0        0     4899 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/scheduler.py
+-rw-r--r--   0        0        0      620 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/__init__.py
+-rw-r--r--   0        0        0     3487 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/big_query_sql_runner.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/__init__.py
+-rw-r--r--   0        0        0      231 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/linting/__init__.py
+-rw-r--r--   0        0        0     1846 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/linting/test_column_linting.py
+-rw-r--r--   0        0        0     1691 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/models/test_manifest.py
+-rw-r--r--   0        0        0     2761 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/models/test_profile.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/__init__.py
+-rw-r--r--   0        0        0    15828 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_model_runner.py
+-rw-r--r--   0        0        0     1019 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_node_runner.py
+-rw-r--r--   0        0        0     2482 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_seed_runner.py
+-rw-r--r--   0        0        0     9693 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_snapshot_runner.py
+-rw-r--r--   0        0        0     2938 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_test_runner.py
+-rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/sql_runner/__init__.py
+-rw-r--r--   0        0        0     4436 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
+-rw-r--r--   0        0        0     5503 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_columns_metadata.py
+-rw-r--r--   0        0        0     2678 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_execution.py
+-rw-r--r--   0        0        0     8855 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_literals.py
+-rw-r--r--   0        0        0     2337 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_result_reporter.py
+-rw-r--r--   0        0        0     3831 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_scheduler.py
+-rw-r--r--   0        0        0     1879 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/utils.py
+-rw-r--r--   0        0        0      184 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/version.py
+-rw-r--r--   0        0        0     2057 2023-04-13 10:33:14.676043 dbt_dry_run-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    13340 1970-01-01 00:00:00.000000 dbt_dry_run-0.6.6/PKG-INFO
```

### Comparing `dbt_dry_run-0.6.5/LICENSE` & `dbt_dry_run-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/README.md` & `dbt_dry_run-0.6.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 dbt-dry-run default --project-dir /my_org_dbt/ --profiles-dir /my_org_dbt/profiles/ --target local
 ```
 
 The full CLI help is shown below, anything prefixed with [dbt] can be used in the same way as a normal dbt parameter:
 
 ```
   ❯ dbt-dry-run --help
-   Usage: python -m dbt_dry_run [OPTIONS]
+   Usage: dbt-dry-run [OPTIONS]
    
    Options:
      --profiles-dir TEXT             [dbt] Where to search for `profiles.yml`
                                      [default: /Users/connor.charles/.dbt]
      --project-dir TEXT              [dbt] Where to search for `dbt_project.yml`
                                      [default: /Users/connor.charles/Code/dbt-
                                      dry-run]
@@ -67,14 +67,23 @@
      --report-path TEXT              Json path to dump report to
      --skip-not-compiled             Whether or not the dry run should ignore
                                      models that are not compiled. This has
                                      several caveats that make this not a
                                      recommended option. The dbt manifest should
                                      generally be compiled with `--select *` to
                                      ensure good  coverage
+     --extra-check-columns-metadata-key TEXT
+                                     An extra metadata key that can be used in
+                                     place of `dry_run.check_columns` for
+                                     verifying column metadata has been specified
+                                     correctly. `dry_run.check_columns` will
+                                     always take precedence. The metadata key
+                                     should be of boolean type or it will be cast
+                                     to a boolean to be 'True/Falsey`
+     --version
      --install-completion [bash|zsh|fish|powershell|pwsh]
                                      Install completion for the specified shell.
      --show-completion [bash|zsh|fish|powershell|pwsh]
                                      Show completion for the specified shell, to
                                      copy it or customize the installation.
      --help                          Show this message and exit.
 ```
@@ -107,16 +116,17 @@
 
 The process will also return exit code 1
 
 ### Column and Metadata Linting
 
 The dry runner can also be configured to inspect your metadata YAML and assert that the predicted schema of your dbt
 projects data warehouse matches what is documented in the metadata. To enable this for your models specify the key
-`dry_run.check_columns: true`. The dry runner will then fail if the model's documentation does not match. For example
-the full metadata for this model:
+`dry_run.check_columns: true`. The dry runner will then fail if the model's documentation does not match. You can also
+specify a custom extra key to enable `check_columns` by setting the CLI argument `--extra-check-columns-metadata-key`.
+For example the full metadata for this model:
 
 ```yaml
 models:
   - name: badly_documented_model
     description: This model is missing some columns in its docs
     meta:
       dry_run.check_columns: true
```

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/adapter/service.py` & `dbt_dry_run-0.6.6/dbt_dry_run/adapter/service.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/cli.py` & `dbt_dry_run-0.6.6/dbt_dry_run/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,35 @@
 from typer import Option
 
 from dbt_dry_run.adapter.service import DbtArgs, ProjectService
 from dbt_dry_run.exception import ManifestValidationError
 from dbt_dry_run.execution import dry_run_manifest
 from dbt_dry_run.flags import Flags, set_flags
 from dbt_dry_run.result_reporter import ResultReporter
+from dbt_dry_run.version import VERSION
 
 app = typer.Typer()
 
 
 def dry_run(
     project_dir: str,
     profiles_dir: str,
     target: Optional[str],
     verbose: bool = False,
     report_path: Optional[str] = None,
     cli_vars: str = "{}",
     skip_not_compiled: bool = False,
+    extra_check_columns_metadata_key: Optional[str] = None,
 ) -> int:
-    set_flags(Flags(skip_not_compiled=skip_not_compiled))
+    set_flags(
+        Flags(
+            skip_not_compiled=skip_not_compiled,
+            extra_check_columns_metadata_key=extra_check_columns_metadata_key,
+        )
+    )
     args = DbtArgs(
         project_dir=project_dir,
         profiles_dir=os.path.abspath(profiles_dir),
         target=target,
         vars=cli_vars,
     )
     project = ProjectService(args)
@@ -52,14 +59,26 @@
 
 _SKIP_NOT_COMPILED_HELP = """
     Whether or not the dry run should ignore models that are not compiled. This has several caveats that make this 
     not a recommended option. The dbt manifest should generally be compiled with `--select *` to ensure good 
     coverage
 """
 
+_EXTRA_CHECK_COLUMNS_METADATA_KEY_HELP = """
+    An extra metadata key that can be used in place of `dry_run.check_columns` for verifying column metadata has been
+    specified correctly. `dry_run.check_columns` will always take precedence. The metadata key should be of boolean type
+    or it will be cast to a boolean to be 'True/Falsey`
+"""
+
+
+def version_callback(value: bool) -> None:
+    if value:
+        print(f"dbt-dry-run v{VERSION}")
+        raise typer.Exit()
+
 
 @app.command()
 def run(
     profiles_dir: str = Option(
         DEFAULT_PROFILES_DIR, help="[dbt] Where to search for `profiles.yml`"
     ),
     project_dir: str = Option(
@@ -68,17 +87,30 @@
     vars: str = Option("{}", help="[dbt] CLI Variables to pass to dbt"),
     target: Optional[str] = Option(None, help="[dbt] Target profile"),
     verbose: bool = Option(False, help="Output verbose error messages"),
     report_path: Optional[str] = Option(None, help="Json path to dump report to"),
     skip_not_compiled: bool = Option(
         False, "--skip-not-compiled", help=_SKIP_NOT_COMPILED_HELP
     ),
+    extra_check_columns_metadata_key: Optional[str] = Option(
+        None,
+        "--extra-check-columns-metadata-key",
+        help=_EXTRA_CHECK_COLUMNS_METADATA_KEY_HELP,
+    ),
+    _: Optional[bool] = Option(None, "--version", callback=version_callback),
 ) -> None:
     exit_code = dry_run(
-        project_dir, profiles_dir, target, verbose, report_path, vars, skip_not_compiled
+        project_dir,
+        profiles_dir,
+        target,
+        verbose,
+        report_path,
+        vars,
+        skip_not_compiled,
+        extra_check_columns_metadata_key,
     )
     if exit_code > 0:
         raise typer.Exit(exit_code)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/columns_metadata.py` & `dbt_dry_run-0.6.6/dbt_dry_run/columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/exception.py` & `dbt_dry_run-0.6.6/dbt_dry_run/exception.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/execution.py` & `dbt_dry_run-0.6.6/dbt_dry_run/execution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from concurrent import futures
 from concurrent.futures.thread import ThreadPoolExecutor
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple
 
+from dbt_dry_run import flags
 from dbt_dry_run.adapter.service import ProjectService
 from dbt_dry_run.linting.column_linting import lint_columns
 from dbt_dry_run.sql_runner import SQLRunner
 
 if TYPE_CHECKING:
     from mypy.typeshed.stdlib.concurrent.futures._base import Future
 else:
@@ -44,20 +45,34 @@
         raise ValueError(f"Unknown resource type '{node.resource_type}'")
     validation_result = runner.validate_node(node)
     if validation_result:
         return validation_result
     return runner.run(node)
 
 
+def should_check_columns(node: Node) -> bool:
+    check_column = node.get_combined_metadata("dry_run.check_columns")
+    if check_column is not None:
+        return bool(check_column)
+
+    if flags.EXTRA_CHECK_COLUMNS_METADATA_KEY is not None:
+        extra_check_column = node.get_combined_metadata(
+            flags.EXTRA_CHECK_COLUMNS_METADATA_KEY
+        )
+        return bool(extra_check_column) if extra_check_column is not None else False
+
+    return False
+
+
 def dry_run_node(runners: Dict[str, NodeRunner], node: Node, results: Results) -> None:
     """
     This method must be thread safe
     """
     dry_run_result = dispatch_node(node, runners)
-    if node.get_should_check_columns():
+    if should_check_columns(node):
         dry_run_result = lint_columns(node, dry_run_result)
     results.add_result(node.unique_id, dry_run_result)
 
 
 @contextmanager
 def create_context(
     project: ProjectService,
```

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/linting/column_linting.py` & `dbt_dry_run-0.6.6/dbt_dry_run/linting/column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/literals.py` & `dbt_dry_run-0.6.6/dbt_dry_run/literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/models/profile.py` & `dbt_dry_run-0.6.6/dbt_dry_run/models/profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/models/report.py` & `dbt_dry_run-0.6.6/dbt_dry_run/models/report.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/models/table.py` & `dbt_dry_run-0.6.6/dbt_dry_run/models/table.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/node_runner/__init__.py` & `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/node_runner/model_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/node_runner/node_test_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/node_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/node_runner/seed_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/node_runner/snapshot_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/node_runner/source_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/source_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/result_reporter.py` & `dbt_dry_run-0.6.6/dbt_dry_run/result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/results.py` & `dbt_dry_run-0.6.6/dbt_dry_run/results.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/scheduler.py` & `dbt_dry_run-0.6.6/dbt_dry_run/scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/sql_runner/__init__.py` & `dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/sql_runner/big_query_sql_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/linting/test_column_linting.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/linting/test_column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/models/test_profile.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/models/test_profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_model_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_model_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_node_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_node_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_seed_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_snapshot_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/node_runner/test_test_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/test_columns_metadata.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/test_columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/test_literals.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/test_literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/test_result_reporter.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/test_result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/test_scheduler.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/dbt_dry_run/test/utils.py` & `dbt_dry_run-0.6.6/dbt_dry_run/test/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.5/pyproject.toml` & `dbt_dry_run-0.6.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 [tool.poetry]
 name = "dbt-dry-run"
-version = "0.6.5"
+version = "0.6.6"
 description = "Dry run dbt projects"
 authors = ["Connor Charles <connor.charles@autotrader.co.uk>",
            "Phil hope <philip.hope@autotrader.co.uk>",
            "Angelos Georgiadis <angelos.georgiadis@autotrader.co.uk>",
            "Richard Wilmer <richard.wilmer@autotrader.co.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/autotraderuk/dbt-dry-run"
 
 [tool.poetry.scripts]
 dbt-dry-run = "dbt_dry_run.__main__:main"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.10"
+python = ">=3.8,<3.12"
 agate = "^1.6"
 google-cloud-bigquery = "^3"
 pydantic = "^1.9.0"
-tenacity = "^8.0.1"
+tenacity = "^8.2"
 networkx = "^2.6"
 pyyaml = "~6"
 typer = "^0.6.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22"
 isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.931"
 types-PyYAML = "^6.0.4"
 pytest-cov = "^4.0.0"
 twine = "^3.8.0"
 types-setuptools = "^57.4.9"
 pytest-mock = "^3.7.0"
-dbt-bigquery = "^1.4.0"
+dbt-bigquery = "^1.4.1"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "dbt_dry_run/test"
 filterwarnings = [
-    "error"
+    "error",
+    "ignore:Deprecated call to",
+    "ignore:pkg_resources is deprecated as an API",
+    "ignore:invalid escape sequence",
+    "ignore:unclosed",
+    "ignore:'cgi' is deprecated and slated for removal"
 ]
 pythonpath = [
   "."
 ]
 
 [tool.coverage.run]
 source = ["dbt_dry_run"]
```

### Comparing `dbt_dry_run-0.6.5/PKG-INFO` & `dbt_dry_run-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: dbt-dry-run
-Version: 0.6.5
+Version: 0.6.6
 Summary: Dry run dbt projects
 Home-page: https://github.com/autotraderuk/dbt-dry-run
 License: Apache-2.0
 Author: Connor Charles
 Author-email: connor.charles@autotrader.co.uk
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: agate (>=1.6,<2.0)
 Requires-Dist: google-cloud-bigquery (>=3,<4)
 Requires-Dist: networkx (>=2.6,<3.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: pyyaml (>=6,<7)
-Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Requires-Dist: tenacity (>=8.2,<9.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Project-URL: Repository, https://github.com/autotraderuk/dbt-dry-run
 Description-Content-Type: text/markdown
 
 # dbt-dry-run
 
 [dbt][dbt-home] is a tool that helps manage data transformations using templated SQL queries. These SQL queries are
@@ -70,15 +72,15 @@
 dbt-dry-run default --project-dir /my_org_dbt/ --profiles-dir /my_org_dbt/profiles/ --target local
 ```
 
 The full CLI help is shown below, anything prefixed with [dbt] can be used in the same way as a normal dbt parameter:
 
 ```
   ❯ dbt-dry-run --help
-   Usage: python -m dbt_dry_run [OPTIONS]
+   Usage: dbt-dry-run [OPTIONS]
    
    Options:
      --profiles-dir TEXT             [dbt] Where to search for `profiles.yml`
                                      [default: /Users/connor.charles/.dbt]
      --project-dir TEXT              [dbt] Where to search for `dbt_project.yml`
                                      [default: /Users/connor.charles/Code/dbt-
                                      dry-run]
@@ -90,14 +92,23 @@
      --report-path TEXT              Json path to dump report to
      --skip-not-compiled             Whether or not the dry run should ignore
                                      models that are not compiled. This has
                                      several caveats that make this not a
                                      recommended option. The dbt manifest should
                                      generally be compiled with `--select *` to
                                      ensure good  coverage
+     --extra-check-columns-metadata-key TEXT
+                                     An extra metadata key that can be used in
+                                     place of `dry_run.check_columns` for
+                                     verifying column metadata has been specified
+                                     correctly. `dry_run.check_columns` will
+                                     always take precedence. The metadata key
+                                     should be of boolean type or it will be cast
+                                     to a boolean to be 'True/Falsey`
+     --version
      --install-completion [bash|zsh|fish|powershell|pwsh]
                                      Install completion for the specified shell.
      --show-completion [bash|zsh|fish|powershell|pwsh]
                                      Show completion for the specified shell, to
                                      copy it or customize the installation.
      --help                          Show this message and exit.
 ```
@@ -130,16 +141,17 @@
 
 The process will also return exit code 1
 
 ### Column and Metadata Linting
 
 The dry runner can also be configured to inspect your metadata YAML and assert that the predicted schema of your dbt
 projects data warehouse matches what is documented in the metadata. To enable this for your models specify the key
-`dry_run.check_columns: true`. The dry runner will then fail if the model's documentation does not match. For example
-the full metadata for this model:
+`dry_run.check_columns: true`. The dry runner will then fail if the model's documentation does not match. You can also
+specify a custom extra key to enable `check_columns` by setting the CLI argument `--extra-check-columns-metadata-key`.
+For example the full metadata for this model:
 
 ```yaml
 models:
   - name: badly_documented_model
     description: This model is missing some columns in its docs
     meta:
       dry_run.check_columns: true
```

