# Comparing `tmp/TapisCL-ICICLE-0.0.22.tar.gz` & `tmp/TapisCL-ICICLE-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.22.tar", last modified: Wed Apr 12 21:51:32 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.23.tar", last modified: Thu Apr 13 04:40:54 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.22.tar` & `TapisCL-ICICLE-0.0.23.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:51:32.605950 TapisCL-ICICLE-0.0.22/
--rw-rw-rw-   0        0        0    35823 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.22/LICENSE
--rw-rw-rw-   0        0        0    43024 2023-04-12 21:51:32.605950 TapisCL-ICICLE-0.0.22/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-04-12 05:02:25.000000 TapisCL-ICICLE-0.0.22/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 21:51:32.595952 TapisCL-ICICLE-0.0.22/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 18:30:28.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1408 2023-04-12 20:12:15.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    11151 2023-04-12 21:12:56.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     6873 2023-04-12 21:08:42.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 03:10:40.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     4985 2023-04-12 20:49:51.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     1049 2023-04-12 16:16:32.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10512 2023-04-12 21:18:32.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-12 17:45:30.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    16274 2023-04-12 21:21:11.000000 TapisCL-ICICLE-0.0.22/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:51:32.603957 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43024 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 21:51:32.000000 TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-12 21:50:58.000000 TapisCL-ICICLE-0.0.22/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 21:51:32.605950 TapisCL-ICICLE-0.0.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 04:40:54.013614 TapisCL-ICICLE-0.0.23/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/LICENSE
+-rw-rw-rw-   0        0        0    43856 2023-04-13 04:40:54.012595 TapisCL-ICICLE-0.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0     1946 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 04:40:54.003737 TapisCL-ICICLE-0.0.23/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    11151 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     4985 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10512 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    18336 2023-04-13 04:36:57.000000 TapisCL-ICICLE-0.0.23/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 04:40:54.011093 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43856 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 04:40:53.000000 TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-13 04:40:14.000000 TapisCL-ICICLE-0.0.23/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 04:40:54.013614 TapisCL-ICICLE-0.0.23/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.22/LICENSE` & `TapisCL-ICICLE-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/PKG-INFO` & `TapisCL-ICICLE-0.0.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.22
+Version: 0.0.23
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,19 +690,33 @@
 
 # TapisCLI
 ## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
-* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/requirements.txt)
+* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
 1. `pip install TapisCL-ICICLE`
-2. `python -m TapisCL-ICICLE`
+2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
-1. to see a list of all commands and their parameters, just enter help
+**Full Terminal Interface:**
+1. run ``python -m TapisCLICICLE``
+2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
+3. enter your username and password when prompted
+4. if all went well the console should open. You can run `help` to see command options
+5. to exit the application, run `exit`
+
+**Command Line:**
+
+Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
+
+`python -m TapisCLICICLE pods -c help`
+
+this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
+
```

### Comparing `TapisCL-ICICLE-0.0.22/README.md` & `TapisCL-ICICLE-0.0.23/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 # TapisCLI
 ## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
-* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/requirements.txt)
+* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
 1. `pip install TapisCL-ICICLE`
