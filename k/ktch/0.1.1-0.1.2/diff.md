# Comparing `tmp/ktch-0.1.1.tar.gz` & `tmp/ktch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktch-0.1.1.tar", max compression
+gzip compressed data, was "ktch-0.1.2.tar", max compression
```

## Comparing `ktch-0.1.1.tar` & `ktch-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11356 2021-09-20 07:55:48.345883 ktch-0.1.1/LICENSE
--rw-r--r--   0        0        0      185 2022-12-11 04:06:13.956410 ktch-0.1.1/README.md
--rw-r--r--   0        0        0      929 2022-12-11 04:56:13.380102 ktch-0.1.1/ktch/__init__.py
--rw-r--r--   0        0        0     7074 2021-09-21 01:54:32.248280 ktch-0.1.1/ktch/_template.py
--rw-r--r--   0        0        0      597 2021-09-21 01:54:18.848246 ktch-0.1.1/ktch/_version.py
--rw-r--r--   0        0        0      393 2022-08-07 05:12:34.491806 ktch-0.1.1/ktch/datasets/__init__.py
--rw-r--r--   0        0        0     9685 2023-04-08 08:40:42.385256 ktch-0.1.1/ktch/datasets/_base.py
--rw-r--r--   0        0        0        0 2022-12-11 05:38:36.524177 ktch-0.1.1/ktch/datasets/data/__init__.py
--rw-r--r--   0        0        0    46290 2022-08-04 14:54:31.590989 ktch-0.1.1/ktch/datasets/data/data_landmark_mosquito_wings.csv
--rw-r--r--   0        0        0    88299 2022-08-05 14:24:20.181451 ktch-0.1.1/ktch/datasets/data/data_outline_bottles.csv
--rw-r--r--   0        0        0   285403 2022-08-04 15:02:34.740790 ktch-0.1.1/ktch/datasets/data/data_outline_mosquito_wings.csv
--rw-r--r--   0        0        0      799 2022-08-04 14:54:31.592162 ktch-0.1.1/ktch/datasets/data/meta_landmark_mosquito_wings.csv
--rw-r--r--   0        0        0      846 2022-08-05 14:24:29.858660 ktch-0.1.1/ktch/datasets/data/meta_outline_bottles.csv
--rw-r--r--   0        0        0      792 2022-12-28 15:03:59.552650 ktch-0.1.1/ktch/datasets/data/meta_outline_mosquito_wings.csv
--rw-r--r--   0        0        0    18006 2022-08-06 16:19:26.502747 ktch-0.1.1/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv
--rw-r--r--   0        0        0    17900 2022-08-06 16:21:05.211446 ktch-0.1.1/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv
--rw-r--r--   0        0        0        0 2022-12-11 05:38:47.499486 ktch-0.1.1/ktch/datasets/descr/__init__.py
--rw-r--r--   0        0        0       71 2022-08-04 13:17:19.062753 ktch-0.1.1/ktch/datasets/descr/data_landmark_mosquito_wings.rst
--rw-r--r--   0        0        0       68 2022-08-05 14:26:37.531493 ktch-0.1.1/ktch/datasets/descr/data_outline_bottles.rst
--rw-r--r--   0        0        0       68 2022-08-04 15:14:08.538505 ktch-0.1.1/ktch/datasets/descr/data_outline_mosquito_wings.rst
--rw-r--r--   0        0        0     3935 2023-04-08 07:02:24.214041 ktch-0.1.1/ktch/landmark/_Procrustes_analysis.py
--rw-r--r--   0        0        0      835 2023-03-24 02:11:14.247029 ktch-0.1.1/ktch/landmark/__init__.py
--rw-r--r--   0        0        0     3992 2021-09-21 01:54:55.378710 ktch-0.1.1/ktch/landmark/_landmark.py
--rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901541 ktch-0.1.1/ktch/landmark/tests/__init__.py
--rw-r--r--   0        0        0     1213 2023-03-24 03:32:50.549630 ktch-0.1.1/ktch/outline/__init__.py
--rw-r--r--   0        0        0    14088 2023-04-08 15:02:35.382797 ktch-0.1.1/ktch/outline/_elliptic_Fourier_analysis.py
--rw-r--r--   0        0        0      548 2022-08-28 14:14:38.988405 ktch-0.1.1/ktch/outline/_plot/reconstructed_shapes.py
--rw-r--r--   0        0        0     7401 2023-01-07 02:23:20.969778 ktch-0.1.1/ktch/outline/_spherical_harmonic_analysis.py
--rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901733 ktch-0.1.1/ktch/outline/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-04-08 14:46:24.968361 ktch-0.1.1/ktch/outline/tests/test_elliptic_Fourier_analysis.py
--rw-r--r--   0        0        0        0 2021-07-21 14:32:32.343272 ktch-0.1.1/ktch/tests/__init__.py
--rw-r--r--   0        0        0     2313 2023-04-08 15:26:47.810801 ktch-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1519 1970-01-01 00:00:00.000000 ktch-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2021-09-20 07:55:48.345883 ktch-0.1.2/LICENSE
+-rw-r--r--   0        0        0      316 2023-04-13 04:50:43.332584 ktch-0.1.2/README.md
+-rw-r--r--   0        0        0      929 2022-12-11 04:56:13.380102 ktch-0.1.2/ktch/__init__.py
+-rw-r--r--   0        0        0     7074 2021-09-21 01:54:32.248280 ktch-0.1.2/ktch/_template.py
+-rw-r--r--   0        0        0      597 2021-09-21 01:54:18.848246 ktch-0.1.2/ktch/_version.py
+-rw-r--r--   0        0        0      393 2022-08-07 05:12:34.491806 ktch-0.1.2/ktch/datasets/__init__.py
+-rw-r--r--   0        0        0     9685 2023-04-08 08:40:42.385256 ktch-0.1.2/ktch/datasets/_base.py
+-rw-r--r--   0        0        0        0 2022-12-11 05:38:36.524177 ktch-0.1.2/ktch/datasets/data/__init__.py
+-rw-r--r--   0        0        0    46290 2022-08-04 14:54:31.590989 ktch-0.1.2/ktch/datasets/data/data_landmark_mosquito_wings.csv
+-rw-r--r--   0        0        0    88299 2022-08-05 14:24:20.181451 ktch-0.1.2/ktch/datasets/data/data_outline_bottles.csv
+-rw-r--r--   0        0        0   285403 2022-08-04 15:02:34.740790 ktch-0.1.2/ktch/datasets/data/data_outline_mosquito_wings.csv
+-rw-r--r--   0        0        0      799 2022-08-04 14:54:31.592162 ktch-0.1.2/ktch/datasets/data/meta_landmark_mosquito_wings.csv
+-rw-r--r--   0        0        0      846 2022-08-05 14:24:29.858660 ktch-0.1.2/ktch/datasets/data/meta_outline_bottles.csv
+-rw-r--r--   0        0        0      792 2022-12-28 15:03:59.552650 ktch-0.1.2/ktch/datasets/data/meta_outline_mosquito_wings.csv
+-rw-r--r--   0        0        0    18006 2022-08-06 16:19:26.502747 ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv
+-rw-r--r--   0        0        0    17900 2022-08-06 16:21:05.211446 ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv
+-rw-r--r--   0        0        0        0 2022-12-11 05:38:47.499486 ktch-0.1.2/ktch/datasets/descr/__init__.py
+-rw-r--r--   0        0        0       71 2022-08-04 13:17:19.062753 ktch-0.1.2/ktch/datasets/descr/data_landmark_mosquito_wings.rst
+-rw-r--r--   0        0        0       68 2022-08-05 14:26:37.531493 ktch-0.1.2/ktch/datasets/descr/data_outline_bottles.rst
+-rw-r--r--   0        0        0       68 2022-08-04 15:14:08.538505 ktch-0.1.2/ktch/datasets/descr/data_outline_mosquito_wings.rst
+-rw-r--r--   0        0        0     3935 2023-04-08 07:02:24.214041 ktch-0.1.2/ktch/landmark/_Procrustes_analysis.py
+-rw-r--r--   0        0        0      835 2023-03-24 02:11:14.247029 ktch-0.1.2/ktch/landmark/__init__.py
+-rw-r--r--   0        0        0     3992 2021-09-21 01:54:55.378710 ktch-0.1.2/ktch/landmark/_landmark.py
+-rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901541 ktch-0.1.2/ktch/landmark/tests/__init__.py
+-rw-r--r--   0        0        0     1213 2023-03-24 03:32:50.549630 ktch-0.1.2/ktch/outline/__init__.py
+-rw-r--r--   0        0        0    14124 2023-04-13 04:50:43.333810 ktch-0.1.2/ktch/outline/_elliptic_Fourier_analysis.py
+-rw-r--r--   0        0        0      548 2022-08-28 14:14:38.988405 ktch-0.1.2/ktch/outline/_plot/reconstructed_shapes.py
+-rw-r--r--   0        0        0     7401 2023-01-07 02:23:20.969778 ktch-0.1.2/ktch/outline/_spherical_harmonic_analysis.py
+-rw-r--r--   0        0        0        0 2022-01-15 09:33:16.901733 ktch-0.1.2/ktch/outline/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-08 14:46:24.968361 ktch-0.1.2/ktch/outline/tests/test_elliptic_Fourier_analysis.py
+-rw-r--r--   0        0        0        0 2021-07-21 14:32:32.343272 ktch-0.1.2/ktch/tests/__init__.py
+-rw-r--r--   0        0        0     2313 2023-04-13 04:51:27.590332 ktch-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 ktch-0.1.2/PKG-INFO
```

### Comparing `ktch-0.1.1/LICENSE` & `ktch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/__init__.py` & `ktch-0.1.2/ktch/__init__.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/_template.py` & `ktch-0.1.2/ktch/_template.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/_version.py` & `ktch-0.1.2/ktch/_version.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/_base.py` & `ktch-0.1.2/ktch/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/data_landmark_mosquito_wings.csv` & `ktch-0.1.2/ktch/datasets/data/data_landmark_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/data_outline_bottles.csv` & `ktch-0.1.2/ktch/datasets/data/data_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/data_outline_mosquito_wings.csv` & `ktch-0.1.2/ktch/datasets/data/data_outline_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/meta_landmark_mosquito_wings.csv` & `ktch-0.1.2/ktch/datasets/data/meta_landmark_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/meta_outline_bottles.csv` & `ktch-0.1.2/ktch/datasets/data/meta_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/meta_outline_mosquito_wings.csv` & `ktch-0.1.2/ktch/datasets/data/meta_outline_mosquito_wings.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv` & `ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_false_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv` & `ktch-0.1.2/ktch/datasets/data/test_coef_nharm_6_norm_true_outline_bottles.csv`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/landmark/_Procrustes_analysis.py` & `ktch-0.1.2/ktch/landmark/_Procrustes_analysis.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/landmark/__init__.py` & `ktch-0.1.2/ktch/landmark/__init__.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/landmark/_landmark.py` & `ktch-0.1.2/ktch/landmark/_landmark.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/outline/__init__.py` & `ktch-0.1.2/ktch/outline/__init__.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/outline/_elliptic_Fourier_analysis.py` & `ktch-0.1.2/ktch/outline/_elliptic_Fourier_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
 from typing import Literal
 
 from operator import index
 import numpy as np
 import numpy.typing as npt
 import scipy as sp
```

