# Comparing `tmp/yohsin3d-0.2.0.tar.gz` & `tmp/yohsin3d-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yohsin3d-0.2.0.tar", last modified: Sun Apr  9 09:55:45 2023, max compression
+gzip compressed data, was "yohsin3d-0.3.0.tar", last modified: Wed Apr 12 23:18:25 2023, max compression
```

## Comparing `yohsin3d-0.2.0.tar` & `yohsin3d-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/communicators/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/bit_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/communicator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/core/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/behavior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/core/body/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/body_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/nao_joint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/agent_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/ground_truth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/communicator/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/communicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/communicator/base_communicator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/localizer/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/localizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/localizer/base_localizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/network/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/world/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/world/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/world/world_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/localizers/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/localizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/localizers/ground_truth_localizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/communicators/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/bit_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/communicator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/behavior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/core/body/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/body_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/nao_joint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/agent_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/ground_truth_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/joints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/communicator/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/communicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/communicator/base_communicator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/localizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/localizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/localizer/base_localizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/spawner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/world/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/world/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/world/world_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/localizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/localizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/localizers/ground_truth_localizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/movement/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/movement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/movement/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/movement/y3d_movements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/top_level.txt
```

### Comparing `yohsin3d-0.2.0/LICENSE` & `yohsin3d-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.2.0/PKG-INFO` & `yohsin3d-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yohsin3d
-Version: 0.2.0
+Version: 0.3.0
 Summary: Program your own RoboCup 3D soccer playing agents in python
 Home-page: https://github.com/FC-Yohsin/yohsin3d
 Author: Habib Shahzad, Abuzar Rasool, Faaz Abidi
 Author-email: habibshehzad55@gmail.com, availabuzar@gmail.com, hasanfaaz10@gmail.com
 License: MIT
 Keywords: robocup,soccer,3d,simulation,agents,robotics,machine learning,python,artificial intelligence,locomotion,localization
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![CodeFactor](https://www.codefactor.io/repository/github/fc-yohsin/yohsin3d/badge)](https://www.codefactor.io/repository/github/fc-yohsin/yohsin3d)
+
 # Yohsin3d: Python Framework for RoboCup 3D Soccer Agents
 
 Yohsin3d is an open-source Python framework that simplifies the development of RoboCup 3D soccer agents. It handles low-level details like server communication, basic locomotion, and localization, allowing you to focus on adding functionality to the agents. With extensive machine learning support and a thriving community, Python is an excellent choice for building intelligent and adaptive soccer agents.
 
 ## RoboCup 3D Simulation League
 
 The [RoboCup 3D Simulation League](https://ssim.robocup.org/3d-simulation/) is a platform that enables software agents to control humanoid robots, running on a realistic physics engine to simulate soccer matches. It serves as a challenging and exciting way for researchers to explore robotics and AI.
```

### Comparing `yohsin3d-0.2.0/README.md` & `yohsin3d-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![CodeFactor](https://www.codefactor.io/repository/github/fc-yohsin/yohsin3d/badge)](https://www.codefactor.io/repository/github/fc-yohsin/yohsin3d)
+
 # Yohsin3d: Python Framework for RoboCup 3D Soccer Agents
 
 Yohsin3d is an open-source Python framework that simplifies the development of RoboCup 3D soccer agents. It handles low-level details like server communication, basic locomotion, and localization, allowing you to focus on adding functionality to the agents. With extensive machine learning support and a thriving community, Python is an excellent choice for building intelligent and adaptive soccer agents.
 
 ## RoboCup 3D Simulation League
 
 The [RoboCup 3D Simulation League](https://ssim.robocup.org/3d-simulation/) is a platform that enables software agents to control humanoid robots, running on a realistic physics engine to simulate soccer matches. It serves as a challenging and exciting way for researchers to explore robotics and AI.
```

### Comparing `yohsin3d-0.2.0/setup.py` & `yohsin3d-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yohsin3d',
-    version='0.2.0',
+    version='0.3.0',
     description='Program your own RoboCup 3D soccer playing agents in python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Habib Shahzad, Abuzar Rasool, Faaz Abidi',
     author_email='habibshehzad55@gmail.com, availabuzar@gmail.com, hasanfaaz10@gmail.com',
     url='https://github.com/FC-Yohsin/yohsin3d',
     license="MIT",
@@ -33,8 +33,8 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="robocup, soccer, 3d, simulation, agents, robotics, machine learning, python, artificial intelligence, locomotion, localization",
     packages=find_packages(),
     install_requires=[],
     python_requires=">=3.6",
-)
+)
```

### Comparing `yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/bit_codec.py` & `yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/bit_codec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import List
-communication_alphabet =  "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789*#"
+communication_alphabet = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789*#"
 
 
 class BitCodec:
 
     @staticmethod
     def bits_to_int(bits: List, start, end):
         if start < 0 or end >= len(bits):
-            return 0 
+            return 0
 
         n = 0
         for i in range(start, end+1):
             n *= 2
             n += bits[i]
 
         return n
-    
+
     @staticmethod
     def int_to_bits(n: int, num_bits: int) -> List[int]:
         if n < 0:
             return []
 
         bits = [0] * num_bits
         for i in range(num_bits-1, -1, -1):
             bits[i] = n % 2
             n //= 2
 
         return bits
-    
+
     @staticmethod
     def bits_to_string(bitfield_list):
         message = ""
 
         index = []
         index_size = (len(bitfield_list) + 5) // 6
         index = [0] * index_size
@@ -62,21 +62,20 @@
                 binary_value = bin(index)[2:].zfill(6)
                 bits.extend([int(bit) for bit in binary_value])
             except ValueError:
                 print("string_to_bits: character not in alphabet!")
                 return None
 
         return bits
-    
 
     @staticmethod
     def encode_float(number, min_value, max_value, num_bits=10):
         clipped = min(max(number, min_value), max_value)
         max_size = (1 << num_bits) - 1
-        value = int(((clipped - min_value) * max_size) / (max_value - min_value) + 0.5)
+        value = int(((clipped - min_value) * max_size) /
+                    (max_value - min_value) + 0.5)
         return BitCodec.int_to_bits(value, num_bits)
-    
+
     @staticmethod
     def decode_bit_array(bits, min_value, max_value, num_bits=10):
         value = BitCodec.bits_to_int(bits, 0, num_bits - 1)
         return min_value + (value * (max_value - min_value)) / ((1 << num_bits) - 1)
-
```

### Comparing `yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/communicator.py` & `yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/communicator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from ...core.common.constants import *
 from ...core import BaseCommunicator
 from .bit_codec import BitCodec
 
+
 class CommunicationData:
     def __init__(self, heard_from=None, time=None, ball_x=None, ball_y=None, my_x=None, my_y=None):
         self.heard_from = heard_from
         self.time = time
         self.ball_x = ball_x
         self.ball_y = ball_y
         self.my_x = my_x
         self.my_y = my_y
 
+    def __str__(self):
+        return f"Agent {self.heard_from} heard: time={self.time}, ball_x={self.ball_x}, ball_y={self.ball_y}, position = ({self.my_x}, {self.my_y})"
+
 
 class Y3dCommunicator(BaseCommunicator):
 
     def __init__(self) -> None:
         super().__init__()
         self.heard_data = CommunicationData()
         self.heard_data_type = CommunicationData
@@ -34,37 +38,36 @@
         bits.extend(ball_y_bits)
         bits.extend(my_x_bits)
         bits.extend(my_y_bits)
 
         return bits
 
     def say(self):
-        ball = self.localizer.ball_position        
+        ball = self.localizer.ball_position
         me = self.localizer.my_location.position
         bits = self.data_to_bits(
             self.world_model.get_time(),
             ball[0],
             ball[1],
             me[0],
             me[1],
-        )        
+        )
 
         message = BitCodec.bits_to_string(bits)
         self.said_message = message
 
-
     def bits_to_data(self, bits):
         time, ballX, ballY, agentX, agentY = 0, 0, 0, 0, 0
 
         ctr = 0
 
         cycles = BitCodec.bits_to_int(bits, ctr, ctr + 15)
         time = cycles * 0.02
         ctr += 16
-        
+
         bx_bits = bits[ctr:ctr+10]
         ballX = BitCodec.decode_bit_array(bx_bits, min_ball_x, max_ball_x)
         ctr += 10
 
         by_bits = bits[ctr:ctr+10]
         ballY = BitCodec.decode_bit_array(by_bits, min_ball_y, max_ball_y)
         ctr += 10
@@ -75,28 +78,27 @@
 
         ay_bits = bits[ctr:ctr+10]
         agentY = BitCodec.decode_bit_array(ay_bits, min_agent_y, max_agent_y)
         ctr += 10
 
         return time, ballX, ballY, agentX, agentY
 
-
-    def hear(self) -> None:   
+    def hear(self) -> None:
         heard_message = self.heard_message
         message = heard_message.message
 
         if message is None:
             self.heard_data = CommunicationData()
-            return 
-    
+            return
+
         bits = BitCodec.string_to_bits(message)
         time, ballX, ballY, agentX, agentY = self.bits_to_data(bits)
 
         heard_time = heard_message.heard_time
         delta_game_time = self.world_model.get_time() - self.world_model.get_gametime()
         heard_server_time = heard_time + delta_game_time
 
         time += int((heard_server_time-time)/1310.72)*1310.72
         cycles = int(time * 50 + 0.1)
         unum = (cycles % (NUM_AGENTS*2)) // 2 + 1
-        self.heard_data = CommunicationData(unum, time, ballX, ballY, agentX, agentY)
-    
+        self.heard_data = CommunicationData(
+            unum, time, ballX, ballY, agentX, agentY)
```

### Comparing `yohsin3d-0.2.0/yohsin3d/core/agent.py` & `yohsin3d-0.3.0/yohsin3d/core/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,15 +83,22 @@
                             behavior.get_monitor_message())
 
                 except Exception as e:
                     print(traceback.format_exc())
                     self.done()
                     exit()
 
