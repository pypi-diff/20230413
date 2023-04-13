# Comparing `tmp/fotoobo-0.7.0.tar.gz` & `tmp/fotoobo-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fotoobo-0.7.0.tar", max compression
+gzip compressed data, was "fotoobo-0.8.0.tar", max compression
```

## Comparing `fotoobo-0.7.0.tar` & `fotoobo-0.8.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     7633 2023-04-06 11:48:01.689492 fotoobo-0.7.0/LICENSE
--rw-r--r--   0        0        0     2797 2023-04-06 11:48:01.689492 fotoobo-0.7.0/README.md
--rw-r--r--   0        0        0      256 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/__init__.py
--rw-r--r--   0        0        0      206 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/__init__.py
--rw-r--r--   0        0        0     1516 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/convert.py
--rw-r--r--   0        0        0       20 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/ems/__init__.py
--rw-r--r--   0        0        0     1431 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/ems/get_commands.py
--rw-r--r--   0        0        0      717 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/ems/main.py
--rw-r--r--   0        0        0     7665 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/ems/monitor.py
--rw-r--r--   0        0        0       20 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/faz/__init__.py
--rw-r--r--   0        0        0      944 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/faz/get_commands.py
--rw-r--r--   0        0        0      593 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/faz/main.py
--rw-r--r--   0        0        0       20 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fgt/__init__.py
--rw-r--r--   0        0        0     1553 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fgt/check_commands.py
--rw-r--r--   0        0        0     1303 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fgt/config_commands.py
--rw-r--r--   0        0        0     1147 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fgt/get_commands.py
--rw-r--r--   0        0        0     1759 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fgt/main.py
--rw-r--r--   0        0        0       20 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fmg/__init__.py
--rw-r--r--   0        0        0     2620 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fmg/get_commands.py
--rw-r--r--   0        0        0     1948 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/fmg/main.py
--rw-r--r--   0        0        0      948 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/get.py
--rw-r--r--   0        0        0     4081 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/cli/main.py
--rw-r--r--   0        0        0      196 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/exceptions/__init__.py
--rw-r--r--   0        0        0     1966 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/exceptions/exceptions.py
--rw-r--r--   0        0        0      190 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/__init__.py
--rw-r--r--   0        0        0    13955 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/convert.py
--rw-r--r--   0        0        0     1023 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/fortianalyzer.py
--rw-r--r--   0        0        0     5431 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/forticlientems.py
--rw-r--r--   0        0        0     2878 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/fortigate.py
--rw-r--r--   0        0        0    11342 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/fortigate_config.py
--rw-r--r--   0        0        0     8668 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/fortigate_config_check.py
--rw-r--r--   0        0        0      584 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/fortigate_info.py
--rw-r--r--   0        0        0    10419 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/fortimanager.py
--rw-r--r--   0        0        0     6468 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/fortinet/fortinet.py
--rw-r--r--   0        0        0      322 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/helpers/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/helpers/cli.py
--rw-r--r--   0        0        0     3435 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/helpers/config.py
--rw-r--r--   0        0        0     6414 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/helpers/files.py
--rw-r--r--   0        0        0    10407 2023-04-06 11:48:01.693492 fotoobo-0.7.0/fotoobo/helpers/log.py
--rw-r--r--   0        0        0     9300 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/helpers/output.py
--rw-r--r--   0        0        0      128 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/inventory/__init__.py
--rw-r--r--   0        0        0      568 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/inventory/generic.py
--rw-r--r--   0        0        0     4296 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/inventory/inventory.py
--rwxr-xr-x   0        0        0     1359 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/main.py
--rw-r--r--   0        0        0      440 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/convert.py
--rw-r--r--   0        0        0       92 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/ems/__init__.py
--rw-r--r--   0        0        0     1518 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/ems/get.py
--rw-r--r--   0        0        0     7725 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/ems/monitor.py
--rw-r--r--   0        0        0       56 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/faz/__init__.py
--rw-r--r--   0        0        0      779 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/faz/get.py
--rw-r--r--   0        0        0      125 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fgt/__init__.py
--rw-r--r--   0        0        0     4583 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fgt/check.py
--rw-r--r--   0        0        0     3423 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fgt/config.py
--rw-r--r--   0        0        0     1114 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fgt/get.py
--rw-r--r--   0        0        0     3286 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fgt/main.py
--rw-r--r--   0        0        0      140 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fmg/__init__.py
--rw-r--r--   0        0        0     4271 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fmg/get.py
--rw-r--r--   0        0        0     2569 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fmg/main.py
--rw-r--r--   0        0        0     1093 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/fmg/set_.py
--rw-r--r--   0        0        0     2035 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/get.py
--rw-r--r--   0        0        0     1306 2023-04-06 11:48:01.697492 fotoobo-0.7.0/fotoobo/utils/greet.py
--rw-r--r--   0        0        0     3730 2023-04-06 11:48:01.697492 fotoobo-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fotoobo-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-04-13 12:43:19.567977 fotoobo-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2797 2023-04-13 12:43:19.567977 fotoobo-0.8.0/README.md
+-rw-r--r--   0        0        0      256 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/__init__.py
+-rw-r--r--   0        0        0     1584 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/convert.py
+-rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/__init__.py
+-rw-r--r--   0        0        0     1488 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/get_commands.py
+-rw-r--r--   0        0        0      784 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/main.py
+-rw-r--r--   0        0        0     7418 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/faz/__init__.py
+-rw-r--r--   0        0        0      995 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/faz/get_commands.py
+-rw-r--r--   0        0        0      639 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/faz/main.py
+-rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/__init__.py
+-rw-r--r--   0        0        0     1537 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/config_commands.py
+-rw-r--r--   0        0        0     1283 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/get_commands.py
+-rw-r--r--   0        0        0     1951 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/main.py
+-rw-r--r--   0        0        0     1711 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fmg/__init__.py
+-rw-r--r--   0        0        0     2582 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fmg/get_commands.py
+-rw-r--r--   0        0        0     2199 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fmg/main.py
+-rw-r--r--   0        0        0     1033 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/get.py
+-rw-r--r--   0        0        0     4743 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/main.py
+-rw-r--r--   0        0        0      196 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/exceptions/__init__.py
+-rw-r--r--   0        0        0     1966 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/exceptions/exceptions.py
+-rw-r--r--   0        0        0      190 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/__init__.py
+-rw-r--r--   0        0        0    13955 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/convert.py
+-rw-r--r--   0        0        0     1023 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortianalyzer.py
+-rw-r--r--   0        0        0     5431 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/forticlientems.py
+-rw-r--r--   0        0        0     2878 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate.py
+-rw-r--r--   0        0        0    11342 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate_config.py
+-rw-r--r--   0        0        0     8668 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate_config_check.py
+-rw-r--r--   0        0        0      584 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate_info.py
+-rw-r--r--   0        0        0    10421 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortimanager.py
+-rw-r--r--   0        0        0     6468 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortinet.py
+-rw-r--r--   0        0        0      322 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/cli.py
+-rw-r--r--   0        0        0     3435 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/config.py
+-rw-r--r--   0        0        0     6414 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/files.py
+-rw-r--r--   0        0        0    10407 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/log.py
+-rw-r--r--   0        0        0     9300 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/output.py
+-rw-r--r--   0        0        0      128 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/inventory/__init__.py
+-rw-r--r--   0        0        0      568 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/inventory/generic.py
+-rw-r--r--   0        0        0     4296 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/inventory/inventory.py
+-rwxr-xr-x   0        0        0     1359 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/main.py
+-rw-r--r--   0        0        0      440 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/convert.py
+-rw-r--r--   0        0        0       92 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/ems/__init__.py
+-rw-r--r--   0        0        0     1518 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/ems/get.py
+-rw-r--r--   0        0        0     7725 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/ems/monitor.py
+-rw-r--r--   0        0        0       56 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/faz/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/faz/get.py
+-rw-r--r--   0        0        0      129 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/__init__.py
+-rw-r--r--   0        0        0     3468 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/config.py
+-rw-r--r--   0        0        0     1114 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/get.py
+-rw-r--r--   0        0        0     3286 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/main.py
+-rw-r--r--   0        0        0     4583 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/monitor.py
+-rw-r--r--   0        0        0      105 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/__init__.py
+-rw-r--r--   0        0        0     4271 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/get.py
+-rw-r--r--   0        0        0     2534 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/main.py
+-rw-r--r--   0        0        0     1059 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/post_.py
+-rw-r--r--   0        0        0     2152 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/get.py
+-rw-r--r--   0        0        0     1306 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/greet.py
+-rw-r--r--   0        0        0     3730 2023-04-13 12:43:19.575977 fotoobo-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fotoobo-0.8.0/PKG-INFO
```

### Comparing `fotoobo-0.7.0/LICENSE` & `fotoobo-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/README.md` & `fotoobo-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/cli/convert.py` & `fotoobo-0.8.0/fotoobo/cli/convert.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.utils import convert
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The fotoobo convert command callback
@@ -20,41 +20,41 @@
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-@app.command()
+@app.command(no_args_is_help=True)
 def checkpoint(
     infile: str = typer.Argument(
         ...,
-        help="The json file to read the Checkpoint objects from",
+        help="The json file to read the Checkpoint objects from.",
         show_default=False,
         metavar="[infile]",
     ),
     outfile: str = typer.Argument(
         ...,
-        help="The json file to write the converted objects to",
+        help="The json file to write the converted objects to.",
         show_default=False,
         metavar="[outfile]",
     ),
     obj_type: str = typer.Argument(
         ...,
-        help="The type of objects to convert",
+        help="The type of objects to convert.",
         show_default=False,
         metavar="[type]",
     ),
     cache_dir: str = typer.Argument(
         None,
-        help="The cache directory to use",
+        help="The cache directory to use.",
         show_default=False,
         metavar="[cache_dir]",
     ),
 ) -> None:
     """
-    Convert Checkpoint assets into Fortinet objects
+    Convert Checkpoint assets into Fortinet objects.
 
-    The Checkpoint objects have to be prepared in a json file. See convert.md for the syntax.
-    The argument [type] defines what object type to convert.
+    The Checkpoint objects have to be prepared in a json file. See
+    https://fotoobo.readthedocs.io/en/latest/usage/convert.html for more information.
     """
     convert.checkpoint(infile, outfile, obj_type, cache_dir)
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/ems/get_commands.py` & `fotoobo-0.8.0/fotoobo/cli/ems/get_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.output import print_datatable
 from fotoobo.utils import ems
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The ems get subcommand callback
@@ -25,32 +25,32 @@
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
 @app.command()
 def version(
     host: str = typer.Argument(
         "ems",
-        help="The FortiClientEMS hostname to access (must be defined in inventory)",
+        help="The FortiClientEMS hostname to access (must be defined in the inventory).",
         metavar="[host]",
     )
 ) -> None:
     """
-    Get the FortiClient EMS version
+    Get the FortiClient EMS version.
     """
     data = ems.get.version(host)
     print_datatable(data, title="FortiClient EMS Version", headers=["FortiClient EMS", "Version"])
 
 
 @app.command()
 def workgroups(
     host: str = typer.Argument(
         "ems",
-        help="The FortiClientEMS hostname to access (must be defined in inventory)",
+        help="The FortiClientEMS hostname to access (must be defined in the inventory).",
         metavar="[host]",
     ),
     custom: bool = typer.Option(False, "--custom", "-c", help="Only show custom groups"),
 ) -> None:
     """
-    Get the FortiClient EMS workgroups
+    Get the FortiClient EMS workgroups.
     """
     data = ems.get.workgroups(host, custom)
     print_datatable(data, title="FortiClient EMS Workgroups", auto_header=True)
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/ems/main.py` & `fotoobo-0.8.0/fotoobo/cli/ems/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 The FortiClient EMS commands
 """
 import logging
 
 import typer
 
 from fotoobo.cli.ems import get_commands as get
-from fotoobo.cli.ems import monitor
+from fotoobo.cli.ems import monitor_commands as monitor
 from fotoobo.helpers import cli_path
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The ems subcommand callback
@@ -21,9 +21,9 @@
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-app.add_typer(get.app, name="get", help="FortiClient EMS get commands")
-app.add_typer(monitor.app, name="monitor", help="FortiClient EMS monitor commands")
+app.add_typer(get.app, name="get", help="FortiClient EMS get commands.")
+app.add_typer(monitor.app, name="monitor", help="FortiClient EMS monitor commands.")
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/ems/monitor.py` & `fotoobo-0.8.0/fotoobo/cli/ems/monitor_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,58 +7,66 @@
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.files import save_json_file, save_with_template
 from fotoobo.helpers.output import print_dicttable
 from fotoobo.utils.ems import monitor
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
+HELP_TEXT_ARGUMENT_EMS = (
+    "The FortiClient EMS hostname to access (must be defined in the inventory)."
+)
+HELP_TEXT_OPTION_OUTPUT_FILE = "The file to write the output to."
+HELP_TEXT_OPTION_TEMPLATE = "The jinja2 template to use (use with -o)."
+HELP_TEXT_TEMPLATE = (
+    "If you add a template with the -t option you may render the output with any Jinja2 template "
+    "file. You may use any of the given data returned from the FortiClient EMS. Additionally there "
+    "are enriched variables under 'fotoobo' which you may also use in your template."
+)
+
+
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The ems get subcommand callback
 
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-@app.command()
+@app.command(help="Monitor the FortiClient EMS connections.\n\n" + HELP_TEXT_TEMPLATE)
 def connections(
     host: str = typer.Argument(
         "ems",
-        help="The FortiClient EMS hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_ARGUMENT_EMS,
         metavar="[host]",
     ),
     output_file: str = typer.Option(
         "",
         "--output",
         "-o",
-        help="The file to write the output to",
+        help=HELP_TEXT_OPTION_OUTPUT_FILE,
         metavar="[output]",
     ),
     template_file: str = typer.Option(
         "",
         "--template",
         "-t",
-        help="The jinja2 template to use (use with -o)",
+        help=HELP_TEXT_OPTION_TEMPLATE,
         metavar="[template]",
     ),
 ) -> None:
     """
