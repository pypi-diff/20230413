# Comparing `tmp/ECSctrl-0.2.2.tar.gz` & `tmp/ECSctrl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ECSctrl-0.2.2.tar", last modified: Mon Jun 27 12:28:55 2022, max compression
+gzip compressed data, was "ECSctrl-0.3.0.tar", last modified: Thu Apr 13 17:41:55 2023, max compression
```

## Comparing `ECSctrl-0.2.2.tar` & `ECSctrl-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 12:28:55.689942 ECSctrl-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 12:28:55.689942 ECSctrl-0.2.2/ECSctrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6824 2022-06-27 12:28:55.000000 ECSctrl-0.2.2/ECSctrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-06-27 12:28:55.000000 ECSctrl-0.2.2/ECSctrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 12:28:55.000000 ECSctrl-0.2.2/ECSctrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-27 12:28:55.000000 ECSctrl-0.2.2/ECSctrl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 12:28:53.000000 ECSctrl-0.2.2/ECSctrl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-27 12:28:55.000000 ECSctrl-0.2.2/ECSctrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-27 12:28:55.000000 ECSctrl-0.2.2/ECSctrl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6824 2022-06-27 12:28:55.689942 ECSctrl-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6370 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 12:28:55.689942 ECSctrl-0.2.2/ecsctrl/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-27 12:28:45.000000 ECSctrl-0.2.2/ecsctrl/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/ecsctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/ecsctrl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/ecsctrl/boto_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    11497 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/ecsctrl/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/ecsctrl/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/ecsctrl/service_updater.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/ecsctrl/yaml_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 12:28:55.689942 ECSctrl-0.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-27 12:28:55.689942 ECSctrl-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-06-27 12:28:43.000000 ECSctrl-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.599025 ECSctrl-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/ECSctrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/ecsctrl/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 17:41:48.000000 ECSctrl-0.3.0/ecsctrl/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/boto_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/service_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/yaml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:41:55.599025 ECSctrl-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/tests/test_yaml_converter.py
```

### Comparing `ECSctrl-0.2.2/ECSctrl.egg-info/PKG-INFO` & `ECSctrl-0.3.0/ECSctrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ECSctrl
-Version: 0.2.2
+Version: 0.3.0
 Summary: ECSctrl - utility to deploy ECS services for humans
 Home-page: http://github.com/wlatanowicz/ecsctrl
 Author: Wiktor Latanowicz
 Author-email: ecsctrl@wiktor.latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ECSctrl-0.2.2/PKG-INFO` & `ECSctrl-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ECSctrl
-Version: 0.2.2
+Version: 0.3.0
 Summary: ECSctrl - utility to deploy ECS services for humans
 Home-page: http://github.com/wlatanowicz/ecsctrl
 Author: Wiktor Latanowicz
 Author-email: ecsctrl@wiktor.latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ECSctrl-0.2.2/README.md` & `ECSctrl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ECSctrl-0.2.2/ecsctrl/cli.py` & `ECSctrl-0.3.0/ecsctrl/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,86 @@
-from email.policy import default
 import os
-import click
 import re
+from email.policy import default
+
+import click
 
 from ecsctrl.loader import VarsLoader
 
 from .boto_client import BotoClient
+from .service_updater import ServiceUpdater, TaskDefinitionServiceUpdater, WaitForUpdate
 from .yaml_converter import yaml_file_to_dict
 
-from .service_updater import TaskDefinitionServiceUpdater, WaitForUpdate, ServiceUpdater
-
 
 def check_var(ctx, param, value):
     for v in value:
         if not re.match("^[^=]+=.*$", v):
             raise click.BadParameter(
                 f"'{v}'. Variable has to be in format variable=value"
             )
     return value
 
 
+# fmt: off
 @click.group()
-@click.option(
-    "--dry-run", is_flag=True, default=False, help="Do not call actual AWS API"
-)
+@click.option("--dry-run", is_flag=True, default=False, help="Do not call actual AWS API")
 @click.pass_context
