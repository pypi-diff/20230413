# Comparing `tmp/ccs_fit-0.21.0.tar.gz` & `tmp/ccs_fit-0.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs_fit-0.21.0.tar", max compression
+gzip compressed data, was "ccs_fit-0.21.1.tar", max compression
```

## Comparing `ccs_fit-0.21.0.tar` & `ccs_fit-0.21.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-04-05 14:45:25.736808 ccs_fit-0.21.0/LICENSE
--rw-r--r--   0        0        0     7895 2023-04-05 14:45:25.736808 ccs_fit-0.21.0/README.md
--rw-r--r--   0        0        0     2483 2023-04-05 14:46:16.783775 ccs_fit-0.21.0/pyproject.toml
--rw-r--r--   0        0        0     1027 2023-04-05 14:45:26.848873 ccs_fit-0.21.0/src/ccs_fit/__init__.py
--rw-r--r--   0        0        0     9636 2023-04-05 14:45:26.848873 ccs_fit-0.21.0/src/ccs_fit/ase_calculator/buck.py
--rw-r--r--   0        0        0     7934 2023-04-05 14:45:26.848873 ccs_fit-0.21.0/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
--rw-r--r--   0        0        0    10653 2023-04-05 14:45:26.848873 ccs_fit-0.21.0/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
--rw-r--r--   0        0        0      488 2023-04-05 14:45:26.848873 ccs_fit-0.21.0/src/ccs_fit/common/__init__.py
--rw-r--r--   0        0        0      628 2023-04-05 14:45:26.848873 ccs_fit-0.21.0/src/ccs_fit/common/exceptions.py
--rw-r--r--   0        0        0     1476 2023-04-05 14:45:26.848873 ccs_fit-0.21.0/src/ccs_fit/common/io.py
--rw-r--r--   0        0        0      486 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/common/math/__init__.py
--rw-r--r--   0        0        0     1071 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/common/math/ewald.py
--rw-r--r--   0        0        0     2156 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/common/neighborlist.py
--rw-r--r--   0        0        0      488 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/data/__init__.py
--rw-r--r--   0        0        0      854 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/data/conversion.py
--rw-r--r--   0        0        0      805 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/debugging_tools/timing.py
--rw-r--r--   0        0        0      488 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/fitting/__init__.py
--rw-r--r--   0        0        0    13479 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/fitting/main copy.py
--rw-r--r--   0        0        0    14597 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/fitting/main.py
--rw-r--r--   0        0        0    23883 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/fitting/objective.py
--rw-r--r--   0        0        0    11717 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/fitting/spline_functions.py
--rw-r--r--   0        0        0    20046 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/ppmd_interface/ccs_ppmd.py
--rw-r--r--   0        0        0     6913 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/regression_tool/regression.py
--rw-r--r--   0        0        0      488 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/__init__.py
--rw-r--r--   0        0        0     7361 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_build_db copy.py
--rw-r--r--   0        0        0     7229 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_build_db.py
--rw-r--r--   0        0        0     8555 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_export_FF.py
--rw-r--r--   0        0        0     4155 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_export_sktable.py
--rw-r--r--   0        0        0     8503 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_fetch.py
--rw-r--r--   0        0        0     2537 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_fit.py
--rw-r--r--   0        0        0     6482 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_prune.py
--rw-r--r--   0        0        0     6371 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_validate.py
--rw-r--r--   0        0        0     1784 2023-04-05 14:45:26.852874 ccs_fit-0.21.0/src/ccs_fit/scripts/jsonTotable.py
--rw-r--r--   0        0        0     9120 1970-01-01 00:00:00.000000 ccs_fit-0.21.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-13 09:39:49.098690 ccs_fit-0.21.1/LICENSE
+-rw-r--r--   0        0        0     7895 2023-04-13 09:39:49.098690 ccs_fit-0.21.1/README.md
+-rw-r--r--   0        0        0     2483 2023-04-13 09:40:44.554871 ccs_fit-0.21.1/pyproject.toml
+-rw-r--r--   0        0        0     1027 2023-04-13 09:39:50.266694 ccs_fit-0.21.1/src/ccs_fit/__init__.py
+-rw-r--r--   0        0        0     9636 2023-04-13 09:39:50.266694 ccs_fit-0.21.1/src/ccs_fit/ase_calculator/buck.py
+-rw-r--r--   0        0        0     7934 2023-04-13 09:39:50.266694 ccs_fit-0.21.1/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
+-rw-r--r--   0        0        0    10653 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
+-rw-r--r--   0        0        0      488 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/common/__init__.py
+-rw-r--r--   0        0        0      628 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/common/exceptions.py
+-rw-r--r--   0        0        0     1476 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/common/io.py
+-rw-r--r--   0        0        0      486 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/common/math/__init__.py
+-rw-r--r--   0        0        0     1071 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/common/math/ewald.py
+-rw-r--r--   0        0        0     2156 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/common/neighborlist.py
+-rw-r--r--   0        0        0      488 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/data/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/data/conversion.py
+-rw-r--r--   0        0        0      805 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/debugging_tools/timing.py
+-rw-r--r--   0        0        0      488 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/fitting/__init__.py
+-rw-r--r--   0        0        0    13479 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/fitting/main copy.py
+-rw-r--r--   0        0        0    14597 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/fitting/main.py
+-rw-r--r--   0        0        0    23883 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/fitting/objective.py
+-rw-r--r--   0        0        0    11717 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/fitting/spline_functions.py
+-rw-r--r--   0        0        0    20046 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/ppmd_interface/ccs_ppmd.py
+-rw-r--r--   0        0        0     6913 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/regression_tool/regression.py
+-rw-r--r--   0        0        0      488 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/__init__.py
+-rw-r--r--   0        0        0     7361 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_build_db copy.py
+-rw-r--r--   0        0        0     7229 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_build_db.py
+-rw-r--r--   0        0        0     8555 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_export_FF.py
+-rw-r--r--   0        0        0     4155 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_export_sktable.py
+-rw-r--r--   0        0        0     8503 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_fetch.py
+-rw-r--r--   0        0        0     2537 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_fit.py
+-rw-r--r--   0        0        0     6482 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_prune.py
+-rw-r--r--   0        0        0     6730 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_validate.py
+-rw-r--r--   0        0        0     1784 2023-04-13 09:39:50.270694 ccs_fit-0.21.1/src/ccs_fit/scripts/jsonTotable.py
+-rw-r--r--   0        0        0     9120 1970-01-01 00:00:00.000000 ccs_fit-0.21.1/PKG-INFO
```

### Comparing `ccs_fit-0.21.0/LICENSE` & `ccs_fit-0.21.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/README.md` & `ccs_fit-0.21.1/README.md`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/pyproject.toml` & `ccs_fit-0.21.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ccs_fit"
-version = "0.21.0"
+version = "0.21.1"
 description = "Fitting tools for repulsive two body interactions using curvature constrained splines."
 authors = [
     "Akshay Krishna AK",
     "Jolla Kullgren <jolla.kullgren@kemi.uu.se>",
     "Eddie Wadbro <eddie.wadbro@umu.se>"
     ]
 maintainers = [
```

