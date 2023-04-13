# Comparing `tmp/jz-hydra-submitit-launcher-0.1.4.tar.gz` & `tmp/jz-hydra-submitit-launcher-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jz-hydra-submitit-launcher-0.1.4.tar", last modified: Thu Aug 18 15:42:00 2022, max compression
+gzip compressed data, was "jz-hydra-submitit-launcher-0.1.5.tar", last modified: Thu Apr 13 09:31:10 2023, max compression
```

## Comparing `jz-hydra-submitit-launcher-0.1.4.tar` & `jz-hydra-submitit-launcher-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 15:42:00.339933 jz-hydra-submitit-launcher-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-08-18 15:42:00.339933 jz-hydra-submitit-launcher-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 15:42:00.335933 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 15:42:00.339933 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-18 15:41:53.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 15:42:00.339933 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/bin/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/bin/hydra-submitit-launch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 15:42:00.335933 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 15:42:00.339933 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/4gpus_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/4gpus_t3.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/4gpus_t4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/base.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/dev.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/t3.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/t4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/searchpath_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 15:42:00.339933 jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-08-18 15:42:00.000000 jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-18 15:42:00.000000 jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 15:42:00.000000 jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 15:42:00.000000 jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-18 15:42:00.000000 jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-18 15:42:00.000000 jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 15:42:00.339933 jz-hydra-submitit-launcher-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-08-18 15:41:52.000000 jz-hydra-submitit-launcher-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:31:10.268117 jz-hydra-submitit-launcher-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-13 09:31:10.268117 jz-hydra-submitit-launcher-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:31:10.264117 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:31:10.264117 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 09:31:00.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:31:10.268117 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/bin/hydra-submitit-launch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:31:10.264117 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:31:10.268117 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/4gpus_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/4gpus_t3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/4gpus_t4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/t3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/hydra/launcher/t4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/searchpath_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:31:10.268117 jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-13 09:31:10.000000 jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-13 09:31:10.000000 jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:31:10.000000 jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:31:10.000000 jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 09:31:10.000000 jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 09:31:10.000000 jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:31:10.268117 jz-hydra-submitit-launcher-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 09:30:59.000000 jz-hydra-submitit-launcher-0.1.5/setup.py
```

### Comparing `jz-hydra-submitit-launcher-0.1.4/LICENSE` & `jz-hydra-submitit-launcher-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jz-hydra-submitit-launcher-0.1.4/PKG-INFO` & `jz-hydra-submitit-launcher-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: jz-hydra-submitit-launcher
-Version: 0.1.4
-Summary: Jean Zay tailored Hydra submitit launcher.
-Home-page: https://github.com/zaccharieramzi/jz-hydra-submitit-launcher
-Author: Zaccharie Ramzi
-Author-email: zaccharie.ramzi@gmail.com
-License: MIT
-Keywords: hydra,submitit,jean-zay
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JZ-hydra-submitit-launcher
 
 ![GitHub Workflow Build Status](https://github.com/zaccharieramzi/jz-hydra-submitit-launcher/workflows/Continuous%20testing/badge.svg)
 
 A Jean Zay (JZ) tailored Hydra submitit launcher based on [Hydra](https://hydra.cc/docs/intro/) and its [submitit-launcher plugin](https://hydra.cc/docs/plugins/submitit_launcher/).
 Basically it extends the submitit-launcher plugin with defaults that make sense for JZ.
 
@@ -31,14 +15,23 @@
 You can also install it from source:
 ```
 git clone https://github.com/zaccharieramzi/jz-hydra-submitit-launcher.git
 cd jz-hydra-submitit-launcher
 pip install --user .
 ```
 
+The main command is then installed in your local binaries.
+You need to add them to your path in order for the command to be found (and avoid the error `-bash: hydra-submitit-launch: command not found`):
+
+```
+echo "export PATH=$PATH:$HOME/.local/bin" >> $HOME/.bashrc
+```
+
+Don't forget to `source $HOME/.bashrc` before using the command.
+
 ## Use
 
 The primary use is with the `hydra-submitit-launch` command with your script name and the config type:
 ```
 hydra-submitit-launch my_app.py dev
 ```
 
@@ -59,16 +52,20 @@
 For example, if you want to use the gpu_p2 partition, you would need to do:
 ```
 hydra-submitit-launch my_app.py dev hydra.launcher.setup=null hydra.launcher.partition=gpu_p2 hydra.launcher.cpus_per_task=3
 ```
 
 In order to change the timeout on the SLURM job to for example 10 hours, you would need to do:
 ```
-hydra-submitit-launch my_app.py base +hydra.launcher.hours=10
+hydra-submitit-launch my_app.py base +hours=10
 ```
-This will automatically select the right qos for you.
+This will automatically select the right qos for you (and if you want to force a certain qos, you can always add `hydra.launcher.qos=<your-qos>`).
+
+### Logs
+Your SLURM logs are stored in the following path: `launch-dir/multirun/day-of-launch/time-of-launch/.submitit/job_array_task_id/`
+This is the default from `hydra` and `submitit` and this can be changed using both the `submitit` plugin parameters (see [here](https://hydra.cc/docs/plugins/submitit_launcher/#usage)) and the `hydra` job configurations (see [here](https://hydra.cc/docs/configure_hydra/job/)). 
 
 ## References
 - Hydra: https://hydra.cc/docs/intro/
 - submitit-launcher: https://hydra.cc/docs/plugins/submitit_launcher/
 - submitit: https://github.com/facebookincubator/submitit
 - JZ docs: http://www.idris.fr/ or https://jean-zay-doc.readthedocs.io/en/latest/
```

### Comparing `jz-hydra-submitit-launcher-0.1.4/hydra_plugins/jz_hydra_submitit_launcher/searchpath_config.py` & `jz-hydra-submitit-launcher-0.1.5/hydra_plugins/jz_hydra_submitit_launcher/searchpath_config.py`

 * *Files identical despite different names*

### Comparing `jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/PKG-INFO` & `jz-hydra-submitit-launcher-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jz-hydra-submitit-launcher
-Version: 0.1.4
+Version: 0.1.5
 Summary: Jean Zay tailored Hydra submitit launcher.
 Home-page: https://github.com/zaccharieramzi/jz-hydra-submitit-launcher
 Author: Zaccharie Ramzi
 Author-email: zaccharie.ramzi@gmail.com
 License: MIT
 Keywords: hydra,submitit,jean-zay
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,23 @@
 You can also install it from source:
 ```
 git clone https://github.com/zaccharieramzi/jz-hydra-submitit-launcher.git
 cd jz-hydra-submitit-launcher
 pip install --user .
 ```
 
+The main command is then installed in your local binaries.
+You need to add them to your path in order for the command to be found (and avoid the error `-bash: hydra-submitit-launch: command not found`):
+
+```
+echo "export PATH=$PATH:$HOME/.local/bin" >> $HOME/.bashrc
+```
+
+Don't forget to `source $HOME/.bashrc` before using the command.
+
 ## Use
 
 The primary use is with the `hydra-submitit-launch` command with your script name and the config type:
 ```
 hydra-submitit-launch my_app.py dev
 ```
 
@@ -59,16 +68,20 @@
 For example, if you want to use the gpu_p2 partition, you would need to do:
 ```
 hydra-submitit-launch my_app.py dev hydra.launcher.setup=null hydra.launcher.partition=gpu_p2 hydra.launcher.cpus_per_task=3
 ```
 
 In order to change the timeout on the SLURM job to for example 10 hours, you would need to do:
 ```
-hydra-submitit-launch my_app.py base +hydra.launcher.hours=10
+hydra-submitit-launch my_app.py base +hours=10
 ```
-This will automatically select the right qos for you.
+This will automatically select the right qos for you (and if you want to force a certain qos, you can always add `hydra.launcher.qos=<your-qos>`).
+
+### Logs
+Your SLURM logs are stored in the following path: `launch-dir/multirun/day-of-launch/time-of-launch/.submitit/job_array_task_id/`
+This is the default from `hydra` and `submitit` and this can be changed using both the `submitit` plugin parameters (see [here](https://hydra.cc/docs/plugins/submitit_launcher/#usage)) and the `hydra` job configurations (see [here](https://hydra.cc/docs/configure_hydra/job/)). 
 
 ## References
 - Hydra: https://hydra.cc/docs/intro/
 - submitit-launcher: https://hydra.cc/docs/plugins/submitit_launcher/
 - submitit: https://github.com/facebookincubator/submitit
 - JZ docs: http://www.idris.fr/ or https://jean-zay-doc.readthedocs.io/en/latest/
```

### Comparing `jz-hydra-submitit-launcher-0.1.4/jz_hydra_submitit_launcher.egg-info/SOURCES.txt` & `jz-hydra-submitit-launcher-0.1.5/jz_hydra_submitit_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jz-hydra-submitit-launcher-0.1.4/setup.py` & `jz-hydra-submitit-launcher-0.1.5/setup.py`

 * *Files identical despite different names*