-    Monitoring the FortiClient EMS connections.
-
-    If you add a template with the -t option you may render the output with any Jinja2 template
-    file. You may use any of the given data returned from the license endpoint. Additionally there
-    are enriched variables under 'fotoobo' which you also may use in your template.
+    Monitor the FortiClient EMS connections.
     """
     data = monitor.connections(host)
 
     if output_file:
         log.debug("output_file is: %s", output_file)
 
         if template_file:
@@ -68,41 +76,40 @@
             # write to file without a template (raw output)
             save_json_file(output_file, data)
 
     else:
         print_dicttable(data, title="FortiClient EMS connections")
 
 
-@app.command()
+@app.command(
+    help="Monitor the endpoint management status in FortiClient EMS.\n\n" + HELP_TEXT_TEMPLATE
+)
 def endpoint_management_status(
     host: str = typer.Argument(
         "ems",
-        help="The FortiClient EMS hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_ARGUMENT_EMS,
         metavar="[host]",
     ),
     output_file: str = typer.Option(
         "",
         "--output",
         "-o",
-        help="The file to write the output to",
+        help=HELP_TEXT_OPTION_OUTPUT_FILE,
         metavar="[output]",
     ),
     template_file: str = typer.Option(
         "",
         "--template",
         "-t",
-        help="The jinja2 template to use (use with -o)",
+        help=HELP_TEXT_OPTION_TEMPLATE,
         metavar="[template]",
     ),
 ) -> None:
     """