+# fmt: on
 def cli(ctx, dry_run):
     ctx.ensure_object(dict)
     ctx.obj["dry_run"] = dry_run
     ctx.obj["boto_client"] = BotoClient("ecs", dry_run=dry_run)
 
 
 @cli.group(name="task-definition")
 @click.pass_context
 def task_definition(ctx):
     """Task definition management."""
 
 
+def common_options(fn):
+    # fmt: off
+    fn = click.option("--env-file", "-e", multiple=True, type=str, help="Path to env-style file with variables")(fn)
+    fn = click.option("--json-file", "-j", multiple=True, type=str, help="Path to json file with variable")(fn)
+    fn = click.option("--var", "-v", multiple=True, type=str, callback=check_var, help="Single variable in format name=value")(fn)
+    fn = click.option("--sys-env/--no-sys-env", is_flag=True, default=False, help="Uses system env as a source for template variables")(fn)
+    # fmt: on
+    return fn
+
+
+def wait_options(wait_for, many=False):
+    def wrapper(fn):
+        s = "s" if many else ""
+        # fmt: off
+        fn = click.option("--wait", "-w", is_flag=True, help=f"Waits for service{s} to finish {wait_for}")(fn)
+        fn = click.option("--wait-timeout", default=600, type=int, help=f"Custom timeout in seconds (defaults to 600s)")(fn)
+        # fmt: on
+        return fn
+
+    return wrapper
+
+
 # fmt: off
 @task_definition.command()
 @click.argument("spec-file", type=str)
-@click.option("--env-file", "-e", multiple=True, type=str, help="Path to env-style file with variables")
-@click.option("--json-file", "-j", multiple=True, type=str, help="Path to json file with variable")
-@click.option("--var", "-v", multiple=True, type=str, callback=check_var, help="Single variable in format name=value")
-@click.option("--sys-env/--no-sys-env", is_flag=True, default=False, help="Uses system env as a source for template variables")
+@common_options
 @click.option("--update-services-in-cluster", "-c", multiple=True, type=str, help="Updates all services deployed with this task in a particular cluster")
-@click.option("--wait", "-w", is_flag=True, help="Waits for services to finish update")
+@wait_options(wait_for="update", many=True)
 @click.pass_context
 # fmt: on
 def register(
     ctx,
     spec_file,
     env_file,
     json_file,
     var,
     sys_env,
     update_services_in_cluster,
     wait,
+    wait_timeout,
 ):
     """Register task definition."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
     spec = yaml_file_to_dict(spec_file, vars)
     task_family = spec.get("family", "N/A")
     click.echo(f"🗂 Registering task definition {task_family}.")
@@ -76,34 +96,39 @@
                 ctx.obj["boto_client"], task_definition_arn, cluster_name
             )
             updated_services_in_cluster = updater.update()
             updated_services[cluster_name] = updated_services_in_cluster
 
         if wait:
             waiter = WaitForUpdate(ctx.obj["boto_client"], updated_services)
+            waiter.timeout = wait_timeout
             waiter.wait_for_all()
 
 
 @cli.group(name="service")
 @click.pass_context
 def service(ctx):
     """Service management."""
 
 
-# fmt: off
 @service.command()
 @click.argument("spec-file", type=str)
-@click.option("--env-file", "-e", multiple=True, type=str, help="Path to env-style file with variables")
-@click.option("--json-file", "-j", multiple=True, type=str, help="Path to json file with variable")
-@click.option("--var", "-v", multiple=True, type=str, callback=check_var, help="Single variable in format name=value")
-@click.option("--sys-env/--no-sys-env", is_flag=True, default=False, help="Uses system env as a source for template variables")
-@click.option("--wait", "-w", is_flag=True, help="Waits for services to finish creation")
+@common_options
+@wait_options(wait_for="creation")
 @click.pass_context
-# fmt: on
-def create(ctx, spec_file, env_file, json_file, var, sys_env, wait):
+def create(
+    ctx,
+    spec_file,
+    env_file,
+    json_file,
+    var,
+    sys_env,
+    wait,
+    wait_timeout,
+):
     """Create a new service."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
     spec = yaml_file_to_dict(spec_file, vars)
     service_name = spec.get("serviceName")
     cluster_name = spec.get("cluster")
     click.echo(f"🏸 Creating service {service_name}.")