-    def start(self):
+    def handler(self):
         def signal_handler(sig, _):
             print('\nExiting!')
             sys.exit(0)
 
         signal.signal(signal.SIGINT, signal_handler)
+
+    def start(self, custom_handler=None):
+        if custom_handler:
+            custom_handler()
+        else:
+            self.handler()
+
         self.run()
         self.done()
```

### Comparing `yohsin3d-0.2.0/yohsin3d/core/behavior.py` & `yohsin3d-0.3.0/yohsin3d/core/behavior.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .body import *
 from .world import *
 from .localizer import BaseLocalizer
 from .network import Parser
 from .communicator import BaseCommunicator
-from .common import AgentLocation
+from .common import AgentLocation, Joint
 
 
 class BaseBehavior:
 
     def __init__(self, beam_location: AgentLocation, localizer: BaseLocalizer = None, communicator: BaseCommunicator = None) -> None:
         self.beam_location = beam_location
         self.monitor_msg = ""
@@ -18,18 +18,17 @@
 
     def initialize(self, team_name):
         self.world_model = WorldModel(team_name)
         self.body_model = BodyModel(self.world_model)
 
         self.parser = Parser(world_model=self.world_model,
                              body_model=self.body_model,
-                             communicator=self.communicator                             
+                             communicator=self.communicator
                              )