-    Monitoring the endpoint management status in FortiClient EMS.
-
-    If you add a template with the -t option you may render the output with any Jinja2 template
-    file.
+    Monitor the endpoint management status in FortiClient EMS.
     """
     data = monitor.endpoint_management_status(host)
 
     if output_file:
         log.debug("output_file is: %s", output_file)
 
         if template_file:
@@ -113,41 +120,41 @@
             save_json_file(output_file, data)
 
     else:
         # if no output file is given just print the output to the console
         print_dicttable(data, title="FortiClient EMS endpoints")
 
 
-@app.command()
+@app.command(
+    help="Get the amount of FortiClient EMS devices which are online but policy is not in sync.\n\n"
+    + HELP_TEXT_TEMPLATE
+)
 def endpoint_outofsync(
     host: str = typer.Argument(
         "ems",
-        help="The FortiClient EMS hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_ARGUMENT_EMS,
         metavar="[host]",
     ),
     output_file: str = typer.Option(
         "",
         "--output",
         "-o",
-        help="The file to write the output to",
+        help=HELP_TEXT_OPTION_OUTPUT_FILE,
         metavar="[output]",
     ),
     template_file: str = typer.Option(
         "",
         "--template",
         "-t",
-        help="The jinja2 template to use (use with -o)",
+        help=HELP_TEXT_OPTION_TEMPLATE,
         metavar="[template]",
     ),
 ) -> None:
     """
     Get amount of FortiClient EMS devices which are online but policy not in sync.
-
-    If you add a template with the -t option you may render the output with any Jinja2 template
-    file.
     """
     data = monitor.endpoint_online_outofsync(host)
 
     if output_file:
         log.debug("output_file is: %s", output_file)
 
         if template_file:
@@ -158,41 +165,38 @@
             save_json_file(output_file, data)
 
     else:
         # if no output file is given just print the output to the console
         print_dicttable(data, title="FortiClient EMS endpoints")
 
 
-@app.command()
+@app.command(help="Monitor the endpoint OS versions in FortiClient EMS.\n\n" + HELP_TEXT_TEMPLATE)
 def endpoint_os_versions(
     host: str = typer.Argument(
         "ems",
-        help="The FortiClient EMS hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_ARGUMENT_EMS,
         metavar="[host]",
     ),
     output_file: str = typer.Option(
         "",
         "--output",
         "-o",
-        help="The file to write the output to",
+        help=HELP_TEXT_OPTION_OUTPUT_FILE,
         metavar="[output]",
     ),
     template_file: str = typer.Option(
         "",
         "--template",
         "-t",
-        help="The jinja2 template to use (use with -o)",
+        help=HELP_TEXT_OPTION_TEMPLATE,
         metavar="[template]",
     ),
 ) -> None:
     """