@@ -112,28 +137,33 @@
     click.echo("\t✅ done.")
 
     if wait:
         waiter = WaitForUpdate(
             ctx.obj["boto_client"],
             {cluster_name: [(service_arn, service_name)]},
         )
+        waiter.timeout = wait_timeout
         waiter.wait_for_all()
 
 
-# fmt: off
 @service.command()
 @click.argument("spec-file", type=str)
-@click.option("--env-file", "-e", multiple=True, type=str, help="Path to env-style file with variables")
-@click.option("--json-file", "-j", multiple=True, type=str, help="Path to json file with variable")
-@click.option("--var", "-v", multiple=True, type=str, callback=check_var, help="Single variable in format name=value")
-@click.option("--sys-env/--no-sys-env", is_flag=True, default=False, help="Uses system env as a source for template variables")
-@click.option("--wait", "-w", is_flag=True, help="Waits for services to finish update")
+@common_options
+@wait_options(wait_for="update")
 @click.pass_context
-# fmt: on
-def update(ctx, spec_file, env_file, json_file, var, sys_env, wait):
+def update(
+    ctx,
+    spec_file,
+    env_file,
+    json_file,
+    var,
+    sys_env,
+    wait,
+    wait_timeout,
+):
     """Update an existing service."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
     spec = yaml_file_to_dict(spec_file, vars)
     service_name = spec.get("serviceName")
     cluster_name = spec.get("cluster")
     click.echo(f"🏸 Updating service {service_name}.")
@@ -144,28 +174,33 @@
     click.echo("\t✅ done.")
 
     if wait:
         waiter = WaitForUpdate(
             ctx.obj["boto_client"],
             {cluster_name: [(service_arn, service_name)]},
         )
+        waiter.timeout = wait_timeout
         waiter.wait_for_all()
 
 
-# fmt: off
 @service.command("create-or-update")
 @click.argument("spec-file", type=str)
-@click.option("--env-file", "-e", multiple=True, type=str, help="Path to env-style file with variables")
-@click.option("--json-file", "-j", multiple=True, type=str, help="Path to json file with variable")
-@click.option("--var", "-v", multiple=True, type=str, callback=check_var, help="Single variable in format name=value")
-@click.option("--sys-env/--no-sys-env", is_flag=True, default=False, help="Uses system env as a source for template variables")
-@click.option("--wait", "-w", is_flag=True, help="Waits for services to finish update")
+@common_options
+@wait_options(wait_for="update")
 @click.pass_context
-# fmt: on
-def create_or_update(ctx, spec_file, env_file, json_file, var, sys_env, wait):
+def create_or_update(
+    ctx,
+    spec_file,
+    env_file,
+    json_file,
+    var,
+    sys_env,
+    wait,
+    wait_timeout,
+):
     """Check if service exists and update it or create a new one."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
     spec = yaml_file_to_dict(spec_file, vars)
     service_name = spec.get("serviceName")
     cluster_name = spec.get("cluster")
 
@@ -189,33 +224,36 @@
     service_arn = response["service"]["serviceArn"]
 
     if wait:
         waiter = WaitForUpdate(
             ctx.obj["boto_client"],
             {cluster_name: [(service_arn, service_name)]},
         )
+        waiter.timeout = wait_timeout
         waiter.wait_for_all()
 
 
 @cli.group(name="secrets")
 @click.pass_context
 def secrets(ctx):
     """Secrets management."""
 
 
-# fmt: off
 @secrets.command()
 @click.argument("spec-file", type=str)
