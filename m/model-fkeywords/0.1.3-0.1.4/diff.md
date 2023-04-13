# Comparing `tmp/model_fkeywords-0.1.3.tar.gz` & `tmp/model_fkeywords-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_fkeywords-0.1.3.tar", last modified: Thu Apr 13 00:11:53 2023, max compression
+gzip compressed data, was "model_fkeywords-0.1.4.tar", last modified: Thu Apr 13 01:46:53 2023, max compression
```

## Comparing `model_fkeywords-0.1.3.tar` & `model_fkeywords-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 00:11:53.331330 model_fkeywords-0.1.3/
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    11357 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/LICENSE
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    13259 2023-04-13 00:11:53.331330 model_fkeywords-0.1.3/PKG-INFO
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     2213 2023-04-13 00:06:07.000000 model_fkeywords-0.1.3/README.md
-drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 00:11:53.327330 model_fkeywords-0.1.3/api_model/
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)       92 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/api_model/__init__.py
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    22777 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/api_model/nlextract.py
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     8318 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/api_model/nlsuper.py
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    15692 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/api_model/nlvisualization.py
-drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 00:11:53.331330 model_fkeywords-0.1.3/api_model/utils/
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     1483 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/api_model/utils/colorize.py
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     8405 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/api_model/utils/functions.py
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     1809 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/api_model/utils/logger.py
-drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 00:11:53.331330 model_fkeywords-0.1.3/model_fkeywords.egg-info/
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    13259 2023-04-13 00:11:52.000000 model_fkeywords-0.1.3/model_fkeywords.egg-info/PKG-INFO
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)      436 2023-04-13 00:11:52.000000 model_fkeywords-0.1.3/model_fkeywords.egg-info/SOURCES.txt
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)      115 2023-04-13 00:11:52.000000 model_fkeywords-0.1.3/model_fkeywords.egg-info/dependency_links.txt
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)        1 2023-04-13 00:10:53.000000 model_fkeywords-0.1.3/model_fkeywords.egg-info/not-zip-safe
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)      242 2023-04-13 00:11:52.000000 model_fkeywords-0.1.3/model_fkeywords.egg-info/requires.txt
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)       10 2023-04-13 00:11:52.000000 model_fkeywords-0.1.3/model_fkeywords.egg-info/top_level.txt
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)       38 2023-04-13 00:11:53.331330 model_fkeywords-0.1.3/setup.cfg
--rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     1180 2023-04-12 23:41:03.000000 model_fkeywords-0.1.3/setup.py
+drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 01:46:53.278384 model_fkeywords-0.1.4/
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    11569 2023-04-13 01:34:56.000000 model_fkeywords-0.1.4/LICENSE
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    13500 2023-04-13 01:46:53.278384 model_fkeywords-0.1.4/PKG-INFO
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     9311 2023-04-13 01:18:54.000000 model_fkeywords-0.1.4/README.md
+drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 01:46:53.274384 model_fkeywords-0.1.4/api_model/
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)       92 2023-04-12 23:41:03.000000 model_fkeywords-0.1.4/api_model/__init__.py
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    22777 2023-04-12 23:41:03.000000 model_fkeywords-0.1.4/api_model/nlextract.py
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     8318 2023-04-12 23:41:03.000000 model_fkeywords-0.1.4/api_model/nlsuper.py
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    15692 2023-04-12 23:41:03.000000 model_fkeywords-0.1.4/api_model/nlvisualization.py
+drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 01:46:53.274384 model_fkeywords-0.1.4/api_model/utils/
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     1483 2023-04-12 23:41:03.000000 model_fkeywords-0.1.4/api_model/utils/colorize.py
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     8405 2023-04-12 23:41:03.000000 model_fkeywords-0.1.4/api_model/utils/functions.py
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     1809 2023-04-12 23:41:03.000000 model_fkeywords-0.1.4/api_model/utils/logger.py
+drwxrwxr-x   0 eneasj    (1000) eneasj    (1000)        0 2023-04-13 01:46:53.274384 model_fkeywords-0.1.4/model_fkeywords.egg-info/
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)    13500 2023-04-13 01:46:53.000000 model_fkeywords-0.1.4/model_fkeywords.egg-info/PKG-INFO
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)      436 2023-04-13 01:46:53.000000 model_fkeywords-0.1.4/model_fkeywords.egg-info/SOURCES.txt
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)      115 2023-04-13 01:46:53.000000 model_fkeywords-0.1.4/model_fkeywords.egg-info/dependency_links.txt
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)        1 2023-04-13 01:46:53.000000 model_fkeywords-0.1.4/model_fkeywords.egg-info/not-zip-safe
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)      242 2023-04-13 01:46:53.000000 model_fkeywords-0.1.4/model_fkeywords.egg-info/requires.txt
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)       10 2023-04-13 01:46:53.000000 model_fkeywords-0.1.4/model_fkeywords.egg-info/top_level.txt
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)       38 2023-04-13 01:46:53.278384 model_fkeywords-0.1.4/setup.cfg
+-rw-rw-r--   0 eneasj    (1000) eneasj    (1000)     1177 2023-04-13 01:40:20.000000 model_fkeywords-0.1.4/setup.py
```

### Comparing `model_fkeywords-0.1.3/LICENSE` & `model_fkeywords-0.1.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
+   * Plase visiting the original project to instructions of usage
+   * Link: [https://github.com/EneasJr-Rodrigues/model_fkeywords/blob/main/README.md](https://github.com/EneasJr-Rodrigues/model_fkeywords)            
+
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
       "License" shall mean the terms and conditions for use, reproduction,
       and distribution as defined by Sections 1 through 9 of this document.
 
@@ -182,20 +185,21 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2023] [Eneas Rodrigues]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
+
```

### Comparing `model_fkeywords-0.1.3/PKG-INFO` & `model_fkeywords-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: model_fkeywords
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Natural Language Processing Library
 Home-page: https://github.com/EneasJr-Rodrigues/model_fkeywords
 Author: Eneas Rodrigues
 Author-email: eneas.rodrigues25@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
