# Comparing `tmp/comandor-0.2.3.tar.gz` & `tmp/comandor-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comandor-0.2.3.tar", last modified: Wed Mar 22 14:12:32 2023, max compression
+gzip compressed data, was "comandor-0.2.8.tar", last modified: Thu Apr 13 12:23:47 2023, max compression
```

## Comparing `comandor-0.2.3.tar` & `comandor-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 14:12:32.512782 comandor-0.2.3/
--rw-rw-rw-   0        0        0     1089 2023-03-06 17:33:22.000000 comandor-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     1970 2023-03-22 14:12:32.512782 comandor-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2023-03-09 15:46:07.000000 comandor-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 14:12:32.481531 comandor-0.2.3/comandor/
--rw-rw-rw-   0        0        0        0 2023-03-07 14:42:09.000000 comandor-0.2.3/comandor/__init__.py
--rw-rw-rw-   0        0        0      131 2023-03-09 15:46:07.000000 comandor-0.2.3/comandor/log.py
--rw-rw-rw-   0        0        0     3062 2023-03-22 14:09:34.000000 comandor-0.2.3/comandor/main.py
--rw-rw-rw-   0        0        0      587 2023-03-09 15:46:07.000000 comandor-0.2.3/comandor/models.py
--rw-rw-rw-   0        0        0      687 2023-03-09 15:46:07.000000 comandor-0.2.3/comandor/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:12:32.512782 comandor-0.2.3/comandor.egg-info/
--rw-rw-rw-   0        0        0     1970 2023-03-22 14:12:32.000000 comandor-0.2.3/comandor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-03-22 14:12:32.000000 comandor-0.2.3/comandor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 14:12:32.000000 comandor-0.2.3/comandor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-22 14:12:32.000000 comandor-0.2.3/comandor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-03-22 14:12:32.000000 comandor-0.2.3/comandor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-22 14:12:32.000000 comandor-0.2.3/comandor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 14:12:32.512782 comandor-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-03-22 14:10:41.000000 comandor-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 14:12:32.512782 comandor-0.2.3/test/
--rw-rw-rw-   0        0        0     1145 2023-03-09 15:46:07.000000 comandor-0.2.3/test/test_comandor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 12:23:35.000000 comandor-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 12:23:47.749395 comandor-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 12:23:35.000000 comandor-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/comandor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-13 12:23:35.000000 comandor-0.2.8/comandor/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/comandor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 12:23:47.000000 comandor-0.2.8/comandor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:23:47.749395 comandor-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-13 12:23:35.000000 comandor-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:23:47.749395 comandor-0.2.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-13 12:23:35.000000 comandor-0.2.8/test/test_comandor.py
```

### Comparing `comandor-0.2.3/LICENSE` & `comandor-0.2.8/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 F . Sarmaly
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 F . Sarmaly
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `comandor-0.2.3/PKG-INFO` & `comandor-0.2.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: comandor
-Version: 0.2.3
-Summary: A Very Simple Script for Run your command!
-Home-page: https://github.com/NoobforAl/comandor
-Author: NoobforAl
-Author-email: FarshadSarmali@pm.me
-License: MIT License
-Keywords: command line,script
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# comandor
-Very Simple Script for Run your command!  
-A simple tool to simplify some repetitive 
-tasks such as updating the Linux repository and daily tasks!
-
-### How Install
-
-> pip install comandor
-
-### How Use
-
-- make file .comandor  
-- setup config like this 
-
-```json
-{
-  "name": "Update Apps!",
-  "debug": true, // run debug mode ( not necessary )
-  "logfile": "./logs.log", // where save logs ( not necessary )
-  "actions": [
-    {
-      "action_name": "scoop update pkg",
-      "path": "C:/",
-      "commands": [
-        "scoop update -g *"
-      ],
-      "timeout": 5000
-    }
-    // you can add more action
-  ]
-}
-```  
-
-- you can see .comandor.example for more example  
-- and run this command
-
-> comandor 
-
-### Command Line Help
-
-| Command |                                      Info                                              |
-| -----   | :--------------------------------------------------------------------------------------: |
-| -h      |                                      see help                                            |
-| -l < path log file >  | where save logFile, if don't use this, not save logs |
-| -c  < path config file > | setup yor config file instead of .comandor file |
-| -d   | run program debug mode |
-
+Metadata-Version: 2.1
+Name: comandor
+Version: 0.2.8
+Summary: A Very Simple Script for Run your command!
+Home-page: https://github.com/NoobforAl/comandor
+Author: NoobforAl
+Author-email: FarshadSarmali@pm.me
+License: MIT License
+Keywords: command line,script
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Comandor
+
+Very Simple Script for Run your command!  
+A simple tool to simplify some repetitive
+tasks such as updating the Linux repository and daily tasks!
+
+## How Install
+
+> pip install comandor
+
+### How Use
+
+- make file .comandor  
+- setup config like this
+
+```json
+{
+  "name": "Update Apps!",
+  "debug": true, // run debug mode ( not necessary )
+  "logfile": "./logs.log", // where save logs ( not necessary )
+  "actions": [
+    {
+      "action_name": "scoop update pkg",
+      "path": "C:/",
+      "commands": [
+        "scoop update -g *"
+      ],
+      "timeout": 5000
+    }
+    // you can add more action
+  ]
+}
+```  
+
+- you can see .comandor.example for more example  
+- and run this command
+
+> comandor
+
+### Command Line Help
+
+| Command |                                      Info                                              |
+| -----   | :--------------------------------------------------------------------------------------: |
+| -h      |                                      see help                                            |
+| -l < path log file >  | where save logFile, if don't use this, not save logs |
+| -c  < path config file > | setup yor config file instead of .comandor file |
+| -d   | run program debug mode |
```