-        
-        
+
         if self.communicator is not None:
             self.communicator.initialize(self.world_model, self.localizer)
 
         if self.localizer is not None:
             self.localizer.initialize(self.world_model)
 
     def can_rebeam(self):
@@ -50,18 +49,18 @@
         return self.beam_effector(x, y, self.beam_location.orientation)
 
     def hj_effector(self, name, rate):
         return "({} {:.2f})".format(name, rate)
 
     def compose_action(self):
         message = ""
-        for effector in EffectorJoints:
-            torque = self.body_model.compute_torque(effector)
-            effector_name = effector.to_string()
-            message += self.hj_effector(effector_name, torque)
+        for joint in Joint:
+            torque = self.body_model.compute_torque(joint)
+            joint_name = joint.effector_name
+            message += self.hj_effector(joint_name, torque)
 
         if self.communicator is not None:
             message += self.communicator.make_say_message()
 
         return message
 
     def get_monitor_message(self):
@@ -90,15 +89,15 @@
 
         if not self.__can_initialize() or self.initialized:
             return
 
         self.initialize_body()
         self.initialized = True
         return None
-    
+
     def think(self, message: str) -> str:
 
         parse_success = self.parser.parse(message)
         if not parse_success:
             print("Parser failed to parse message..")
 
         message = self.initialize_nao()
