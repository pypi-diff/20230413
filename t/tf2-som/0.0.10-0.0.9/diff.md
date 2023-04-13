# Comparing `tmp/tf2-som-0.0.10.tar.gz` & `tmp/tf2-som-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2-som-0.0.10.tar", last modified: Thu Apr 13 08:47:00 2023, max compression
+gzip compressed data, was "tf2-som-0.0.9.tar", last modified: Sat Sep 10 08:41:02 2022, max compression
```

## Comparing `tf2-som-0.0.10.tar` & `tf2-som-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-04-13 08:47:00.340527 tf2-som-0.0.10/
--rw-r--r--   0 jodier     (501) staff       (20)      129 2023-04-12 11:49:32.000000 tf2-som-0.0.10/LICENSE.md
--rw-r--r--   0 jodier     (501) staff       (20)     2200 2023-04-13 08:47:00.340282 tf2-som-0.0.10/PKG-INFO
--rw-r--r--   0 jodier     (501) staff       (20)     1717 2023-04-12 17:32:23.000000 tf2-som-0.0.10/README.md
--rw-r--r--   0 jodier     (501) staff       (20)       38 2023-04-13 08:47:00.340615 tf2-som-0.0.10/setup.cfg
--rwxr-xr-x   0 jodier     (501) staff       (20)     1920 2023-04-12 11:49:32.000000 tf2-som-0.0.10/setup.py
-drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-04-13 08:47:00.339039 tf2-som-0.0.10/tf2_som.egg-info/
--rw-r--r--   0 jodier     (501) staff       (20)     2200 2023-04-13 08:47:00.000000 tf2-som-0.0.10/tf2_som.egg-info/PKG-INFO
--rw-r--r--   0 jodier     (501) staff       (20)      223 2023-04-13 08:47:00.000000 tf2-som-0.0.10/tf2_som.egg-info/SOURCES.txt
--rw-r--r--   0 jodier     (501) staff       (20)        1 2023-04-13 08:47:00.000000 tf2-som-0.0.10/tf2_som.egg-info/dependency_links.txt
--rw-r--r--   0 jodier     (501) staff       (20)       91 2023-04-13 08:47:00.000000 tf2-som-0.0.10/tf2_som.egg-info/requires.txt
--rw-r--r--   0 jodier     (501) staff       (20)        7 2023-04-13 08:47:00.000000 tf2-som-0.0.10/tf2_som.egg-info/top_level.txt
-drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-04-13 08:47:00.339834 tf2-som-0.0.10/tf_som/
--rw-r--r--   0 jodier     (501) staff       (20)    34566 2023-04-13 08:39:45.000000 tf2-som-0.0.10/tf_som/__init__.py
--rw-r--r--   0 jodier     (501) staff       (20)      237 2023-04-12 17:28:17.000000 tf2-som-0.0.10/tf_som/metadata.json
+drwxr-xr-x   0 jodier     (502) staff       (20)        0 2022-09-10 08:41:02.017850 tf2-som-0.0.9/
+-rw-r--r--   0 jodier     (502) staff       (20)      129 2022-09-06 21:45:08.000000 tf2-som-0.0.9/LICENSE.md
+-rw-r--r--   0 jodier     (502) staff       (20)     2165 2022-09-10 08:41:02.017446 tf2-som-0.0.9/PKG-INFO
+-rw-r--r--   0 jodier     (502) staff       (20)     1683 2022-09-10 08:37:08.000000 tf2-som-0.0.9/README.md
+-rw-r--r--   0 jodier     (502) staff       (20)       38 2022-09-10 08:41:02.017928 tf2-som-0.0.9/setup.cfg
+-rwxr-xr-x   0 jodier     (502) staff       (20)     1920 2022-09-10 08:36:18.000000 tf2-som-0.0.9/setup.py
+drwxr-xr-x   0 jodier     (502) staff       (20)        0 2022-09-10 08:41:02.016384 tf2-som-0.0.9/tf2_som.egg-info/
+-rw-r--r--   0 jodier     (502) staff       (20)     2165 2022-09-10 08:41:01.000000 tf2-som-0.0.9/tf2_som.egg-info/PKG-INFO
+-rw-r--r--   0 jodier     (502) staff       (20)      223 2022-09-10 08:41:01.000000 tf2-som-0.0.9/tf2_som.egg-info/SOURCES.txt
+-rw-r--r--   0 jodier     (502) staff       (20)        1 2022-09-10 08:41:01.000000 tf2-som-0.0.9/tf2_som.egg-info/dependency_links.txt
+-rw-r--r--   0 jodier     (502) staff       (20)       91 2022-09-10 08:41:01.000000 tf2-som-0.0.9/tf2_som.egg-info/requires.txt
+-rw-r--r--   0 jodier     (502) staff       (20)        7 2022-09-10 08:41:01.000000 tf2-som-0.0.9/tf2_som.egg-info/top_level.txt
+drwxr-xr-x   0 jodier     (502) staff       (20)        0 2022-09-10 08:41:02.017050 tf2-som-0.0.9/tf_som/
+-rw-r--r--   0 jodier     (502) staff       (20)    30566 2022-09-10 08:36:43.000000 tf2-som-0.0.9/tf_som/__init__.py
+-rw-r--r--   0 jodier     (502) staff       (20)      236 2022-09-10 08:40:48.000000 tf2-som-0.0.9/tf_som/metadata.json
```

### Comparing `tf2-som-0.0.10/PKG-INFO` & `tf2-som-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf2-som
-Version: 0.0.10
+Version: 0.0.9
 Summary: Tensorflow 2 implementation of the Self Organizing Maps (SOM)
 Home-page: https://odier-io.github.io/tf2-som/
 Author: Jérôme ODIER, Nora ACHBAK
 Author-email: jerome.odier@lpsc.in2p3.fr, nora.achbak@lpsc.in2p3.fr
 License: CeCILL-C
 Keywords: som,self organizing map,machine learning
 Description-Content-Type: text/markdown
