# Comparing `tmp/gitlab-runner-tart-driver-0.1.0.tar.gz` & `tmp/gitlab-runner-tart-driver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.1.0.tar", last modified: Mon Apr 10 12:42:57 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.1.1.tar", last modified: Thu Apr 13 05:38:28 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.1.0.tar` & `gitlab-runner-tart-driver-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.657450 gitlab-runner-tart-driver-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    13443 2023-04-10 12:42:57.657450 gitlab-runner-tart-driver-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12922 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.650449 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.655449 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)     5005 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     3300 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.656450 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     5231 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 12:42:57.653449 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13443 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      986 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-10 12:42:57.000000 gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 12:42:57.657450 gitlab-runner-tart-driver-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-10 12:42:45.000000 gitlab-runner-tart-driver-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.762127 gitlab-runner-tart-driver-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    13625 2023-04-13 05:38:28.761127 gitlab-runner-tart-driver-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13104 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.756127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.759127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5787 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.761127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5231 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.758127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13625 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 05:38:28.762127 gitlab-runner-tart-driver-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.1.0/LICENSE.txt` & `gitlab-runner-tart-driver-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/PKG-INFO` & `gitlab-runner-tart-driver-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -127,14 +127,16 @@
 
 Now restart the gitlab-runner with `gitlab-runner restart`
 
 ## GitLab CI
 
 One of the great advantages in using [Tart](https://tart.run) is that it gives almost all functionality to we are used from the standard `docker` executors allowing us to write GitLabCI piplines that do not need any or minimal adaptions for OSX.
 
+> **ATTENTION:** The driver will always automatically login to your GitLab Registry using `CI_REGISTRY_USER`, `CI_REGISTRY_PASSWORD` and `CI_REGISTRY`
+
 ```yaml
 stages:
  - build
 
 run-on-tart:
   image: ghcr.io/cirruslabs/macos-ventura-base:latest
   stage:
@@ -157,17 +159,17 @@
 You can provide a default login registry using the `CLI` parameters (see **Command `prepare`**) but also provide the credentials from with each job variable definition
 
 ```yaml
 stages:
  - build
 
 variables:
-    TART_OCI_USERNAME: myuser@myregistry.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.registry.io
+    TART_REGISTRY_USERNAME: myuser@myregistry.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.registry.io
 
 job1:
   image: private.registry.io/tart/xcode14:latest
   stage:
     - build
   tags:
     - tart
@@ -179,17 +181,17 @@
     paths:
       - artifact.txt
 
 job2:
   image: private.other.io/tart/xcode14:latest
   variables:
     # override the OCI login information for this job only
-    TART_OCI_USERNAME: myuser@other.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.other.io
+    TART_REGISTRY_USERNAME: myuser@other.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.other.io
   stage:
     - build
   tags:
     - tart
   before_script:
     - brew install gitlab-runner # you will need to make sure `gitlab-runner` executable is available to be able to upload artifacts
   script:
@@ -204,17 +206,17 @@
 The [Tart managed images](https://tart.run) come with a default user `admin` and password `admin` which will be used to establish an ssh connection. If you decide to provide your own images, you might opt for a different user and password. You can provide the default user and password using the `config.toml` within the `run` section using `--default-ssh-user` and `--default-ssh-password` or provide it from within your job
 
 ```yaml
 job2:
   image: private.other.io/tart/xcode14:latest
   variables:
     # override the OCI login information for this job only
-    TART_OCI_USERNAME: myuser@other.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.other.io
+    TART_REGISTRY_USERNAME: myuser@other.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.other.io
     TART_SSH_USERNAME: gitlab
     TART_SSH_PASSWORD: gitlab
   stage:
     - build
   tags:
     - tart
   before_script:
@@ -321,17 +323,17 @@
 
   Prepare the environment and start the tart VM.
 
 Options:
   --pull-policy [always|if-not-present|never]
                                   define how runners pull tart images from
                                   registries
-  --oci-username TEXT             username to login to a oci registry
-  --oci-password TEXT             passowrd to login to a oci registry
-  --oci-host TEXT                 username to login to a oci registry
+  --registry-username TEXT        username to login to a oci registry
+  --registry-password TEXT        passowrd to login to a oci registry
+  --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
```

### Comparing `gitlab-runner-tart-driver-0.1.0/README.md` & `gitlab-runner-tart-driver-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,16 @@
 
 Now restart the gitlab-runner with `gitlab-runner restart`
 
 ## GitLab CI
 
 One of the great advantages in using [Tart](https://tart.run) is that it gives almost all functionality to we are used from the standard `docker` executors allowing us to write GitLabCI piplines that do not need any or minimal adaptions for OSX.
 
+> **ATTENTION:** The driver will always automatically login to your GitLab Registry using `CI_REGISTRY_USER`, `CI_REGISTRY_PASSWORD` and `CI_REGISTRY`
+
 ```yaml
 stages:
  - build
 
 run-on-tart:
   image: ghcr.io/cirruslabs/macos-ventura-base:latest
   stage:
@@ -142,17 +144,17 @@
 You can provide a default login registry using the `CLI` parameters (see **Command `prepare`**) but also provide the credentials from with each job variable definition
 
 ```yaml
 stages:
  - build
 
 variables:
-    TART_OCI_USERNAME: myuser@myregistry.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.registry.io
+    TART_REGISTRY_USERNAME: myuser@myregistry.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.registry.io
 
 job1:
   image: private.registry.io/tart/xcode14:latest
   stage:
     - build
   tags:
     - tart
@@ -164,17 +166,17 @@
     paths:
       - artifact.txt
 
 job2:
   image: private.other.io/tart/xcode14:latest
   variables:
     # override the OCI login information for this job only
-    TART_OCI_USERNAME: myuser@other.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.other.io
+    TART_REGISTRY_USERNAME: myuser@other.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.other.io
   stage:
     - build
   tags:
     - tart
   before_script:
     - brew install gitlab-runner # you will need to make sure `gitlab-runner` executable is available to be able to upload artifacts
   script:
@@ -189,17 +191,17 @@
 The [Tart managed images](https://tart.run) come with a default user `admin` and password `admin` which will be used to establish an ssh connection. If you decide to provide your own images, you might opt for a different user and password. You can provide the default user and password using the `config.toml` within the `run` section using `--default-ssh-user` and `--default-ssh-password` or provide it from within your job
 
 ```yaml
 job2:
   image: private.other.io/tart/xcode14:latest
   variables:
     # override the OCI login information for this job only
-    TART_OCI_USERNAME: myuser@other.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.other.io
+    TART_REGISTRY_USERNAME: myuser@other.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.other.io
     TART_SSH_USERNAME: gitlab
     TART_SSH_PASSWORD: gitlab
   stage:
     - build
   tags:
     - tart
   before_script:
@@ -306,17 +308,17 @@
 
   Prepare the environment and start the tart VM.
 
 Options:
   --pull-policy [always|if-not-present|never]
                                   define how runners pull tart images from
                                   registries
-  --oci-username TEXT             username to login to a oci registry
-  --oci-password TEXT             passowrd to login to a oci registry
-  --oci-host TEXT                 username to login to a oci registry
+  --registry-username TEXT        username to login to a oci registry
+  --registry-password TEXT        passowrd to login to a oci registry
+  --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
```

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 @click.command()
 @click.option(
     "--pull-policy",
     default="if-not-present",
     type=click.Choice(["always", "if-not-present", "never"]),
     help="define how runners pull tart images from registries",
 )
-@click.option("--oci-username", required=False, default=None, type=str, help="username to login to a oci registry")
-@click.option("--oci-password", required=False, default=None, type=str, help="passowrd to login to a oci registry")
-@click.option("--oci-host", required=False, default=None, type=str, help="username to login to a oci registry")
+@click.option("--registry-username", required=False, default=None, type=str, help="username to login to a oci registry")
+@click.option("--registry-password", required=False, default=None, type=str, help="passowrd to login to a oci registry")
+@click.option("--registry", required=False, default=None, type=str, help="username to login to a oci registry")
 @click.option("--cpu", required=False, default=None, type=int, help="Number of CPUs associated to VM")
 @click.option("--memory", required=False, default=None, type=int, help="VM memory size in megabytes associated to VM")
 @click.option(
     "--display",
     required=False,
     default=None,
     type=str,
@@ -40,17 +40,17 @@
     required=False,
     default=1,
     type=int,
     help="Number of concurrent processes that are supported. ATTENTION tart currently only support two concurrent VMs",
 )
 @click.option("-x", "--tart-executable", required=False, default="tart", type=str, help="Path to the tart executable.")
 def prepare(
-    oci_username,
-    oci_password,
-    oci_host,
+    registry_username,
+    registry_password,
+    registry,
     cpu,
     memory,
     display,
     pull_policy,
     auto_resources,
     concurrency,
     tart_executable,
@@ -69,32 +69,51 @@
 
     # for k,v in os.environ.items():
     #     click.echo(f'{k}={v}')
 
     ######################################################################
     # OCI LOGIN
     ######################################################################
-    if oci_username and oci_password and oci_host:
-        click.echo(f"[INFO] Logging into OCI Registry '{oci_host}'")
-        tart.login(username=oci_username, password=oci_password, host=oci_host)
-
-    if p.tart_oci_username and p.tart_oci_password and p.tart_oci_host:
-        click.echo(f"[INFO] Logging into OCI Registry '{p.tart_oci_host}'")
-        tart.login(username=p.tart_oci_username, password=p.tart_oci_password, host=p.tart_oci_host)
+    click.echo(f"[INFO] Logging into GitLab Registry '{p.ci_registry}'")
+    try:
+        tart.login(username=p.ci_registry_user, password=p.ci_registry_password, host=p.ci_registry)
+    except:
+        click.secho(f"[ERROR] Failed to login to '{p.ci_registry}'", fg="red")
+        sys.exit(1)
+
+    if registry_username and registry_password and registry:
+        click.echo(f"[INFO] Logging into OCI Registry '{registry}'")
+        try:
+            tart.login(username=registry_username, password=registry_password, host=registry)
+        except:
+            click.secho(f"[ERROR] Failed to login to '{registry}'", fg="red")
+            sys.exit(1)
+
+    if p.tart_registry_username and p.tart_registry_password and p.tart_registry:
+        click.echo(f"[INFO] Logging into custom OCI Registry '{p.tart_registry}'")
+        try:
+            tart.login(username=p.tart_registry_username, password=p.tart_registry_password, host=p.tart_registry)
+        except:
+            click.secho(f"[ERROR] Failed to login to '{p.tart_registry}'", fg="red")
+            sys.exit(1)
 
     ######################################################################
     # PULL
     ######################################################################
     if (
         (pull_policy == "always")
         or (p.ci_job_image not in tart_vm_map and pull_policy != "never")
         or (p.ci_job_image not in tart_vm_map and pull_policy == "if-not-present")
     ):
         click.echo(f"[INFO] Pulling '{p.ci_job_image}' [pull_policy={pull_policy}]")
-        tart.pull(p.ci_job_image)
+        try:
+            tart.pull(p.ci_job_image)
+        except:
+            click.secho(f"[ERROR] Failed to pull image '{p.ci_job_image}'", fg="red")
+            sys.exit(1)
     else:
         click.echo(f"[INFO] Skipping '{p.ci_job_image}' [pull_policy={pull_policy}]")
 
     ######################################################################
     # Create VM
     ######################################################################
     tart_vm_name = p.vm_name()
```

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/run.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,18 +7,22 @@
     """Config parameters needed throughout the process read from the environment"""
 
     ci_job_image: str
     ci_pipeline_id: str
     ci_job_id: str
     ci_concurrent_id: str
     ci_project_name: str
+    ci_registry: str
+    ci_registry_user: str
+    ci_registry_password: str
+
+    tart_registry_username: Optional[str]
+    tart_registry_password: Optional[str]
+    tart_registry: Optional[str]
 
-    tart_oci_username: Optional[str]
-    tart_oci_password: Optional[str]
-    tart_oci_host: Optional[str]
     tart_ssh_username: Optional[str]
     tart_ssh_password: Optional[str]
 
     class Config:
         """Define the prefix used by GitLab for all environment variables passed to a custom driver.
         see https://docs.gitlab.com/runner/executors/custom.html#stages
         """
```

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/tart.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -127,14 +127,16 @@
 
 Now restart the gitlab-runner with `gitlab-runner restart`
 
 ## GitLab CI
 
 One of the great advantages in using [Tart](https://tart.run) is that it gives almost all functionality to we are used from the standard `docker` executors allowing us to write GitLabCI piplines that do not need any or minimal adaptions for OSX.
 
+> **ATTENTION:** The driver will always automatically login to your GitLab Registry using `CI_REGISTRY_USER`, `CI_REGISTRY_PASSWORD` and `CI_REGISTRY`
+
 ```yaml
 stages:
  - build
 
 run-on-tart:
   image: ghcr.io/cirruslabs/macos-ventura-base:latest
   stage:
@@ -157,17 +159,17 @@
 You can provide a default login registry using the `CLI` parameters (see **Command `prepare`**) but also provide the credentials from with each job variable definition
 
 ```yaml
 stages:
  - build
 
 variables:
-    TART_OCI_USERNAME: myuser@myregistry.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.registry.io
+    TART_REGISTRY_USERNAME: myuser@myregistry.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.registry.io
 
 job1:
   image: private.registry.io/tart/xcode14:latest
   stage:
     - build
   tags:
     - tart
@@ -179,17 +181,17 @@
     paths:
       - artifact.txt
 
 job2:
   image: private.other.io/tart/xcode14:latest
   variables:
     # override the OCI login information for this job only
-    TART_OCI_USERNAME: myuser@other.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.other.io
+    TART_REGISTRY_USERNAME: myuser@other.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.other.io
   stage:
     - build
   tags:
     - tart
   before_script:
     - brew install gitlab-runner # you will need to make sure `gitlab-runner` executable is available to be able to upload artifacts
   script:
@@ -204,17 +206,17 @@
 The [Tart managed images](https://tart.run) come with a default user `admin` and password `admin` which will be used to establish an ssh connection. If you decide to provide your own images, you might opt for a different user and password. You can provide the default user and password using the `config.toml` within the `run` section using `--default-ssh-user` and `--default-ssh-password` or provide it from within your job
 
 ```yaml
 job2:
   image: private.other.io/tart/xcode14:latest
   variables:
     # override the OCI login information for this job only
-    TART_OCI_USERNAME: myuser@other.com
-    TART_OCI_PASSWORD: <some_secret>
-    TART_OCI_HOST: private.other.io
+    TART_REGISTRY_USERNAME: myuser@other.com
+    TART_REGISTRY_PASSWORD: <some_secret>
+    TART_REGISTRY: private.other.io
     TART_SSH_USERNAME: gitlab
     TART_SSH_PASSWORD: gitlab
   stage:
     - build
   tags:
     - tart
   before_script:
@@ -321,17 +323,17 @@
 
   Prepare the environment and start the tart VM.
 
 Options:
   --pull-policy [always|if-not-present|never]
                                   define how runners pull tart images from
                                   registries
-  --oci-username TEXT             username to login to a oci registry
-  --oci-password TEXT             passowrd to login to a oci registry
-  --oci-host TEXT                 username to login to a oci registry
+  --registry-username TEXT        username to login to a oci registry
+  --registry-password TEXT        passowrd to login to a oci registry
+  --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
```

### Comparing `gitlab-runner-tart-driver-0.1.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.0/setup.py` & `gitlab-runner-tart-driver-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1.0"
+version = "0.1.1"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```