@@ -113,13 +112,13 @@
 
         action = ""
         self.act()
 
         if self.communicator is not None:
             self.communicator.say()
             self.communicator.hear()
-            
+
         action += self.compose_action()
         return action
 
     def act(self):
         raise NotImplementedError
```

### Comparing `yohsin3d-0.2.0/yohsin3d/core/body/body_model.py` & `yohsin3d-0.3.0/yohsin3d/core/body/body_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,165 +1,168 @@
 
 import math
 from .enums import *
 from .nao_joint import NaoJoint
 from ..world.world_model import WorldModel
+from ..common import Joint
+
+from typing import List
 
 
 class BodyModel:
     def __init__(self, worldModel: WorldModel) -> None:
         self.gyro_rates = (0, 0, 0)
         self.prev_gyro_rates = (0, 0, 0)
         self.accel_rates = (0, 0, 0)
         self.walk_angle = None
 
-        self.worldModel = worldModel
-        self.joints_list: list[NaoJoint] = [
-            None for _ in range(len(EffectorJoints))
+        self.world_model = worldModel
+        self.joints_list: List[NaoJoint] = [
+            None for _ in range(len(Joint))
         ]
 
         self.previous_joints_list: list[NaoJoint] = [
-            None for _ in range(len(EffectorJoints))
+            None for _ in range(len(Joint))
         ]
 
-        self.initialise_effectors()
+        self.initialise_joints()
 
     def set_initial_head(self):
 
-        self.set_target_angle(EffectorJoints.EFF_H1, 0)
-        self.set_target_angle(EffectorJoints.EFF_H2, -45)
+        self.set_target_angle(Joint.H1, 0)
+        self.set_target_angle(Joint.H2, -45)
 
-    def target_reached(self, effector_id: EffectorJoints):
-        return abs(self.joints_list[effector_id].current_angle -
-                   self.joints_list[effector_id].target_angle
-                   ) < self.joints_list[effector_id].error_tolerance
+    def target_reached(self, joint: Joint):
+        return abs(self.joints_list[joint].current_angle -
+                   self.joints_list[joint].target_angle
+                   ) < self.joints_list[joint].error_tolerance
 
     def set_initial_arm(self, arm) -> bool:
 
         ang1 = -50.0
         ang2 = 30.0
         ang3 = 0
         ang4 = -50.0
 
         if (arm == BodyParts.ARM_LEFT):
 
-            self.set_target_angle(EffectorJoints.EFF_LA1, ang1)
-            self.set_target_angle(EffectorJoints.EFF_LA2, ang2)
-            self.set_target_angle(EffectorJoints.EFF_LA3, ang3)
-            self.set_target_angle(EffectorJoints.EFF_LA4, ang4)
+            self.set_target_angle(Joint.LA1, ang1)
+            self.set_target_angle(Joint.LA2, ang2)
+            self.set_target_angle(Joint.LA3, ang3)
+            self.set_target_angle(Joint.LA4, ang4)
 
         else:
 
-            self.set_target_angle(EffectorJoints.EFF_RA1, ang1)
-            self.set_target_angle(EffectorJoints.EFF_RA2, -ang2)
-            self.set_target_angle(EffectorJoints.EFF_RA3, -ang3)
-            self.set_target_angle(EffectorJoints.EFF_RA4, -ang4)
+            self.set_target_angle(Joint.RA1, ang1)
+            self.set_target_angle(Joint.RA2, -ang2)
+            self.set_target_angle(Joint.RA3, -ang3)
+            self.set_target_angle(Joint.RA4, -ang4)
 
     def set_initial_leg(self, leg) -> bool:
 
         ang1 = 0
         ang2 = 6.0
         ang3 = 18.0
         ang4 = -30.0
         ang5 = 18.0
         ang6 = -6.0
 
         if (leg == BodyParts.LEG_LEFT):
 
-            self.set_target_angle(EffectorJoints.EFF_LL1, ang1)
-            self.set_target_angle(EffectorJoints.EFF_LL2, ang2)
-            self.set_target_angle(EffectorJoints.EFF_LL3, ang3)
-            self.set_target_angle(EffectorJoints.EFF_LL4, ang4)
-            self.set_target_angle(EffectorJoints.EFF_LL5, ang5)
-            self.set_target_angle(EffectorJoints.EFF_LL6, ang6)
+            self.set_target_angle(Joint.LL1, ang1)
+            self.set_target_angle(Joint.LL2, ang2)
+            self.set_target_angle(Joint.LL3, ang3)
+            self.set_target_angle(Joint.LL4, ang4)
+            self.set_target_angle(Joint.LL5, ang5)
+            self.set_target_angle(Joint.LL6, ang6)
 
         else:
 
-            self.set_target_angle(EffectorJoints.EFF_RL1, ang1)
-            self.set_target_angle(EffectorJoints.EFF_RL2, -ang2)
-            self.set_target_angle(EffectorJoints.EFF_RL3, ang3)
-            self.set_target_angle(EffectorJoints.EFF_RL4, ang4)
-            self.set_target_angle(EffectorJoints.EFF_RL5, ang5)
-            self.set_target_angle(EffectorJoints.EFF_RL6, -ang6)
-
-    def set_current_angle(self, effector_id: EffectorJoints, angle):
-        self.previous_joints_list[effector_id] = self.joints_list[
-            effector_id].current_angle
-        self.joints_list[effector_id].current_angle = angle
+            self.set_target_angle(Joint.RL1, ang1)
+            self.set_target_angle(Joint.RL2, -ang2)
+            self.set_target_angle(Joint.RL3, ang3)
+            self.set_target_angle(Joint.RL4, ang4)
+            self.set_target_angle(Joint.RL5, ang5)
+            self.set_target_angle(Joint.RL6, -ang6)
+
+    def set_current_angle(self, joint: Joint, angle):
+        self.previous_joints_list[joint] = self.joints_list[
+            joint].current_angle
+        self.joints_list[joint].current_angle = angle
 
-    def gettarget_angle(self, effector_id: EffectorJoints):
-        return self.joints_list[effector_id].target_angle
+    def gettarget_angle(self, joint: Joint):
+        return self.joints_list[joint].target_angle
 
     def update_speed(self, gain):
-        for effector in EffectorJoints:
-            self.set_angle_gain(effector, gain)
+        for joint in Joint:
+            self.set_angle_gain(joint, gain)
 
     def get_change_in_gyro_rate(self):
         return (self.gyro_rates[0] - self.prev_gyro_rates[0],
                 self.gyro_rates[1] - self.prev_gyro_rates[1],
                 self.gyro_rates[2] - self.prev_gyro_rates[2])
 
-    def get_change_in_angle(self, effector_id: EffectorJoints):
+    def get_change_in_angle(self, joint: Joint):
         return self.joints_list[
-            effector_id].current_angle - self.previous_joints_list[effector_id]
+            joint].current_angle - self.previous_joints_list[joint]
 