@@ -26,17 +26,17 @@
 <a href="http://www.in2p3.fr/"               target="_blank" style="margin-right: 2rem;"><img src="https://ami.web.cern.ch/images/logo_in2p3.png" alt="IN2P3" height="72" /></a>
 &nbsp;&nbsp;&nbsp;
 <a href="http://www.univ-grenoble-alpes.fr/" target="_blank" style="margin-right: 0rem;"><img src="https://ami.web.cern.ch/images/logo_uga.png" alt="UGA" height="72" /></a>
 
 TF2-SOM
 =======
 
-This is a fast Tensorflow 2 implementation of the Self Organizing Maps (SOM) running on arbitrarily large datasets.
+This is a fast Tensorflow 2 implementation of the Self Organizing Maps (SOM).
 
-<img src="https://odier-io.github.io/tf2-som/som.png" alt="" height="250" />
+<img src="https://odier-xyz.github.io/tf2-som/som.png" alt="som" height="250" />
 
 Documentation
 =============
 
 https://odier-io.github.io/tf2-som/
 
 Demo
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: tf2-som Version: 0.0.10 Summary: Tensorflow 2
+Metadata-Version: 2.1 Name: tf2-som Version: 0.0.9 Summary: Tensorflow 2
 implementation of the Self Organizing Maps (SOM) Home-page: https://odier-
 io.github.io/tf2-som/ Author: JÃ©rÃ´me ODIER, Nora ACHBAK Author-email:
 jerome.odier@lpsc.in2p3.fr, nora.achbak@lpsc.in2p3.fr License: CeCILL-
 C Keywords: som,self organizing map,machine learning Description-Content-Type:
 text/markdown Provides-Extra: pandas Provides-Extra: astropy Provides-Extra:
 matplotlib License-File: LICENSE.md [![][License img]][License]   [![][MainRepo
 img]][MainRepo]   [![][AltRepo img]][AltRepo]
 [LPSC]     [IN2P3]     [UGA] TF2-SOM ======= This is a fast Tensorflow 2
