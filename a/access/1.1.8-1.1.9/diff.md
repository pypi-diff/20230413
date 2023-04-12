# Comparing `tmp/access-1.1.8.tar.gz` & `tmp/access-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access-1.1.8.tar", last modified: Sat Jun  4 20:15:29 2022, max compression
+gzip compressed data, was "access-1.1.9.tar", last modified: Wed Apr 12 23:51:22 2023, max compression
```

## Comparing `access-1.1.8.tar` & `access-1.1.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 20:15:29.623121 access-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-06-04 20:14:56.000000 access-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-06-04 20:14:56.000000 access-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-06-04 20:15:29.623121 access-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-04 20:14:56.000000 access-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 20:15:29.619120 access-1.1.8/access/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-04 20:14:56.000000 access-1.1.8/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    72980 2022-06-04 20:14:56.000000 access-1.1.8/access/access.py
--rw-r--r--   0 runner    (1001) docker     (121)     2236 2022-06-04 20:14:56.000000 access-1.1.8/access/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)    18812 2022-06-04 20:14:56.000000 access-1.1.8/access/fca.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-06-04 20:14:56.000000 access-1.1.8/access/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7430 2022-06-04 20:14:56.000000 access-1.1.8/access/raam.py
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-06-04 20:14:56.000000 access-1.1.8/access/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 20:15:29.623121 access-1.1.8/access.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-06-04 20:15:29.000000 access-1.1.8/access.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-06-04 20:15:29.000000 access-1.1.8/access.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 20:15:29.000000 access-1.1.8/access.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 20:15:29.000000 access-1.1.8/access.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-06-04 20:15:29.000000 access-1.1.8/access.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-04 20:15:29.000000 access-1.1.8/access.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-04 20:14:56.000000 access-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-04 20:14:56.000000 access-1.1.8/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-04 20:14:56.000000 access-1.1.8/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-04 20:15:29.623121 access-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-06-04 20:14:56.000000 access-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:51:22.211968 access-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 23:50:43.000000 access-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 23:50:43.000000 access-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-12 23:51:22.211968 access-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-12 23:50:43.000000 access-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:51:22.211968 access-1.1.9/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 23:50:43.000000 access-1.1.9/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 23:51:22.211968 access-1.1.9/access/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73300 2023-04-12 23:50:43.000000 access-1.1.9/access/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-12 23:50:43.000000 access-1.1.9/access/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-04-12 23:50:43.000000 access-1.1.9/access/fca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-12 23:50:43.000000 access-1.1.9/access/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-12 23:50:43.000000 access-1.1.9/access/raam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-12 23:50:43.000000 access-1.1.9/access/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:51:22.211968 access-1.1.9/access.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-12 23:51:22.000000 access-1.1.9/access.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 23:51:22.000000 access-1.1.9/access.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:51:22.000000 access-1.1.9/access.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:51:22.000000 access-1.1.9/access.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 23:51:22.000000 access-1.1.9/access.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 23:51:22.000000 access-1.1.9/access.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 23:50:43.000000 access-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 23:50:43.000000 access-1.1.9/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 23:50:43.000000 access-1.1.9/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 23:51:22.211968 access-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-12 23:50:43.000000 access-1.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-12 23:50:43.000000 access-1.1.9/versioneer.py
```

### Comparing `access-1.1.8/LICENSE` & `access-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `access-1.1.8/PKG-INFO` & `access-1.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: access
-Version: 1.1.8
+Version: 1.1.9
 Summary: Calculate spatial accessibility metrics.
 Home-page: https://access.readthedocs.io/en/latest/
 Maintainer: James Saxon
 Maintainer-email: jsaxon@uchicago.edu
 License: 3-Clause BSD
 Keywords: spatial statistics access
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: BSD License
@@ -23,13 +22,14 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # Spatial Access
 
-This package provides classical and novel measures of spatial accessibility to services.
-
-For full documentation, see [access.readthedocs.io](https://access.readthedocs.io/en/latest/).
-
+![tag](https://img.shields.io/github/v/release/pysal/access?include_prereleases&sort=semver)
+[![Documentation](https://img.shields.io/static/v1.svg?label=docs&message=current&color=9cf)](http://pysal.org/access/)
+[![Continuous Integration](https://github.com/pysal/access/actions/workflows/unittests.yml/badge.svg)](https://github.com/pysal/access/actions/workflows/unittests.yml)
 
+This package provides classical and novel measures of spatial accessibility to services.
 
+For full documentation, see [here](https://pysal.org/access/).
```

### Comparing `access-1.1.8/access/access.py` & `access-1.1.9/access/access.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from . import fca
 from . import raam
 from . import weights
 from . import helpers
 from .datasets import Datasets
 
 access_log_stream = logging.StreamHandler()
-access_log_format = logging.Formatter('%(name)s %(levelname)-8s :: %(message)s')
+access_log_format = logging.Formatter("%(name)s %(levelname)-8s :: %(message)s")
 access_log_stream.setFormatter(access_log_format)
 
-class Access():
+
+class Access:
     """
     Spatial Access Class
 
     Parameters
     ----------
     demand_df            : `pandas.DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`_ or `geopandas.GeoDataFrame <http://geopandas.org/reference/geopandas.GeoDataFrame.html>`_
                            The origins dataframe, containing a location index and, optionally, a level of demand and geometry.
@@ -59,18 +60,31 @@
                            Lists currently-available measures of access.
     cost_metadata        : pandas.DataFrame
                            Describes each of the currently-available supply to demand costs.
     """
 
     logger_initialized = False
 
-    def __init__(self, demand_df, demand_value, supply_df, supply_value=False,
-                 demand_index = True, supply_index = True,
-                 cost_df = None, cost_origin = None, cost_dest = None, cost_name = None,
-                 neighbor_cost_df = None, neighbor_cost_origin = None, neighbor_cost_dest = None, neighbor_cost_name = None):
+    def __init__(
+        self,
+        demand_df,
+        demand_value,
+        supply_df,
+        supply_value=False,
+        demand_index=True,
+        supply_index=True,
+        cost_df=None,
+        cost_origin=None,
+        cost_dest=None,
+        cost_name=None,
+        neighbor_cost_df=None,
+        neighbor_cost_origin=None,
+        neighbor_cost_dest=None,
+        neighbor_cost_name=None,
+    ):
 
         """
         Initialize the class.
 
         Examples
         --------
 
@@ -126,149 +140,175 @@
             Access.logger_initialized = True
 
         self.supply_value_provided = True
 
         ### First all the dummy checks...
 
         if demand_index is not True and demand_index not in demand_df.columns:
-            raise ValueError("demand_index must either be True -- or it must be a column of demand_df")
+            raise ValueError(
+                "demand_index must either be True -- or it must be a column of demand_df"
+            )
 
         if demand_value not in demand_df.columns:
-            raise ValueError("demand_value must either be True -- or it must be a column of demand_df")
+            raise ValueError(
+                "demand_value must either be True -- or it must be a column of demand_df"
+            )
 
         if supply_index is not True and supply_index not in supply_df.columns:
-            raise ValueError("supply_index must either be True -- or it must be a column of supply_df")
+            raise ValueError(
+                "supply_index must either be True -- or it must be a column of supply_df"
+            )
 
         if type(supply_value) is str and supply_value not in supply_df.columns:
             raise ValueError("supply_value must be a column of supply_df")
 
         if type(supply_value) is list:
             if any([sv not in supply_df.columns for sv in supply_value]):
                 raise ValueError("supply_value must be columns of supply_df")
 
         if cost_df is not None:
 
-          if cost_origin not in cost_df.columns:
-              raise ValueError("cost_origin must be a column of cost_df")
+            if cost_origin not in cost_df.columns:
+                raise ValueError("cost_origin must be a column of cost_df")
 
-          if cost_dest   not in cost_df.columns:
-              raise ValueError("cost_dest must be a column of cost_df")
+            if cost_dest not in cost_df.columns:
+                raise ValueError("cost_dest must be a column of cost_df")
 
-          if type(cost_name) is str and cost_name not in cost_df.columns:
-              raise ValueError("cost_name must be a column of cost_df")
+            if type(cost_name) is str and cost_name not in cost_df.columns:
+                raise ValueError("cost_name must be a column of cost_df")
 
-          if type(cost_name) is list:
-              if any([cn not in cost_df.columns for cn in cost_name]):
-                  raise ValueError("cost_name must be columns of cost_df")
+            if type(cost_name) is list:
+                if any([cn not in cost_df.columns for cn in cost_name]):
+                    raise ValueError("cost_name must be columns of cost_df")
 
         if neighbor_cost_df is not None:
 
-          if neighbor_cost_origin not in neighbor_cost_df.columns:
-              raise ValueError("neighbor_cost_origin must be a column of neighbor_cost_df")
-
-          if neighbor_cost_dest   not in neighbor_cost_df.columns:
-              raise ValueError("neighbor_cost_dest must be a column of neighbor_cost_df")
-
-          if type(neighbor_cost_name) is str and neighbor_cost_name not in neighbor_cost_df.columns:
-              raise ValueError("neighbor_cost_name must be a column of cost_df")
-
-          if type(neighbor_cost_name) is list:
-              if any([cn not in neighbor_cost_df.columns for cn in neighbor_cost_name]):
-                  raise ValueError("neighbor_cost_names must be columns of cost_df")
-
+            if neighbor_cost_origin not in neighbor_cost_df.columns:
+                raise ValueError(
+                    "neighbor_cost_origin must be a column of neighbor_cost_df"
+                )
+
+            if neighbor_cost_dest not in neighbor_cost_df.columns:
+                raise ValueError(
+                    "neighbor_cost_dest must be a column of neighbor_cost_df"
+                )
+
+            if (
+                type(neighbor_cost_name) is str
+                and neighbor_cost_name not in neighbor_cost_df.columns
+            ):
+                raise ValueError("neighbor_cost_name must be a column of cost_df")
+
+            if type(neighbor_cost_name) is list:
+                if any(
+                    [cn not in neighbor_cost_df.columns for cn in neighbor_cost_name]
+                ):
+                    raise ValueError("neighbor_cost_names must be columns of cost_df")
 
         ### Now load the demand DFs.
 
-        self.demand_df    = demand_df.copy()
+        self.demand_df = demand_df.copy()
         self.demand_value = demand_value
         if demand_index is not True:
-            self.demand_df.set_index(demand_index, inplace = True)
+            self.demand_df.set_index(demand_index, inplace=True)
 
         ### And now the supply DFs.
 
-        self.supply_df    = supply_df.copy()
+        self.supply_df = supply_df.copy()
 
         if supply_value == False:
-            self.log.info('''Warning: A supply value was not provided, so a default
+            self.log.info(
+                """Warning: A supply value was not provided, so a default
                              supply value of 1 was created in the column named "value".
                              Note that without a supply value, you cannot use any of the