### Comparing `ktch-0.1.1/ktch/outline/_plot/reconstructed_shapes.py` & `ktch-0.1.2/ktch/outline/_plot/reconstructed_shapes.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/outline/_spherical_harmonic_analysis.py` & `ktch-0.1.2/ktch/outline/_spherical_harmonic_analysis.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/ktch/outline/tests/test_elliptic_Fourier_analysis.py` & `ktch-0.1.2/ktch/outline/tests/test_elliptic_Fourier_analysis.py`

 * *Files identical despite different names*

### Comparing `ktch-0.1.1/pyproject.toml` & `ktch-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 description = "**ktch** is a python package for model-based morphometrics."
 homepage = "https://doc.ktch.dev/index.html"
 keywords = ["morphometrics", "theoretical morphology"]
 license = "Apache-2.0"
 name = "ktch"
 readme = "README.md"
 repository = "https://github.com/noshita/ktch"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 numpy = "^1.22"
 pandas = "^1.4"
 python = ">= 3.8, < 3.12"
 scikit-learn = "^1.2"
 scipy = "^1.8"
```

### Comparing `ktch-0.1.1/PKG-INFO` & `ktch-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktch
-Version: 0.1.1
+Version: 0.1.2
 Summary: **ktch** is a python package for model-based morphometrics.
 Home-page: https://doc.ktch.dev/index.html
 License: Apache-2.0
 Keywords: morphometrics,theoretical morphology
 Author: Noshita, Koji
 Author-email: noshita@morphometrics.jp
 Requires-Python: >=3.8,<3.12
@@ -30,14 +30,16 @@
 Requires-Dist: scikit-learn (>=1.2,<2.0)
 Requires-Dist: scipy (>=1.8,<2.0)
 Project-URL: Repository, https://github.com/noshita/ktch
 Description-Content-Type: text/markdown
 
 # ktch - A python package for model-based morphometrics
 
+[![codecov](https://codecov.io/gh/noshita/ktch/branch/main/graph/badge.svg?token=SJN66K7KJY)](https://codecov.io/gh/noshita/ktch)
+
 **ktch** is a python package for model-based morphometrics.
 
 
 ## License
 
 ktch is licensed under the Apache License, Version2.0
```