-2. `python -m TapisCL-ICICLE`
+2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
-1. to see a list of all commands and their parameters, just enter help
+**Full Terminal Interface:**
+1. run ``python -m TapisCLICICLE``
+2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
+3. enter your username and password when prompted
+4. if all went well the console should open. You can run `help` to see command options
+5. to exit the application, run `exit`
+
+**Command Line:**
+
+Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
+
+`python -m TapisCLICICLE pods -c help`
+
+this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
+
```

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/helpers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.23/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import json
 import pyperclip
 import tapipy
 from tapipy.tapis import TapisResult
 from py2neo import Graph
 import typing
+import os
 try:
     from . import helpers
     from . import decorators
 except:
     import helpers 
     import decorators
 
 
+__location__ = os.path.realpath(
+    os.path.join(os.getcwd(), os.path.dirname(__file__)))
+server_path = os.path.join(__location__, 'server.py')
+
+
 class tapisObject(helpers.OperationsHelper, decorators.DecoratorSetup, helpers.DynamicHelpUtility):
     def __init__(self, tapis_instance, username, password, connection, command_map=None):
         self.t = tapis_instance
         self.username = username
         self.password = password
         self.connection = connection
 
@@ -61,18 +67,30 @@
             'help':self.help
         }
         super().__init__(tapis_instance, username, password, connection, command_map=command_map)
 
     def return_formatter(self, info):
         return f"id: {info.id}\nhost: {info.host}\n\n"
 
+    def __keygen(self):
+        local_files = os.listdir(__location__)
+        if "id_rsa" not in local_files or "id_rsa.pub" not in local_files:
+            os.system(f'ssh-keygen -q -m PEM -f {__location__}\\id_rsa -N ""')
+            with open(f"{__location__}\\id_rsa", 'r') as f:
+                formatted_key = ""
+                for line in f.readlines()[1:-1]:
+                    formatted_key += line.strip()
+
+            with open(f"{__location__}\\id_rsa", 'w') as f:
+                f.write(formatted_key)
+
     def get_systems(self, verbose: bool):
         """
         @help: Gets and returns the list of systems the current Tapis service and account have access to
-        @doc: this is an example of the doc segment of the docstring
+        @doc: this is an example of the doc segment of the docstring. not included in help message
         """
         systems = self.t.systems.getSystems()
         if systems and verbose:
             return str(systems)
         systems = [self.return_formatter(system) for system in systems]
         systems_string = ''
         for system in systems:
@@ -88,23 +106,27 @@
             return str(system_info)
         return self.return_formatter(system_info)
     
     def create_system(self, file: str) -> str: # create a tapius system. Takes a path to a json file with all system information, as well as an ID
         """
         @help: create a system. Must have a properly configured system file.
         see the template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/system-config.json
+        this command will automatically create and upload the ssh keys
         """
+        self.__keygen()
         with open(file, 'r') as f:
             system = json.loads(f.read())
-        self.t.systems.createSystem(**system)
-        return str
+        return_value = self.t.systems.createSystem(**system)
+        self.system_credential_upload(id=system['id'], file=f"{__location__}\\id_rsa,{__location__}\\id_rsa.pub")
+        return str(return_value)
     
-    def system_credential_upload(self, file: str) -> str: # upload key credentials for the system
+    def system_credential_upload(self, id: str, file: str) -> str: # upload key credentials for the system
         """
         @help: upload system credentials to a system. Must generate keys first using 'ssh-keygen -m PEM -f id_rsa', and format with, 'awk -v ORS='\\n' '1' <private_key_name>
+        file argument must contain the path to the private and public keys respectively, separated by a ','
         """
         with open(file.split(",")[0], 'r') as f:
             private_key = f.read()
 
         with open(file.split(",")[1], 'r') as f:
             public_key = f.read()
 
@@ -170,17 +192,19 @@
     def __init__(self, tapis_instance, username, password, connection):
         command_map = {
                 'get_pods':self.get_pods,
                 'create_pod':self.create_pod,
                 'restart_pod':self.restart_pod,
                 'delete_pod':self.delete_pod,
                 'set_pod_perms':self.set_pod_perms,
+                'stop_pod':self.stop_pod,
                 'delete_pod_perms':self.delete_pod_perms,
                 'get_perms':self.get_perms,
                 'copy_pod_password':self.copy_pod_password,
+                'get_logs':self.get_pod_logs,
                 'help':self.help
             }
         super().__init__(tapis_instance, username, password, connection, command_map=command_map)
 
     def return_formatter(self, info):
         return f"Pod ID: {info.pod_id}\nPod Template: {info.pod_template}\nStatus: {info.status_requested}\n\n"
 
@@ -222,15 +246,23 @@
         """
         @help: initiate a pod restart
         """
         return_information = self.t.pods.restart_pod(pod_id=id)
         if verbose:
             return str(return_information)
         return return_information
-
+    
+    @decorators.NeedsConfirmation
+    def stop_pod(self, id: str):
+        """
+        @help: stop a pod's operations
+        """
+        return_information = self.t.pods.stop_pod(pod_id=id)
+        return return_information
+        
     @decorators.NeedsConfirmation
     def delete_pod(self, id: str, verbose: bool) -> str: 
         """
         @help: delete select pod
         """
         return_information = self.t.pods.delete_pod(pod_id=id)
         if verbose:
@@ -264,14 +296,25 @@
         """
         @help: copy the pod password to the clipboard
         """
         password = self.t.pods.get_pod_credentials(pod_id=id).user_password
         pyperclip.copy(password)
         password = None
         return 'copied to clipboard'
+    
+    def get_pod_logs(self, id: str, file=None):
+        """
+        @help: retrieve the logs of an active pod and either print them to the console, or write them to the specified file
+        """
+        logs = self.t.pods.get_pod_logs(pod_id=id)
+        if file:
+            with open(file, 'w') as f:
+                f.write(logs)
+            return f"Log saved at {file}"
+        return logs
 
 
 class Files(tapisObject):
     """
     @help: Access Tapis files through the connected service
     """
     def __init__(self, tapis_instance, username, password, connection):
@@ -294,26 +337,28 @@
         if verbose:
             return str(file_list)
         file_list = [self.return_formatter(f) for f in file_list]
         return str(file_list)
 
     def upload(self, file: str, id: str) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
         """
-        @help: upload a file to the system
+        @help: upload a file to the system 
+        the source and destination files must both be in the file argument, respectively, separated by a comma
         """
         source = file.split(",")[0]
         destination = file.split(",")[1]
         self.t.upload(system_id=id,
                 source_file_path=source,
                 dest_file_path=destination)
         return f'successfully uploaded {source} to {destination}'
             
     def download(self, file: str, id: str) -> str: # download a remote file using tapis, operates basically the same as upload
         """
         @help: download a file from the system
+        the source and destination files must both be in the file argument, respectively, separated by a comma
         """
         source = file.split(",")[0]
         destination = file.split(",")[1]
         file_info = self.t.files.getContents(systemId=id,
                             path=source)
 
         file_info = file_info.decode('utf-8')
@@ -393,8 +438,9 @@
     def download_job_output(self, uuid: str, file: str)->str: # download the output of a job with its Uuid
         """
         @help: download a job output from the system 
         """
         jobs_output = self.t.jobs.getJobOutputDownload(jobUuid=uuid, outputPath='tapisjob.out')
         with open(file, 'w') as f:
             f.write(jobs_output)
-        return f"Successfully downloaded job output to {file}"
+        return f"Successfully downloaded job output to {file}"
+
```

### Comparing `TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.22
+Version: 0.0.23
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,19 +690,33 @@
 
 # TapisCLI
 ## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
-* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/requirements.txt)
+* Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
 1. `pip install TapisCL-ICICLE`
-2. `python -m TapisCL-ICICLE`
+2. `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
 3. `python cli.py`
 ### Operations
-1. to see a list of all commands and their parameters, just enter help
+**Full Terminal Interface:**
+1. run ``python -m TapisCLICICLE``
+2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be https://icicle.tapis.io
+3. enter your username and password when prompted
+4. if all went well the console should open. You can run `help` to see command options
+5. to exit the application, run `exit`
+
+**Command Line:**
+
+Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
+
+`python -m TapisCLICICLE pods -c help`
+
+this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
+
```

### Comparing `TapisCL-ICICLE-0.0.22/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.23/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.22/pyproject.toml` & `TapisCL-ICICLE-0.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.22"
+version = "0.0.23"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

