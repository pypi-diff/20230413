# Comparing `tmp/flow360-0.2.0b1.tar.gz` & `tmp/flow360-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b1.tar", max compression
+gzip compressed data, was "flow360-0.2.0b2.tar", max compression
```

## Comparing `flow360-0.2.0b1.tar` & `flow360-0.2.0b2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    26526 2023-04-12 14:58:52.250627 flow360-0.2.0b1/LICENSE
--rw-r--r--   0        0        0     1473 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cli/__init__.py
--rw-r--r--   0        0        0     1126 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     2869 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1466 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     8842 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      687 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/__init__.py
--rw-r--r--   0        0        0    22372 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/constants.py
--rw-r--r--   0        0        0    32080 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/flow360_params.py
--rw-r--r--   0        0        0      220 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     6145 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/meshing/params.py
--rw-r--r--   0        0        0    18009 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/params_base.py
--rw-r--r--   0        0        0     7550 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/resource_base.py
--rw-r--r--   0        0        0    10105 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2326 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/types.py
--rw-r--r--   0        0        0     1019 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/utils.py
--rw-r--r--   0        0        0     2940 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/validator.py
--rw-r--r--   0        0        0    21661 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2137 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/environment.py
--rw-r--r--   0        0        0      237 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5515 2023-04-12 14:58:52.254627 flow360-0.2.0b1/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-04-12 14:58:52.258627 flow360-0.2.0b1/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-04-12 14:58:52.262627 flow360-0.2.0b1/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0     2305 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1354 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/exceptions.py
--rw-r--r--   0        0        0     5810 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/solver_version.py
--rw-r--r--   0        0        0       38 2023-04-12 14:58:52.266627 flow360-0.2.0b1/flow360/version.py
--rw-r--r--   0        0        0     1480 2023-04-12 14:59:09.794860 flow360-0.2.0b1/pyproject.toml
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 flow360-0.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-04-13 03:45:55.319405 flow360-0.2.0b2/LICENSE
+-rw-r--r--   0        0        0     1473 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     1126 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     2869 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1466 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     8842 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      687 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/__init__.py
+-rw-r--r--   0        0        0    22372 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/constants.py
+-rw-r--r--   0        0        0    32080 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/flow360_params.py
+-rw-r--r--   0        0        0      220 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     6145 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0    18009 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/params_base.py
+-rw-r--r--   0        0        0     7550 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    10105 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2326 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/types.py
+-rw-r--r--   0        0        0     1019 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/utils.py
+-rw-r--r--   0        0        0     2940 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/validator.py
+-rw-r--r--   0        0        0    21661 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2137 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/environment.py
+-rw-r--r--   0        0        0      237 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5515 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-04-13 03:45:55.327405 flow360-0.2.0b2/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0     2305 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1354 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/exceptions.py
+-rw-r--r--   0        0        0     5810 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/solver_version.py
+-rw-r--r--   0        0        0       38 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/version.py
+-rw-r--r--   0        0        0     1480 2023-04-13 03:46:12.223660 flow360-0.2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 flow360-0.2.0b2/PKG-INFO
```

### Comparing `flow360-0.2.0b1/LICENSE` & `flow360-0.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/__init__.py` & `flow360-0.2.0b2/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/cli/app.py` & `flow360-0.2.0b2/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/cloud/http_util.py` & `flow360-0.2.0b2/flow360/cloud/http_util.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/cloud/rest_api.py` & `flow360-0.2.0b2/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/cloud/s3_utils.py` & `flow360-0.2.0b2/flow360/cloud/s3_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/cloud/security.py` & `flow360-0.2.0b2/flow360/cloud/security.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/case.py` & `flow360-0.2.0b2/flow360/component/case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/flow360_params.py` & `flow360-0.2.0b2/flow360/component/flow360_params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/meshing/params.py` & `flow360-0.2.0b2/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/params_base.py` & `flow360-0.2.0b2/flow360/component/params_base.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/resource_base.py` & `flow360-0.2.0b2/flow360/component/resource_base.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/surface_mesh.py` & `flow360-0.2.0b2/flow360/component/surface_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/types.py` & `flow360-0.2.0b2/flow360/component/types.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/utils.py` & `flow360-0.2.0b2/flow360/component/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/validator.py` & `flow360-0.2.0b2/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/component/volume_mesh.py` & `flow360-0.2.0b2/flow360/component/volume_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/environment.py` & `flow360-0.2.0b2/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b2/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b2/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b2/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b2/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/base_test_case.py` & `flow360-0.2.0b2/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b2/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b2/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b2/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b2/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b2/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/exceptions.py` & `flow360-0.2.0b2/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/log.py` & `flow360-0.2.0b2/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/flow360/solver_version.py` & `flow360-0.2.0b2/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b1/pyproject.toml` & `flow360-0.2.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b1"
+version = "v0.2.0b2"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
```

### Comparing `flow360-0.2.0b1/PKG-INFO` & `flow360-0.2.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b1
+Version: 0.2.0b2
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

