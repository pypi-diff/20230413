# Comparing `tmp/OpenGeode_Geosciences-6.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Geosciences-7.0.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3364 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       76 b- defN 23-Apr-13 07:14 opengeode_geosciences/__init__.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-Apr-13 07:14 opengeode_geosciences/geosciences.py
--rw-rw-rw-  2.0 fat     3233 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      536 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/RECORD
-6 files, 5214 bytes uncompressed, 2380 bytes compressed:  54.4%
+Zip file size: 4264 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Apr-13 13:10 opengeode_geosciences/__init__.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 23-Apr-13 13:10 opengeode_geosciences/explicit.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 23-Apr-13 13:10 opengeode_geosciences/implicit.py
+-rw-rw-rw-  2.0 fat     3232 b- defN 23-Apr-13 13:12 OpenGeode_Geosciences-7.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 13:12 OpenGeode_Geosciences-7.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-13 13:12 OpenGeode_Geosciences-7.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      623 b- defN 23-Apr-13 13:12 OpenGeode_Geosciences-7.0.0.dist-info/RECORD
+7 files, 6553 bytes uncompressed, 3144 bytes compressed:  52.0%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: opengeode_geosciences/__init__.py
 Comment: 
 
-Filename: opengeode_geosciences/geosciences.py
+Filename: opengeode_geosciences/explicit.py
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.1.0.dist-info/METADATA
+Filename: opengeode_geosciences/implicit.py
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.1.0.dist-info/WHEEL
+Filename: OpenGeode_Geosciences-7.0.0.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.1.0.dist-info/top_level.txt
+Filename: OpenGeode_Geosciences-7.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.1.0.dist-info/RECORD
+Filename: OpenGeode_Geosciences-7.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: OpenGeode_Geosciences-7.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciences/__init__.py

```diff
@@ -1,3 +1,4 @@
 ## Copyright (c) 2019 - 2023 Geode-solutions
 
-from .geosciences import *
+from .explicit import *
+from .implicit import *
```

## Comparing `opengeode_geosciences/geosciences.py` & `opengeode_geosciences/implicit.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import opengeode
 
-from .bin.opengeode_geosciences_py_geosciences import *
+from .bin.opengeode_geosciences_py_implicit import *
 
-OpenGeodeGeosciencesGeosciences.initialize()
+GeosciencesImplicitLibrary.initialize()
```

## Comparing `OpenGeode_Geosciences-6.1.0.dist-info/METADATA` & `OpenGeode_Geosciences-7.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Geosciences
-Version: 6.1.0
+Version: 7.0.0
 Summary: OpenGeode module for Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==13.*,>=13.4.15)
+Requires-Dist: opengeode-core (==14.*,>=14.0.0)
 
 <h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 6.1.0 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 7.0.0 Summary:
 OpenGeode module for Geosciences Home-page: https://github.com/Geode-solutions/
 OpenGeode-Geosciences Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: MIT Platform: UNKNOWN Description-Content-Type: text/
-markdown Requires-Dist: opengeode-core (==13.*,>=13.4.15)
+markdown Requires-Dist: opengeode-core (==14.*,>=14.0.0)
              ****** OpenGeode-Geosciencesby Geode-solutions ******
                   **** OpenGeode module for Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-Geosciences is a module of [OpenGeode] provides
 data structures for geological models and geological objects. [OpenGeode]:
```