-    Monitoring the endpoint os versions in FortiClient EMS.
-
-    If you add a template with the -t option you may render the output with any Jinja2 template
-    file.
+    Monitor the endpoint os versions in FortiClient EMS.
     """
     data = monitor.endpoint_os_versions(host)
 
     if output_file:
         log.debug("output_file is: %s", output_file)
 
         if template_file:
@@ -203,42 +207,38 @@
             save_json_file(output_file, data)
 
     else:
         # if no output file is given just print the output to the console
         print_dicttable(data, title="FortiClient EMS endpoints")
 
 
-@app.command()
+@app.command(help="Monitor the FortiClient EMS license.\n\n" + HELP_TEXT_TEMPLATE)
 def license(  # pylint: disable=redefined-builtin
     host: str = typer.Argument(
         "ems",
-        help="The FortiClient EMS hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_ARGUMENT_EMS,
         metavar="[host]",
     ),
     output_file: str = typer.Option(
         "",
         "--output",
         "-o",
-        help="The file to write the output to",
+        help=HELP_TEXT_OPTION_OUTPUT_FILE,
         metavar="[output]",
     ),
     template_file: str = typer.Option(
         "",
         "--template",
         "-t",
-        help="The jinja2 template to use (use with -o)",
+        help=HELP_TEXT_OPTION_TEMPLATE,
         metavar="[template]",
     ),
 ) -> None:
     """
-    Monitoring the FortiClient EMS license.
-
-    If you add a template with the -t option you may render the output with any Jinja2 template
-    file. You may use any of the given data returned from the license endpoint. Additionally there
-    are enriched variables under 'fotoobo' which you also may use in your template.
+    Monitor the FortiClient EMS license.
     """
     data = monitor.license(host)
 
     if output_file:
         log.debug("output_file is: %s", output_file)
 
         if template_file:
@@ -253,19 +253,19 @@
         print_dicttable(data, title="FortiClient EMS license information")
 
 
 @app.command()
 def system(
     host: str = typer.Argument(
         "ems",
-        help="The FortiClient EMS hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_ARGUMENT_EMS,
         metavar="[host]",
     ),
 ) -> None:
     """
-    Monitoring the FortiClient EMS system information.
+    Monitor the FortiClient EMS system information.
     """
     data = monitor.system(host)
 
     license_data = data.pop("license", {})  # pop "license" key to print that in another table
     print_dicttable(data, title="FortiClient EMS system information")
     print_dicttable(license_data, title="FortiClient EMS system.license information")
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/faz/get_commands.py` & `fotoobo-0.8.0/fotoobo/cli/faz/get_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.output import print_datatable
 from fotoobo.utils import faz
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The faz get subcommand callback
@@ -25,16 +25,16 @@
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
 @app.command()
 def version(
     host: str = typer.Argument(
         "faz",
-        help="The FortiAnalyzer hostname to access (must be defined in inventory)",
+        help="The FortiAnalyzer hostname to access (must be defined in the inventory).",
         metavar="[host]",
     )
 ) -> None:
     """
-    Get the FortiAnalyzer version
+    Get the FortiAnalyzer version.
     """
     data = faz.get.version(host)
     print_datatable(data, title="FortiAnalyzer Version", headers=["FortiAnalyzer", "Version"])
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/faz/main.py` & `fotoobo-0.8.0/fotoobo/cli/faz/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 
 import typer
 
 from fotoobo.cli.faz import get_commands as get
 from fotoobo.helpers import cli_path
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The faz subcommand callback
@@ -20,8 +20,8 @@
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-app.add_typer(get.app, name="get", help="FortiAnalyzer get commands")
+app.add_typer(get.app, name="get", help="FortiAnalyzer get commands.")
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/fgt/check_commands.py` & `fotoobo-0.8.0/fotoobo/cli/fgt/monitor_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 The FortiGate check commands
 """
+# pylint: disable=anomalous-backslash-in-string
+
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.output import print_datatable
 from fotoobo.utils import fgt
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The fgt check subcommand callback
@@ -25,28 +27,32 @@
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
 @app.command()
 def hamaster(
     host: str = typer.Argument(
         "fmg",
-        help="The FortiManager hostname to access (must be defined in inventory)",
+        help="The FortiManager hostname to access (must be defined in the inventory).",
         metavar="[host]",
     ),
     smtp_server: str = typer.Option(
-        None, "--smtp", help="the smtp configuration from the inventory", metavar="server"
+        None,
+        "--smtp",
+        help="The smtp configuration from the inventory.",
+        metavar="server",
+        show_default=False,
     ),
 ) -> None:
     """
-    Check the FortiGate HA master
+    Check the FortiGate HA master.
 
     Although this command checks the HA master status of FortiGates you have to specify a
     FortiManager to access. The command searches for all FortiGate clusters in the FortiManager
     and checks if the designated primary node really is the HA master node.
 
-    The optional argument [host] makes this command somewhat magic. If you omit [host] it searches
+    The optional argument \[host] makes this command somewhat magic. If you omit \[host] it searches
     for all devices in the default FortiManager (fmg) in the inventory.
     """
-    data = fgt.check.hamaster(host, smtp_server)
+    data = fgt.monitor.hamaster(host, smtp_server)
     print_datatable(
         data, title="FortiGate HA master status", headers=["FortiGate Cluster", "Status"]
     )
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/fgt/get_commands.py` & `fotoobo-0.8.0/fotoobo/cli/fgt/get_commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 The FortiGate get commands
 """
+# pylint: disable=anomalous-backslash-in-string
+
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.output import print_datatable
 from fotoobo.utils import fgt
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The fgt get subcommand callback
@@ -25,20 +27,21 @@
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
 @app.command()
 def version(
     host: str = typer.Argument(
         "",
-        help="The FortiGate hostname to access (must be defined in inventory)",
+        help="The FortiGate hostname to access (must be defined in the inventory). "
+        "\[default: <all>]",
         show_default=False,
         metavar="[host]",
     )
 ) -> None:
     """