### Comparing `ccs_fit-0.21.0/src/ccs_fit/__init__.py` & `ccs_fit-0.21.1/src/ccs_fit/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/ase_calculator/buck.py` & `ccs_fit-0.21.1/src/ccs_fit/ase_calculator/buck.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/ase_calculator/ccs_ase_G2B.py` & `ccs_fit-0.21.1/src/ccs_fit/ase_calculator/ccs_ase_G2B.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/ase_calculator/ccs_ase_calculator.py` & `ccs_fit-0.21.1/src/ccs_fit/ase_calculator/ccs_ase_calculator.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/common/exceptions.py` & `ccs_fit-0.21.1/src/ccs_fit/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/common/io.py` & `ccs_fit-0.21.1/src/ccs_fit/common/io.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/common/math/ewald.py` & `ccs_fit-0.21.1/src/ccs_fit/common/math/ewald.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/common/neighborlist.py` & `ccs_fit-0.21.1/src/ccs_fit/common/neighborlist.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/data/conversion.py` & `ccs_fit-0.21.1/src/ccs_fit/data/conversion.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/debugging_tools/timing.py` & `ccs_fit-0.21.1/src/ccs_fit/debugging_tools/timing.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/fitting/main copy.py` & `ccs_fit-0.21.1/src/ccs_fit/fitting/main copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/fitting/main.py` & `ccs_fit-0.21.1/src/ccs_fit/fitting/main.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/fitting/objective.py` & `ccs_fit-0.21.1/src/ccs_fit/fitting/objective.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,15 @@
             two_body_dict["exp_a"] = self.l_twb[k].expcoeffs[0]
             if not isnan(self.l_twb[k].expcoeffs[1]):
                 two_body_dict["exp_b"] = self.l_twb[k].expcoeffs[1]
             else: 
                 print("WARNING: THE EXPONENTIAL FOR PAIR {} IS POORLY RESOLVED, PROCEED WITH CAUTION!".format(self.l_twb[k].name))
                 two_body_dict["exp_b"] = 0
             if not isnan(self.l_twb[k].expcoeffs[2]):
