# Comparing `tmp/OpenGeode_Geosciences-6.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Geosciences-6.1.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,8 @@
-Zip file size: 4562 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       76 b- defN 23-Apr-04 14:23 opengeode_geosciences/__init__.py
--rw-rw-rw-  2.0 fat     1243 b- defN 23-Apr-04 14:23 opengeode_geosciences/geosciences.py
--rw-rw-rw-  2.0 fat       96 b- defN 23-Apr-04 14:25 opengeode_geosciences/opengeode_geosciences.py
--rw-rw-rw-  2.0 fat     1242 b- defN 23-Apr-04 14:25 opengeode_geosciences/opengeode_geosciences_geosciences.py
--rw-rw-rw-  2.0 fat     3183 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      752 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/RECORD
-8 files, 6714 bytes uncompressed, 3218 bytes compressed:  52.1%
+Zip file size: 3364 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       76 b- defN 23-Apr-13 07:14 opengeode_geosciences/__init__.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-Apr-13 07:14 opengeode_geosciences/geosciences.py
+-rw-rw-rw-  2.0 fat     3233 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      536 b- defN 23-Apr-13 07:16 OpenGeode_Geosciences-6.1.0.dist-info/RECORD
+6 files, 5214 bytes uncompressed, 2380 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -1,25 +1,19 @@
 Filename: opengeode_geosciences/__init__.py
 Comment: 
 
 Filename: opengeode_geosciences/geosciences.py
 Comment: 
 
-Filename: opengeode_geosciences/opengeode_geosciences.py
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/METADATA
 Comment: 
 
-Filename: opengeode_geosciences/opengeode_geosciences_geosciences.py
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/METADATA
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/WHEEL
-Comment: 
-
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/top_level.txt
-Comment: 
-
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/RECORD
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciences/geosciences.py

```diff
@@ -16,10 +16,10 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import opengeode
 
-from .opengeode_geosciences_py_geosciences import *
+from .bin.opengeode_geosciences_py_geosciences import *
 
 OpenGeodeGeosciencesGeosciences.initialize()
```

## Comparing `OpenGeode_Geosciences-6.0.3.dist-info/METADATA` & `OpenGeode_Geosciences-6.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Geosciences
-Version: 6.0.3
+Version: 6.1.0
 Summary: OpenGeode module for Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: opengeode-core (==13.*,>=13.4.15)
 
 <h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 6.0.3 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 6.1.0 Summary:
 OpenGeode module for Geosciences Home-page: https://github.com/Geode-solutions/
 OpenGeode-Geosciences Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: MIT Platform: UNKNOWN Description-Content-Type: text/
-markdown
+markdown Requires-Dist: opengeode-core (==13.*,>=13.4.15)
              ****** OpenGeode-Geosciencesby Geode-solutions ******
                   **** OpenGeode module for Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-Geosciences is a module of [OpenGeode] provides
 data structures for geological models and geological objects. [OpenGeode]:
```