-    def set_target_angle(self, effector_id: EffectorJoints, angle, gain=None):
-        self.joints_list[effector_id].set_target_angle(angle)
+    def set_target_angle(self, joint: Joint, angle, gain=None):
+        self.joints_list[joint].set_target_angle(angle)
         if gain is not None:
-            self.set_angle_gain(effector_id, gain)
+            self.set_angle_gain(joint, gain)
 
     def increase_target_angle(self,
-                              effector_id: EffectorJoints,
+                              joint: Joint,
                               angle_increase,
                               gain=None):
-        self.joints_list[effector_id].set_target_angle(
-            self.joints_list[effector_id].target_angle + angle_increase)
+        self.joints_list[joint].set_target_angle(
+            self.joints_list[joint].target_angle + angle_increase)
 
         if gain is not None:
-            self.set_angle_gain(effector_id, gain)
+            self.set_angle_gain(joint, gain)
 
-    def get_scale(self, effector_id: EffectorJoints):
-        return self.joints_list[effector_id].scale
+    def get_scale(self, joint: Joint):
+        return self.joints_list[joint].scale
 
-    def set_angle_gain(self, effector_id: EffectorJoints, scale):
-        self.joints_list[effector_id].scale = scale
+    def set_angle_gain(self, joint: Joint, scale):
+        self.joints_list[joint].scale = scale
 