-    Get the FortiGate version
+    Get the FortiGate(s) version(s).
 
-    The optional argument [host] makes this command somewhat magic. If you omit [host] it searches
+    The optional argument [host] makes this command somewhat magic. If you omit \[host] it searches
     for all devices of type 'fortigate' in the inventory and tries to get their FortiOS version.
     """
     data = fgt.get.version(host)
     print_datatable(data, title="FortiGate Versions", headers=["FortiGate", "Version"])
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/fgt/main.py` & `fotoobo-0.8.0/fotoobo/cli/fgt/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 The FortiGate commands
 """
 import logging
 
 import typer
 
 from fotoobo import utils
-from fotoobo.cli.fgt import check_commands as check
+from fotoobo.cli.fgt import monitor_commands as monitor
 from fotoobo.cli.fgt import config_commands as config
 from fotoobo.cli.fgt import get_commands as get
 from fotoobo.helpers import cli_path
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The fgt subcommand callback
@@ -23,39 +23,48 @@
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-app.add_typer(get.app, name="get", help="FortiGate get commands")
-app.add_typer(check.app, name="check", help="FortiGate check commands")
-app.add_typer(config.app, name="config", help="FortiGate config file commands")
+app.add_typer(get.app, name="get", help="FortiGate get commands.")
+app.add_typer(monitor.app, name="monitor", help="FortiGate monitor commands.")
+app.add_typer(config.app, name="config", help="FortiGate config file commands.")
 
 
 @app.command()
 def backup(
     host: str = typer.Argument(
         "",
-        help="The FortiGate to backup (must be defined in inventory). Backups all if left empty.",
+        help="The FortiGate to backup (must be defined in the inventory). "
+        "Backups all if left empty.",
         show_default=False,
         metavar="[host]",
     ),
     backup_dir: str = typer.Option(
         None,
         "--backup-dir",
         "-b",
         help="The directory to save the backup(s) to. Default is the current working directory.",
         show_default=False,
         metavar="backup_dir",
     ),
     ftp_server: str = typer.Option(
-        None, "--ftp", "-f", help="the ftp configuration from the inventory", metavar="server"
+        None,
+        "--ftp",
+        "-f",
+        help="The ftp configuration from the inventory to send the backup to.",
+        metavar="server",
     ),
     smtp_server: str = typer.Option(
-        None, "--smtp", "-s", help="the smtp configuration from the inventory", metavar="server"
+        None,
+        "--smtp",
+        "-s",
+        help="The smtp configuration from the inventory to send potential errors to.",
+        metavar="server",
     ),
 ) -> None:
     """
-    Backup one or more FortiGate(s)
+    Backup one or more FortiGate(s).
     """
     utils.fgt.backup(host, backup_dir, ftp_server, smtp_server)
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/fmg/get_commands.py` & `fotoobo-0.8.0/fotoobo/cli/fmg/get_commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.output import print_datatable, write_policy_to_html
 from fotoobo.utils import fmg
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
+HELP_TEXT_HOST = "The FortiManager to access (must be defined in the inventory)."
+
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The fmg get subcommand callback
 
     Args:
@@ -25,81 +27,74 @@
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
 @app.command()
 def adoms(
     host: str = typer.Argument(
         "fmg",
-        help="The FortiManager hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_HOST,
         metavar="[host]",
     )
 ) -> None:
     """
-    Get the FortiManager ADOM list
+    Get the FortiManager ADOM list.
     """
     data = fmg.get.adoms(host)
     print_datatable(data, title="FortiManager ADOMs", headers=["Name", "Version"])
 
 
 @app.command()
 def devices(
     host: str = typer.Argument(
         "fmg",
-        help="The FortiManager hostname to access (must be defined in inventory)",
+        help=HELP_TEXT_HOST,
         metavar="[host]",
     )
 ) -> None:
     """
-    Get the FortiManager logical devices list
+    Get the FortiManager logical devices list.
 
-    Be aware that if a device is a cluster only the cluster device is returned, not all its
-    physical nodes.
+    Be aware that if a device is a cluster only the cluster
+    device is returned, not all its physical nodes.
     """
     data = fmg.get.devices(host)
     print_datatable(
         data,
         title="Fortinet devices",
         headers=["Device Name", "Version", "HA", "Platform", "Description"],
     )
 
 
-@app.command()
+@app.command(no_args_is_help=True)
 def policy(
-    host: str = typer.Argument(
-        ...,
-        help="The FortiManager hostname to access (must be defined in inventory)",
-        metavar="[host]",
-    ),
     adom: str = typer.Argument(
-        ..., help="The FortiManager ADOM to get the firewall policy from", metavar="[adom]"
+        ...,
+        help="The FortiManager ADOM to get the firewall policy from.",
+        metavar="[adom]",
+        show_default=False,
     ),
     policy_name: str = typer.Argument(
-        ...,
-        help="The policy name to get",
-        metavar="[policy]",
+        ..., help="The name of the policy to get.", metavar="[policy]", show_default=False
     ),
     filename: str = typer.Argument(
-        ...,
-        help="the filename to write the policy to",
-        metavar="[file]",
+        ..., help="The filename to write the policy to.", metavar="[file]", show_default=False
+    ),
+    host: str = typer.Argument(
+        "fmg",
+        help=HELP_TEXT_HOST,
+        metavar="[host]",
     ),
 ) -> None:
     """
-    Get a FortiManager policy
+    Get a FortiManager policy.
     """
     data = fmg.get.policy(host, adom, policy_name)
     write_policy_to_html(data, filename)
 
 
 @app.command()
