# Comparing `tmp/Shiphelm-0.7.2b0.tar.gz` & `tmp/Shiphelm-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shiphelm-0.7.2b0.tar", last modified: Tue Apr 11 22:41:07 2023, max compression
+gzip compressed data, was "Shiphelm-0.7.3.tar", last modified: Thu Apr 13 17:02:57 2023, max compression
```

## Comparing `Shiphelm-0.7.2b0.tar` & `Shiphelm-0.7.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:41:07.562827 Shiphelm-0.7.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-04-11 22:41:07.562827 Shiphelm-0.7.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 22:41:07.562827 Shiphelm-0.7.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:41:07.558827 Shiphelm-0.7.2b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:41:07.562827 Shiphelm-0.7.2b0/src/Shiphelm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-04-11 22:41:07.000000 Shiphelm-0.7.2b0/src/Shiphelm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 22:41:07.000000 Shiphelm-0.7.2b0/src/Shiphelm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:41:07.000000 Shiphelm-0.7.2b0/src/Shiphelm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 22:41:07.000000 Shiphelm-0.7.2b0/src/Shiphelm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 22:41:07.000000 Shiphelm-0.7.2b0/src/Shiphelm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:41:07.562827 Shiphelm-0.7.2b0/src/shiphelm/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/src/shiphelm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/src/shiphelm/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/src/shiphelm/helmdocker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/src/shiphelm/helmkube.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/src/shiphelm/helmtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:41:07.562827 Shiphelm-0.7.2b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 22:40:57.000000 Shiphelm-0.7.2b0/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 17:02:57.873741 Shiphelm-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/src/Shiphelm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 17:02:57.000000 Shiphelm-0.7.3/src/Shiphelm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/src/shiphelm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmdocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmswarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/src/shiphelm/helmtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:02:57.869741 Shiphelm-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 17:02:47.000000 Shiphelm-0.7.3/tests/test_module1.py
```

### Comparing `Shiphelm-0.7.2b0/LICENSE` & `Shiphelm-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.2b0/PKG-INFO` & `Shiphelm-0.7.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,59 @@
-Metadata-Version: 2.1
-Name: Shiphelm
-Version: 0.7.2b0
-Summary: Docker and kubernetes integration library
-Home-page: https://gameplex-software.github.io/ShipHelm/
-Author: Gameplex Software
-Author-email: info@gameplexsoftware.com
-Keywords: SkiffUI,kubernetes,docker
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
 <a href="https://gameplex-software.github.io/ShipHelm/">
 <img src="https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-44cc-8d42-91378ced6708.png" width="400" />
 </a>
 </p>
 
 # Shiphelm
 