+           * Plase visiting the original project to instructions of usage
+           * Link: [https://github.com/EneasJr-Rodrigues/model_fkeywords/blob/main/README.md](https://github.com/EneasJr-Rodrigues/model_fkeywords)            
+        
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
         
               "License" shall mean the terms and conditions for use, reproduction,
               and distribution as defined by Sections 1 through 9 of this document.
         
@@ -189,23 +192,24 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright [2023] [Eneas Rodrigues]
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Requires-Python: ==3.7.13
+        
+Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `model_fkeywords-0.1.3/api_model/nlextract.py` & `model_fkeywords-0.1.4/api_model/nlextract.py`

 * *Files identical despite different names*

### Comparing `model_fkeywords-0.1.3/api_model/nlsuper.py` & `model_fkeywords-0.1.4/api_model/nlsuper.py`

 * *Files identical despite different names*

### Comparing `model_fkeywords-0.1.3/api_model/nlvisualization.py` & `model_fkeywords-0.1.4/api_model/nlvisualization.py`

 * *Files identical despite different names*

### Comparing `model_fkeywords-0.1.3/api_model/utils/colorize.py` & `model_fkeywords-0.1.4/api_model/utils/colorize.py`

 * *Files identical despite different names*

### Comparing `model_fkeywords-0.1.3/api_model/utils/functions.py` & `model_fkeywords-0.1.4/api_model/utils/functions.py`

 * *Files identical despite different names*

### Comparing `model_fkeywords-0.1.3/api_model/utils/logger.py` & `model_fkeywords-0.1.4/api_model/utils/logger.py`

 * *Files identical despite different names*

### Comparing `model_fkeywords-0.1.3/model_fkeywords.egg-info/PKG-INFO` & `model_fkeywords-0.1.4/model_fkeywords.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: model-fkeywords
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Natural Language Processing Library
 Home-page: https://github.com/EneasJr-Rodrigues/model_fkeywords
 Author: Eneas Rodrigues
 Author-email: eneas.rodrigues25@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
+           * Plase visiting the original project to instructions of usage
+           * Link: [https://github.com/EneasJr-Rodrigues/model_fkeywords/blob/main/README.md](https://github.com/EneasJr-Rodrigues/model_fkeywords)            
+        
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
         
               "License" shall mean the terms and conditions for use, reproduction,
               and distribution as defined by Sections 1 through 9 of this document.
         
@@ -189,23 +192,24 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright [2023] [Eneas Rodrigues]
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Requires-Python: ==3.7.13
+        
+Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `model_fkeywords-0.1.3/setup.py` & `model_fkeywords-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     version=INFO['version'],
     author=INFO['author'],
     author_email=INFO['author_email'],
     url=INFO['url'],    
     license=open(os.path.join(PROJECT_DIR, 'LICENSE')).read(),
     packages=find_namespace_packages(include=['api_model','api_model.utils']),
     install_requires=[d for d in DEPENDENCIES if '://' not in d],
-    python_requires='==3.7.13',
+    python_requires='>=3.8',
     #TO-DO: Fix dependency links : not working with bdist_wheel
     dependency_links = ["git+https://github.com/explosion/spacy-models/releases/download/pt_core_news_sm-3.2.0/pt_core_news_sm-3.2.0.tar.gz"],
     tests_require=['pytest', 'parameterized'],
     zip_safe=False
 )
```