-    def initialise_effectors(self):
-        for effector in EffectorJoints:
-            effector_range = effector.to_range()
-            self.joints_list[effector] = NaoJoint(effector_range[0],
-                                                  effector_range[1],
-                                                  2.0)
+    def initialise_joints(self):
+        for joint in Joint:
+            joint_range = joint.range
+            self.joints_list[joint] = NaoJoint(joint_range[0],
+                                               joint_range[1],
+                                               2.0)
 
     def get_accel_rates(self):
         return self.accel_rates
 
     def set_accel_rates(self, accel_rates):
         self.accel_rates = accel_rates
 
     def set_gyro_rates(self, rates):
         self.prev_gyro_rates = self.gyro_rates
         self.gyro_rates = rates
 
     def get_gyro_rates(self):
         return self.gyro_rates
 
-    def compute_torque(self, effector_id: EffectorJoints):
+    def compute_torque(self, joint: Joint):
 
-        effector = self.joints_list[effector_id]
-        gain = effector.scale
-        angle = effector.target_angle
+        nao_joint = self.joints_list[joint]
+        gain = nao_joint.scale
+        angle = nao_joint.target_angle
 
-        current_angle = effector.current_angle
+        current_angle = nao_joint.current_angle
 
-        if angle >= effector.max_angle:
-            angle = effector.max_angle
+        if angle >= nao_joint.max_angle:
+            angle = nao_joint.max_angle
 
-        elif angle <= effector.min_angle:
-            angle = effector.min_angle
+        elif angle <= nao_joint.min_angle:
+            angle = nao_joint.min_angle
 
-        if abs(angle - current_angle) < effector.error_tolerance:
+        if abs(angle - current_angle) < nao_joint.error_tolerance:
             return 0
         elif current_angle < angle:
             return math.radians(abs(angle - current_angle)) * gain
         elif current_angle > angle:
             return -math.radians(abs(angle - current_angle)) * gain
```

### Comparing `yohsin3d-0.2.0/yohsin3d/core/body/nao_joint.py` & `yohsin3d-0.3.0/yohsin3d/core/body/nao_joint.py`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.2.0/yohsin3d/core/communicator/base_communicator.py` & `yohsin3d-0.3.0/yohsin3d/core/communicator/base_communicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,44 +13,43 @@
     def update(self, message, heard_time, team_name, voice_orientation):
         self.message = message
         self.heard_time = heard_time
         self.team_name = team_name
         self.voice_orientation = voice_orientation
 
 
-
 class BaseCommunicator:
 
     def __init__(self) -> None:
         self.said_message: str = ""
         self.heard_message: HeardMessage = HeardMessage()
         self.world_model: WorldModel = None
         self.localizer: BaseLocalizer = None
 
     def initialize(self, world_model: WorldModel, localizer: BaseLocalizer) -> None:
         self.world_model = world_model
         self.localizer = localizer
 
-    def can_say(self): 
-        
+    def can_say(self):
+
         if not self.world_model.is_my_number_set():
             return False
-        
+
         server_time = self.world_model.get_time()
         cycles = int(server_time * 50 + 0.1)
-        is_my_turn = (cycles % (NUM_AGENTS * 2) == (self.world_model.my_number - 1) * 2)
-        is_message_valid = (self.said_message.strip() != "" and self.said_message is not None)
+        is_my_turn = (cycles % (NUM_AGENTS * 2) ==
+                      (self.world_model.my_number - 1) * 2)
+        is_message_valid = (self.said_message.strip() !=
+                            "" and self.said_message is not None)
 
         return is_my_turn and is_message_valid
-        
+
     def make_say_message(self):
         if self.can_say():
             return "(say " + self.said_message + ")"
         return ""
-    
+
     def hear(self):
         raise NotImplementedError
 
     def say(self):
         raise NotImplementedError
-    
-
```

### Comparing `yohsin3d-0.2.0/yohsin3d/core/network/parser.py` & `yohsin3d-0.3.0/yohsin3d/core/network/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import re
 from typing import List
 from ..body import *
 from ..world import *
 from ..communicator import *
 from .constants import *
+from ..common import perceptor_to_joint
 
 
 class Parser:
 
     def __init__(self,
                  world_model,
                  body_model,
                  communicator,
                  ) -> None:
 
         self.world_model: WorldModel = world_model
         self.body_model: BodyModel = body_model
         self.communicator: BaseCommunicator = communicator