-@click.option("--env-file", "-e", multiple=True, type=str, help="Path to env-style file with variables")
-@click.option("--json-file", "-j", multiple=True, type=str, help="Path to json file with variable")
-@click.option("--var", "-v", multiple=True, type=str, callback=check_var, help="Single variable in format name=value")
-@click.option("--sys-env/--no-sys-env", is_flag=True, default=False, help="Uses system env as a source for template variables")
+@common_options
 @click.pass_context
-# fmt: on
-def store(ctx, spec_file, env_file, json_file, var, sys_env):
+def store(
+    ctx,
+    spec_file,
+    env_file,
+    json_file,
+    var,
+    sys_env,
+):
     """Store secret is Parameter Store."""
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
     spec = yaml_file_to_dict(spec_file, vars)
     ssm = BotoClient("ssm", dry_run=ctx.obj["boto_client"].dry_run)
 
     for secret_name, value in spec.items():
         ssm_params = {
@@ -224,34 +262,30 @@
             "Type": "SecureString",
         }
         click.echo(f"🔑 Storing secret {secret_name}.")
         response = ssm.call("put_parameter", **ssm_params)
         click.echo(f"\t✅ done, parameter version: {response['Version']}")
 
 
-# fmt: off
 @service.command()
 @click.argument("task-definition-spec-file", type=str)
 @click.argument("service-spec-file", type=str)
-@click.option("--env-file", "-e", multiple=True, type=str, help="Path to env-style file with variables")
-@click.option("--json-file", "-j", multiple=True, type=str, help="Path to json file with variable")
-@click.option("--var", "-v", multiple=True, type=str, callback=check_var, help="Single variable in format name=value")
-@click.option("--sys-env/--no-sys-env", is_flag=True, default=False, help="Uses system env as a source for template variables")
-@click.option("--wait", "-w", is_flag=True, help="Waits for services to finish update")
+@common_options
+@wait_options(wait_for="update")
 @click.pass_context
