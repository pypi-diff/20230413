# Comparing `tmp/dbt_coves-1.4.3.tar.gz` & `tmp/dbt_coves-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.4.3.tar", max compression
+gzip compressed data, was "dbt_coves-1.4.4.tar", max compression
```

## Comparing `dbt_coves-1.4.3.tar` & `dbt_coves-1.4.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11357 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/LICENSE
--rw-r--r--   0        0        0    21434 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/README.md
--rw-r--r--   0        0        0       22 2023-04-06 17:02:45.263833 dbt_coves-1.4.3/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0     9630 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0      650 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     4914 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     2956 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0     4297 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    11765 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4512 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    18472 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     1520 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10562 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8880 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    13956 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2653 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    22617 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0     2153 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    17204 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0     1744 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/setup/all.py
--rw-r--r--   0        0        0     4215 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6689 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1183 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0    10142 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      685 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0     4608 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/airbyte_api.py
--rw-r--r--   0        0        0    12118 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    13747 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1132 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/log.py
--rw-r--r--   0        0        0      791 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     1010 2023-04-06 17:01:46.243742 dbt_coves-1.4.3/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3520 2023-04-06 17:02:45.263833 dbt_coves-1.4.3/pyproject.toml
--rw-r--r--   0        0        0    23417 1970-01-01 00:00:00.000000 dbt_coves-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 13:15:51.625551 dbt_coves-1.4.4/LICENSE
+-rw-r--r--   0        0        0    21434 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/README.md
+-rw-r--r--   0        0        0       22 2023-04-13 13:16:49.815541 dbt_coves-1.4.4/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0     9630 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0      650 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     4914 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     2956 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0     4308 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    11765 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4512 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    18472 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     1520 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10562 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8880 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    13956 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2653 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    22617 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0     2153 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    17204 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0     1744 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/setup/all.py
+-rw-r--r--   0        0        0     4215 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6689 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1183 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0    10142 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      685 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0     4608 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/airbyte_api.py
+-rw-r--r--   0        0        0    12118 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    13747 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1132 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0      791 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     1010 2023-04-13 13:15:51.629551 dbt_coves-1.4.4/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3520 2023-04-13 13:16:49.815541 dbt_coves-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0    23417 1970-01-01 00:00:00.000000 dbt_coves-1.4.4/PKG-INFO
```

### Comparing `dbt_coves-1.4.3/LICENSE` & `dbt_coves-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/README.md` & `dbt_coves-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/config/config.py` & `dbt_coves-1.4.4/dbt_coves/config/config.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/core/exceptions.py` & `dbt_coves-1.4.4/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/core/main.py` & `dbt_coves-1.4.4/dbt_coves/core/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/base.py` & `dbt_coves-1.4.4/dbt_coves/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.4.4/dbt_coves/tasks/dbt/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         )
 
         return ext_subparser
 
     def run(self) -> int:
         project_dir = self.get_config_value("project_dir")
         if not project_dir:
-            project_dir = os.environ.get("DBT_PROJECT_DIR", os.environ.get("DBT_HOME"))
+            project_dir = os.environ.get("DBT_PROJECT_DIR", os.environ.get("DATACOVES__DBT_HOME"))
         if not project_dir:
             console.print("[red]No dbt project specified[/red].")
             return -1
 
         command = self.get_config_value("command")
         if self.is_readonly(project_dir):
             tmp_dir = tempfile.NamedTemporaryFile().name
```

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.4.4/dbt_coves/tasks/extract/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.4.4/dbt_coves/tasks/extract/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.4.4/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.4.4/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.4.4/dbt_coves/tasks/generate/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.4.4/dbt_coves/tasks/generate/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.4.4/dbt_coves/tasks/generate/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.4.4/dbt_coves/tasks/generate/sources.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.4.4/dbt_coves/tasks/generate/templates.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.4.4/dbt_coves/tasks/load/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/load/base.py` & `dbt_coves-1.4.4/dbt_coves/tasks/load/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.4.4/dbt_coves/tasks/load/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/load/main.py` & `dbt_coves-1.4.4/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/setup/all.py` & `dbt_coves-1.4.4/dbt_coves/tasks/setup/all.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.4.4/dbt_coves/tasks/setup/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.4.4/dbt_coves/tasks/setup/git.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/setup/main.py` & `dbt_coves-1.4.4/dbt_coves/tasks/setup/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.4.4/dbt_coves/tasks/setup/ssh.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/tasks/setup/utils.py` & `dbt_coves-1.4.4/dbt_coves/tasks/setup/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.4.4/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/ui/traceback.py` & `dbt_coves-1.4.4/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/utils/airbyte_api.py` & `dbt_coves-1.4.4/dbt_coves/utils/airbyte_api.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/utils/api_caller.py` & `dbt_coves-1.4.4/dbt_coves/utils/api_caller.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/utils/flags.py` & `dbt_coves-1.4.4/dbt_coves/utils/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/utils/jinja.py` & `dbt_coves-1.4.4/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/utils/log.py` & `dbt_coves-1.4.4/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/utils/shell.py` & `dbt_coves-1.4.4/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/dbt_coves/utils/yaml.py` & `dbt_coves-1.4.4/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.3/pyproject.toml` & `dbt_coves-1.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.4.3"
+version = "1.4.4"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Information Technology",
```

### Comparing `dbt_coves-1.4.3/PKG-INFO` & `dbt_coves-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-coves
-Version: 1.4.3
+Version: 1.4.4
 Summary: CLI tool for dbt users adopting analytics engineering best practices.
 Home-page: https://datacoves.com
 License: Apache 2.0
 Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
 Author: Datacoves
 Author-email: hello@datacoves.com
 Requires-Python: >=3.7.2,<3.11
```