-implementation of the Self Organizing Maps (SOM) running on arbitrarily large
-datasets.  Documentation ============= https://odier-io.github.io/tf2-som/ Demo
-==== [ð Click there](https://github.com/odier-io/tf2-som/blob/master/demo/
-demo.ipynb) Authors ======= - [JÃ©rÃ´me ODIER](https://annuaire.in2p3.fr/4121-
-4467/jerome-odier) ([CNRS/LPSC](https://lpsc.in2p3.fr/)) - [Nora ACHBAK](https:
-//annuaire.in2p3.fr/7591-10426/nora-achbak) ([CNRS/LPSC](https://lpsc.in2p3.fr/
-)) [License]:http://www.cecill.info/licences/Licence_CeCILL-C_V1-en.txt
-[License img]:https://img.shields.io/badge/license-CeCILL--C-blue.svg
-[MainRepo]:https://gitlab.in2p3.fr/jodier/tf2_som [MainRepo img]:https://
-img.shields.io/badge/Main%20Repo-gitlab.in2p3.fr-success [AltRepo]:https://
-github.com/odier-xyz/tf2_som [AltRepo img]:https://img.shields.io/badge/
-Alt%20Repo-github.com-success
+implementation of the Self Organizing Maps (SOM). [som] Documentation
+============= https://odier-io.github.io/tf2-som/ Demo ==== [ð Click there]
+(https://github.com/odier-io/tf2-som/blob/master/demo/demo.ipynb) Authors
+======= - [JÃ©rÃ´me ODIER](https://annuaire.in2p3.fr/4121-4467/jerome-odier) (
+[CNRS/LPSC](https://lpsc.in2p3.fr/)) - [Nora ACHBAK](https://annuaire.in2p3.fr/
+7591-10426/nora-achbak) ([CNRS/LPSC](https://lpsc.in2p3.fr/)) [License]:http://
+www.cecill.info/licences/Licence_CeCILL-C_V1-en.txt [License img]:https://
+img.shields.io/badge/license-CeCILL--C-blue.svg [MainRepo]:https://
+gitlab.in2p3.fr/jodier/tf2_som [MainRepo img]:https://img.shields.io/badge/
+Main%20Repo-gitlab.in2p3.fr-success [AltRepo]:https://github.com/odier-xyz/
+tf2_som [AltRepo img]:https://img.shields.io/badge/Alt%20Repo-github.com-
+success
```

### Comparing `tf2-som-0.0.10/README.md` & `tf2-som-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 <a href="http://www.in2p3.fr/"               target="_blank" style="margin-right: 2rem;"><img src="https://ami.web.cern.ch/images/logo_in2p3.png" alt="IN2P3" height="72" /></a>
 &nbsp;&nbsp;&nbsp;
 <a href="http://www.univ-grenoble-alpes.fr/" target="_blank" style="margin-right: 0rem;"><img src="https://ami.web.cern.ch/images/logo_uga.png" alt="UGA" height="72" /></a>
 
 TF2-SOM
 =======
 
-This is a fast Tensorflow 2 implementation of the Self Organizing Maps (SOM) running on arbitrarily large datasets.
+This is a fast Tensorflow 2 implementation of the Self Organizing Maps (SOM).
 
-<img src="https://odier-io.github.io/tf2-som/som.png" alt="" height="250" />
+<img src="https://odier-xyz.github.io/tf2-som/som.png" alt="som" height="250" />
 
 Documentation
 =============
 
 https://odier-io.github.io/tf2-som/
 
 Demo
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 [![][License img]][License]   [![][MainRepo img]][MainRepo]   [![][AltRepo
 img]][AltRepo]
 [LPSC]     [IN2P3]     [UGA] TF2-SOM ======= This is a fast Tensorflow 2
-implementation of the Self Organizing Maps (SOM) running on arbitrarily large
-datasets.  Documentation ============= https://odier-io.github.io/tf2-som/ Demo
-==== [ð Click there](https://github.com/odier-io/tf2-som/blob/master/demo/
-demo.ipynb) Authors ======= - [JÃ©rÃ´me ODIER](https://annuaire.in2p3.fr/4121-
-4467/jerome-odier) ([CNRS/LPSC](https://lpsc.in2p3.fr/)) - [Nora ACHBAK](https:
-//annuaire.in2p3.fr/7591-10426/nora-achbak) ([CNRS/LPSC](https://lpsc.in2p3.fr/
-)) [License]:http://www.cecill.info/licences/Licence_CeCILL-C_V1-en.txt
-[License img]:https://img.shields.io/badge/license-CeCILL--C-blue.svg
-[MainRepo]:https://gitlab.in2p3.fr/jodier/tf2_som [MainRepo img]:https://
-img.shields.io/badge/Main%20Repo-gitlab.in2p3.fr-success [AltRepo]:https://
-github.com/odier-xyz/tf2_som [AltRepo img]:https://img.shields.io/badge/
-Alt%20Repo-github.com-success
+implementation of the Self Organizing Maps (SOM). [som] Documentation
+============= https://odier-io.github.io/tf2-som/ Demo ==== [ð Click there]
+(https://github.com/odier-io/tf2-som/blob/master/demo/demo.ipynb) Authors
+======= - [JÃ©rÃ´me ODIER](https://annuaire.in2p3.fr/4121-4467/jerome-odier) (
+[CNRS/LPSC](https://lpsc.in2p3.fr/)) - [Nora ACHBAK](https://annuaire.in2p3.fr/
+7591-10426/nora-achbak) ([CNRS/LPSC](https://lpsc.in2p3.fr/)) [License]:http://
+www.cecill.info/licences/Licence_CeCILL-C_V1-en.txt [License img]:https://
+img.shields.io/badge/license-CeCILL--C-blue.svg [MainRepo]:https://
+gitlab.in2p3.fr/jodier/tf2_som [MainRepo img]:https://img.shields.io/badge/
+Main%20Repo-gitlab.in2p3.fr-success [AltRepo]:https://github.com/odier-xyz/
+tf2_som [AltRepo img]:https://img.shields.io/badge/Alt%20Repo-github.com-
+success
```

### Comparing `tf2-som-0.0.10/setup.py` & `tf2-som-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tf2-som-0.0.10/tf2_som.egg-info/PKG-INFO` & `tf2-som-0.0.9/tf2_som.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf2-som
-Version: 0.0.10
+Version: 0.0.9
 Summary: Tensorflow 2 implementation of the Self Organizing Maps (SOM)
 Home-page: https://odier-io.github.io/tf2-som/
 Author: Jérôme ODIER, Nora ACHBAK
 Author-email: jerome.odier@lpsc.in2p3.fr, nora.achbak@lpsc.in2p3.fr
 License: CeCILL-C
 Keywords: som,self organizing map,machine learning
 Description-Content-Type: text/markdown
@@ -26,17 +26,17 @@
 <a href="http://www.in2p3.fr/"               target="_blank" style="margin-right: 2rem;"><img src="https://ami.web.cern.ch/images/logo_in2p3.png" alt="IN2P3" height="72" /></a>
 &nbsp;&nbsp;&nbsp;
 <a href="http://www.univ-grenoble-alpes.fr/" target="_blank" style="margin-right: 0rem;"><img src="https://ami.web.cern.ch/images/logo_uga.png" alt="UGA" height="72" /></a>
 
 TF2-SOM
 =======
 
-This is a fast Tensorflow 2 implementation of the Self Organizing Maps (SOM) running on arbitrarily large datasets.
+This is a fast Tensorflow 2 implementation of the Self Organizing Maps (SOM).
 
-<img src="https://odier-io.github.io/tf2-som/som.png" alt="" height="250" />
+<img src="https://odier-xyz.github.io/tf2-som/som.png" alt="som" height="250" />
 
 Documentation
 =============
 
 https://odier-io.github.io/tf2-som/
 
 Demo
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: tf2-som Version: 0.0.10 Summary: Tensorflow 2
+Metadata-Version: 2.1 Name: tf2-som Version: 0.0.9 Summary: Tensorflow 2
 implementation of the Self Organizing Maps (SOM) Home-page: https://odier-
 io.github.io/tf2-som/ Author: JÃ©rÃ´me ODIER, Nora ACHBAK Author-email:
 jerome.odier@lpsc.in2p3.fr, nora.achbak@lpsc.in2p3.fr License: CeCILL-
 C Keywords: som,self organizing map,machine learning Description-Content-Type:
 text/markdown Provides-Extra: pandas Provides-Extra: astropy Provides-Extra:
 matplotlib License-File: LICENSE.md [![][License img]][License]   [![][MainRepo
 img]][MainRepo]   [![][AltRepo img]][AltRepo]
 [LPSC]     [IN2P3]     [UGA] TF2-SOM ======= This is a fast Tensorflow 2
-implementation of the Self Organizing Maps (SOM) running on arbitrarily large
-datasets.  Documentation ============= https://odier-io.github.io/tf2-som/ Demo
-==== [ð Click there](https://github.com/odier-io/tf2-som/blob/master/demo/
-demo.ipynb) Authors ======= - [JÃ©rÃ´me ODIER](https://annuaire.in2p3.fr/4121-
-4467/jerome-odier) ([CNRS/LPSC](https://lpsc.in2p3.fr/)) - [Nora ACHBAK](https:
-//annuaire.in2p3.fr/7591-10426/nora-achbak) ([CNRS/LPSC](https://lpsc.in2p3.fr/
-)) [License]:http://www.cecill.info/licences/Licence_CeCILL-C_V1-en.txt
-[License img]:https://img.shields.io/badge/license-CeCILL--C-blue.svg
-[MainRepo]:https://gitlab.in2p3.fr/jodier/tf2_som [MainRepo img]:https://
-img.shields.io/badge/Main%20Repo-gitlab.in2p3.fr-success [AltRepo]:https://
-github.com/odier-xyz/tf2_som [AltRepo img]:https://img.shields.io/badge/
-Alt%20Repo-github.com-success
+implementation of the Self Organizing Maps (SOM). [som] Documentation
+============= https://odier-io.github.io/tf2-som/ Demo ==== [ð Click there]
+(https://github.com/odier-io/tf2-som/blob/master/demo/demo.ipynb) Authors
+======= - [JÃ©rÃ´me ODIER](https://annuaire.in2p3.fr/4121-4467/jerome-odier) (
+[CNRS/LPSC](https://lpsc.in2p3.fr/)) - [Nora ACHBAK](https://annuaire.in2p3.fr/
+7591-10426/nora-achbak) ([CNRS/LPSC](https://lpsc.in2p3.fr/)) [License]:http://
+www.cecill.info/licences/Licence_CeCILL-C_V1-en.txt [License img]:https://
+img.shields.io/badge/license-CeCILL--C-blue.svg [MainRepo]:https://
+gitlab.in2p3.fr/jodier/tf2_som [MainRepo img]:https://img.shields.io/badge/
+Main%20Repo-gitlab.in2p3.fr-success [AltRepo]:https://github.com/odier-xyz/
+tf2_som [AltRepo img]:https://img.shields.io/badge/Alt%20Repo-github.com-
+success
```