-                             floating catchment area methods.''')
+                             floating catchment area methods."""
+            )
             self.supply_value_provided = False
-            supply_value = 'value'
+            supply_value = "value"
             self.supply_df[supply_value] = 1
 
         if type(supply_value) is str:
             self.supply_types = [supply_value]
         elif type(supply_value) is list:
             self.supply_types = supply_value
         else:
             raise ValueError("supply_value must be string or list of strings.")
 
         if supply_index is not True:
-            self.supply_df.set_index(supply_index, inplace = True)
+            self.supply_df.set_index(supply_index, inplace=True)
 
         if cost_df is not None:
 
-            self.cost_df     = cost_df
+            self.cost_df = cost_df
             self.cost_origin = cost_origin
-            self.cost_dest   = cost_dest
+            self.cost_dest = cost_dest
 
             if type(cost_name) is str:
                 self.cost_names = [cost_name]
 
             elif type(cost_name) is list:
                 self.cost_names = cost_name
 
             else:
                 raise ValueError("cost_name must be string or list of strings.")
 
             self._default_cost = self.cost_names[0]
 
         else:
-            self.cost_df = pd.DataFrame(columns = ['origin', 'dest'])
-            self.cost_origin = 'origin'
-            self.cost_dest = 'dest'
+            self.cost_df = pd.DataFrame(columns=["origin", "dest"])
+            self.cost_origin = "origin"
+            self.cost_dest = "dest"
             self.cost_names = []
 
         if neighbor_cost_df is not None:
 
-            self.neighbor_cost_df     = neighbor_cost_df
+            self.neighbor_cost_df = neighbor_cost_df
             self.neighbor_cost_origin = neighbor_cost_origin
-            self.neighbor_cost_dest   = neighbor_cost_dest
-            self.neighbor_cost_name   = neighbor_cost_name
+            self.neighbor_cost_dest = neighbor_cost_dest
+            self.neighbor_cost_name = neighbor_cost_name
 
             if type(neighbor_cost_name) is str:
                 self.neighbor_cost_names = [neighbor_cost_name]
 
             elif type(neighbor_cost_name) is list:
                 self.neighbor_cost_names = neighbor_cost_name
 
             else:
-                raise ValueError("neighbor_cost_name must be string or list of strings.")
+                raise ValueError(
+                    "neighbor_cost_name must be string or list of strings."
+                )
 
             self._neighbor_default_cost = self.neighbor_cost_names[0]
 
         else:
-            self.neighbor_cost_df = pd.DataFrame(columns = ['origin', 'dest'])
-            self.neighbor_cost_origin = 'origin'
-            self.neighbor_cost_dest = 'dest'
+            self.neighbor_cost_df = pd.DataFrame(columns=["origin", "dest"])
+            self.neighbor_cost_origin = "origin"
+            self.neighbor_cost_dest = "dest"
             self.neighbor_cost_names = []
 
         self.access_df = self.demand_df[[self.demand_value]].sort_index()
 
-        self.access = pd.DataFrame(index = self.supply_df.index)
+        self.access = pd.DataFrame(index=self.supply_df.index)
 
-        self.access_metadata = pd.DataFrame(columns = ["name", "distance", "function", "descriptor"])
-        self.cost_metadata   = pd.DataFrame(columns = ["name", "type", "descriptor"])
+        self.access_metadata = pd.DataFrame(
+            columns=["name", "distance", "function", "descriptor"]
+        )
+        self.cost_metadata = pd.DataFrame(columns=["name", "type", "descriptor"])
 
         return
 
-
-    def weighted_catchment(self, name = "catchment", supply_cost = None, supply_values = None,
-                           weight_fn = None, max_cost = None, normalize = False):
+    def weighted_catchment(
+        self,
+        name="catchment",
+        supply_cost=None,
+        supply_values=None,
+        weight_fn=None,
+        max_cost=None,
+        normalize=False,
+    ):
         """
         Calculate the catchment area (buffer) aggregate access score.
 
         Parameters
         ----------
         name                : str
                               Column name for access values
@@ -301,44 +341,57 @@
         Call the floating catchment area with max_cost only
 
         >>> gravity = weights.gravity(scale = 60, alpha = -1)
         >>> illinois_primary_care.weighted_catchment(weight_fn = gravity)
 
         """
 
-        supply_cost   = helpers.sanitize_supply_cost(self, supply_cost, name)
-        supply_values = helpers.sanitize_supplies   (self, supply_values)
+        supply_cost = helpers.sanitize_supply_cost(self, supply_cost, name)
+        supply_values = helpers.sanitize_supplies(self, supply_values)
 
         for s in supply_values:
 
             # Bryan consistently flipped origin and destination in this one -- very confusing.
-            series = fca.weighted_catchment(loc_df = self.supply_df, loc_index = True, loc_value = s,
-                                            cost_df = self.cost_df, cost_source = self.cost_dest,
-                                            cost_dest = self.cost_origin, cost_cost= self._default_cost,
-                                            weight_fn = weight_fn, max_cost = max_cost)
+            series = fca.weighted_catchment(
+                loc_df=self.supply_df,
+                loc_index=True,
+                loc_value=s,
+                cost_df=self.cost_df,
+                cost_source=self.cost_dest,
+                cost_dest=self.cost_origin,
+                cost_cost=self._default_cost,
+                weight_fn=weight_fn,
+                max_cost=max_cost,
+            )
 
             series.name = name + "_" + s
             if series.name in self.access_df.columns:
                 self.log.info("Overwriting {}.".format(series.name))
-                self.access_df.drop(series.name, axis = 1, inplace = True)
+                self.access_df.drop(series.name, axis=1, inplace=True)
 
             # store the raw, un-normalized access values
             self.access_df = self.access_df.join(series)
 
         if normalize:
 
             columns = [name + "_" + s for s in supply_values]
             return helpers.normalized_access(self, columns)
 
-        return self.access_df.filter(regex = "^" + name, axis = 1)
-
+        return self.access_df.filter(regex="^" + name, axis=1)
 
-    def fca_ratio(self, name = "fca", demand_cost = None, supply_cost = None,
-                  supply_values = None, max_cost = None, normalize = False,
-                  noise = 'quiet'):
+    def fca_ratio(
+        self,
+        name="fca",
+        demand_cost=None,
+        supply_cost=None,
+        supply_values=None,
+        max_cost=None,
+        normalize=False,
+        noise="quiet",
+    ):
         """
         Calculate the floating catchment area (buffer) ratio access score.
 
         Parameters
         ----------
         name                : str
                               Column name for access values
@@ -416,54 +469,73 @@
         17031010202  0.001521     0.000908
         ...........  ........     ........
         17197884101  0.000437     0.000442
         17197884103  0.000510     0.000498
         17197980100  0.000488     0.000432
         """
 
-        assert self.supply_value_provided == True, "You must provide a supply value in order to use this functionality."
-
-        supply_cost   = helpers.sanitize_supply_cost(self, supply_cost, name)
-        demand_cost   = helpers.sanitize_demand_cost(self, demand_cost, name)
-        supply_values = helpers.sanitize_supplies   (self, supply_values)
+        assert (
+            self.supply_value_provided == True
+        ), "You must provide a supply value in order to use this functionality."
+
+        supply_cost = helpers.sanitize_supply_cost(self, supply_cost, name)
+        demand_cost = helpers.sanitize_demand_cost(self, demand_cost, name)
+        supply_values = helpers.sanitize_supplies(self, supply_values)
 
         for s in supply_values:
 
-            series = fca.fca_ratio(demand_df = self.demand_df,
-                                   demand_index = self.demand_df.index.name,
-                                   demand_name = self.demand_value,
-                                   supply_df = self.supply_df,
-                                   supply_index = self.supply_df.index.name,
-                                   supply_name = s,
-                                   demand_cost_df = self.neighbor_cost_df,
-                                   supply_cost_df = self.cost_df,
-                                   demand_cost_origin = self.neighbor_cost_origin, demand_cost_dest = self.neighbor_cost_dest, demand_cost_name = demand_cost,
-                                   supply_cost_origin = self.cost_origin,          supply_cost_dest = self.cost_dest,          supply_cost_name = supply_cost,
-                                   max_cost = max_cost, normalize = normalize, noise = noise)
+            series = fca.fca_ratio(
+                demand_df=self.demand_df,
+                demand_index=self.demand_df.index.name,
+                demand_name=self.demand_value,
+                supply_df=self.supply_df,
+                supply_index=self.supply_df.index.name,
+                supply_name=s,
+                demand_cost_df=self.neighbor_cost_df,
+                supply_cost_df=self.cost_df,
+                demand_cost_origin=self.neighbor_cost_origin,
+                demand_cost_dest=self.neighbor_cost_dest,
+                demand_cost_name=demand_cost,
+                supply_cost_origin=self.cost_origin,
+                supply_cost_dest=self.cost_dest,
+                supply_cost_name=supply_cost,
+                max_cost=max_cost,
+                normalize=normalize,
+                noise=noise,
+            )
 
             series.name = name + "_" + s
             if series.name in self.access_df.columns:
                 self.log.info("Overwriting {}.".format(series.name))
-                self.access_df.drop(series.name, axis = 1, inplace = True)
+                self.access_df.drop(series.name, axis=1, inplace=True)
 
             # store the raw, un-normalized access values
             self.access_df = self.access_df.join(series)
 
         if normalize:
 
             columns = [name + "_" + s for s in supply_values]
             return helpers.normalized_access(self, columns)
 
-        return self.access_df.filter(regex = "^" + name, axis = 1)
-
+        return self.access_df.filter(regex="^" + name, axis=1)
 
-    def raam(self, name = "raam", cost = None, supply_values = None, normalize = False,
-             tau = 60, rho = None,
-             max_cycles = 150, initial_step = 0.2, half_life = 50, min_step = 0.005,
-             verbose = False):
+    def raam(
+        self,
+        name="raam",
+        cost=None,
+        supply_values=None,
+        normalize=False,
+        tau=60,
+        rho=None,
+        max_cycles=150,
+        initial_step=0.2,
+        half_life=50,
+        min_step=0.005,
+        verbose=False,
+    ):
         """Calculate the rational agent access model. :cite:`2019_saxon_snow_raam`
 
         Parameters
         ----------
         name                : str
                               Column name for access values
         cost                : str
@@ -587,50 +659,63 @@
         If euclidean costs are available (see :meth:`Access.access.create_euclidean_distance`),
         you can use euclidean distance instead of time to calculate RAAM access measures. Insted of being measured in minutes, tau would now be measured in meters.
 
         >>> chicago_primary_care.raam(name = "raam_euclidean", tau = 100, cost = "euclidean")
 
         """
 
-        assert self.supply_value_provided == True, "You must provide a supply value in order to use this functionality."
+        assert (
+            self.supply_value_provided == True
+        ), "You must provide a supply value in order to use this functionality."
 
-        cost          = helpers.sanitize_supply_cost(self, cost, name)
-        supply_values = helpers.sanitize_supplies   (self, supply_values)
+        cost = helpers.sanitize_supply_cost(self, cost, name)
+        supply_values = helpers.sanitize_supplies(self, supply_values)
 
         for s in supply_values:
 
-            raam_costs = raam.raam(demand_df = self.demand_df, supply_df = self.supply_df, cost_df = self.cost_df,
-                                   demand_name = self.demand_value,
-                                   supply_name = s,
-                                   cost_origin = self.cost_origin, cost_dest = self.cost_dest, cost_name = cost,
-                                   max_cycles = max_cycles,
-                                   tau = tau,
-                                   verbose = verbose,
-                                   initial_step = initial_step,
-                                   min_step = min_step)
+            raam_costs = raam.raam(
+                demand_df=self.demand_df,
+                supply_df=self.supply_df,
+                cost_df=self.cost_df,
+                demand_name=self.demand_value,
+                supply_name=s,
+                cost_origin=self.cost_origin,
+                cost_dest=self.cost_dest,
+                cost_name=cost,
+                max_cycles=max_cycles,
+                tau=tau,
+                verbose=verbose,
+                initial_step=initial_step,
+                min_step=min_step,
+            )
 
             raam_costs.name = name + "_" + s
             if raam_costs.name in self.access_df.columns:
                 self.log.info("Overwriting {}.".format(raam_costs.name))
-                self.access_df.drop(raam_costs.name, axis = 1, inplace = True)
+                self.access_df.drop(raam_costs.name, axis=1, inplace=True)
 
             # store the raw, un-normalized access values
             self.access_df = self.access_df.join(raam_costs)
 
         if normalize:
 
             columns = [name + "_" + s for s in supply_values]
             return helpers.normalized_access(self, columns)
 
+        return self.access_df.filter(regex="^" + name, axis=1)
 
-        return self.access_df.filter(regex = "^" + name, axis = 1)
-
-
-    def two_stage_fca(self, name = "2sfca", cost = None, max_cost = None,
-                      supply_values = None, weight_fn = None, normalize = False):
+    def two_stage_fca(
+        self,
+        name="2sfca",
+        cost=None,
+        max_cost=None,
+        supply_values=None,
+        weight_fn=None,
+        normalize=False,
+    ):
         """Calculate the two-stage floating catchment area access score.
         Note that while the 'traditional' 2SFCA method does not weight inputs,
         most modern implementations do, and `weight_fn` is allowed as an argument.
 
         Parameters
         ----------
         name                : str
@@ -732,15 +817,17 @@
         17031010100  4854   0.000697       0.000402     0.000963         0.000479
         17031010201  6450   0.000754       0.000455     0.000991         0.000551
         17031010202  2818   0.000717       0.000424     0.000973         0.000541
         17197884103  2776   0.000384       0.000291     0.000371         0.000377
         17197980100  3264   0.000457       0.000325     0.000348         0.000314
         """
 
-        assert self.supply_value_provided == True, "You must provide a supply value in order to use this functionality."
+        assert (
+            self.supply_value_provided == True
+        ), "You must provide a supply value in order to use this functionality."
 
         if cost is None:
 
             cost = self._default_cost
             if len(self.cost_names) > 1:
                 self.log.info("Using default cost, {}, for {}.".format(cost, name))
 
@@ -751,41 +838,53 @@
         if type(supply_values) is str:
             supply_values = [supply_values]
         if supply_values is None:
             supply_values = self.supply_types
 
         for s in supply_values:
 
-            series = fca.two_stage_fca(demand_df = self.demand_df,
-                                       demand_index = self.demand_df.index.name,
-                                       demand_name = self.demand_value,
-                                       supply_df = self.supply_df,
-                                       supply_index = self.supply_df.index.name,
-                                       supply_name = s,
-                                       cost_df = self.cost_df,
-                                       cost_origin = self.cost_origin, cost_dest = self.cost_dest, cost_name = cost,
-                                       max_cost = max_cost, weight_fn = weight_fn, normalize = normalize)
+            series = fca.two_stage_fca(
+                demand_df=self.demand_df,
+                demand_index=self.demand_df.index.name,
+                demand_name=self.demand_value,
+                supply_df=self.supply_df,
+                supply_index=self.supply_df.index.name,
+                supply_name=s,
+                cost_df=self.cost_df,
+                cost_origin=self.cost_origin,
+                cost_dest=self.cost_dest,
+                cost_name=cost,
+                max_cost=max_cost,
+                weight_fn=weight_fn,
+                normalize=normalize,
+            )
 
             series.name = name + "_" + s
             if series.name in self.access_df.columns:
                 self.log.info("Overwriting {}.".format(series.name))
-                self.access_df.drop(series.name, axis = 1, inplace = True)
+                self.access_df.drop(series.name, axis=1, inplace=True)
 
             self.access_df = self.access_df.join(series)
 
         if normalize:
 
             columns = [name + "_" + s for s in supply_values]
             return helpers.normalized_access(self, columns)
 
-        return self.access_df.filter(regex = "^" + name, axis = 1)
+        return self.access_df.filter(regex="^" + name, axis=1)
 
-
-    def enhanced_two_stage_fca(self, name = "e2sfca", cost = None, supply_values = None,
-                               max_cost = None, weight_fn = None, normalize = False):
+    def enhanced_two_stage_fca(
+        self,
+        name="e2sfca",
+        cost=None,
+        supply_values=None,
+        max_cost=None,
+        weight_fn=None,
+        normalize=False,
+    ):
         """Calculate the enhanced two-stage floating catchment area access score.
         Note that the only 'practical' difference between this function and the
         :meth:`Access.access.two_stage_fca` is that the weight function from the original paper,
         `weights.step_fn({10 : 1, 20 : 0.68, 30 : 0.22})` is applied if none is provided.
 
         Parameters
         ----------
@@ -894,23 +993,34 @@
         17031010100  4854     0.000970         0.000461     0.000687         0.000394
         17031010201  6450     0.001080         0.000557     0.000750         0.000447
         17031010202  2818     0.001027         0.000531     0.000720         0.000416
         17031010300  6236     0.001030         0.000496     0.000710         0.000402
         17031010400  5042     0.000900         0.000514     0.000786         0.000430
         """
 
-        assert self.supply_value_provided == True, "You must provide a supply value in order to use this functionality."
-
-        if weight_fn is None: weight_fn = weights.step_fn({10 : 1, 20 : 0.68, 30 : 0.22})
-
-        return self.two_stage_fca(name, cost, max_cost, supply_values, weight_fn, normalize)
+        assert (
+            self.supply_value_provided == True
+        ), "You must provide a supply value in order to use this functionality."
 
+        if weight_fn is None:
+            weight_fn = weights.step_fn({10: 1, 20: 0.68, 30: 0.22})
 
-    def three_stage_fca(self, name = "3sfca", cost = None, supply_values = None,
-                        max_cost = None, weight_fn = None, normalize = False):
+        return self.two_stage_fca(
+            name, cost, max_cost, supply_values, weight_fn, normalize
+        )
+
+    def three_stage_fca(
+        self,
+        name="3sfca",
+        cost=None,
+        supply_values=None,
+        max_cost=None,
+        weight_fn=None,
+        normalize=False,
+    ):
         """Calculate the three-stage floating catchment area access score.
 
         Parameters
         ----------
         name                : str
                               Column name for access values
         cost                : str
@@ -993,59 +1103,67 @@
         17031010100   0.001447       0.000698
         17031010201   0.001487       0.000795
         17031010202   0.001420       0.000777
         17031010300   0.001479       0.000742
         17031010400   0.001274       0.000726
         """
 
-        assert self.supply_value_provided == True, "You must provide a supply value in order to use this functionality."
+        assert (
+            self.supply_value_provided == True
+        ), "You must provide a supply value in order to use this functionality."
 
         if weight_fn is None:
-            weight_fn = weights.step_fn({10 : 0.962, 20 : 0.704, 30 : 0.377, 60 : 0.042})
+            weight_fn = weights.step_fn({10: 0.962, 20: 0.704, 30: 0.377, 60: 0.042})
 
-        cost          = helpers.sanitize_supply_cost(self, cost, name)
-        supply_values = helpers.sanitize_supplies   (self, supply_values)
+        cost = helpers.sanitize_supply_cost(self, cost, name)
+        supply_values = helpers.sanitize_supplies(self, supply_values)
 
         for s in supply_values:
 
-            series = fca.three_stage_fca(demand_df = self.demand_df,
-                                         demand_index = self.demand_df.index.name,
-                                         demand_name = self.demand_value,
-                                         supply_df = self.supply_df,
-                                         supply_index = self.supply_df.index.name,
-                                         supply_name = s,
-                                         cost_df = self.cost_df,
-                                         cost_origin = self.cost_origin, cost_dest = self.cost_dest, cost_name = cost,
-                                         max_cost = max_cost, weight_fn = weight_fn, normalize = normalize)
+            series = fca.three_stage_fca(
+                demand_df=self.demand_df,
+                demand_index=self.demand_df.index.name,
+                demand_name=self.demand_value,
+                supply_df=self.supply_df,
+                supply_index=self.supply_df.index.name,
+                supply_name=s,
+                cost_df=self.cost_df,
+                cost_origin=self.cost_origin,
+                cost_dest=self.cost_dest,
+                cost_name=cost,
+                max_cost=max_cost,
+                weight_fn=weight_fn,
+                normalize=normalize,
+            )
 
             series.name = name + "_" + s
             if series.name in self.access_df.columns:
                 self.log.info("Overwriting {}.".format(series.name))
-                self.access_df.drop(series.name, axis = 1, inplace = True)
+                self.access_df.drop(series.name, axis=1, inplace=True)
 
             # store the raw, un-normalized access values
             self.access_df = self.access_df.join(series)
 
         if normalize:
 
             columns = [name + "_" + s for s in supply_values]
             return helpers.normalized_access(self, columns)
 
-        return self.access_df.filter(regex = "^" + name, axis = 1)
-
+        return self.access_df.filter(regex="^" + name, axis=1)
 
     @property
     def norm_access_df(self):
         for column in self.access_df.columns.difference([self.demand_value]):
-            mean_access = (self.access_df[column] * self.access_df[self.demand_value]).sum() / self.access_df[self.demand_value].sum()
+            mean_access = (
+                self.access_df[column] * self.access_df[self.demand_value]
+            ).sum() / self.access_df[self.demand_value].sum()
             self.access_df[column] /= mean_access
         return self.access_df[self.access_df.columns.difference([self.demand_value])]
 
-
-    def score(self, col_dict, name = "score"):
+    def score(self, col_dict, name="score"):
         """Weighted aggregate of multiple already-calculated, normalized access components.
 
         Parameters
         ----------
         name                : str
                               Column name for access values
         col_dict            : dict
@@ -1128,27 +1246,26 @@
         17031010202    0.831578
         ...........    ........
         17197884101    1.677075
         17197884103    1.597554
         17197980100    1.597386
         """
 
-
         for v in col_dict:
             if v not in self.access_df.columns:
                 raise ValueError("{} is not a calculated access value".format(v))
 
         weights = pd.Series(col_dict)
 
         weighted_score = self.norm_access_df[weights.index].dot(weights)
 
         weighted_score.name = name
         if weighted_score.name in self.access_df.columns:
             self.log.info("Overwriting {}.".format(weighted_score.name))
-            self.access_df.drop(weighted_score.name, axis = 1, inplace = True)
+            self.access_df.drop(weighted_score.name, axis=1, inplace=True)
 
         self.access_df = self.access_df.join(weighted_score)
 
         return weighted_score
 
     @property
     def default_cost(self):
@@ -1160,31 +1277,28 @@
 
         if new_cost in self.cost_names:
             self._default_cost = new_cost
 
         else:
             raise ValueError("Tried to set cost not available in cost df")
 
-
     @property
     def neighbor_default_cost(self):
         return self._neighbor_default_cost
 
-
     @neighbor_default_cost.setter
     def neighbor_default_cost(self, new_cost):
         """Change the default cost measure."""
 
         if new_cost in self.neighbor_cost_names:
             self._neighbor_default_cost = new_cost
 
         else:
             raise ValueError("Tried to set cost not available in cost df")
 
-
     def append_user_cost(self, new_cost_df, origin, destination, name):
         """Create a user cost, from demand to supply locations.
 
         Parameters
         ----------
         new_cost_df         : `pandas.DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`_
                               Holds the new cost....
@@ -1268,22 +1382,22 @@
         2  17093890101  17031010202  92.95  63073.735631
         3  17093890101  17031010300  89.40  63520.029749
         4  17093890101  17031010400  84.97  63268.514352
 
         """
 
         # Add it to the list of costs.
-        self.cost_df = self.cost_df.merge(new_cost_df[[origin, destination, name]],
-                                          how = 'outer',
-                                          left_on = [self.cost_origin,
-                                                     self.cost_dest],
-                                          right_on = [origin, destination])
+        self.cost_df = self.cost_df.merge(
+            new_cost_df[[origin, destination, name]],
+            how="outer",
+            left_on=[self.cost_origin, self.cost_dest],
+            right_on=[origin, destination],
+        )
         self.cost_names.append(name)
 
-
     def append_user_cost_neighbors(self, new_cost_df, origin, destination, name):
         """Create a user cost, from supply locations to other supply locations.
 
         Parameters
         ----------
         new_cost_df         : `pandas.DataFrame <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html>`_
                               Holds the new cost....
@@ -1366,23 +1480,25 @@
         1  17093890101  17031010201  92.82          62632.675522
         2  17093890101  17031010202  92.95          63073.735631
         3  17093890101  17031010300  89.40          63520.029749
         4  17093890101  17031010400  84.97          63268.514352
         """
 
         # Add it to the list of costs.
-        self.neighbor_cost_df = self.neighbor_cost_df.merge(new_cost_df[[origin, destination, name]],
-                                                            how = 'outer',
-                                                            left_on = [self.neighbor_cost_origin,
-                                                                       self.neighbor_cost_dest],
-                                                            right_on = [origin, destination])
+        self.neighbor_cost_df = self.neighbor_cost_df.merge(
+            new_cost_df[[origin, destination, name]],
+            how="outer",
+            left_on=[self.neighbor_cost_origin, self.neighbor_cost_dest],
+            right_on=[origin, destination],
+        )
         self.neighbor_cost_names.append(name)
 
-
-    def create_euclidean_distance(self, name = "euclidean", threshold = 0, centroid_o = False, centroid_d = False):
+    def create_euclidean_distance(
+        self, name="euclidean", threshold=0, centroid_o=False, centroid_d=False
+    ):
         """Calculate the Euclidean distance from demand to supply locations.
         This is simply the geopandas `distance` function.
         The user is responsible for putting the geometries into an appropriate reference system.
 
         Parameters
         ----------
         name                : str
@@ -1458,63 +1574,82 @@
         0  17093890101  17031010100  91.20  63630.788476
         1  17093890101  17031010201  92.82  62632.675522
         2  17093890101  17031010202  92.95  63073.735631
         3  17093890101  17031010300  89.40  63520.029749
         4  17093890101  17031010400  84.97  63268.514352
         """
         import geopandas as gpd
-        # TO-DO: check for unprojected geometries
 
+        # TO-DO: check for unprojected geometries
 
         # Continue if the dataframes are geodataframes, else throw an error
         if type(self.demand_df) is not gpd.GeoDataFrame:
-            raise TypeError("Cannot calculate euclidean distance without a geometry of demand side")
+            raise TypeError(
+                "Cannot calculate euclidean distance without a geometry of demand side"
+            )
 
         if type(self.supply_df) is not gpd.GeoDataFrame:
-            raise TypeError("Cannot calculate euclidean distance without a geometry of supply side")
+            raise TypeError(
+                "Cannot calculate euclidean distance without a geometry of supply side"
+            )
 
         # Reset the index so that the geoids are accessible
-        df1 = self.demand_df.rename_axis('origin').reset_index()
-        df2 = self.supply_df.rename_axis('dest').reset_index()
+        df1 = self.demand_df.rename_axis("origin").reset_index()
+        df2 = self.supply_df.rename_axis("dest").reset_index()
 
         # Convert to centroids if so-specified
-        if centroid_o: df1.set_geometry(df1.centroid, inplace = True)
-        if centroid_d: df2.set_geometry(df2.centroid, inplace = True)
+        if centroid_o:
+            df1.set_geometry(df1.centroid, inplace=True)
+        if centroid_d:
+            df2.set_geometry(df2.centroid, inplace=True)
 
         # Calculate the distances.
-        if ((df1.geom_type == "Point").all() & (df2.geom_type == "Point").all()):
+        if (df1.geom_type == "Point").all() & (df2.geom_type == "Point").all():
             # If both geometries are point types, merge on a temporary dummy column
             df1["temp"] = 1
             df2["temp"] = 1
-            df1and2 = df1[["temp", "geometry","origin"]].merge(df2[["temp", "geometry","dest"]].rename(columns = {'geometry':'geomb'}))
-            df1and2.drop("temp", inplace = True, axis = 1)
+            df1and2 = df1[["temp", "geometry", "origin"]].merge(
+                df2[["temp", "geometry", "dest"]].rename(columns={"geometry": "geomb"})
+            )
+            df1and2.drop("temp", inplace=True, axis=1)
             df1and2[name] = df1and2.distance(df1and2.set_geometry("geomb"))
         else:
             # Execute an sjoin for non-point geometries, based upon a buffer zone
-            df1and2 = gpd.sjoin(df1, df2.rename(columns = {'geometry':'geomb'}).set_geometry(df2.buffer(threshold)))
+            df1and2 = gpd.sjoin(
+                df1,
+                df2.rename(columns={"geometry": "geomb"}).set_geometry(
+                    df2.buffer(threshold)
+                ),
+            )
             df1and2[name] = df1and2.distance(df1and2.set_geometry("geomb"))
 
         # Add it to the cost df.
         df1and2 = df1and2[df1and2[name] < threshold]
 
         if name in self.cost_df.columns:
             self.log.info("Overwriting {}.".format(name))
-            self.cost_df.drop(name, axis = 1, inplace = True)
+            self.cost_df.drop(name, axis=1, inplace=True)
 
-        self.cost_df = self.cost_df.merge(df1and2[[name,'origin','dest']], how = 'outer', left_on = [self.cost_origin, self.cost_dest], right_on = ['origin', 'dest'])
+        self.cost_df = self.cost_df.merge(
+            df1and2[[name, "origin", "dest"]],
+            how="outer",
+            left_on=[self.cost_origin, self.cost_dest],
+            right_on=["origin", "dest"],
+        )
 
         # Add it to the list of costs.
         if name not in self.cost_names:
             self.cost_names.append(name)
         # Set the default cost if it does not exist
-        if not hasattr(self, '_default_cost'):
+        if not hasattr(self, "_default_cost"):
             self._default_cost = name
 
-
-    def create_euclidean_distance_neighbors(self, name = "euclidean", threshold = 0, centroid = False):
+    def create_euclidean_distance_neighbors(
+        self, name="euclidean", threshold=0, centroid=False
+    ):
         """Calculate the Euclidean distance among demand locations.
 
         Parameters
         ----------
         name                : str
                               Column name for euclidean distances neighbors
         threshold           : int
@@ -1591,44 +1726,58 @@
         0  17031010100  17031010100             0.000000
         1  17031010100  17031010201           998.259243
         2  17031010100  17031010202           635.203387
         3  17031010100  17031010300           653.415713
         4  17031010100  17031010400          2065.375554
         """
         import geopandas as gpd
-        # TO-DO: check for unprojected geometries
 
+        # TO-DO: check for unprojected geometries
 
         # Continue if the dataframes are geodataframes, else throw an error
         if type(self.demand_df) is not gpd.GeoDataFrame:
-            raise TypeError("Cannot calculate euclidean distance without a geometry of supply side")
+            raise TypeError(
+                "Cannot calculate euclidean distance without a geometry of supply side"
+            )
 
         # Reset the index so that the geoids are accessible
-        df1 = self.demand_df.rename_axis('origin').reset_index()
-        df2 = self.demand_df.rename_axis('dest').reset_index()
+        df1 = self.demand_df.rename_axis("origin").reset_index()
+        df2 = self.demand_df.rename_axis("dest").reset_index()
 
         # Convert to centroids if so-specified
         if centroid:
-            df1.set_geometry(df1.centroid, inplace = True)
-            df2.set_geometry(df2.centroid, inplace = True)
+            df1.set_geometry(df1.centroid, inplace=True)
+            df2.set_geometry(df2.centroid, inplace=True)
 
         # Calculate the distances.
-        if ((df1.geom_type == "Point").all() & (df2.geom_type == "Point").all()):
+        if (df1.geom_type == "Point").all() & (df2.geom_type == "Point").all():
             # If both geometries are point types, merge on a temporary dummy column
             df1["temp"] = 1
             df2["temp"] = 1
-            df1and2 = df1[["temp", "geometry","origin"]].merge(df2[["temp", "geometry","dest"]].rename(columns = {'geometry':'geomb'}))
-            df1and2.drop("temp", inplace = True, axis = 1)
+            df1and2 = df1[["temp", "geometry", "origin"]].merge(
+                df2[["temp", "geometry", "dest"]].rename(columns={"geometry": "geomb"})
+            )
+            df1and2.drop("temp", inplace=True, axis=1)
             df1and2[name] = df1and2.distance(df1and2.set_geometry("geomb"))
         else:
             # Execute an sjoin for non-point geometries, based upon a buffer zone
-            df1and2 = gpd.sjoin(df1, df2.rename(columns = {'geometry':'geomb'}).set_geometry(df2.buffer(threshold)))
+            df1and2 = gpd.sjoin(
+                df1,
+                df2.rename(columns={"geometry": "geomb"}).set_geometry(
+                    df2.buffer(threshold)
+                ),
+            )
             df1and2[name] = df1and2.distance(df1and2.set_geometry("geomb"))
 
         # Add it to the cost df.
         df1and2 = df1and2[df1and2[name] < threshold]
-        self.neighbor_cost_df = self.neighbor_cost_df.merge(df1and2[[name,'origin','dest']], how = 'outer', left_on = [self.neighbor_cost_origin, self.neighbor_cost_dest], right_on = ['origin', 'dest'])
+        self.neighbor_cost_df = self.neighbor_cost_df.merge(
+            df1and2[[name, "origin", "dest"]],
+            how="outer",
+            left_on=[self.neighbor_cost_origin, self.neighbor_cost_dest],
+            right_on=["origin", "dest"],
+        )
         # Add it to the list of costs.
         self.neighbor_cost_names.append(name)
         # Set the default cost if it does not exist
-        if not hasattr(self, '_neighbor_default_cost'):
+        if not hasattr(self, "_neighbor_default_cost"):
             self._neighbor_default_cost = name
```

### Comparing `access-1.1.8/access/datasets.py` & `access-1.1.9/access/datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "chi_euclidean": "chicago_metro_euclidean_costs.csv.bz2",
             "chi_euclidean_neighbors": "chicago_metro_euclidean_cost_neighbors.csv.bz2",
             "cook_county_hospitals": "cook_county_hospitals.csv",
             "cook_county_hospitals_geom": "hospitals_cookcty.geojson",
             "cook_county_tracts": "cook_county_tracts.geojson",
         }
 
-        url = f"https://uchicago-csds-access.s3.amazonaws.com/ex_datasets/{_datasets[key]}"
+        url = f"https://d2r7gabxtstf5s.cloudfront.net/ex_datasets/{_datasets[key]}"
 
         if ".geojson" in url:
             import geopandas as gpd
 
             return gpd.read_file(url)
 
         return pd.read_csv(url)
```

### Comparing `access-1.1.8/access/fca.py` & `access-1.1.9/access/fca.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 import warnings
 import numpy as np
 import pandas as pd
 
 from .weights import step_fn
 
-def weighted_catchment(loc_df, cost_df, max_cost = None, cost_source = "origin", cost_dest = "dest", cost_cost = "cost",
-                       loc_index = "geoid", loc_value = None, weight_fn = None, three_stage_weight = None):
+
+def weighted_catchment(
+    loc_df,
+    cost_df,
+    max_cost=None,
+    cost_source="origin",
+    cost_dest="dest",
+    cost_cost="cost",
+    loc_index="geoid",
+    loc_value=None,
+    weight_fn=None,
+    three_stage_weight=None,
+):
     """
     Calculation of the floating catchment (buffered) accessibility
     sum, from DataFrames with computed distances.
     This catchment may be either a simple buffer -- with cost below
     a single threshold -- or an additional weight may be applied
     as a function of the access cost.
 
@@ -41,42 +52,56 @@
                  note that it applies _along with_ the weight function.
 
     Returns
     -------
     resources  : pandas.Series
                  A -- potentially weighted -- sum of resources, facilities, or consumers.
     """
-    #merge the loc dataframe and cost dataframe together
+    # merge the loc dataframe and cost dataframe together
     if loc_index is True:
-        temp = pd.merge(cost_df, loc_df, left_on = cost_source, right_index = True)
+        temp = pd.merge(cost_df, loc_df, left_on=cost_source, right_index=True)
     else:
-        temp = pd.merge(cost_df, loc_df, left_on = cost_source, right_on = loc_index)
+        temp = pd.merge(cost_df, loc_df, left_on=cost_source, right_on=loc_index)
 
     # constrain by max cost
-    if max_cost is not None: temp = temp[temp[cost_cost] < max_cost].copy()
-
+    if max_cost is not None:
+        temp = temp[temp[cost_cost] < max_cost].copy()
 
-    #apply a weight function if inputted -- either enhanced two stage or three stage
+    # apply a weight function if inputted -- either enhanced two stage or three stage
     if weight_fn:
         if three_stage_weight is not None:
-            new_loc_value_column = temp[loc_value]*temp.W3*temp.G
-            temp = temp.drop([loc_value], axis = 1)
+            new_loc_value_column = temp[loc_value] * temp.W3 * temp.G
+            temp = temp.drop([loc_value], axis=1)
             temp[loc_value] = new_loc_value_column
         else:
             temp[loc_value] *= temp[cost_cost].apply(weight_fn)
 
     return temp.groupby([cost_dest])[loc_value].sum()
 
 
-def fca_ratio(demand_df, supply_df, demand_cost_df, supply_cost_df, max_cost,
-              demand_index = 'geoid', demand_name = "demand",
-              supply_index = 'geoid', supply_name  = "supply",
-              demand_cost_origin = "origin", demand_cost_dest = "dest", demand_cost_name = "cost",
-              supply_cost_origin = "origin", supply_cost_dest = "dest", supply_cost_name = "cost",
-              weight_fn = None, normalize = False, noise = 'quiet'):
+def fca_ratio(
+    demand_df,
+    supply_df,
+    demand_cost_df,
+    supply_cost_df,
+    max_cost,
+    demand_index="geoid",
+    demand_name="demand",
+    supply_index="geoid",
+    supply_name="supply",
+    demand_cost_origin="origin",
+    demand_cost_dest="dest",
+    demand_cost_name="cost",
+    supply_cost_origin="origin",
+    supply_cost_dest="dest",
+    supply_cost_name="cost",
+    weight_fn=None,
+    normalize=False,
+    noise="quiet",
+):
     """Calculation of the floating catchment accessibility
     ratio, from DataFrames with precomputed distances.
     This is accomplished through two calls of the :meth:`Access.access.weighted_catchment` method.
 
     Parameters
     ----------
 
@@ -121,49 +146,82 @@
 
     Returns
     -------
     access     : pandas.Series
                  A -- potentially-weighted -- access ratio.
     """
 
-    #if there is a discrepancy between the demand and supply cost dataframe locations, print it
-    if len(set(demand_df.index.tolist()) - set(supply_cost_df[supply_cost_dest].unique())) != 0:
-        warnings.warn("some tracts may be unaccounted for in supply_cost", stacklevel = 1)
-
-
-    #get a series of the total demand within the buffer zone
-    total_demand_series = weighted_catchment(demand_df, demand_cost_df, max_cost,
-                                          cost_source = demand_cost_dest, cost_dest = demand_cost_origin, cost_cost = demand_cost_name,
-                                          loc_index = demand_index, loc_value = demand_name,
-                                          weight_fn = weight_fn)
-    #get a series of the total supply within the buffer zone
-    total_supply_series = weighted_catchment(supply_df, supply_cost_df, max_cost,
-                                             cost_source = supply_cost_dest, cost_dest = supply_cost_origin, cost_cost = supply_cost_name,
-                                             loc_index = supply_index, loc_value = supply_name,
-                                             weight_fn = weight_fn)
-
-    #join the aggregate demand and the aggregate supply into one dataframe
-    temp = total_supply_series.to_frame(name = 'supply').join(total_demand_series.to_frame(name = 'demand'), how = 'right').fillna(0)
-
-    #calculate the floating catchement area, or supply divided by demand
-    temp['FCA'] = temp['supply'] / temp['demand']
-    base_FCA_series = temp['FCA']
+    # if there is a discrepancy between the demand and supply cost dataframe locations, print it
+    if (
+        len(
+            set(demand_df.index.tolist())
+            - set(supply_cost_df[supply_cost_dest].unique())
+        )
+        != 0
+    ):
+        warnings.warn("some tracts may be unaccounted for in supply_cost", stacklevel=1)
+
+    # get a series of the total demand within the buffer zone
+    total_demand_series = weighted_catchment(
+        demand_df,
+        demand_cost_df,
+        max_cost,
+        cost_source=demand_cost_dest,
+        cost_dest=demand_cost_origin,
+        cost_cost=demand_cost_name,
+        loc_index=demand_index,
+        loc_value=demand_name,
+        weight_fn=weight_fn,
+    )
+    # get a series of the total supply within the buffer zone
+    total_supply_series = weighted_catchment(
+        supply_df,
+        supply_cost_df,
+        max_cost,
+        cost_source=supply_cost_dest,
+        cost_dest=supply_cost_origin,
+        cost_cost=supply_cost_name,
+        loc_index=supply_index,
+        loc_value=supply_name,
+        weight_fn=weight_fn,
+    )
+
+    # join the aggregate demand and the aggregate supply into one dataframe
+    temp = (
+        total_supply_series.to_frame(name="supply")
+        .join(total_demand_series.to_frame(name="demand"), how="right")
+        .fillna(0)
+    )
+
+    # calculate the floating catchement area, or supply divided by demand
+    temp["FCA"] = temp["supply"] / temp["demand"]
+    base_FCA_series = temp["FCA"]
 
-    if noise != 'quiet':
-        #depending on the version history of the census tract data you use, this will print out the tracts that have undefined FCA values
+    if noise != "quiet":
+        # depending on the version history of the census tract data you use, this will print out the tracts that have undefined FCA values
         print(base_FCA_series[pd.isna(base_FCA_series)])
 
     return base_FCA_series
 
 
-def two_stage_fca(demand_df, supply_df, cost_df, max_cost = None,
-                  demand_index = "geoid", demand_name   = "demand",
-                  supply_index = "geoid",   supply_name   = "supply",
-                  cost_origin = "origin", cost_dest = "dest", cost_name = "cost",
-                  weight_fn = None, normalize = False):
+def two_stage_fca(
+    demand_df,
+    supply_df,
+    cost_df,
+    max_cost=None,
+    demand_index="geoid",
+    demand_name="demand",
+    supply_index="geoid",
+    supply_name="supply",
+    cost_origin="origin",
+    cost_dest="dest",
+    cost_name="cost",
+    weight_fn=None,
+    normalize=False,
+):
     """
     Calculation of the two-stage floating catchment accessibility
     ratio, from DataFrames with precomputed distances.
     This is accomplished through a single call of the `access.weighted_catchment` method,
     to retrieve the patients using each provider.
     The ratio of providers per patient is then calculated at each care destination,
     and that ratio is weighted and summed at each corresponding demand site.
@@ -203,49 +261,73 @@
     normalize  : bool
                   True to normalize the FCA series, by default False.
     Returns
     -------
     access     : pandas.Series
                  A -- potentially-weighted -- two-stage access ratio.
     """
-    #get a series of total demand then calculate the supply to total demand ratio for each location
-    total_demand_series = weighted_catchment(demand_df, cost_df, max_cost,
-                                             cost_source = cost_origin, cost_dest = cost_dest, cost_cost = cost_name,
-                                             loc_index = demand_index, loc_value = demand_name,
-                                             weight_fn = weight_fn)
+    # get a series of total demand then calculate the supply to total demand ratio for each location
+    total_demand_series = weighted_catchment(
+        demand_df,
+        cost_df,
+        max_cost,
+        cost_source=cost_origin,
+        cost_dest=cost_dest,
+        cost_cost=cost_name,
+        loc_index=demand_index,
+        loc_value=demand_name,
+        weight_fn=weight_fn,
+    )
 
-    #create a temporary dataframe, temp, that holds the supply and aggregate demand at each location
+    # create a temporary dataframe, temp, that holds the supply and aggregate demand at each location
     total_demand_series.name += "_W"
-    temp = supply_df.join(total_demand_series, how = 'right')
+    temp = supply_df.join(total_demand_series, how="right")
 
-    #there may be NA values due to a shorter supply dataframe than the demand dataframe.
-    #in this case, replace any potential NA values(which correspond to supply locations with no supply) with 0.
-    temp[supply_name].fillna(0, inplace = True)
-
-    #calculate the fractional ratio of supply to aggregate demand at each location, or Rl
-    temp['Rl'] = temp[supply_name] / temp[demand_name + "_W"]
-
-    #separate the fractional ratio of supply to aggregate demand at each location, or Rl, into a new dataframe
-    supply_to_total_demand_frame = pd.DataFrame(data = {'Rl':temp['Rl']})
-    supply_to_total_demand_frame.index.name = 'geoid'
+    # there may be NA values due to a shorter supply dataframe than the demand dataframe.
+    # in this case, replace any potential NA values(which correspond to supply locations with no supply) with 0.
+    temp[supply_name].fillna(0, inplace=True)
+
+    # calculate the fractional ratio of supply to aggregate demand at each location, or Rl
+    temp["Rl"] = temp[supply_name] / temp[demand_name + "_W"]
+
+    # separate the fractional ratio of supply to aggregate demand at each location, or Rl, into a new dataframe
+    supply_to_total_demand_frame = pd.DataFrame(data={"Rl": temp["Rl"]})
+    supply_to_total_demand_frame.index.name = "geoid"
 
     # sum, into a series, the supply to total demand ratios for each location
-    two_stage_fca_series = weighted_catchment(supply_to_total_demand_frame, cost_df, max_cost,
-                                              cost_source = cost_dest, cost_dest = cost_origin, cost_cost = cost_name,
-                                              loc_index = 'geoid', loc_value = "Rl",
-                                              weight_fn = weight_fn)
+    two_stage_fca_series = weighted_catchment(
+        supply_to_total_demand_frame,
+        cost_df,
+        max_cost,
+        cost_source=cost_dest,
+        cost_dest=cost_origin,
+        cost_cost=cost_name,
+        loc_index="geoid",
+        loc_value="Rl",
+        weight_fn=weight_fn,
+    )
 
     return two_stage_fca_series
 
 
-def three_stage_fca(demand_df, supply_df, cost_df, max_cost,
-                  demand_index = "geoid", demand_name   = "demand",
-                  supply_index = "geoid",   supply_name   = "supply",
-                  cost_origin = "origin", cost_dest = "dest", cost_name = "cost",
-                  weight_fn = None, normalize = False):
+def three_stage_fca(
+    demand_df,
+    supply_df,
+    cost_df,
+    max_cost,
+    demand_index="geoid",
+    demand_name="demand",
+    supply_index="geoid",
+    supply_name="supply",
+    cost_origin="origin",
+    cost_dest="dest",
+    cost_name="cost",
+    weight_fn=None,
+    normalize=False,
+):
     """Calculation of the three-stage floating catchment accessibility
     ratio, from DataFrames with precomputed distances.
     This is accomplished through a single call of the :meth:`access.access.weighted_catchment` method,
     to retrieve the patients using each provider.
     The ratio of providers per patient is then calculated at each care destination,
     and that ratio is weighted and summed at each corresponding demand site.
     The only difference weight respect to the 2SFCA method is that,
@@ -287,44 +369,66 @@
 
     Returns
     -------
     access     : pandas.Series
                  A -- potentially-weighted -- three-stage access ratio.
     """
 
-    #create preference weight 'G', which is the weight
+    # create preference weight 'G', which is the weight
     cost_df["W3"] = cost_df[cost_name].apply(weight_fn)
-    W3sum_frame = cost_df[[cost_origin, "W3"]].groupby(cost_origin).sum().rename(columns = {"W3" : "W3sum"}).reset_index()
+    W3sum_frame = (
+        cost_df[[cost_origin, "W3"]]
+        .groupby(cost_origin)
+        .sum()
+        .rename(columns={"W3": "W3sum"})
+        .reset_index()
+    )
     cost_df = pd.merge(cost_df, W3sum_frame)
     cost_df["G"] = cost_df.W3 / cost_df.W3sum
 
-    #get a series of total demand then calculate the supply to total demand ratio for each location
-    total_demand_series = weighted_catchment(demand_df, cost_df, max_cost,
-                                          cost_source = cost_origin, cost_dest = cost_dest, cost_cost = cost_name,
-                                          loc_index = demand_index, loc_value = demand_name,
-                                          weight_fn = weight_fn, three_stage_weight = True)
+    # get a series of total demand then calculate the supply to total demand ratio for each location
+    total_demand_series = weighted_catchment(
+        demand_df,
+        cost_df,
+        max_cost,
+        cost_source=cost_origin,
+        cost_dest=cost_dest,
+        cost_cost=cost_name,
+        loc_index=demand_index,
+        loc_value=demand_name,
+        weight_fn=weight_fn,
+        three_stage_weight=True,
+    )
 
-    #create a temporary dataframe, temp, that holds the supply and aggregate demand at each location
+    # create a temporary dataframe, temp, that holds the supply and aggregate demand at each location
     total_demand_series.name += "_W"
-    temp = supply_df.join(total_demand_series, how = 'right')
+    temp = supply_df.join(total_demand_series, how="right")
 
-    #there may be NA values due to a shorter supply dataframe than the demand dataframe.
-    #in this case, replace any potential NA values(which correspond to supply locations with no supply) with 0.
-    temp[supply_name].fillna(0, inplace = True)
-
-    #calculate the fractional ratio of supply to aggregate demand at each location, or Rl
-    temp['Rl'] = temp[supply_name] / temp[demand_name + "_W"]
-
-    #separate the fractional ratio of supply to aggregate demand at each location, or Rl, into a new dataframe
-    supply_to_total_demand_frame = pd.DataFrame(data = {'Rl' : temp['Rl']})
-    supply_to_total_demand_frame.index.name = 'geoid'
-
-    #sum, into a series, the supply to total demand ratios for each location
-    three_stage_fca_series = weighted_catchment(supply_to_total_demand_frame, cost_df.sort_index(), max_cost,
-                                                cost_source = cost_dest, cost_dest = cost_origin, cost_cost = cost_name,
-                                                loc_index = 'geoid', loc_value = "Rl",
-                                                weight_fn = weight_fn, three_stage_weight = True)
+    # there may be NA values due to a shorter supply dataframe than the demand dataframe.
+    # in this case, replace any potential NA values(which correspond to supply locations with no supply) with 0.
+    temp[supply_name].fillna(0, inplace=True)
+
+    # calculate the fractional ratio of supply to aggregate demand at each location, or Rl
+    temp["Rl"] = temp[supply_name] / temp[demand_name + "_W"]
+
+    # separate the fractional ratio of supply to aggregate demand at each location, or Rl, into a new dataframe
+    supply_to_total_demand_frame = pd.DataFrame(data={"Rl": temp["Rl"]})
+    supply_to_total_demand_frame.index.name = "geoid"
+
+    # sum, into a series, the supply to total demand ratios for each location
+    three_stage_fca_series = weighted_catchment(
+        supply_to_total_demand_frame,
+        cost_df.sort_index(),
+        max_cost,
+        cost_source=cost_dest,
+        cost_dest=cost_origin,
+        cost_cost=cost_name,
+        loc_index="geoid",
+        loc_value="Rl",
+        weight_fn=weight_fn,
+        three_stage_weight=True,
+    )
 
-    #remove the preference weight G from the original costs dataframe
-    cost_df.drop(columns = ["G", "W3", "W3sum"], inplace = True)
+    # remove the preference weight G from the original costs dataframe
+    cost_df.drop(columns=["G", "W3", "W3sum"], inplace=True)
 
     return three_stage_fca_series
```

### Comparing `access-1.1.8/access/helpers.py` & `access-1.1.9/access/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,34 +17,36 @@
 
     if cost is None:
 
         cost = a.neighbor_default_cost
         if len(a.cost_names) > 1:
             a.log.info("Using default neighbor cost, {}, for {}.".format(cost, name))
 
-
     if cost not in a.neighbor_cost_names:
 
         raise ValueError("{} not an available neighbor cost.".format(cost))
 
     return cost
 
 
 def sanitize_supplies(a, supply_values):
 
     if type(supply_values) is str:
         supply_values = [supply_values]
     elif supply_values is None:
         supply_values = a.supply_types
     elif type(supply_values) is not list:
-        raise ValueError("supply_values should be a list or string (or -- default -- None)")
+        raise ValueError(
+            "supply_values should be a list or string (or -- default -- None)"
+        )
 
     return supply_values
 
 
 def normalized_access(a, columns):
 
-    mean_access_values = a.access_df[columns]\
-                          .multiply(a.access_df[a.demand_value], axis = 0).sum()  \
-                          / a.access_df[a.demand_value].sum()
+    mean_access_values = (
+        a.access_df[columns].multiply(a.access_df[a.demand_value], axis=0).sum()
+        / a.access_df[a.demand_value].sum()
+    )
 
     return a.access_df[columns].divide(mean_access_values)
```

### Comparing `access-1.1.8/access/raam.py` & `access-1.1.9/access/raam.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import numpy as np
 import pandas as pd
 
-def iterate_raam(demand, supply, travel,
-                 max_cycles = 151, initial_step = 0.2, min_step = 0.005, half_life = 50,
-                 limit_initial = 20, verbose = False):
+
+def iterate_raam(
+    demand,
+    supply,
+    travel,
+    max_cycles=151,
+    initial_step=0.2,
+    min_step=0.005,
+    half_life=50,
+    limit_initial=20,
+    verbose=False,
+):
 
     norig, ndest = travel.shape
     assignment = np.zeros((norig, ndest))
-    assignment[range(norig), travel.argmin(axis = 1)] = demand
-
+    assignment[range(norig), travel.argmin(axis=1)] = demand
 
     for i in range(max_cycles):
 
-        demand_at_supply = assignment.sum(axis = 0)
-        congestion_cost  = demand_at_supply / supply
-        total_cost       = (congestion_cost + travel)
+        demand_at_supply = assignment.sum(axis=0)
+        congestion_cost = demand_at_supply / supply
+        total_cost = congestion_cost + travel
 
-        max_locations = np.ma.masked_array(total_cost, assignment == 0).argmax(axis = 1)
-        min_locations = total_cost.argmin(axis = 1)
+        max_locations = np.ma.masked_array(total_cost, assignment == 0).argmax(axis=1)
+        min_locations = total_cost.argmin(axis=1)
 
         slmin = supply[min_locations]
         slmax = supply[max_locations]
 
         trlmin = travel[range(norig), min_locations]
         trlmax = travel[range(norig), max_locations]
 
@@ -29,76 +37,93 @@
         drlmax = assignment[range(norig), max_locations]
 
         dr = drlmin + drlmax
 
         drotherlmin = demand_at_supply[min_locations] - drlmin
         drotherlmax = demand_at_supply[max_locations] - drlmax
 
-        drlmin_new = ((slmin * slmax) / (slmin + slmax)) * \
-                     ((trlmax - trlmin) + (dr + drotherlmax) / slmax - drotherlmin / slmin)
+        drlmin_new = ((slmin * slmax) / (slmin + slmax)) * (
+            (trlmax - trlmin) + (dr + drotherlmax) / slmax - drotherlmin / slmin
+        )
 
         delta = drlmin_new - drlmin
 
         delta = np.minimum(delta, drlmax)
         delta = np.where(max_locations == min_locations, 0, delta)
 
         if type(initial_step) is float:
             step_size = initial_step * 0.5 ** (i / half_life)
-            if step_size < min_step: step_size = min_step
+            if step_size < min_step:
+                step_size = min_step
 
             delta = np.minimum(delta, step_size * demand).astype(int)
 
         else:
 
             step_size = int(np.round(initial_step * 0.5 ** (i / half_life)))
-            if step_size < min_step: step_size = min_step
+            if step_size < min_step:
+                step_size = min_step
 
             delta = np.minimum(delta, step_size).astype(int)
 
-
         ## We don't want "attractive locations" getting mobbed.
         ## This will only happen in the first 10-20 cycles.
         ## So only do these (somewhat costly checks) then.
         if i < limit_initial:
 
             delta_mat = np.zeros(travel.shape)
             delta_mat[range(norig), min_locations] += delta
 
-            naive_assignment = delta_mat.sum(axis = 0) / (supply)# * rho)
+            naive_assignment = delta_mat.sum(axis=0) / (supply)  # * rho)
             scale_factor = np.maximum(naive_assignment, 1)
 
             delta_mat = (delta_mat / scale_factor).round().astype(int)
 
-            delta = delta_mat.sum(axis = 1)
-
-
+            delta = delta_mat.sum(axis=1)
 
         assignment[range(norig), min_locations] += delta
         assignment[range(norig), max_locations] -= delta
 
-        assert((assignment.sum(axis = 1) == demand).all())
+        assert (assignment.sum(axis=1) == demand).all()
 
         if not (i % 25):
-            raam_cost = (total_cost * assignment).sum(axis = 1) / assignment.sum(axis = 1)
+            raam_cost = (total_cost * assignment).sum(axis=1) / assignment.sum(axis=1)
 
             if verbose:
-                print("{:d} {:.2f} {:d} {:.3f}".format(i, raam_cost.mean(), delta.sum(), step_size), end = " || ")
+                print(
+                    "{:d} {:.2f} {:d} {:.3f}".format(
+                        i, raam_cost.mean(), delta.sum(), step_size
+                    ),
+                    end=" || ",
+                )
 
-    raam_cost = (total_cost * assignment).sum(axis = 1) / assignment.sum(axis = 1)
+    raam_cost = (total_cost * assignment).sum(axis=1) / assignment.sum(axis=1)
 
     return raam_cost
 
 
-def raam(demand_df, supply_df, cost_df,
-         demand_index = True, demand_name = "demand",
-         supply_index = True, supply_name = "supply",
-         cost_origin   = "origin", cost_dest = "dest", cost_name = "cost",
-         tau = 60, rho = None,
-         max_cycles = 150, initial_step = 0.2, min_step = 0.005, half_life = 50,
-         verbose = False):
+def raam(
+    demand_df,
+    supply_df,
+    cost_df,
+    demand_index=True,
+    demand_name="demand",
+    supply_index=True,
+    supply_name="supply",
+    cost_origin="origin",
+    cost_dest="dest",
+    cost_name="cost",
+    tau=60,
+    rho=None,
+    max_cycles=150,
+    initial_step=0.2,
+    min_step=0.005,
+    half_life=50,
+    verbose=False,
+):
     """Calculate the rational agent access model's total cost --
     a weighted travel and congestion cost.
     The balance of the two costs is expressed by the
     :math:`\\tau` parameter, which corresponds to the travel time
     required to accept of congestion by 100% of the mean demand to supply ratio
     in the study area.
 
@@ -137,48 +162,58 @@
     Returns
     -------
     access     : pandas.Series
 
                   A -- potentially-weighted -- Rational Agent Access Model cost.
     """
 
-    if demand_index is not True: demand_df = demand_df.set_index(demand_index)
-    if supply_index is not True: supply_df = supply_df.set_index(supply_index)
+    if demand_index is not True:
+        demand_df = demand_df.set_index(demand_index)
+    if supply_index is not True:
+        supply_df = supply_df.set_index(supply_index)
 
     demand_df = demand_df[demand_df[demand_name] > 0].copy()
     supply_df = supply_df[supply_df[supply_name] > 0].copy()
 
     demand_locations = list(set(cost_df[cost_origin]) & set(demand_df.index))
-    supply_locations = list(set(cost_df[cost_dest])   & set(supply_df.index))
+    supply_locations = list(set(cost_df[cost_dest]) & set(supply_df.index))
 
     cost_pivot = cost_df.pivot(index=cost_origin, columns=cost_dest, values=cost_name)
     try:
-        travel_np  = cost_pivot.loc[demand_locations, supply_locations].to_numpy().copy()
+        travel_np = cost_pivot.loc[demand_locations, supply_locations].to_numpy().copy()
     except:
         travel_np = cost_pivot.loc[demand_locations, supply_locations].values.copy()
 
-    travel_np  = travel_np / tau
-    travel_np  = np.ma.masked_array(travel_np, np.isnan(travel_np))
+    travel_np = travel_np / tau
+    travel_np = np.ma.masked_array(travel_np, np.isnan(travel_np))
 
     # If it is not specified, rho is the average demand to supply ratio.
-    if rho is None: rho = demand_df[demand_name].sum() / supply_df[supply_name].sum()
+    if rho is None:
+        rho = demand_df[demand_name].sum() / supply_df[supply_name].sum()
 
     try:
         supply_np = supply_df.loc[supply_locations, supply_name].to_numpy().copy()
     except:
         supply_np = supply_df.loc[supply_locations, supply_name].values.copy()
 
     supply_np = supply_np * rho
 
     # Change this -- should be
     try:
         demand_np = demand_df.loc[demand_locations, demand_name].to_numpy().copy()
     except:
         demand_np = demand_df.loc[demand_locations, demand_name].values.copy()
 
-    raam_cost = iterate_raam(demand_np, supply_np, travel_np, verbose = verbose,
-                             max_cycles = max_cycles, initial_step = initial_step,
-                             min_step = min_step, half_life = half_life)
+    raam_cost = iterate_raam(
+        demand_np,
+        supply_np,
+        travel_np,
+        verbose=verbose,
+        max_cycles=max_cycles,
+        initial_step=initial_step,
+        min_step=min_step,
+        half_life=half_life,
+    )
 
-    rs = pd.Series(name = "RAAM", index = demand_locations, data = raam_cost)
+    rs = pd.Series(name="RAAM", index=demand_locations, data=raam_cost)
 
     return rs
```

### Comparing `access-1.1.8/access/weights.py` & `access-1.1.9/access/weights.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+
 def step_fn(step_dict):
     """
     Create a step function from a dictionary.
 
     Parameters
     ----------
     step_dict           : dict
@@ -29,30 +30,31 @@
     >>> fn = weights.step_fn({20 : 1, 40 : 0.68, 60 : 0.22})
 
     >>> {v : fn(v) for v in range(0, 71, 10)}
     {0: 1, 10: 1, 20: 1, 30: 0.68, 40: 0.68, 50: 0.22, 60: 0.22, 70: 0}
     """
 
     if type(step_dict) != dict:
-        raise TypeError('step_dict must be of type dict.')
+        raise TypeError("step_dict must be of type dict.")
 
     for v in step_dict.values():
         if v < 0:
-            raise ValueError('All weights must be positive.')
+            raise ValueError("All weights must be positive.")
 
     def helper(key_to_test):
 
-        for k,v in sorted(step_dict.items()):
+        for k, v in sorted(step_dict.items()):
             if key_to_test <= k:
                 return v
 
         return 0
 
     return helper
 
+
 def gaussian(sigma):
     """
     Create a gaussian weight function, for a specified width, :math:`\sigma`.
     The mean / location parameter is assumed to be 0.
     Note that the standard normalization of the Gaussian, :math:`1 / \sqrt{2\pi\sigma^2}`,
     is *not* applied, so :math:`f(0) = 1` regardless of the value of :math:`\sigma`.
     Of course, this is irrelevant if the ultimate access values are ultimately normalized.
@@ -89,18 +91,18 @@
     >>> {x : np.exp(-x**2/2) for x in range(4)}
     {0: 1.0, 1: 0.6065306597126334, 2: 0.1353352832366127, 3: 0.011108996538242306}
     """
 
     if sigma == 0:
         raise ValueError("Sigma must be non-zero.")
 
-    return lambda x: np.exp(-x*x / (2 * sigma**2)) # / np.sqrt(2*np.pi*sigma**2)
+    return lambda x: np.exp(-x * x / (2 * sigma**2))  # / np.sqrt(2*np.pi*sigma**2)
 
 
-def gravity(scale, alpha, min_dist = 0):
+def gravity(scale, alpha, min_dist=0):
     """
     Create a gravity function from a scale :math:`s` and :math:`\\alpha` parameters
     as well as an optional minimum distance :math:`x_\\text{min}`.
     The function is of the form :math:`f(x) = (\\text{max}(x, x_\\text{min})/s)^\\alpha`.
     Note that there is no overall normalization.
 
     Parameters
```

### Comparing `access-1.1.8/access.egg-info/PKG-INFO` & `access-1.1.9/access.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: access
-Version: 1.1.8
+Version: 1.1.9
 Summary: Calculate spatial accessibility metrics.
 Home-page: https://access.readthedocs.io/en/latest/
 Maintainer: James Saxon
 Maintainer-email: jsaxon@uchicago.edu
 License: 3-Clause BSD
 Keywords: spatial statistics access
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: BSD License
@@ -23,13 +22,14 @@
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # Spatial Access
 
-This package provides classical and novel measures of spatial accessibility to services.
-
-For full documentation, see [access.readthedocs.io](https://access.readthedocs.io/en/latest/).
-
+![tag](https://img.shields.io/github/v/release/pysal/access?include_prereleases&sort=semver)
+[![Documentation](https://img.shields.io/static/v1.svg?label=docs&message=current&color=9cf)](http://pysal.org/access/)
+[![Continuous Integration](https://github.com/pysal/access/actions/workflows/unittests.yml/badge.svg)](https://github.com/pysal/access/actions/workflows/unittests.yml)
 
+This package provides classical and novel measures of spatial accessibility to services.
 
+For full documentation, see [here](https://pysal.org/access/).
```

### Comparing `access-1.1.8/setup.py` & `access-1.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from setuptools import setup, find_packages
 from distutils.command.build_py import build_py
+import versioneer
 
-# Get __version__ from access/__init__.py without importing the package
-# __version__ has to be defined in the first line
-with open("access/__init__.py", "r") as f:
-    exec(f.readline())
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def _get_requirements_from_files(groups_files):
     groups_reqlist = {}
@@ -30,15 +27,16 @@
     }
     reqs = _get_requirements_from_files(_groups_files)
     install_reqs = reqs.pop("base")
     extras_reqs = reqs
 
     setup(
         name="access",  # name of package
-        version=__version__,
+        version=versioneer.get_version(),
+        cmdclass=versioneer.get_cmdclass({"build_py": build_py}),
         description="Calculate spatial accessibility metrics.",  # short <80chr description
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://access.readthedocs.io/en/latest/",  # github repo
         maintainer="James Saxon",
         maintainer_email="jsaxon@uchicago.edu",
         keywords="spatial statistics access",
@@ -57,14 +55,13 @@
             "Programming Language :: Python :: 3.10",
         ],
         license="3-Clause BSD",
         packages=find_packages(),
         install_requires=install_reqs,
         extras_require=extras_reqs,
         zip_safe=False,
-        cmdclass={"build.py": build_py},
     )
 
 
 if __name__ == "__main__":
 
     setup_package()
```