-                two_body_dict["exp_c"] = self.l_twb[k].expcoeffs[1]
+                two_body_dict["exp_c"] = self.l_twb[k].expcoeffs[2]
             else: 
                 two_body_dict["exp_c"] = 0
             if two_body_dict["exp_a"]<0:
                 print("STRONG WARNING: THE EXPONENTIAL WALL IS ACTUALLY ATTRACTIVE!!!!!!!")
             a_values = list(self.l_twb[k].splcoeffs[:, 0])
             a_values.append(0)
             two_body_dict["spl_a"] = a_values
```

### Comparing `ccs_fit-0.21.0/src/ccs_fit/fitting/spline_functions.py` & `ccs_fit-0.21.1/src/ccs_fit/fitting/spline_functions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/ppmd_interface/ccs_ppmd.py` & `ccs_fit-0.21.1/src/ccs_fit/ppmd_interface/ccs_ppmd.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/regression_tool/regression.py` & `ccs_fit-0.21.1/src/ccs_fit/regression_tool/regression.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_build_db copy.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_build_db copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_build_db.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_build_db.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_export_FF.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_export_FF.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_export_sktable.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_export_sktable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_fetch.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_fetch.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_fit.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_fit.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_prune.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_prune.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/ccs_validate.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/ccs_validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             String describing which mode is used, supported modes are:
                 CCS:   CCS_params_file(string) NumberOfSamples(int) DFT.db(string)")
                 CCS+Q: CCS_params_file(string) NumberOfSamples(int) DFT.db(string) charge_dict(string) charge_scaling(bool)")
                 DFTB:  CCS_params_file(string) NumberOfSamples(int) DFT.db(string) DFTB.db(string)")
 
     Returns
     -------
-        What does it return Jolla?
+        To be specified. 
 
     Example usage
     -------------
         ccs_validate MODE [...]
     """
     if os.path.isfile(CCS_DB):
         os.remove(CCS_DB)
@@ -50,19 +50,21 @@
     DFT_DB = db.connect(DFT_DB)
     CCS_DB = db.connect(CCS_DB)
 
     if mode == "DFTB":
         DFTB_DB = db.connect(DFTB_DB)
 
     if isinstance(charge_dict, str):
-        charge_dict = json.loads(charge_dict)
+        charge_dict_orig = json.loads(charge_dict)
+        charge_dict = charge_dict_orig.deepcopy() # Necessary as the dicts act as mutable objects, changes in these functions would change the global dicts, which is not desired
 
     if isinstance(CCS_params, str):
         with open(CCS_params, "r") as f:
-            CCS_params = json.load(f)
+            CCS_params_orig = json.load(f)
+            CCS_params = CCS_params_orig.deepcopy() # Necessary as the dicts act as mutable objects, changes in these functions would change the global dicts, which is not desired
 
     if charge_dict is None:
         charge = False
     else:
         charge = True
 
     f = open("CCS_validate.dat", "w")
```

### Comparing `ccs_fit-0.21.0/src/ccs_fit/scripts/jsonTotable.py` & `ccs_fit-0.21.1/src/ccs_fit/scripts/jsonTotable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.0/PKG-INFO` & `ccs_fit-0.21.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccs-fit
-Version: 0.21.0
+Version: 0.21.1
 Summary: Fitting tools for repulsive two body interactions using curvature constrained splines.
 Home-page: https://github.com/Teoroo-CMC/CCS
 License: GPL-3
 Keywords: Curvature,Constrained,Splines,Two-Body,Interatomic,Repulsive,Fitting
 Author: Akshay Krishna AK
 Maintainer: Jolla Kullgren
 Maintainer-email: jolla.kullgren@kemi.uu.se
```