-def version(
-    host: str = typer.Argument(
-        "fmg",
-        help="The FortiManager hostname to access (must be defined in inventory)",
-        metavar="[host]",
-    )
-) -> None:
+def version(host: str = typer.Argument("fmg", help=HELP_TEXT_HOST, metavar="[host]")) -> None:
     """
-    Get the FortiManager version
+    Get the FortiManager version.
     """
     data = fmg.get.version(host)
     print_datatable(data, title="FortiManager Version", headers=["FortiManager", "Version"])
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/fmg/main.py` & `fotoobo-0.8.0/fotoobo/cli/fmg/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import typer
 
 from fotoobo.cli.fmg import get_commands as get
 from fotoobo.helpers import cli_path
 from fotoobo.utils import fmg
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The fmg subcommand callback
@@ -21,52 +21,60 @@
     Args:
         context (Context): the context object of the typer app
     """
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
-@app.command()
+@app.command(no_args_is_help=True)
 def assign(
-    host: str = typer.Argument(
-        "fmg",
-        help="The FortiManager hostname to access (must be defined in inventory)",
-        metavar="[host]",
-    ),
     adoms: str = typer.Argument(
         ...,
-        help="The ADOMs to assign the global policy/objects. Use 'fmg get adoms' to get a list of "
-        + "available ADOMs. Separate multiple ADOMs by comma (no spaces)",
+        help="The ADOMs to assign the global policy/objects to. Use "
+        "'fotoobo fmg get adoms' to get a list of "
+        "available ADOMs. Separate multiple ADOMs by comma (no spaces).",
         metavar="[adoms]",
         show_default=False,
     ),
+    host: str = typer.Argument(
+        "fmg",
+        help="The FortiManager to access (must be defined in the inventory).",
+        metavar="[host]",
+    ),
     timeout: int = typer.Option(
         60,
         "--timeout",
         "-t",
-        help="The timeout to wait for the FortiManager task to finish",
+        help="The timeout to wait for the FortiManager task to finish.",
         metavar="[timeout]",
     ),
 ) -> None:
     """
-    Assign a global policy to a specified ADOM or to a list of ADOMs
+    Assign a global policy to a specified ADOM or to a list of ADOMs.
     """
     fmg.assign(host, adoms, timeout=timeout)
 
 
-@app.command()
-def set(  # pylint: disable=redefined-builtin
+@app.command(no_args_is_help=True)
+def post(
     host: str = typer.Argument(
         ...,
-        help="The FortiManager hostname to access (must be defined in inventory)",
+        help="The FortiManager to access (must be defined in the inventory).",
         metavar="[host]",
+        show_default=False,
     ),
     file: str = typer.Argument(
-        ..., help="json file with payload(s)", show_default=False, metavar="[file]"
+        ..., help="JSON file with payload(s).", show_default=False, metavar="[file]"
+    ),
+    adom: str = typer.Argument(
+        ..., help="The ADOM to issue the set command(s).", metavar="[adom]", show_default=False
     ),
-    adom: str = typer.Argument(..., help="The ADOM to issue the set command(s)", metavar="[adom]"),
 ) -> None:
-    """FortiManager set command"""
-    fmg.set(host, file, adom)
+    """
+    POST any valid JSON request to the FortiManager.
+
+    Configure the FortiManager with any valid API call(s) given within the JSON file.
+    """
+    fmg.post(host, file, adom)
 
 
-app.add_typer(get.app, name="get", help="FortiManager get commands")
+app.add_typer(get.app, name="get", help="FortiManager get commands.")
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/get.py` & `fotoobo-0.8.0/fotoobo/cli/get.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.utils import get
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 @app.callback()
 def callback(context: typer.Context) -> None:
     """
     The fotoobo get command callback
@@ -23,30 +23,30 @@
     cli_path.append(str(context.invoked_subcommand))
     log.debug("about to execute command: '%s'", context.invoked_subcommand)
 
 
 @app.command()
 def inventory() -> None:
     """
-    Get the fotoobo inventory
+    Print a summary over your fotoobo inventory.
     """
     get.inventory()
 
 
 @app.command()
 def version(
     verbose: bool = typer.Option(
-        False, "-v", help="Verbose output (also show most important modules)"
+        False, "-v", help="Verbose output (also show the most important modules)."
     ),
 ) -> None:
     """
-    Get the fotoobo version
+    Print the fotoobo version.
     """
     get.version(verbose)
 
 
 @app.command()
 def commands() -> None:
     """
-    Get the fotoobo commands
+    Print the fotoobo commands structure.
     """
     get.commands()
```

### Comparing `fotoobo-0.7.0/fotoobo/cli/main.py` & `fotoobo-0.8.0/fotoobo/cli/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 This is the main cli module. If fotoobo is started from the command line the main script starts
 app() from within here. Every level of the command line tool is represented by a subdirectory.
 If you extend the cli make sure you are in the correct directory or create a new one if there are
 more than a few subcommands.
 
 Caution: Use docstrings with care as they are used to print help texts on any command.
 """
+# pylint: disable=anomalous-backslash-in-string
+
 import logging
+import os
 import sys
 from typing import Optional, Union
 
 import typer
 
 from fotoobo import utils
 from fotoobo.cli import convert, get
@@ -19,15 +22,19 @@
 from fotoobo.cli.fgt import main as fgt
 from fotoobo.cli.fmg import main as fmg
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.config import config
 from fotoobo.helpers.log import Log
 from fotoobo.helpers.output import print_logo
 
-app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
+app = typer.Typer(
+    context_settings={"help_option_names": ["-h", "--help"]},
+    no_args_is_help=True,
+    rich_markup_mode="rich",
+)
 log = logging.getLogger("fotoobo")
 
 
 def version_callback(value: bool) -> None:
     """The version callback"""
     if value:
         utils.get.version()
@@ -37,36 +44,42 @@
 @app.callback()
 def callback(  # pylint: disable=too-many-arguments
     context: typer.Context,
     config_file: Union[str, None] = typer.Option(
         None,
         "--config",
         "-c",
-        help="The fotoobo configuration file",
+        help="Set the fotoobo configuration file. \[default: fotoobo.yaml]",
         show_default=False,
         metavar="[file]",
     ),
-    log_switch: bool = typer.Option(None, "--log", "-l", help="Enable logging"),
+    log_switch: bool = typer.Option(
+        None, "--log", "-l", help="Enable logging. \[default: disabled]"
+    ),
     log_level: str = typer.Option(
         None,
         "--loglevel",
-        help="The logging level. Choose from CRITICAL, ERROR, WARNING, INFO, DEBUG",
+        help="Set the log level. Choose from CRITICAL, ERROR, WARNING, INFO, DEBUG.",
         metavar="[level]",
+        show_default=False,
     ),
-    nologo: bool = typer.Option(None, "--nologo", help="Disable the logo"),
+    nologo: bool = typer.Option(None, "--nologo", help="Do not print the beautiful fotoobo logo."),
     version: Optional[bool] = typer.Option(  # pylint: disable=unused-argument
-        None, "--version", "-V", help="Get fotoobo version", callback=version_callback
+        None, "--version", "-V", help="Print the fotoobo version.", callback=version_callback
     ),
 ) -> None:
     """
     The Fortinet Toolbox (fotoobo) - make IT easy
 