-# fmt: on
 def deploy(
     ctx,
     task_definition_spec_file,
     service_spec_file,
     env_file,
     json_file,
     var,
     sys_env,
     wait,
+    wait_timeout,
 ):
     """All-in-one - register task definition and create or update service."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
     task_definition_spec = yaml_file_to_dict(task_definition_spec_file, vars)
     task_family = task_definition_spec.get("family", "N/A")
     click.echo(f"🗂 Registering task definition {task_family}.")
@@ -286,8 +320,9 @@
     service_arn = response["service"]["serviceArn"]
 
     if wait:
         waiter = WaitForUpdate(
             ctx.obj["boto_client"],
             {cluster_name: [(service_arn, service_name)]},
         )
+        waiter.timeout = wait_timeout
         waiter.wait_for_all()
```

### Comparing `ECSctrl-0.2.2/ecsctrl/loader.py` & `ECSctrl-0.3.0/ecsctrl/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import os
-import logging
 import json
+import logging
+import os
 from typing import Dict, List
 
-from jinja2 import Environment, FileSystemLoader, make_logging_undefined, Undefined
+from jinja2 import Environment, FileSystemLoader, Undefined, make_logging_undefined
 from jinja2.exceptions import TemplateNotFound
 from jinja2.utils import open_if_exists
 
-
 logger = logging.getLogger(__name__)
 
 
 class EnvFileLoader:
     def __init__(self, file_path: str):
         self.file_path = file_path
```

### Comparing `ECSctrl-0.2.2/ecsctrl/service_updater.py` & `ECSctrl-0.3.0/ecsctrl/service_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import math
+import os
 import re
+import sys
+from datetime import datetime, timezone
 from time import sleep, time
 from typing import Dict, List
-from datetime import datetime, timezone
-import sys
-import math
-import os
+
 import click
 
 
 class TaskDefinitionServiceUpdater:
     def __init__(
         self, boto_client, task_definition_arn: str, cluster_name: str
     ) -> None:
@@ -62,14 +63,17 @@
         )
 
 
 class WaitForUpdate:
     def __init__(self, boto_client, services_in_clusters: Dict[str, str]) -> None:
         self.boto_client = boto_client
         self.services_in_clusters = services_in_clusters
+        self.timeout = 600
+        self.wait_time = 60
+        self.min_task_age = 60
 
     def describe_all_services(self):
         described_services = []
         for cluster, services in self.services_in_clusters.items():
             arns = [service_arn for service_arn, service_name in services]
             while arns:
                 response = self.boto_client.call(
@@ -82,17 +86,15 @@
                 arns = arns[10:]
 
         return described_services
 
     def wait_for_all(self):
         total_failures = 1
         total_critical = False
-        timeout = 600
-        wait_time = 60
-        deadline = time() + timeout
+        deadline = time() + self.timeout
         start_time = time()
 
         while total_failures and not total_critical:
             total_failures = 0
             total_critical = False
             services = self.describe_all_services()
             for service in services:
@@ -116,22 +118,22 @@
                     click.echo(
                         f"⏳ Waiting for things to settle ({total_failures} check/s/ failed)"
                     )
 
                     pause_time = time()
                     if not os.environ.get("CI"):
                         animation = "🕐🕑🕒🕓🕔🕕🕖🕗🕘🕙🕚🕛"
-                        for i in range(wait_time * 10):
+                        for i in range(self.wait_time * 10):
                             sys.stdout.write("\r" + animation[i % len(animation)])
                             sys.stdout.flush()
                             sleep(0.1)
                         sys.stdout.write("\r")
                         sys.stdout.flush()
                     else:
-                        sleep(wait_time)
+                        sleep(self.wait_time)
 
                     time_passed = math.floor(time() - start_time)
                     resumed_after = math.floor(time() - pause_time)
                     click.echo("")
                     click.echo(
                         f"🚀 Resuming after {resumed_after}s ({time_passed}s passed from the beginning) "
                     )
@@ -142,16 +144,14 @@
         cluster_name = service_description["clusterName"]
         service_name = service_description["serviceName"]
         service_task_definition = service_description["taskDefinition"]
         service_task_desired_count = service_description["desiredCount"]
         service_task_running_count = service_description["runningCount"]
         service_task_pending_count = service_description["pendingCount"]
 
-        min_task_age = 60  # @TODO get from cli arguments
-
         deployments = service_description["deployments"]
         primary_deployment = [d for d in deployments if d["status"] == "PRIMARY"][0]
 
         click.echo("🔍 Running checks")
         click.echo(f"🌎 Cluster: {cluster_name}")
         click.echo(f"🏓 Service: {service_name}")
 
@@ -182,19 +182,19 @@
 
             task_age = int(
                 datetime.now().replace(tzinfo=timezone.utc).timestamp()
                 - task["createdAt"].replace(tzinfo=timezone.utc).timestamp()
             )
             task_task_definition = task["taskDefinitionArn"]
 
-            if task_age >= min_task_age:
+            if task_age >= self.min_task_age:
                 click.echo(f"\t😀 Task {task_arn} age is OK")
             else:
                 click.echo(
-                    f"\t😱 Task {task_arn} is to young ({task_age}s, {min_task_age}s minimum)"
+                    f"\t😱 Task {task_arn} is to young ({task_age}s, {self.min_task_age}s minimum)"
                 )
                 failures += 1
 
             if task_task_definition == service_task_definition:
                 click.echo(f"\t😀 Task {task_arn} task definition is OK")
             else:
                 click.echo(
```

### Comparing `ECSctrl-0.2.2/ecsctrl/yaml_converter.py` & `ECSctrl-0.3.0/ecsctrl/yaml_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from functools import partial
 from typing import Dict, List
+
 import yaml
 
 from .loader import SpecFileLoader
-from functools import partial
 
 TASK_DEFINITION = "taskDefinition"
 SERVICE = "service"
 
 
 def expand_key_value_list(key_field: str, value_field: str, obj: dict):
     if isinstance(obj, dict):
```

### Comparing `ECSctrl-0.2.2/setup.py` & `ECSctrl-0.3.0/setup.py`

 * *Files identical despite different names*

