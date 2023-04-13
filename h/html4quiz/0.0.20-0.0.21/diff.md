# Comparing `tmp/html4quiz-0.0.20.tar.gz` & `tmp/html4quiz-0.0.21.tar.gz`

## Comparing `html4quiz-0.0.20.tar` & `html4quiz-0.0.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 html4quiz-0.0.20/Embedding Images in HTMLs.url
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 html4quiz-0.0.20/Packaging.url
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 html4quiz-0.0.20/certutil -encode mypicture.png mypicture.txt.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 html4quiz-0.0.20/up8c18p01.png
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 html4quiz-0.0.20/up8c18p01.txt
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 html4quiz-0.0.20/updatePackage.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.20/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 html4quiz-0.0.20/src/html4quiz/_common.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.20/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.20/src/html4quiz/_generateMakeHTMLs.py
--rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 html4quiz-0.0.20/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.20/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.20/LICENSE.txt
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 html4quiz-0.0.20/README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.20/pyproject.toml
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 html4quiz-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 html4quiz-0.0.21/Embedding Images in HTMLs.url
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 html4quiz-0.0.21/Packaging.url
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 html4quiz-0.0.21/certutil -encode mypicture.png mypicture.txt.txt
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 html4quiz-0.0.21/up8c18p01.png
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 html4quiz-0.0.21/up8c18p01.txt
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 html4quiz-0.0.21/updatePackage.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_generateMakeHTMLs.py
+-rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.21/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.21/LICENSE.txt
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 html4quiz-0.0.21/README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 html4quiz-0.0.21/PKG-INFO
```

### Comparing `html4quiz-0.0.20/up8c18p01.png` & `html4quiz-0.0.21/up8c18p01.png`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.20/up8c18p01.txt` & `html4quiz-0.0.21/up8c18p01.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.20/src/html4quiz/_common.py` & `html4quiz-0.0.21/src/html4quiz/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math, random, re, json
 from urllib.request import urlopen
 
 def getFigure(file: str):
-    return json.loads(urlopen(f'https://generateNscore.github.io/htmlfilesforquiz/JS/{file}.json').read())
+    return json.loads(urlopen(f'https://generateNscore.github.io/html4quiz/JS/{file}.json').read())
 
 def round2MSF(a):
     if not a or (isinstance(a, int) and abs(a)<1000) : return a
 
     sfN=3
     signFlag=False
     if a<0: a=-a; signFlag=True
```

### Comparing `html4quiz-0.0.20/src/html4quiz/_generateEm.py` & `html4quiz-0.0.21/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.20/src/html4quiz/_generateMakeHTMLs.py` & `html4quiz-0.0.21/src/html4quiz/_generateMakeHTMLs.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.20/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.21/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.20/src/html4quiz/makeChoices.py` & `html4quiz-0.0.21/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.20/LICENSE.txt` & `html4quiz-0.0.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.20/README.md` & `html4quiz-0.0.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 
+<li>Version 0.0.21</li>
+<ul><li>Package name has been changed from htmlfilesforquiz to html4quiz</li>
+<li>So is the name of repository in GitHub.</li></ul>
+
 <li>Version 0.0.20</li>
 
 <ul><li>Finallized a way to upload/download Javascript scripts saved in JSON files for figures.<a href="https://github.com/generateNscore/html4quiz/wiki#h-download-json-file-of-javascript-code-for-figure-contents">H. Download Json file of Javascript code for figure contents</a></li></ul>
 <br>
 
 <li>Version 0.0.16</li>
```

#### html2text {}

```diff
@@ -21,14 +21,17 @@
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
     *
       pip install html4quiz
 ## Dependencies
     * None
 ## Changes
+Version 0.0.21
+    * Package name has been changed from htmlfilesforquiz to html4quiz
+    * So is the name of repository in GitHub.
 Version 0.0.20
     * Finallized a way to upload/download Javascript scripts saved in JSON
       files for figures.H._Download_Json_file_of_Javascript_code_for_figure
       contents
 
 Version 0.0.16
     * In addition to typical short-answer questions that can be answered on the
```

### Comparing `html4quiz-0.0.20/pyproject.toml` & `html4quiz-0.0.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.20"
+version = "0.0.21"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.20/PKG-INFO` & `html4quiz-0.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.20
+Version: 0.0.21
 Summary: A package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -52,14 +52,18 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 
+<li>Version 0.0.21</li>
+<ul><li>Package name has been changed from htmlfilesforquiz to html4quiz</li>
+<li>So is the name of repository in GitHub.</li></ul>
+
 <li>Version 0.0.20</li>
 
 <ul><li>Finallized a way to upload/download Javascript scripts saved in JSON files for figures.<a href="https://github.com/generateNscore/html4quiz/wiki#h-download-json-file-of-javascript-code-for-figure-contents">H. Download Json file of Javascript code for figure contents</a></li></ul>
 <br>
 
 <li>Version 0.0.16</li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.20 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.21 Summary: A package that
 generates question papers as HTML files to be distributed over the network and
 grades the answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
 :: End Users/Desktop Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,17 @@
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
     *
       pip install html4quiz
 ## Dependencies
     * None
 ## Changes
+Version 0.0.21
+    * Package name has been changed from htmlfilesforquiz to html4quiz
+    * So is the name of repository in GitHub.
 Version 0.0.20
     * Finallized a way to upload/download Javascript scripts saved in JSON
       files for figures.H._Download_Json_file_of_Javascript_code_for_figure
       contents
 
 Version 0.0.16
     * In addition to typical short-answer questions that can be answered on the
```