-    This tool lets you interact with Fortinet assets like devices and their configuration.
+    ─────────────────────────────────────────────
+
+    This is fotoobo, the mighty [bold]Fo[/bold]rtinet [bold]too[/bold]l[bold]bo[/bold]x for
+    managing your Fortinet environment. It is meant to be extendable to your needs.
 
-    For help see the README.md or theAttribute specific documentation in the docs folder.
+    For detailed documentation see https://fotoobo.readthedocs.io.
     """
     config.load_configuration(config_file)
     config.no_logo = True if nologo else config.no_logo
 
     if log_level:
         log_level = log_level.upper()
 
@@ -92,28 +105,33 @@
     # save_json_file("data/cli.json", info)
     config.cli_info = context.to_info_dict()
 
 
 @app.command(hidden=True)
 def greet(
     name: Optional[str] = typer.Argument(
-        "", help="The name of the person to greet", show_default=False, metavar="[name]"
+        None, help="The name of the person to greet.", show_default=False, metavar="[name]"
     ),
-    bye: bool = typer.Option(False, "--bye", "-b", help="Also write bye at the end"),
-    log_enabled: bool = typer.Option(False, "--log", "-l", help="Enable logging"),
+    bye: bool = typer.Option(False, "--bye", "-b", help='Also write "bye" at the end.'),
+    log_enabled: bool = typer.Option(False, "--log", "-l", help="Enable logging."),
 ) -> None:
     """
-    This is the hidden Greeting function.
+    This is the hidden greeting function.
     It allows you to greet someone with different colors in different languages.
     """
+    if not name:
+        try:
+            name = os.getlogin().capitalize()
+        except OSError:  # We need this, will fail on GitHub otherwise...
+            name = ""
     utils.greet(str(name), bye, log_enabled)
 
 
 # fotoobo specific commands
-app.add_typer(convert.app, name="convert", help="Convert commands for fotoobo")
-app.add_typer(get.app, name="get", help="get commands for fotoobo")
+app.add_typer(convert.app, name="convert", help="Convert commands for fotoobo.")
+app.add_typer(get.app, name="get", help="Get information about fotoobo or your configuration.")
 
 # commands for the Fortinet products
-app.add_typer(ems.app, name="ems", help="Commands for FortiClient EMS")
-app.add_typer(faz.app, name="faz", help="Commands for FortiAnalyzer")
-app.add_typer(fgt.app, name="fgt", help="Commands for FortiGate")
-app.add_typer(fmg.app, name="fmg", help="Commands for FortiManager")
+app.add_typer(ems.app, name="ems", help="Commands for FortiClient EMS.")
+app.add_typer(faz.app, name="faz", help="Commands for FortiAnalyzer.")
+app.add_typer(fgt.app, name="fgt", help="Commands for FortiGate.")
+app.add_typer(fmg.app, name="fmg", help="Commands for FortiManager.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fotoobo-0.7.0/fotoobo/exceptions/exceptions.py` & `fotoobo-0.8.0/fotoobo/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/convert.py` & `fotoobo-0.8.0/fotoobo/fortinet/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/fortianalyzer.py` & `fotoobo-0.8.0/fotoobo/fortinet/fortianalyzer.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/forticlientems.py` & `fotoobo-0.8.0/fotoobo/fortinet/forticlientems.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/fortigate.py` & `fotoobo-0.8.0/fotoobo/fortinet/fortigate.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/fortigate_config.py` & `fotoobo-0.8.0/fotoobo/fortinet/fortigate_config.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/fortigate_config_check.py` & `fotoobo-0.8.0/fotoobo/fortinet/fortigate_config_check.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/fortigate_info.py` & `fotoobo-0.8.0/fotoobo/fortinet/fortigate_info.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/fortimanager.py` & `fotoobo-0.8.0/fotoobo/fortinet/fortimanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,17 +220,17 @@
             "method": "exec",
             "params": [{"url": "/sys/logout"}],
             "session": self.sessionkey,
         }
         response = self.api("post", payload=payload)
         return response.status_code
 
-    def set(self, adom: str, payloads: Any) -> int:
+    def post(self, adom: str, payloads: Any) -> int:
         """
-        Set method to FortiManager.
+        POST method to FortiManager.
 
         You can pass a single payload (Dict) or a list of payloads (List of Dict).
 
         Args:
             adom (str): the ADOM name to issue the set commands to. If you wish to update the
             Global ADOM specify 'global' as ADOM.
