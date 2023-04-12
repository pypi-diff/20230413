# Comparing `tmp/probability_calculator-0.0.1.tar.gz` & `tmp/probability_calculator-0.1.0.tar.gz`

## Comparing `probability_calculator-0.0.1.tar` & `probability_calculator-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 probability_calculator-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 probability_calculator-0.0.1/src/probability-calculator/DiscreteDensity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probability_calculator-0.0.1/src/probability-calculator/__init__.py
--rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 probability_calculator-0.0.1/LICENSE
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 probability_calculator-0.0.1/README.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 probability_calculator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 probability_calculator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/src/probability_calculator/__init__.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/src/probability_calculator/density.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/src/probability_calculator/outcome.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/src/probability_calculator/plot.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/.gitignore
+-rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/LICENSE
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/README.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 probability_calculator-0.1.0/PKG-INFO
```

### Comparing `probability_calculator-0.0.1/LICENSE` & `probability_calculator-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `probability_calculator-0.0.1/pyproject.toml` & `probability_calculator-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "probability-calculator"
-version = "0.0.1"
+name = "probability_calculator"
+version = "0.1.0"
 authors = [
   { name="Hendrik Roehm", email="git@roehm.ws" },
 ]
 description = "Calculate with and analyze probability densities."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -13,12 +13,19 @@
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 3 - Alpha"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/HendrikRoehm/probability-calculator"
+"Homepage" = "https://github.com/HendrikRoehm/probability_calculator"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
+
+[tool.hatch.build]
+exclude = [
+  "/.vscode",
+  "/Makefile",
+  "/tests"
+]
```

### Comparing `probability_calculator-0.0.1/PKG-INFO` & `probability_calculator-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
-Name: probability-calculator
-Version: 0.0.1
+Name: probability_calculator
+Version: 0.1.0
 Summary: Calculate with and analyze probability densities.
-Project-URL: Homepage, https://github.com/HendrikRoehm/probability-calculator
+Project-URL: Homepage, https://github.com/HendrikRoehm/probability_calculator
 Author-email: Hendrik Roehm <git@roehm.ws>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# probability-calculator
+# probability_calculator
 
 Calculate with and analyze probability densities.
 
 More description will be added soon™.
 
 ## Contributing
-We greatly appreciate fixes and new features for [probability-calculator](https://github.com/HendrikRoehm/probability-calculator). All contributions to this project should be sent as pull requests on github.
+We greatly appreciate fixes and new features for [probability_calculator](https://github.com/HendrikRoehm/probability_calculator). All contributions to this project should be sent as pull requests on github.
 
 ## License
 
 [Apache License 2.0](LICENSE)
```