+## Table of Contents
+
+- [Shiphelm](#shiphelm)
+  - [Installation](#installation)
+  - [Docker usage example](#docker-usage-example)
+    - [Get a List of Running Containers](#get-a-list-of-running-containers)
+    - [Get a running container by ID](#get-a-running-container-by-id)
+    - [Get Stats and Ports for a Container by ID](#get-stats-and-ports-for-a-container-by-id)
+    - [Search for Containers by Name](#search-for-containers-by-name)
+    - [Change the Ports of a Container](#change-the-ports-of-a-container)
+    - [Rename a Container](#rename-a-container)
+    - [Add and Remove Containers from Networks](#add-and-remove-containers-from-networks)
+    - [Create and Delete Networks](#create-and-delete-networks)
+    - [Run a New Container](#run-a-new-container)
+    - [Get and Set Environment Variables for a Container](#get-and-set-environment-variables-for-a-container)
+    - [Get and Set Volumes for a Container](#get-and-set-volumes-for-a-container)
+    - [Example code](#example-code)
+  - [Kubernetes (K8S) usage example](#kubernetes-k8s-usage-example)
+    - [Get a List of Running Containers](#get-a-list-of-running-containers-1)
+    - [Get Stats and Ports for a Container by ID](#get-stats-and-ports-for-a-container-by-id-1)
+    - [Search for Containers by Name](#search-for-containers-by-name-1)
+    - [Change the Ports of a Container](#change-the-ports-of-a-container-1)
+    - [Rename a Container](#rename-a-container-1)
+    - [Add and Remove Containers from Networks](#add-and-remove-containers-from-networks-1)
+    - [Create and Delete Networks](#create-and-delete-networks-1)
+    - [Run a New Container](#run-a-new-container-1)
+    - [Get and Set Environment Variables for a Container](#get-and-set-environment-variables-for-a-container-1)
+    - [Get and Set Volumes for a Container](#get-and-set-volumes-for-a-container-1)
+    - [Example code](#example-code-1)
+    - [Dynamic engine selection](#dynamic-engine-selection)
+    - [Remote engines via GUI](#remote-engines-via-gui)
+- [Contributing](#contributing)
+
+
 Shiphelm is a Python library for interacting with containers more easily. With Shiphelm, you can:
 
 - Get a list of all running containers
 - Get usage statistics and used ports for a given container by ID
 - Search containers by name or ID
 - Change the open ports of a container
 - Run new containers
-- Work with Docker, Docker-Swarm, and Kubernetes
+- Work with Docker, and Kubernetes
 - Use Kubernetes clusters and Docker Swarm
+- work on clusters, and swarms of container hosts
 
 ## Installation
 
 You can install Shiphelm using pip:
 
 ```
 pip install shiphelm
@@ -54,50 +67,69 @@
 <img src="https://user-images.githubusercontent.com/34868944/231290469-900a253f-1236-4dd3-a126-85177931ce53.png" width="1000" />
 </p>
 
 ## Docker usage example
 
 This code will allow you to manage the local container engine
 
+
+### Standalone Docker installation
 ```
 from shiphelm.helm import helm
 
-hd = helm.helm() # create an instance of helm
+hd = helm() # create an instance of helm
 
 helm.set_engine_manual("docker")
 ```
 
+### Remote standalone Docker installation
+
 This code will allow you to manage any compatible remote container engine
 ```
 from shiphelm.helm import helm
 
 hd = helm.reomte_connect('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
 ```
 
+### Remote Docker swarm installation
+
+```
+from shiphelm.helm import helm
+
+hd = helm.helm() # create an instance of helm
+
+helm.set_engine_manual(engine_select="docker", remoteAddress="YOUR ADDRESS HERE", remoteSecurity=<True|False>)
+```
+
 ### Get a List of Running Containers
 
 ```
 running_containers = hd.get_running_containers()
 ``` 
 
+### Get a running container by ID
+
+```
+get_container_by_id(container_id)
+```
+
 ### Get Stats and Ports for a Container by ID
 
 ```
 container_stats = hd.get_container_stats(container_id)
 container_ports = hd.get_container_ports(container_id)
 ```
 
 ### Search for Containers by Name
 
 ```
 containers_by_name = hd.search_containers(name)
 ``` 
 
 ### Change the Ports of a Container
-
 ```
 hd.change_container_ports(container_id, ports)
 ``` 
 
 ### Rename a Container
 
 ```
@@ -310,7 +342,24 @@
 
 helm.remote_popup()
 ```
 
 # Contributing
 
 If you would like to contribute to SkiffUI, please feel free to open a pull request or issue on the [GitHub repository](https://github.com/Gameplex-Software/SkiffUI).
+
+<script src="https://giscus.app/client.js"
+        data-repo="Gameplex-Software/ShipHelm"
+        data-repo-id="R_kgDOJGgWLg"
+        data-category="General"
+        data-category-id="DIC_kwDOJGgWLs4CVv98"
+        data-mapping="pathname"
+        data-strict="0"
+        data-reactions-enabled="1"
+        data-emit-metadata="0"
+        data-input-position="bottom"
+        data-theme="light"
+        data-lang="en"
+        data-loading="lazy"
+        crossorigin="anonymous"
+        async>
+</script>
```

#### html2text {}

```diff
@@ -1,44 +1,64 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.2b0 Summary: Docker and
-kubernetes integration library Home-page: https://gameplex-software.github.io/
-ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
-Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
-:: Software Development :: Build Tools Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev License-File:
-LICENSE
  [https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-
                           44cc-8d42-91378ced6708.png]
-# Shiphelm Shiphelm is a Python library for interacting with containers more
-easily. With Shiphelm, you can: - Get a list of all running containers - Get
-usage statistics and used ports for a given container by ID - Search containers
-by name or ID - Change the open ports of a container - Run new containers -
-Work with Docker, Docker-Swarm, and Kubernetes - Use Kubernetes clusters and
-Docker Swarm ## Installation You can install Shiphelm using pip: ``` pip
+# Shiphelm ## Table of Contents - [Shiphelm](#shiphelm) - [Installation]
+(#installation) - [Docker usage example](#docker-usage-example) - [Get a List
+of Running Containers](#get-a-list-of-running-containers) - [Get a running
+container by ID](#get-a-running-container-by-id) - [Get Stats and Ports for a
+Container by ID](#get-stats-and-ports-for-a-container-by-id) - [Search for
+Containers by Name](#search-for-containers-by-name) - [Change the Ports of a
+Container](#change-the-ports-of-a-container) - [Rename a Container](#rename-a-
+container) - [Add and Remove Containers from Networks](#add-and-remove-
+containers-from-networks) - [Create and Delete Networks](#create-and-delete-
+networks) - [Run a New Container](#run-a-new-container) - [Get and Set
+Environment Variables for a Container](#get-and-set-environment-variables-for-
+a-container) - [Get and Set Volumes for a Container](#get-and-set-volumes-for-
+a-container) - [Example code](#example-code) - [Kubernetes (K8S) usage example]
+(#kubernetes-k8s-usage-example) - [Get a List of Running Containers](#get-a-
+list-of-running-containers-1) - [Get Stats and Ports for a Container by ID]
+(#get-stats-and-ports-for-a-container-by-id-1) - [Search for Containers by
+Name](#search-for-containers-by-name-1) - [Change the Ports of a Container]
+(#change-the-ports-of-a-container-1) - [Rename a Container](#rename-a-
+container-1) - [Add and Remove Containers from Networks](#add-and-remove-
+containers-from-networks-1) - [Create and Delete Networks](#create-and-delete-
+networks-1) - [Run a New Container](#run-a-new-container-1) - [Get and Set
+Environment Variables for a Container](#get-and-set-environment-variables-for-
+a-container-1) - [Get and Set Volumes for a Container](#get-and-set-volumes-
+for-a-container-1) - [Example code](#example-code-1) - [Dynamic engine
+selection](#dynamic-engine-selection) - [Remote engines via GUI](#remote-
+engines-via-gui) - [Contributing](#contributing) Shiphelm is a Python library
+for interacting with containers more easily. With Shiphelm, you can: - Get a
+list of all running containers - Get usage statistics and used ports for a
+given container by ID - Search containers by name or ID - Change the open ports
+of a container - Run new containers - Work with Docker, and Kubernetes - Use
+Kubernetes clusters and Docker Swarm - work on clusters, and swarms of
+container hosts ## Installation You can install Shiphelm using pip: ``` pip
 install shiphelm ``` PyPI: [https://pypi.org/project/Shiphelm/]() GitHub
 Releases [https://github.com/Gameplex-Software/ShipHelm/releases]()
  [https://user-images.githubusercontent.com/34868944/231290469-900a253f-1236-
                           4dd3-a126-85177931ce53.png]
 ## Docker usage example This code will allow you to manage the local container
-engine ``` from shiphelm.helm import helm hd = helm.helm() # create an instance
-of helm helm.set_engine_manual("docker") ``` This code will allow you to manage
-any compatible remote container engine ``` from shiphelm.helm import helm hd =
+engine ### Standalone Docker installation ``` from shiphelm.helm import helm hd
+= helm() # create an instance of helm helm.set_engine_manual("docker") ``` ###
+Remote standalone Docker installation This code will allow you to manage any
+compatible remote container engine ``` from shiphelm.helm import helm hd =
 helm.reomte_connect('tcp://remote-docker-host:2375') # create an instance of
-helmdocker for romote management ``` ### Get a List of Running Containers ```
-running_containers = hd.get_running_containers() ``` ### Get Stats and Ports
-for a Container by ID ``` container_stats = hd.get_container_stats
-(container_id) container_ports = hd.get_container_ports(container_id) ``` ###
-Search for Containers by Name ``` containers_by_name = hd.search_containers
-(name) ``` ### Change the Ports of a Container ``` hd.change_container_ports
-(container_id, ports) ``` ### Rename a Container ``` hd.rename_container
-(container_id, new_name) ``` ### Add and Remove Containers from Networks ```
+helmdocker for romote management ``` ### Remote Docker swarm installation ```
+from shiphelm.helm import helm hd = helm.helm() # create an instance of helm
+helm.set_engine_manual(engine_select="docker", remoteAddress="YOUR ADDRESS
+HERE", remoteSecurity=
+False>) ``` ### Get a List of Running Containers ``` running_containers =
+hd.get_running_containers() ``` ### Get a running container by ID ```
+get_container_by_id(container_id) ``` ### Get Stats and Ports for a Container
+by ID ``` container_stats = hd.get_container_stats(container_id)
+container_ports = hd.get_container_ports(container_id) ``` ### Search for
+Containers by Name ``` containers_by_name = hd.search_containers(name) ``` ###
+Change the Ports of a Container ``` hd.change_container_ports(container_id,
+ports) ``` ### Rename a Container ``` hd.rename_container(container_id,
+new_name) ``` ### Add and Remove Containers from Networks ```
 hd.add_container_to_network(container_id, network_name)
 hd.remove_container_from_network(container_id, network_name) ``` ### Create and
 Delete Networks ``` hd.create_network(network_name) hd.delete_network
 (network_name) ``` ### Run a New Container ``` container = hd.run_container
 ( image=image, command=command, detach=detach, ports=ports,
 environment=environment, volumes=volumes ) ``` ### Get and Set Environment
 Variables for a Container ``` container_environment =
@@ -95,7 +115,8 @@
 helm helm.set_engine_auto() ``` ## Remote engines via GUI To use remote engines
 you can use the following the examples above to connect programatically or use
 the below code to open a GUI configuration wizard: ``` from shiphelm.helm
 import helm hd = helm.helm() # create an instance of helm helm.remote_popup()
 ``` # Contributing If you would like to contribute to SkiffUI, please feel free
 to open a pull request or issue on the [GitHub repository](https://github.com/
 Gameplex-Software/SkiffUI).
+
```

### Comparing `Shiphelm-0.7.2b0/setup.py` & `Shiphelm-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.7.2b0/src/Shiphelm.egg-info/PKG-INFO` & `Shiphelm-0.7.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.7.2b0
+Version: 0.7.3
 Summary: Docker and kubernetes integration library
 Home-page: https://gameplex-software.github.io/ShipHelm/
 Author: Gameplex Software
 Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -24,23 +24,58 @@
 <a href="https://gameplex-software.github.io/ShipHelm/">
 <img src="https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-44cc-8d42-91378ced6708.png" width="400" />
 </a>
 </p>
 
 # Shiphelm
 
+## Table of Contents
+
+- [Shiphelm](#shiphelm)
+  - [Installation](#installation)
+  - [Docker usage example](#docker-usage-example)
+    - [Get a List of Running Containers](#get-a-list-of-running-containers)
+    - [Get a running container by ID](#get-a-running-container-by-id)
+    - [Get Stats and Ports for a Container by ID](#get-stats-and-ports-for-a-container-by-id)
+    - [Search for Containers by Name](#search-for-containers-by-name)
+    - [Change the Ports of a Container](#change-the-ports-of-a-container)
+    - [Rename a Container](#rename-a-container)
+    - [Add and Remove Containers from Networks](#add-and-remove-containers-from-networks)
+    - [Create and Delete Networks](#create-and-delete-networks)
+    - [Run a New Container](#run-a-new-container)
+    - [Get and Set Environment Variables for a Container](#get-and-set-environment-variables-for-a-container)
+    - [Get and Set Volumes for a Container](#get-and-set-volumes-for-a-container)
+    - [Example code](#example-code)
+  - [Kubernetes (K8S) usage example](#kubernetes-k8s-usage-example)
+    - [Get a List of Running Containers](#get-a-list-of-running-containers-1)
+    - [Get Stats and Ports for a Container by ID](#get-stats-and-ports-for-a-container-by-id-1)
+    - [Search for Containers by Name](#search-for-containers-by-name-1)
+    - [Change the Ports of a Container](#change-the-ports-of-a-container-1)
+    - [Rename a Container](#rename-a-container-1)
+    - [Add and Remove Containers from Networks](#add-and-remove-containers-from-networks-1)
+    - [Create and Delete Networks](#create-and-delete-networks-1)
+    - [Run a New Container](#run-a-new-container-1)
+    - [Get and Set Environment Variables for a Container](#get-and-set-environment-variables-for-a-container-1)
+    - [Get and Set Volumes for a Container](#get-and-set-volumes-for-a-container-1)
+    - [Example code](#example-code-1)
+    - [Dynamic engine selection](#dynamic-engine-selection)
+    - [Remote engines via GUI](#remote-engines-via-gui)
+- [Contributing](#contributing)
+
+
 Shiphelm is a Python library for interacting with containers more easily. With Shiphelm, you can:
 
 - Get a list of all running containers
 - Get usage statistics and used ports for a given container by ID
 - Search containers by name or ID
 - Change the open ports of a container
 - Run new containers
-- Work with Docker, Docker-Swarm, and Kubernetes
+- Work with Docker, and Kubernetes
 - Use Kubernetes clusters and Docker Swarm
+- work on clusters, and swarms of container hosts
 
 ## Installation
 
 You can install Shiphelm using pip:
 
 ```
 pip install shiphelm
@@ -54,50 +89,69 @@
 <img src="https://user-images.githubusercontent.com/34868944/231290469-900a253f-1236-4dd3-a126-85177931ce53.png" width="1000" />
 </p>
 
 ## Docker usage example
 
 This code will allow you to manage the local container engine
 
+
+### Standalone Docker installation
 ```
 from shiphelm.helm import helm
 
-hd = helm.helm() # create an instance of helm
+hd = helm() # create an instance of helm
 
 helm.set_engine_manual("docker")
 ```
 
+### Remote standalone Docker installation
+
 This code will allow you to manage any compatible remote container engine
 ```
 from shiphelm.helm import helm
 
 hd = helm.reomte_connect('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
 ```
 
+### Remote Docker swarm installation
+
+```
+from shiphelm.helm import helm
+
+hd = helm.helm() # create an instance of helm
+
+helm.set_engine_manual(engine_select="docker", remoteAddress="YOUR ADDRESS HERE", remoteSecurity=<True|False>)
+```
+
 ### Get a List of Running Containers
 
 ```
 running_containers = hd.get_running_containers()
 ``` 
 
+### Get a running container by ID
+
+```
+get_container_by_id(container_id)
+```
+
 ### Get Stats and Ports for a Container by ID
 
 ```
 container_stats = hd.get_container_stats(container_id)
 container_ports = hd.get_container_ports(container_id)
 ```
 
 ### Search for Containers by Name
 
 ```
 containers_by_name = hd.search_containers(name)
 ``` 
 
 ### Change the Ports of a Container
-
 ```
 hd.change_container_ports(container_id, ports)
 ``` 
 
 ### Rename a Container
 
 ```
@@ -310,7 +364,24 @@
 
 helm.remote_popup()
 ```
 
 # Contributing
 
 If you would like to contribute to SkiffUI, please feel free to open a pull request or issue on the [GitHub repository](https://github.com/Gameplex-Software/SkiffUI).
+
+<script src="https://giscus.app/client.js"
+        data-repo="Gameplex-Software/ShipHelm"
+        data-repo-id="R_kgDOJGgWLg"
+        data-category="General"
+        data-category-id="DIC_kwDOJGgWLs4CVv98"
+        data-mapping="pathname"
+        data-strict="0"
+        data-reactions-enabled="1"
+        data-emit-metadata="0"
+        data-input-position="bottom"
+        data-theme="light"
+        data-lang="en"
+        data-loading="lazy"
+        crossorigin="anonymous"
+        async>
+</script>
```

#### html2text {}

```diff
@@ -1,44 +1,76 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.2b0 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.3 Summary: Docker and
 kubernetes integration library Home-page: https://gameplex-software.github.io/
 ShipHelm/ Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,kubernetes,docker Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
 LICENSE
  [https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-
                           44cc-8d42-91378ced6708.png]
-# Shiphelm Shiphelm is a Python library for interacting with containers more
-easily. With Shiphelm, you can: - Get a list of all running containers - Get
-usage statistics and used ports for a given container by ID - Search containers
-by name or ID - Change the open ports of a container - Run new containers -
-Work with Docker, Docker-Swarm, and Kubernetes - Use Kubernetes clusters and
-Docker Swarm ## Installation You can install Shiphelm using pip: ``` pip
+# Shiphelm ## Table of Contents - [Shiphelm](#shiphelm) - [Installation]
+(#installation) - [Docker usage example](#docker-usage-example) - [Get a List
+of Running Containers](#get-a-list-of-running-containers) - [Get a running
+container by ID](#get-a-running-container-by-id) - [Get Stats and Ports for a
+Container by ID](#get-stats-and-ports-for-a-container-by-id) - [Search for
+Containers by Name](#search-for-containers-by-name) - [Change the Ports of a
+Container](#change-the-ports-of-a-container) - [Rename a Container](#rename-a-
+container) - [Add and Remove Containers from Networks](#add-and-remove-
+containers-from-networks) - [Create and Delete Networks](#create-and-delete-
+networks) - [Run a New Container](#run-a-new-container) - [Get and Set
+Environment Variables for a Container](#get-and-set-environment-variables-for-
+a-container) - [Get and Set Volumes for a Container](#get-and-set-volumes-for-
+a-container) - [Example code](#example-code) - [Kubernetes (K8S) usage example]
+(#kubernetes-k8s-usage-example) - [Get a List of Running Containers](#get-a-
+list-of-running-containers-1) - [Get Stats and Ports for a Container by ID]
+(#get-stats-and-ports-for-a-container-by-id-1) - [Search for Containers by
+Name](#search-for-containers-by-name-1) - [Change the Ports of a Container]
+(#change-the-ports-of-a-container-1) - [Rename a Container](#rename-a-
+container-1) - [Add and Remove Containers from Networks](#add-and-remove-
+containers-from-networks-1) - [Create and Delete Networks](#create-and-delete-
+networks-1) - [Run a New Container](#run-a-new-container-1) - [Get and Set
+Environment Variables for a Container](#get-and-set-environment-variables-for-
+a-container-1) - [Get and Set Volumes for a Container](#get-and-set-volumes-
+for-a-container-1) - [Example code](#example-code-1) - [Dynamic engine
+selection](#dynamic-engine-selection) - [Remote engines via GUI](#remote-
+engines-via-gui) - [Contributing](#contributing) Shiphelm is a Python library
+for interacting with containers more easily. With Shiphelm, you can: - Get a
+list of all running containers - Get usage statistics and used ports for a
+given container by ID - Search containers by name or ID - Change the open ports
+of a container - Run new containers - Work with Docker, and Kubernetes - Use
+Kubernetes clusters and Docker Swarm - work on clusters, and swarms of
+container hosts ## Installation You can install Shiphelm using pip: ``` pip
 install shiphelm ``` PyPI: [https://pypi.org/project/Shiphelm/]() GitHub
 Releases [https://github.com/Gameplex-Software/ShipHelm/releases]()
  [https://user-images.githubusercontent.com/34868944/231290469-900a253f-1236-
                           4dd3-a126-85177931ce53.png]
 ## Docker usage example This code will allow you to manage the local container
-engine ``` from shiphelm.helm import helm hd = helm.helm() # create an instance
-of helm helm.set_engine_manual("docker") ``` This code will allow you to manage
-any compatible remote container engine ``` from shiphelm.helm import helm hd =
+engine ### Standalone Docker installation ``` from shiphelm.helm import helm hd
+= helm() # create an instance of helm helm.set_engine_manual("docker") ``` ###
+Remote standalone Docker installation This code will allow you to manage any
+compatible remote container engine ``` from shiphelm.helm import helm hd =
 helm.reomte_connect('tcp://remote-docker-host:2375') # create an instance of
-helmdocker for romote management ``` ### Get a List of Running Containers ```
-running_containers = hd.get_running_containers() ``` ### Get Stats and Ports
-for a Container by ID ``` container_stats = hd.get_container_stats
-(container_id) container_ports = hd.get_container_ports(container_id) ``` ###
-Search for Containers by Name ``` containers_by_name = hd.search_containers
-(name) ``` ### Change the Ports of a Container ``` hd.change_container_ports
-(container_id, ports) ``` ### Rename a Container ``` hd.rename_container
-(container_id, new_name) ``` ### Add and Remove Containers from Networks ```
+helmdocker for romote management ``` ### Remote Docker swarm installation ```
+from shiphelm.helm import helm hd = helm.helm() # create an instance of helm
+helm.set_engine_manual(engine_select="docker", remoteAddress="YOUR ADDRESS
+HERE", remoteSecurity=
+False>) ``` ### Get a List of Running Containers ``` running_containers =
+hd.get_running_containers() ``` ### Get a running container by ID ```
+get_container_by_id(container_id) ``` ### Get Stats and Ports for a Container
+by ID ``` container_stats = hd.get_container_stats(container_id)
+container_ports = hd.get_container_ports(container_id) ``` ### Search for
+Containers by Name ``` containers_by_name = hd.search_containers(name) ``` ###
+Change the Ports of a Container ``` hd.change_container_ports(container_id,
+ports) ``` ### Rename a Container ``` hd.rename_container(container_id,
+new_name) ``` ### Add and Remove Containers from Networks ```
 hd.add_container_to_network(container_id, network_name)
 hd.remove_container_from_network(container_id, network_name) ``` ### Create and
 Delete Networks ``` hd.create_network(network_name) hd.delete_network
 (network_name) ``` ### Run a New Container ``` container = hd.run_container
 ( image=image, command=command, detach=detach, ports=ports,
 environment=environment, volumes=volumes ) ``` ### Get and Set Environment
 Variables for a Container ``` container_environment =
@@ -95,7 +127,8 @@
 helm helm.set_engine_auto() ``` ## Remote engines via GUI To use remote engines
 you can use the following the examples above to connect programatically or use
 the below code to open a GUI configuration wizard: ``` from shiphelm.helm
 import helm hd = helm.helm() # create an instance of helm helm.remote_popup()
 ``` # Contributing If you would like to contribute to SkiffUI, please feel free
 to open a pull request or issue on the [GitHub repository](https://github.com/
 Gameplex-Software/SkiffUI).
+
```

### Comparing `Shiphelm-0.7.2b0/src/shiphelm/helm.py` & `Shiphelm-0.7.3/src/shiphelm/helm.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,78 +10,89 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ----------------------------------------------------------------------------
 
-import helmdocker, helmkube
+from . import  helmdocker, helmkube
 from kubernetes import client
 from typing import TYPE_CHECKING
 import docker
 import tkinter as tk
 from tkinter import ttk
 
 #Fix name conflict between docker nad kubernetes client
 kubeclient = client
 
 #Fix editor auto completes that are broken by the dynamic functions
 if TYPE_CHECKING:
-    from . import helmdocker, helmkube
+    from . import helmdocker, helmkube, helmswarm
     from helmdocker import helmdocker
     from helmdocker import *
     from helmkube import helmkube
     from helmkube import *
 
 class helm:
     def __init__(self, engine=None):
         helm.engine = helm.set_engine_auto()
         helm.get_helm_client()
 
+    @staticmethod
     def set_engine_auto():
         helm.engine = None
         try:
             v1 = kubeclient.CoreV1Api()
             api = v1.CoreV1Api()
             helm.engine = "kubernetes"
             namespaces = api.list_namespace().items
             print("Found Kubernetes engine on local system using Kubernetes container engine")
         except:
             pass
+
         if not helm.engine:
             try:
                 docker.from_env()
                 print("Found Docker engine on local system using Docker container engine")
                 helm.engine = "docker"
             except:
                 print("[Debug] No compatible engine found, prompting for remote connection")
                 helm.remote_popup()
                 print("Popup got engine data:", helm.engineAddress, helm.engineType)
 
         return helm.engine
     
-    def set_engine_manual(engine_select):
+    @staticmethod
+    def set_engine_manual(engine_select='docker', remoteAddress=None, remoteSecurity=""):
         helm.engine = None
         if engine_select == "docker":
             try:
                 docker.from_env()
                 helm.engine = "docker"
             except Exception as e:
-                print("Error connecting to Docker daemon this could be due to the current user permissions or an incompatible engine. The error is as follows:", e)
+                print("Error connecting to Docker daemon. This could be due to the current user permissions or an incompatible engine. The error is as follows:", e)
         elif engine_select == "kubernetes":
             try:
                 kubeclient.CoreV1Api()
                 helm.engine = "kubernetes"
             except Exception as e:
-                print("Error connecting to Kubernetes daemon this could be due to the current user permissions or an incompatible engine. The error is as follows:", e)
+                print("Error connecting to Kubernetes daemon. This could be due to the current user permissions or an incompatible engine. The error is as follows:", e)
+        elif engine_select == "swarm" or engine_select == "dockerswarm":
+            try:
+                helm.engine = "swarm"
+                helm.remoteAddress = remoteAddress
+                helm.remoteSecurity = remoteSecurity
+            except Exception as e:
+                print("Error connecting to the swarm. This could be due to the current user permissions, an invalid address, or an incompatible engine. The error is as follows:", e)
         else:
             print("Invalid engine", engine_select, ". Supported options are 'docker' or 'kubernetes'")
 
         return helm.engine
-    
+
+    @staticmethod
     def remote_popup():
         # Create a popup window
         window = tk.Tk()
         window.title("Remote Address")
 
         # Create a label and text input field for the remote address
         tk.Label(window, text="Remote Address:").grid(row=0, column=0)
@@ -114,8 +125,11 @@
     def get_helm_client():
         print("Selected engine for runner:", helm.engine)
         if helm.engine == "docker":
             helm.add_methods(helmdocker.helmdocker)
             return helmdocker.helmdocker()
         elif helm.engine == "kubernetes":
             helm.add_methods(helmkube.helmkube)
-            return helmkube.helmkube()
+            return helmkube.helmkube()
+        elif helm.engine == "swarm":
+            helm.add_methods(helmswarm.helmswarm)
+            return helmswarm.helmswarm(remote_address=helm.remoteAddress, remote_is_TLS=helm.RemoteSecurity)
```

### Comparing `Shiphelm-0.7.2b0/src/shiphelm/helmdocker.py` & `Shiphelm-0.7.3/src/shiphelm/helmdocker.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,118 +11,105 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ----------------------------------------------------------------------------
 import docker
 
-
-
 class helmdocker:
-    def __init__(self, remote_address = None, remote_is_TLS = None):
-      try:
-         self.client = docker.from_env()
-      except:
-         client = docker.from_env(base_url=remote_address, tls=remote_is_TLS)
+    def __init__(remote_address = None, remote_is_TLS = None):
+        try:
+            helmdocker.client = docker.from_env()
+        except:
+            helmdocker.client = docker.from_env(base_url=remote_address, tls=remote_is_TLS)
 
     @staticmethod
     def get_running_containers():
-        client = docker.from_env()
-        return client.containers.list()
+        return helmdocker.client.containers.list()
+
+    @staticmethod
+    def get_container_by_id(container_id):
+        return helmdocker.client.containers.get(container_id)
 
     @staticmethod
     def get_container_stats(container_id):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         stats = container.stats(stream=False)
         return stats
 
     @staticmethod
     def get_container_ports(container_id):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         ports = container.attrs['NetworkSettings']['Ports']
         return ports
 
     @staticmethod
     def search_containers(name):
-        client = docker.from_env()
-        return client.containers.list(filters={"name": name})
+        return helmdocker.containers.list(filters={"name": name})
 
     @staticmethod
     def change_container_ports(container_id, ports):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         container.reload()
         container.ports.update(ports)
 
     @staticmethod
     def rename_container(container_id, new_name):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         container.rename(new_name)
 
     @staticmethod
     def add_container_to_network(container_id, network_name):
-        client = docker.from_env()
-        network = client.networks.get(network_name)
-        container = client.containers.get(container_id)
+        network = helmdocker.client.networks.get(network_name)
+        container = helmdocker.client.containers.get(container_id)
         network.connect(container)
 
     @staticmethod
     def remove_container_from_network(container_id, network_name):
-        client = docker.from_env()
-        network = client.networks.get(network_name)
-        container = client.containers.get(container_id)
+        network = helmdocker.client.networks.get(network_name)
+        container = helmdocker.client.containers.get(container_id)
         network.disconnect(container)
 
     @staticmethod
     def create_network(network_name):
-        client = docker.from_env()
-        client.networks.create(network_name)
+        helmdocker.client.networks.create(network_name)
 
     @staticmethod
     def delete_network(network_name):
-        client = docker.from_env()
-        network = client.networks.get(network_name)
+        network = helmdocker.client.networks.get(network_name)
         network.remove()
 
     @staticmethod
     def run_container(image, command=None, detach=False, ports=None, environment=None, volumes=None):
-        client = docker.from_env()
-        container = client.containers.run(
+        container = helmdocker.client.containers.run(
             image=image,
             command=command,
             detach=detach,
             ports=ports,
             environment=environment,
             volumes=volumes
         )
         return container
 
     @staticmethod
     def get_container_environment(container_id):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         environment = container.attrs['Config']['Env']
         return environment
 
     @staticmethod
     def set_container_environment(container_id, environment):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         container.reload()
         container.update(env=environment)
 
     @staticmethod
     def get_container_volumes(container_id):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         volumes = container.attrs['HostConfig']['Binds']
         return volumes
 
     @staticmethod
     def set_container_volumes(container_id, volumes):
-        client = docker.from_env()
-        container = client.containers.get(container_id)
+        container = helmdocker.client.containers.get(container_id)
         container.reload()
         container.update(binds=volumes)
```

### Comparing `Shiphelm-0.7.2b0/src/shiphelm/helmkube.py` & `Shiphelm-0.7.3/src/shiphelm/helmkube.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# ----------------------------------------------------------------------------
+# ShipHelm Copyright 2020-2023 by Gameplex Software and contributors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ----------------------------------------------------------------------------
+
 from kubernetes import client, config
 
 class helmkube:
     def __init__(remote_address = None, remote_is_TLS = None):
       try:
         helmkube.kubeclient = client
         helmkube.api_client = helmkube.kubeclient.ApiClient()
@@ -17,14 +33,18 @@
         containers = []
         for pod in pods.items:
             for container in pod.spec.containers:
                 containers.append(container)
         return containers
 
     @staticmethod
+    def get_container_by_id(container_id):
+        return helmkube.get_container_by_id(container_id)
+
+    @staticmethod
     def get_container_stats(container_id):
         api_instance = helmkube.kubeclient.CoreV1Api(helmkube.api_client)
         namespace = "default"  # modify as needed
         pod_name = container_id  # use container ID as pod name
         container_name = container_id  # use container ID as container name
         container_stats = api_instance.read_namespaced_pod_container_status(
             name=pod_name,
```