```

### Comparing `fotoobo-0.7.0/fotoobo/fortinet/fortinet.py` & `fotoobo-0.8.0/fotoobo/fortinet/fortinet.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/helpers/cli.py` & `fotoobo-0.8.0/fotoobo/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/helpers/config.py` & `fotoobo-0.8.0/fotoobo/helpers/config.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/helpers/files.py` & `fotoobo-0.8.0/fotoobo/helpers/files.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/helpers/log.py` & `fotoobo-0.8.0/fotoobo/helpers/log.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/helpers/output.py` & `fotoobo-0.8.0/fotoobo/helpers/output.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/inventory/generic.py` & `fotoobo-0.8.0/fotoobo/inventory/generic.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/inventory/inventory.py` & `fotoobo-0.8.0/fotoobo/inventory/inventory.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/main.py` & `fotoobo-0.8.0/fotoobo/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/convert.py` & `fotoobo-0.8.0/fotoobo/utils/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/ems/get.py` & `fotoobo-0.8.0/fotoobo/utils/ems/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/ems/monitor.py` & `fotoobo-0.8.0/fotoobo/utils/ems/monitor.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/faz/get.py` & `fotoobo-0.8.0/fotoobo/utils/faz/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/fgt/check.py` & `fotoobo-0.8.0/fotoobo/utils/fgt/monitor.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/fgt/config.py` & `fotoobo-0.8.0/fotoobo/utils/fgt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from fotoobo.exceptions import GeneralError, GeneralWarning
 from fotoobo.fortinet.fortigate_config import FortiGateConfig
 from fotoobo.fortinet.fortigate_config_check import FortiGateConfigCheck
 from fotoobo.helpers.files import load_yaml_file
 from fotoobo.helpers.output import Output
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True, rich_markup_mode="rich")
 log = logging.getLogger("fotoobo")
 
 
 def check(config: str, bundles: str) -> None:
     """
     The FortiGate configuration check
```

### Comparing `fotoobo-0.7.0/fotoobo/utils/fgt/get.py` & `fotoobo-0.8.0/fotoobo/utils/fgt/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/fgt/main.py` & `fotoobo-0.8.0/fotoobo/utils/fgt/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/fmg/get.py` & `fotoobo-0.8.0/fotoobo/utils/fmg/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/fotoobo/utils/fmg/main.py` & `fotoobo-0.8.0/fotoobo/utils/fmg/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             if message["history"]:
                 for line in message["history"]:
                     getattr(log, level)("- %s", line["detail"])
 
     fmg.logout()
 
 
-def set(host: str, file: str, adom: str) -> None:  # pylint: disable=redefined-builtin
+def post(host: str, file: str, adom: str) -> None:
     """
     Set the given configuration from a JSON file to the FortiManager
 
     Args:
         host (str): The FortiManager defined in inventory
         file (str): The configuration file to oad the configuration from
         adom (str): The ADOM to assign the global policy to
@@ -73,9 +73,9 @@
     inventory = Inventory(config.inventory_file)
     fmg = inventory.get(host, "fortimanager")[host]
     fmg.login()
 
     log.debug("FortiManager set command ...")
     log.info("start setting assets to '%s'", host + "/" + adom)
 
-    fmg.set(adom, payloads)
+    fmg.post(adom, payloads)
     fmg.logout()
```

### Comparing `fotoobo-0.7.0/fotoobo/utils/fmg/set_.py` & `fotoobo-0.8.0/fotoobo/utils/fmg/post_.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from fotoobo.helpers.config import config
 from fotoobo.helpers.files import load_json_file
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
 
 
-def set(host: str, file: str, adom: str) -> None:  # pylint: disable=redefined-builtin
+def post(host: str, file: str, adom: str) -> None:
     """
-    Set the given configuration from a JSON file to the FortiManager
+    POST the given configuration from a JSON file to the FortiManager
 
     Args:
         host (str): The FortiManager defined in inventory
         file (str): The configuration file to oad the configuration from
         adom (str): The ADOM to assign the global policy to
 
     Raises:
@@ -29,9 +29,9 @@
     inventory = Inventory(config.inventory_file)
     fmg = inventory.get(host, "fortimanager")[host]
     fmg.login()
 
     log.debug("FortiManager set command ...")
     log.info("start setting assets to '%s'", host + "/" + adom)
 
-    fmg.set(adom, payloads)
+    fmg.post(adom, payloads)
     fmg.logout()
```

### Comparing `fotoobo-0.7.0/fotoobo/utils/get.py` & `fotoobo-0.8.0/fotoobo/utils/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         data_table.append({"host": host, "hostname": data.hostname, "type": data.type})
     print_datatable(data_table, title="fotoobo inventory", headers=["Device", "Hostname", "Type"])
 
 
 def version(verbose: bool = False) -> None:
     """Get the fotoobo version"""
     log.debug("printing fotoobo version information: %s", __version__)
-    versions = [{"module": "fotoobo", "version": __version__}]
+    if not verbose:
+        versions = [{"module": "fotoobo", "version": __version__}]
+    else:
+        versions = [{"module": "[bold]fotoobo[/]", "version": "[bold]" + __version__ + "[/]"}]
+        modules = ["pysnmp", "jinja2", "PyYAML", "requests", "rich", "typer"]
 
-    modules = ["pysnmp", "jinja2", "PyYAML", "requests", "rich", "typer"]
-    if verbose:
         for module in modules:
             versions.append({"module": module, "version": importlib.metadata.version(module)})
 
     print_datatable(versions, title="fotoobo version")
```

### Comparing `fotoobo-0.7.0/fotoobo/utils/greet.py` & `fotoobo-0.8.0/fotoobo/utils/greet.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.7.0/pyproject.toml` & `fotoobo-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fotoobo"
-version = "0.7.0"
+version = "0.8.0"
 description = "The awesome Fortinet Toolbox"
 authors = ["Patrik Spiess <patrik.spiess@mgb.ch>", "Lukas Murer-Jäckle <lukas.murer@mgb.ch>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.12"
 typer = "~0.6.0"
```

### Comparing `fotoobo-0.7.0/PKG-INFO` & `fotoobo-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fotoobo
-Version: 0.7.0
+Version: 0.8.0
 Summary: The awesome Fortinet Toolbox
 Author: Patrik Spiess
 Author-email: patrik.spiess@mgb.ch
 Requires-Python: >=3.8.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