-        
+
         self.side = Sides.LEFT
 
     def tokenise(self, s) -> List[str]:
         string = re.sub(r'[\(\)]', ' ', s)
         result = re.split(r'\s+', string.strip())
         return result
 
@@ -102,15 +103,15 @@
         self.body_model.set_accel_rates(
             (correctedRateX, correctedRateY, correctedRateZ))
 
     def __segment(self, string):
         return re.findall(r'\(([^()]*(?:\(([^()]*(?:\((?:[^()]*(?:\([^()]*\)[^()]*)*)\)[^()]*)*)\)[^()]*)*)\)', string)
 
     def __parse_hinge_joint(self, string):
-        effector_name = joint_to_effector[self.__parser_helper("n", string)]
+        effector_name = perceptor_to_joint[self.__parser_helper("n", string)]
         effector_angle = float(self.__parser_helper("ax", string))
 
         self.body_model.set_current_angle(effector_name, effector_angle)
         return True
 
     def __parse_FRP(self, str):
         name = self.__parser_helper("n", str)
@@ -171,18 +172,20 @@
                 "llowerarm": (float(tokens[17]), float(tokens[18]), float(tokens[19])),
                 "rfoot": (float(tokens[22]), float(tokens[23]), float(tokens[24])),
                 "lfoot": (float(tokens[27]), float(tokens[28]), float(tokens[29]))
             }
 
             if team_name == self.world_model.my_team_name:
                 self.world_model.teammate_info[agent_num].is_visible = True
-                self.world_model.teammate_info[agent_num].update_from_dict(player_info)
+                self.world_model.teammate_info[agent_num].update_from_dict(
+                    player_info)
             else:
                 self.world_model.opponent_info[agent_num].is_visible = True
-                self.world_model.opponent_info[agent_num].update_from_dict(player_info)
+                self.world_model.opponent_info[agent_num].update_from_dict(
+                    player_info)
 
         return valid
 
     def __reset_simple_non_visible_objects(self, string):
         for object in VisibleObjects:
             if not re.search(f"[(]{object.value}\s", string):
                 self.world_model.simple_vision_objects[object] = None
@@ -262,65 +265,62 @@
             elif (segment[0] == 'L'):
                 valid = self.__parse_line(segment)
 
             else:
                 valid = False
 
         return valid
-    
-
 
     def __parse_hear(self: 'Parser', string):
 
         tokens = self.tokenise(string)
         valid = False
 
         heard_time = 0.0
         is_self = False
         message = ""
 
         valid = len(tokens) == 5
 
-    
         if not valid:
             return valid
 
         i = 1
 
         if len(tokens) == 5:
             team = tokens[i]
-            i+=1
+            i += 1
             if team != self.world_model.my_team_name:
                 self.world_model.opponent_team_name = team
                 return True
 
         heard_time = float(tokens[i])
 
         if tokens[i + 1] == "self":
             is_self = True
         else:
             is_self = False
-        
+
         i += 2
 
         if i >= len(tokens):
             return False
 
         message = tokens[i]
         delta_game_time = self.world_model.get_time() - self.world_model.get_gametime()
         hear_game_time = heard_time + delta_game_time
         orientation = tokens[3]
 
         self.communicator.heard_message.update(
             message=message,
-            heard_time=hear_game_time, 
+            heard_time=hear_game_time,
             team_name=team,
             voice_orientation=orientation
-            )
-   
+        )
+
         return valid
 
     def parse(self, string):
 
         valid = True
 
         inputSegments = self.__segment(string)
```

### Comparing `yohsin3d-0.2.0/yohsin3d/core/network/server.py` & `yohsin3d-0.3.0/yohsin3d/core/network/server.py`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.2.0/yohsin3d/core/world/enums.py` & `yohsin3d-0.3.0/yohsin3d/core/world/enums.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     DIRECT_FREE_KICK_RIGHT = "direct_free_kick_right"
     PASS_LEFT = "pass_left"
     PASS_RIGHT = "pass_right"
 
 
 class ForceResistancePerceptors(Enum):
     RF = 'rf'
+    RF1 = 'rf1'
     LF = 'lf'
+    LF1 = 'lf1'
 
 
 class VisibleObjects(Enum):
     F1L = 'F1L'
     F1R = 'F1R'
     F2L = 'F2L'
     F2R = 'F2R'
```