### Comparing `comandor-0.2.3/README.md` & `comandor-0.2.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# comandor
-Very Simple Script for Run your command!  
-A simple tool to simplify some repetitive 
-tasks such as updating the Linux repository and daily tasks!
-
-### How Install
-
-> pip install comandor
-
-### How Use
-
-- make file .comandor  
-- setup config like this 
-
-```json
-{
-  "name": "Update Apps!",
-  "debug": true, // run debug mode ( not necessary )
-  "logfile": "./logs.log", // where save logs ( not necessary )
-  "actions": [
-    {
-      "action_name": "scoop update pkg",
-      "path": "C:/",
-      "commands": [
-        "scoop update -g *"
-      ],
-      "timeout": 5000
-    }
-    // you can add more action
-  ]
-}
-```  
-
-- you can see .comandor.example for more example  
-- and run this command
-
-> comandor 
-
-### Command Line Help
-
-| Command |                                      Info                                              |
-| -----   | :--------------------------------------------------------------------------------------: |
-| -h      |                                      see help                                            |
-| -l < path log file >  | where save logFile, if don't use this, not save logs |
-| -c  < path config file > | setup yor config file instead of .comandor file |
-| -d   | run program debug mode |
-
+# Comandor
+
+Very Simple Script for Run your command!  
+A simple tool to simplify some repetitive
+tasks such as updating the Linux repository and daily tasks!
+
+## How Install
+
+> pip install comandor
+
+### How Use
+
+- make file .comandor  
+- setup config like this
+
+```json
+{
+  "name": "Update Apps!",
+  "debug": true, // run debug mode ( not necessary )
+  "logfile": "./logs.log", // where save logs ( not necessary )
+  "actions": [
+    {
+      "action_name": "scoop update pkg",
+      "path": "C:/",
+      "commands": [
+        "scoop update -g *"
+      ],
+      "timeout": 5000
+    }
+    // you can add more action
+  ]
+}
+```  
+
+- you can see .comandor.example for more example  
+- and run this command
+
+> comandor
+
+### Command Line Help
+
+| Command |                                      Info                                              |
+| -----   | :--------------------------------------------------------------------------------------: |
+| -h      |                                      see help                                            |
+| -l < path log file >  | where save logFile, if don't use this, not save logs |
+| -c  < path config file > | setup yor config file instead of .comandor file |
+| -d   | run program debug mode |
```

### Comparing `comandor-0.2.3/comandor/settings.py` & `comandor-0.2.8/comandor/settings.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from pydantic import ValidationError
-
-from comandor.models import Setting
-from comandor.log import log
-
-import json
-import os
-
-
-# load setting form file and return setting
-# default use ./.comandor
-def loadSetting(file: str = ".comandor") -> Setting:
-    if not os.path.exists(file):
-        raise Exception("Config file not found!")
-
-    setting: Setting
-    with open(file, "r") as f:
-        try:
-            op = json.load(f)
-            setting = Setting(**op)
-
-        except ValidationError as e:
-            log.error(e)
-            raise e
-
-        except json.JSONDecodeError as e:
-            log.error(e)
-            raise e
-
-    return setting
+from pydantic import ValidationError
+
+from comandor.models import Setting
+from comandor.log import log
+
+import json
+import os
+
+
+# load setting form file and return setting
+# default use ./.comandor
+def loadSetting(file: str = ".comandor") -> Setting:
+    if not os.path.exists(file):
+        raise Exception("Config file not found!")
+
+    setting: Setting
+    with open(file, "r") as f:
+        try:
+            op = json.load(f)
+            setting = Setting(**op)
+
+        except ValidationError as e:
+            log.error(e)
+            raise e
+
+        except json.JSONDecodeError as e:
+            log.error(e)
+            raise e
+
+    return setting
```

### Comparing `comandor-0.2.3/comandor.egg-info/PKG-INFO` & `comandor-0.2.8/comandor.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: comandor
-Version: 0.2.3
-Summary: A Very Simple Script for Run your command!
-Home-page: https://github.com/NoobforAl/comandor
-Author: NoobforAl
-Author-email: FarshadSarmali@pm.me
-License: MIT License
-Keywords: command line,script
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# comandor
-Very Simple Script for Run your command!  
-A simple tool to simplify some repetitive 
-tasks such as updating the Linux repository and daily tasks!
-
-### How Install
-
-> pip install comandor
-
-### How Use
-
-- make file .comandor  
-- setup config like this 
-
-```json
-{
-  "name": "Update Apps!",
-  "debug": true, // run debug mode ( not necessary )
-  "logfile": "./logs.log", // where save logs ( not necessary )
-  "actions": [
-    {
-      "action_name": "scoop update pkg",
-      "path": "C:/",
-      "commands": [
-        "scoop update -g *"
-      ],
-      "timeout": 5000
-    }
-    // you can add more action
-  ]
-}
-```  
-
-- you can see .comandor.example for more example  
-- and run this command
-
-> comandor 
-
-### Command Line Help
-
-| Command |                                      Info                                              |
-| -----   | :--------------------------------------------------------------------------------------: |
-| -h      |                                      see help                                            |
-| -l < path log file >  | where save logFile, if don't use this, not save logs |
-| -c  < path config file > | setup yor config file instead of .comandor file |
-| -d   | run program debug mode |
-
+Metadata-Version: 2.1
+Name: comandor
+Version: 0.2.8
+Summary: A Very Simple Script for Run your command!
+Home-page: https://github.com/NoobforAl/comandor
+Author: NoobforAl
+Author-email: FarshadSarmali@pm.me
+License: MIT License
+Keywords: command line,script
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Comandor
+
+Very Simple Script for Run your command!  
+A simple tool to simplify some repetitive
+tasks such as updating the Linux repository and daily tasks!
+
+## How Install
+
+> pip install comandor
+
+### How Use
+
+- make file .comandor  
+- setup config like this
+
+```json
+{
+  "name": "Update Apps!",
+  "debug": true, // run debug mode ( not necessary )
+  "logfile": "./logs.log", // where save logs ( not necessary )
+  "actions": [
+    {
+      "action_name": "scoop update pkg",
+      "path": "C:/",
+      "commands": [
+        "scoop update -g *"
+      ],
+      "timeout": 5000
+    }
+    // you can add more action
+  ]
+}
+```  
+
+- you can see .comandor.example for more example  
+- and run this command
+
+> comandor
+
+### Command Line Help
+
+| Command |                                      Info                                              |
+| -----   | :--------------------------------------------------------------------------------------: |
+| -h      |                                      see help                                            |
+| -l < path log file >  | where save logFile, if don't use this, not save logs |
+| -c  < path config file > | setup yor config file instead of .comandor file |
+| -d   | run program debug mode |
```