### Comparing `yohsin3d-0.2.0/yohsin3d/core/world/world_model.py` & `yohsin3d-0.3.0/yohsin3d/core/world/world_model.py`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.2.0/yohsin3d/localizers/ground_truth_localizer.py` & `yohsin3d-0.3.0/yohsin3d/localizers/ground_truth_localizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from ..core import BaseLocalizer
 
 
 GROUNDTRUTH_NOT_ENABLED_ERROR = "Ground truth not enabled"
 
+
 class GroundTruthLocalizer(BaseLocalizer):
     def _init_(self) -> None:
         super()._init_()
 
     def check_validity(self) -> None:
         assert self.world_model.groundtruth.is_enabled(), GROUNDTRUTH_NOT_ENABLED_ERROR
```

### Comparing `yohsin3d-0.2.0/yohsin3d.egg-info/PKG-INFO` & `yohsin3d-0.3.0/yohsin3d.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yohsin3d
-Version: 0.2.0
+Version: 0.3.0
 Summary: Program your own RoboCup 3D soccer playing agents in python
 Home-page: https://github.com/FC-Yohsin/yohsin3d
 Author: Habib Shahzad, Abuzar Rasool, Faaz Abidi
 Author-email: habibshehzad55@gmail.com, availabuzar@gmail.com, hasanfaaz10@gmail.com
 License: MIT
 Keywords: robocup,soccer,3d,simulation,agents,robotics,machine learning,python,artificial intelligence,locomotion,localization
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![CodeFactor](https://www.codefactor.io/repository/github/fc-yohsin/yohsin3d/badge)](https://www.codefactor.io/repository/github/fc-yohsin/yohsin3d)
+
 # Yohsin3d: Python Framework for RoboCup 3D Soccer Agents
 
 Yohsin3d is an open-source Python framework that simplifies the development of RoboCup 3D soccer agents. It handles low-level details like server communication, basic locomotion, and localization, allowing you to focus on adding functionality to the agents. With extensive machine learning support and a thriving community, Python is an excellent choice for building intelligent and adaptive soccer agents.
 
 ## RoboCup 3D Simulation League
 
 The [RoboCup 3D Simulation League](https://ssim.robocup.org/3d-simulation/) is a platform that enables software agents to control humanoid robots, running on a realistic physics engine to simulate soccer matches. It serves as a challenging and exciting way for researchers to explore robotics and AI.
```

### Comparing `yohsin3d-0.2.0/yohsin3d.egg-info/SOURCES.txt` & `yohsin3d-0.3.0/yohsin3d.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 yohsin3d/communicators/__init__.py
 yohsin3d/communicators/y3d_communicator/__init__.py
 yohsin3d/communicators/y3d_communicator/bit_codec.py
 yohsin3d/communicators/y3d_communicator/communicator.py
 yohsin3d/core/__init__.py
 yohsin3d/core/agent.py
 yohsin3d/core/behavior.py
+yohsin3d/core/spawner.py
 yohsin3d/core/body/__init__.py
 yohsin3d/core/body/body_model.py
 yohsin3d/core/body/enums.py
 yohsin3d/core/body/nao_joint.py
 yohsin3d/core/common/__init__.py
 yohsin3d/core/common/agent_location.py
 yohsin3d/core/common/constants.py
 yohsin3d/core/common/ground_truth_model.py
+yohsin3d/core/common/joints.py
 yohsin3d/core/communicator/__init__.py
 yohsin3d/core/communicator/base_communicator.py
 yohsin3d/core/localizer/__init__.py
 yohsin3d/core/localizer/base_localizer.py
 yohsin3d/core/network/__init__.py
 yohsin3d/core/network/constants.py
 yohsin3d/core/network/parser.py
 yohsin3d/core/network/server.py
 yohsin3d/core/world/__init__.py
 yohsin3d/core/world/enums.py
 yohsin3d/core/world/world_model.py
 yohsin3d/localizers/__init__.py
-yohsin3d/localizers/ground_truth_localizer.py
+yohsin3d/localizers/ground_truth_localizer.py
+yohsin3d/movement/__init__.py
+yohsin3d/movement/movement.py
+yohsin3d/movement/y3d_movements.py
```

