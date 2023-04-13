# Comparing `tmp/fio_planet-1.0a3.tar.gz` & `tmp/fio_planet-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio_planet-1.0a3.tar", last modified: Fri Mar 24 23:17:08 2023, max compression
+gzip compressed data, was "fio_planet-1.0b1.tar", last modified: Thu Apr 13 20:04:26 2023, max compression
```

## Comparing `fio_planet-1.0a3.tar` & `fio_planet-1.0b1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0      665 2023-03-24 23:15:42.038604 fio_planet-1.0a3/CHANGES
--rw-r--r--   0        0        0     1986 2023-02-23 00:01:33.519549 fio_planet-1.0a3/CODE_OF_CONDUCT
--rw-r--r--   0        0        0    11357 2022-08-17 03:32:15.691492 fio_planet-1.0a3/LICENSE
--rw-r--r--   0        0        0     5691 2023-03-23 18:41:02.025156 fio_planet-1.0a3/README.md
--rw-r--r--   0        0        0     1379 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/custom_theme/main.html
--rw-r--r--   0        0        0     7116 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/images/Planet_primarymark_RGB_White.png
--rw-r--r--   0        0        0    36552 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg
--rw-r--r--   0        0        0      655 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/images/logo.svg
--rw-r--r--   0        0        0     5379 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/index.md
--rw-r--r--   0        0        0     2091 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0       72 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/topics/index.md
--rw-r--r--   0        0        0     3216 2023-03-23 18:41:02.025156 fio_planet-1.0a3/docs/topics/simplification.md
--rw-r--r--   0        0        0     1729 2023-03-23 18:41:02.025156 fio_planet-1.0a3/mkdocs.yml
--rw-r--r--   0        0        0     1103 2023-03-24 23:05:30.009346 fio_planet-1.0a3/pyproject.toml
--rw-r--r--   0        0        0      722 2023-03-24 23:15:32.755139 fio_planet-1.0a3/src/fio_planet/__init__.py
--rw-r--r--   0        0        0     7860 2023-02-24 22:53:46.364309 fio_planet-1.0a3/src/fio_planet/cli.py
--rw-r--r--   0        0        0      215 2023-02-22 22:59:34.511203 fio_planet-1.0a3/src/fio_planet/errors.py
--rw-r--r--   0        0        0     9132 2023-03-24 23:13:15.822377 fio_planet-1.0a3/src/fio_planet/features.py
--rw-r--r--   0        0        0     8341 2023-03-24 23:05:30.009346 fio_planet-1.0a3/src/fio_planet/snuggs.py
--rw-r--r--   0        0        0    12885 2023-03-01 18:07:06.527365 fio_planet-1.0a3/tests/data/rmnp.geojson
--rw-r--r--   0        0        0     1555 2022-07-19 23:23:14.749589 fio_planet-1.0a3/tests/data/trio.geojson
--rw-r--r--   0        0        0      805 2022-07-19 23:23:14.749589 fio_planet-1.0a3/tests/data/trio.seq
--rw-r--r--   0        0        0     3370 2023-03-24 23:05:30.009346 fio_planet-1.0a3/tests/test_cli.py
--rw-r--r--   0        0        0    10638 2023-03-24 23:05:30.009346 fio_planet-1.0a3/tests/test_mod.py
--rw-r--r--   0        0        0      436 2023-03-24 23:05:30.009346 fio_planet-1.0a3/tox.ini
--rw-r--r--   0        0        0     6500 1970-01-01 00:00:00.000000 fio_planet-1.0a3/PKG-INFO
+-rw-r--r--   0        0        0      164 2023-03-30 20:10:41.857799 fio_planet-1.0b1/.readthedocs.yml
+-rw-r--r--   0        0        0      809 2023-04-13 19:55:49.739453 fio_planet-1.0b1/CHANGES
+-rw-r--r--   0        0        0     1986 2023-03-30 20:10:41.857799 fio_planet-1.0b1/CODE_OF_CONDUCT
+-rw-r--r--   0        0        0    11357 2023-03-30 20:10:41.857799 fio_planet-1.0b1/LICENSE
+-rw-r--r--   0        0        0     4507 2023-04-13 19:52:55.913276 fio_planet-1.0b1/README.md
+-rw-r--r--   0        0        0     1428 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/commands.md
+-rw-r--r--   0        0        0     1379 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/custom_theme/main.html
+-rw-r--r--   0        0        0     4827 2023-04-13 19:52:55.913276 fio_planet-1.0b1/docs/expressions.md
+-rw-r--r--   0        0        0     7116 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/images/Planet_primarymark_RGB_White.png
+-rw-r--r--   0        0        0    36552 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg
+-rw-r--r--   0        0        0      655 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/images/logo.svg
+-rw-r--r--   0        0        0     3955 2023-04-13 19:53:16.401533 fio_planet-1.0b1/docs/index.md
+-rw-r--r--   0        0        0      169 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/requirements.txt
+-rw-r--r--   0        0        0     2091 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0       72 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/topics/index.md
+-rw-r--r--   0        0        0     4010 2023-03-30 20:10:41.857799 fio_planet-1.0b1/docs/topics/simplification.md
+-rw-r--r--   0        0        0     1795 2023-04-13 19:52:55.913276 fio_planet-1.0b1/mkdocs.yml
+-rw-r--r--   0        0        0     1107 2023-04-13 19:52:55.913276 fio_planet-1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      722 2023-04-13 19:53:56.058030 fio_planet-1.0b1/src/fio_planet/__init__.py
+-rw-r--r--   0        0        0     7860 2023-04-12 20:23:10.271883 fio_planet-1.0b1/src/fio_planet/cli.py
+-rw-r--r--   0        0        0      215 2023-03-30 20:10:41.857799 fio_planet-1.0b1/src/fio_planet/errors.py
+-rw-r--r--   0        0        0     9132 2023-04-12 20:23:10.271883 fio_planet-1.0b1/src/fio_planet/features.py
+-rw-r--r--   0        0        0     8341 2023-03-30 20:10:41.857799 fio_planet-1.0b1/src/fio_planet/snuggs.py
+-rw-r--r--   0        0        0    12885 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/data/rmnp.geojson
+-rw-r--r--   0        0        0     1555 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/data/trio.geojson
+-rw-r--r--   0        0        0      805 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/data/trio.seq
+-rw-r--r--   0        0        0     3370 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/test_cli.py
+-rw-r--r--   0        0        0    10638 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tests/test_mod.py
+-rw-r--r--   0        0        0      436 2023-03-30 20:10:41.857799 fio_planet-1.0b1/tox.ini
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 fio_planet-1.0b1/PKG-INFO
```

### Comparing `fio_planet-1.0a3/CHANGES` & `fio_planet-1.0b1/CHANGES`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes
 =======
 
+1.0b1 (2023-04-18)
+------------------
+
+- Require pyparsing >= 3.0 (#29).
+- Added a documentation site hosted on Read the Docs (#26, #28, #32).
+
 1.0a3 (2023-03-24)
 ------------------
 
 - Add shapely.ops functions (#23).
 - Add builtin buffer, distance, length, simplify, and set_precision functions
   which allow projected computation of these values (#27).
```

### Comparing `fio_planet-1.0a3/CODE_OF_CONDUCT` & `fio_planet-1.0b1/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/LICENSE` & `fio_planet-1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/README.md` & `fio_planet-1.0b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,143 +1,126 @@
+Metadata-Version: 2.1
+Name: fio_planet
+Version: 1.0b1
+Summary: fio_planet: Fiona CLI plugins from Planet Labs.
+Keywords: GeoJSON,GIS,CLI
+Author: Sean Gillies
+Maintainer-email: Planet Developer Relations <developers@planet.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: click
+Requires-Dist: fiona
+Requires-Dist: pyparsing>=3.0
+Requires-Dist: shapely>=2.0
+Requires-Dist: mkdocs ; extra == "docs"
+Requires-Dist: mkdocs-material ; extra == "docs"
+Requires-Dist: mkdocs-click ; extra == "docs"
+Requires-Dist: mkdocstrings ; extra == "docs"
+Requires-Dist: pytest-cov ; extra == "test"
+Provides-Extra: docs
+Provides-Extra: test
+
 fio-planet
 ==========
 
 A package of Fiona CLI plugins from Planet Labs.
 
 [![](https://github.com/planetlabs/fio-planet/actions/workflows/check.yml/badge.svg)](https://github.com/planetlabs/fio-planet/actions/workflows/check.yml)
-
 [![](https://github.com/planetlabs/fio-planet/actions/workflows/test.yml/badge.svg)](https://github.com/planetlabs/fio-planet/actions/workflows/test.yml)
+[![Documentation Status](https://readthedocs.org/projects/fio-planet/badge/?version=latest)](https://fio-planet.readthedocs.io/en/latest/?badge=latest)
 
-These commands are for creating Unix pipelines which manipulate streams of
+These CLI commands are for creating Unix pipelines which manipulate streams of
 GeoJSON features. Such pipelines provide a subset of the functionality of more
-complicated tools such as PostGIS or GeoPandas and are intended for use with
-streams of hundreds to thousands of features, where the overhead of JSON
-serialization between pieces of a pipeline is tolerable.
+complicated tools such as GeoPandas, PostGIS, or QGIS, and are intended for use
+with streams of hundreds of features, where the overhead of JSON serialization
+between pieces of a pipeline is tolerable.
+
 
 Installation
 ------------
 
 ```
 python -m pip install --user --pre fio-planet
 ```
 
 Usage
 -----
 
 fio-planet adds `filter`, `map`, and `reduce` commands to Fiona's `fio`
-program. fio-filter evaluates an expression for each feature in a stream of
-GeoJSON features, passing those for which the expression is true. fio-map maps
-an expression over a stream of GeoJSON features, producing a stream of new
-features or other values. fio-reduce applies an expression to a sequence of
-GeoJSON features, reducing them to a single feature or other value.
-
-These commands provide some of the features of spatial SQL, but act on
-features in a GeoJSON feature sequence instead of rows in a spatial table.
-fio-filter decimates a seqence of features, fio-map multiplies features, and
-fio-reduce turns a sequence of many features into a sequence of exactly one.
-In combination, many transformations are possible.
+program. These commands afford some of the capabilities of spatial SQL, but act
+on features of a GeoJSON feature sequence instead of rows of a spatial RDBMS
+table.  fio-filter decimates a seqence of features, fio-map multiplies and
+transforms features, and fio-reduce turns a sequence of many features into a
+sequence of exactly one.  In combination, many transformations are possible.
 
 Expressions take the form of parenthesized lists which may contain other
 expressions. The first item in a list is the name of a function or method, or
 an expression that evaluates to a function. The second item is the function's
 first argument or the object to which the method is bound. The remaining list
 items are the positional and keyword arguments for the named function or
-method. The list of functions and callables available in expressions includes:
+method. The list of functions and callables available in an expression
+includes:
 
+* Python operators such as `+`, `/`, and `<=`
 * Python builtins such as `dict`, `list`, and `map`
-* From functools: `reduce`.
 * All public functions from itertools, e.g. `islice`, and `repeat`
-* All functions importable from Shapely 2.0, e.g. `Point`, and
-  `unary_union`
-* All methods of Shapely geometry classes.
-
-Here's an expression that evaluates to a Shapely Point instance. `Point` is a
-callable instance constructor and the pair of `0` values are positional
-arguments. Note that the outermost parentheses of an expression are optional.
+* All functions importable from Shapely 2.0, e.g. `Point`, and `unary_union`
+* All methods of Shapely geometry classes
+* Functions specific to fio-planet
+
+Here's an expression that evaluates to a Shapely Point instance.
 
 ```lisp
 (Point 0 0)
 ```
 
-Here's an expression that evaluates to a Polygon, using `buffer`. The inner
-expression `(Point 0 0)` evaluates to a Shapely Point instance, `buffer`
-evaluates to its instance method, and `:distance 1.0` assigns a value of 1.0
-to that method's `distance` keyword argument.
+`Point` is a callable instance constructor and the pair of `0` values are
+positional arguments. Note that the outermost parentheses of an expression are
+optional.
+
+Here's an expression that evaluates to a Polygon, using `buffer`.
 
 ```lisp
 buffer (Point 0 0) :distance 1.0
 ```
 
+The inner expression `(Point 0 0)` evaluates to a Shapely Point instance,
+`buffer` evaluates to `shapely.buffer()`, and `:distance 1.0` assigns a value
+of 1.0 to that method's `distance` keyword argument.
+
+In a fio-planet expression, all coordinates and geometry objects are in the
+`OGC:CRS84` reference system, like GeoJSON. However, function arguments related
+to length or area, such as buffer's distance argument, are understood to have
+units of meters.
+
 fio-filter and fio-map evaluate expressions in the context of a GeoJSON feature
-and its geometry attribute. These are named `f` and `g`. For example, here
-is an expression that tests whether the input feature is within a distance
-`1.0` of a given point.
+and its geometry attribute. These are named `f` and `g`. For example, here is
+an expression that tests whether the input feature is within 50 meters of the
+given point.
 
 ```lisp
-<= (distance g (Point 0 0)) 1.0
+<= (distance g (Point -105.0 39.753056)) 50.0
 ```
 
 fio-reduce evaluates expressions in the context of the sequence of all input
 geometries, which is named `c`. For example, this expression dissolves input
 geometries using Shapely's `unary_union`.
 
 ```lisp
 unary_union c
 ```
 
-fio-filter
-----------
-
-For each feature read from stdin, fio-filter evaluates a pipeline of one or
-more steps described using methods from the Shapely library in Lisp-like
-expressions. If the pipeline expression evaluates to True, the feature passes
-through the filter. Otherwise the feature does not pass.
-
-For example, this pipeline expression
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio filter '< (distance g (Point -109.0 38.5)) 1'
-```
-
-lets through all features that are less than one unit from the given point and
-filters out all other features.
-
-fio-map
--------
-
-For each feature read from stdin, fio-map applies a transformation pipeline and
-writes a copy of the feature, containing the modified geometry, to stdout. For
-example, polygonal features can be "cleaned" by using a `buffer g 0`
-pipeline.
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio map 'buffer g 0'
-```
-
-fio-reduce
-----------
-
-Given a sequence of GeoJSON features (RS-delimited or not) on stdin this prints
-a single value using a provided transformation pipeline.  The set of geometries
-of the input features in the context of these expressions is named "c".
-
-For example, the pipeline expression
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio reduce 'unary_union c'
-```
-
-dissolves the geometries of input features.
-
 Support
 -------
 
+Documentation is hosted at Read the Docs: https://fio-planet.readthedocs.io/en/latest/.
+
 For usage help, please use the project discussion forum or email
 developers@planet.com.
 
 If you think you've found a bug, please use the project issue tracker.
 
 Roadmap
 -------
@@ -167,7 +150,8 @@
 
 * Sean Gillies <sean.gillies@planet.com>
 
 License
 -------
 
 Apache License, Version 2.0.
+
```

### Comparing `fio_planet-1.0a3/docs/custom_theme/main.html` & `fio_planet-1.0b1/docs/custom_theme/main.html`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/docs/images/Planet_primarymark_RGB_White.png` & `fio_planet-1.0b1/docs/images/Planet_primarymark_RGB_White.png`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg` & `fio_planet-1.0b1/docs/images/SatelliteOrbits-main100Dove4RapidEye6Skysat-100mm01-pulsing.svg`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/docs/images/logo.svg` & `fio_planet-1.0b1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/docs/index.md` & `fio_planet-1.0b1/docs/index.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,136 +1,93 @@
 fio-planet
 ==========
 
-A package of Fiona CLI plugins from Planet Labs.
+A package of [Fiona CLI](https://fiona.readthedocs.io/en/stable/cli.html)
+plugins from Planet Labs.
 
-These commands are for creating Unix pipelines which manipulate streams of
+These CLI commands are for creating Unix pipelines which manipulate streams of
 GeoJSON features. Such pipelines provide a subset of the functionality of more
-complicated tools such as PostGIS or GeoPandas and are intended for use with
-streams of hundreds to thousands of features, where the overhead of JSON
-serialization between pieces of a pipeline is tolerable.
+complicated tools such as GeoPandas, PostGIS, or QGIS, and are intended for use
+with streams of hundreds of features, where the overhead of JSON serialization
+between pieces of a pipeline is tolerable.
 
 Installation
 ------------
 
 ```
 python -m pip install --user --pre fio-planet
 ```
 
 Usage
 -----
 
 fio-planet adds `filter`, `map`, and `reduce` commands to Fiona's `fio`
-program. fio-filter evaluates an expression for each feature in a stream of
-GeoJSON features, passing those for which the expression is true. fio-map maps
-an expression over a stream of GeoJSON features, producing a stream of new
-features or other values. fio-reduce applies an expression to a sequence of
-GeoJSON features, reducing them to a single feature or other value.
-
-These commands provide some of the features of spatial SQL, but act on
-features in a GeoJSON feature sequence instead of rows in a spatial table.
-fio-filter decimates a seqence of features, fio-map multiplies features, and
-fio-reduce turns a sequence of many features into a sequence of exactly one.
-In combination, many transformations are possible.
+program. These commands afford some of the capabilities of spatial SQL, but act
+on features of a GeoJSON feature sequence instead of rows of a spatial RDBMS
+table.  fio-filter decimates a seqence of features, fio-map multiplies and
+transforms features, and fio-reduce turns a sequence of many features into a
+sequence of exactly one.  In combination, many transformations are possible.
 
 Expressions take the form of parenthesized lists which may contain other
 expressions. The first item in a list is the name of a function or method, or
 an expression that evaluates to a function. The second item is the function's
 first argument or the object to which the method is bound. The remaining list
 items are the positional and keyword arguments for the named function or
-method. The list of functions and callables available in expressions includes:
+method. The list of functions and callables available in an expression
+includes:
 
 * Python builtins such as `dict`, `list`, and `map`
 * From functools: `reduce`.
 * All public functions from itertools, e.g. `islice`, and `repeat`
 * All functions importable from Shapely 2.0, e.g. `Point`, and
   `unary_union`
 * All methods of Shapely geometry classes.
 
-Here's an expression that evaluates to a Shapely Point instance. `Point` is a
-callable instance constructor and the pair of `0` values are positional
-arguments. Note that the outermost parentheses of an expression are optional.
+Here's an expression that evaluates to a Shapely Point instance.
 
 ```lisp
 (Point 0 0)
 ```
 
-Here's an expression that evaluates to a Polygon, using `buffer`. The inner
-expression `(Point 0 0)` evaluates to a Shapely Point instance, `buffer`
-evaluates to its instance method, and `:distance 1.0` assigns a value of 1.0
-to that method's `distance` keyword argument.
+`Point` is a callable instance constructor and the pair of `0` values are
+positional arguments. Note that the outermost parentheses of an expression are
+optional.
+
+Here's an expression that evaluates to a Polygon, using `buffer`.
 
 ```lisp
 buffer (Point 0 0) :distance 1.0
 ```
 
+The inner expression `(Point 0 0)` evaluates to a Shapely Point instance,
+`buffer` evaluates to `shapely.buffer()`, and `:distance 1.0` assigns a value
+of 1.0 to that method's `distance` keyword argument.
+
+In a fio-planet expression, all coordinates and geometry objects are in the
+`OGC:CRS84` reference system, like GeoJSON. However, function arguments related
+to length or area, such as buffer's distance argument, are understood to have
+units of meters.
+
 fio-filter and fio-map evaluate expressions in the context of a GeoJSON feature
-and its geometry attribute. These are named `f` and `g`. For example, here
-is an expression that tests whether the input feature is within a distance
-`1.0` of a given point.
+and its geometry attribute. These are named `f` and `g`. For example, here is
+an expression that tests whether the input feature is within 50 meters of the
+given point.
 
 ```lisp
-<= (distance g (Point 0 0)) 1.0
+<= (distance g (Point -105.0 39.753056)) 50.0
 ```
 
 fio-reduce evaluates expressions in the context of the sequence of all input
 geometries, which is named `c`. For example, this expression dissolves input
 geometries using Shapely's `unary_union`.
 
 ```lisp
 unary_union c
 ```
 
-fio-filter
-----------
-
-For each feature read from stdin, fio-filter evaluates a pipeline of one or
-more steps described using methods from the Shapely library in Lisp-like
-expressions. If the pipeline expression evaluates to True, the feature passes
-through the filter. Otherwise the feature does not pass.
-
-For example, this pipeline expression
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio filter '< (distance g (Point -109.0 38.5)) 1'
-```
-
-lets through all features that are less than one unit from the given point and
-filters out all other features.
-
-fio-map
--------
-
-For each feature read from stdin, fio-map applies a transformation pipeline and
-writes a copy of the feature, containing the modified geometry, to stdout. For
-example, polygonal features can be "cleaned" by using a `buffer g 0`
-pipeline.
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio map 'buffer g 0'
-```
-
-fio-reduce
-----------
-
-Given a sequence of GeoJSON features (RS-delimited or not) on stdin this prints
-a single value using a provided transformation pipeline.  The set of geometries
-of the input features in the context of these expressions is named "c".
-
-For example, the pipeline expression
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio reduce 'unary_union c'
-```
-
-dissolves the geometries of input features.
-
 Support
 -------
 
 For usage help, please use the project discussion forum or email
 developers@planet.com.
 
 If you think you've found a bug, please use the project issue tracker.
```

### Comparing `fio_planet-1.0a3/docs/stylesheets/extra.css` & `fio_planet-1.0b1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/docs/topics/simplification.md` & `fio_planet-1.0b1/docs/topics/simplification.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Simplifying shapes
-==================
+Sizing up and simplifying shapes with fio-planet
+================================================
 
 Here are a few examples related to the Planet Developers Blog deep dive into
 [simplifying areas of interest](https://developers.planet.com/blog/2022/Dec/15/simplifying-your-complex-area-of-interest-a-planet-developers-deep-dive/).
 The examples use a 25-feature shapefile. You can get it from [rmnp.zip](https://github.com/planetlabs/fio-planet/files/10045442/rmnp.zip) or access
 it in a streaming fashion as shown in the examples below.
 
 Counting vertices in a feature collection
@@ -28,22 +28,37 @@
 
 Counting vertices after making a simplified buffer
 --------------------------------------------------
 
 One traditional way of simplifying an area of interest is to buffer and
 simplify. There's no need to use jq here because fio-reduce prints out a
 sequence of exactly one feature. The effectiveness of this method depends a bit
-on the nature of the data, especially the distance between vertices.
+on the nature of the data, especially the distance between vertices. The total
+length of the perimeters of all zones is 889 kilometers.
+
+```
+fio cat zip+https://github.com/planetlabs/fio-planet/files/10045442/rmnp.zip \
+| fio map 'length g' --raw \
+| jq -s 'add'
+889332.0900809917
+```
+
+The mean distance between vertices on the edges of zones is 889332 / 28915, or
+30.7 meters.  You need to buffer and simplify by this value or more to get a
+significant reduction in the number of vertices. Choosing 40 as a buffer
+distance and simplification tolerance results in a shape with 469 vertices.
+It's a suitable area of interest for Planet APIs that require this number to be
+less than 500.
 
 ```
 fio cat zip+https://github.com/planetlabs/fio-planet/files/10045442/rmnp.zip \
 | fio reduce 'unary_union c' \
-| fio map 'simplify (buffer g 0.001) 0.001' \
+| fio map 'simplify (buffer g 40) 40' \
 | fio map 'vertex_count g' --raw
-274
+469
 ```
 
 ![](https://user-images.githubusercontent.com/33697/202821086-5bfd4437-3c42-420e-84cf-d3e1287d2d8c.png)
 
 Counting vertices after dissolving convex hulls of features
 -----------------------------------------------------------
 
@@ -62,19 +77,21 @@
 ```
 
 ![](https://user-images.githubusercontent.com/33697/202820595-491c590c-0f5a-4cdb-89de-7cd2067cbf90.png)
 
 Counting vertices after dissolving concave hulls of features
 ------------------------------------------------------------
 
-Convex hulls simplify, but also dilate concave areas of interest. This can be
-undesirable. Concave hulls inflate your areas less.
+Convex hulls simplify, but also dilate concave areas of interest. They fill the
+"bays", so to speak, and this can be undesirable. Concave hulls do a better job
+at preserving the concave nature of a shape and result in a smaller increase of
+area.
 
 ```
 fio cat zip+https://github.com/planetlabs/fio-planet/files/10045442/rmnp.zip \
-| fio map 'concave_hull g 0.4' --dump-parts \
+| fio map 'concave_hull g :ratio 0.4' --dump-parts \
 | fio reduce 'unary_union c' \
 | fio map 'vertex_count g' --raw
 301
 ```
 
 ![](https://user-images.githubusercontent.com/33697/218189621-446b743e-daba-4e3c-bc24-7ce74771fb8a.png)
```

### Comparing `fio_planet-1.0a3/mkdocs.yml` & `fio_planet-1.0b1/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,16 @@
               - "^__init__$"  # but always include __init__ modules and methods
       watch:
         - src/fio_planet
         - docs/custom_theme/
 
 nav:
   - "Home": 'index.md'
+  - "Commands": 'commands.md'
+  - "Expressions": 'expressions.md'
   - "Topics": 'topics'
 
 markdown_extensions:
   - pymdownx.highlight
   - pymdownx.superfences
   - mkdocs-click
   - admonition
```

### Comparing `fio_planet-1.0a3/pyproject.toml` & `fio_planet-1.0b1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 dynamic = ["version", "description"]
 readme = "README.md"
 authors = [{name = "Sean Gillies"}]
 maintainers = [
     {name = "Planet Developer Relations", email = "developers@planet.com"}
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 keywords = [
     "GeoJSON",
     "GIS",
     "CLI",
 ]
 license = {text = "Apache License, Version 2.0"}
 requires-python = ">=3.7"
 dependencies = [
     "click",
     "fiona",
-    "pyparsing",
+    "pyparsing>=3.0",
     "shapely>=2.0",
 ]
 
 [tool.flit.sdist]
 exclude = [".github/", ".gitignore"]
 
 [project.optional-dependencies]
```

### Comparing `fio_planet-1.0a3/src/fio_planet/__init__.py` & `fio_planet-1.0b1/src/fio_planet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """fio_planet: Fiona CLI plugins from Planet Labs."""
 
-__version__ = "1.0a3"
+__version__ = "1.0b1"
```

### Comparing `fio_planet-1.0a3/src/fio_planet/cli.py` & `fio_planet-1.0b1/src/fio_planet/cli.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/src/fio_planet/features.py` & `fio_planet-1.0b1/src/fio_planet/features.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/src/fio_planet/snuggs.py` & `fio_planet-1.0b1/src/fio_planet/snuggs.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/tests/data/rmnp.geojson` & `fio_planet-1.0b1/tests/data/rmnp.geojson`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/tests/data/trio.geojson` & `fio_planet-1.0b1/tests/data/trio.geojson`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/tests/data/trio.seq` & `fio_planet-1.0b1/tests/data/trio.seq`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/tests/test_cli.py` & `fio_planet-1.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/tests/test_mod.py` & `fio_planet-1.0b1/tests/test_mod.py`

 * *Files identical despite different names*

### Comparing `fio_planet-1.0a3/PKG-INFO` & `fio_planet-1.0b1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,167 +1,102 @@
-Metadata-Version: 2.1
-Name: fio_planet
-Version: 1.0a3
-Summary: fio_planet: Fiona CLI plugins from Planet Labs.
-Keywords: GeoJSON,GIS,CLI
-Author: Sean Gillies
-Maintainer-email: Planet Developer Relations <developers@planet.com>
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: click
-Requires-Dist: fiona
-Requires-Dist: pyparsing
-Requires-Dist: shapely>=2.0
-Requires-Dist: mkdocs ; extra == "docs"
-Requires-Dist: mkdocs-material ; extra == "docs"
-Requires-Dist: mkdocs-click ; extra == "docs"
-Requires-Dist: mkdocstrings ; extra == "docs"
-Requires-Dist: pytest-cov ; extra == "test"
-Provides-Extra: docs
-Provides-Extra: test
-
 fio-planet
 ==========
 
 A package of Fiona CLI plugins from Planet Labs.
 
 [![](https://github.com/planetlabs/fio-planet/actions/workflows/check.yml/badge.svg)](https://github.com/planetlabs/fio-planet/actions/workflows/check.yml)
-
 [![](https://github.com/planetlabs/fio-planet/actions/workflows/test.yml/badge.svg)](https://github.com/planetlabs/fio-planet/actions/workflows/test.yml)
+[![Documentation Status](https://readthedocs.org/projects/fio-planet/badge/?version=latest)](https://fio-planet.readthedocs.io/en/latest/?badge=latest)
 
-These commands are for creating Unix pipelines which manipulate streams of
+These CLI commands are for creating Unix pipelines which manipulate streams of
 GeoJSON features. Such pipelines provide a subset of the functionality of more
-complicated tools such as PostGIS or GeoPandas and are intended for use with
-streams of hundreds to thousands of features, where the overhead of JSON
-serialization between pieces of a pipeline is tolerable.
+complicated tools such as GeoPandas, PostGIS, or QGIS, and are intended for use
+with streams of hundreds of features, where the overhead of JSON serialization
+between pieces of a pipeline is tolerable.
+
 
 Installation
 ------------
 
 ```
 python -m pip install --user --pre fio-planet
 ```
 
 Usage
 -----
 
 fio-planet adds `filter`, `map`, and `reduce` commands to Fiona's `fio`
-program. fio-filter evaluates an expression for each feature in a stream of
-GeoJSON features, passing those for which the expression is true. fio-map maps
-an expression over a stream of GeoJSON features, producing a stream of new
-features or other values. fio-reduce applies an expression to a sequence of
-GeoJSON features, reducing them to a single feature or other value.
-
-These commands provide some of the features of spatial SQL, but act on
-features in a GeoJSON feature sequence instead of rows in a spatial table.
-fio-filter decimates a seqence of features, fio-map multiplies features, and
-fio-reduce turns a sequence of many features into a sequence of exactly one.
-In combination, many transformations are possible.
+program. These commands afford some of the capabilities of spatial SQL, but act
+on features of a GeoJSON feature sequence instead of rows of a spatial RDBMS
+table.  fio-filter decimates a seqence of features, fio-map multiplies and
+transforms features, and fio-reduce turns a sequence of many features into a
+sequence of exactly one.  In combination, many transformations are possible.
 
 Expressions take the form of parenthesized lists which may contain other
 expressions. The first item in a list is the name of a function or method, or
 an expression that evaluates to a function. The second item is the function's
 first argument or the object to which the method is bound. The remaining list
 items are the positional and keyword arguments for the named function or
-method. The list of functions and callables available in expressions includes:
+method. The list of functions and callables available in an expression
+includes:
 
+* Python operators such as `+`, `/`, and `<=`
 * Python builtins such as `dict`, `list`, and `map`
-* From functools: `reduce`.
 * All public functions from itertools, e.g. `islice`, and `repeat`
-* All functions importable from Shapely 2.0, e.g. `Point`, and
-  `unary_union`
-* All methods of Shapely geometry classes.
-
-Here's an expression that evaluates to a Shapely Point instance. `Point` is a
-callable instance constructor and the pair of `0` values are positional
-arguments. Note that the outermost parentheses of an expression are optional.
+* All functions importable from Shapely 2.0, e.g. `Point`, and `unary_union`
+* All methods of Shapely geometry classes
+* Functions specific to fio-planet
+
+Here's an expression that evaluates to a Shapely Point instance.
 
 ```lisp
 (Point 0 0)
 ```
 
-Here's an expression that evaluates to a Polygon, using `buffer`. The inner
-expression `(Point 0 0)` evaluates to a Shapely Point instance, `buffer`
-evaluates to its instance method, and `:distance 1.0` assigns a value of 1.0
-to that method's `distance` keyword argument.
+`Point` is a callable instance constructor and the pair of `0` values are
+positional arguments. Note that the outermost parentheses of an expression are
+optional.
+
+Here's an expression that evaluates to a Polygon, using `buffer`.
 
 ```lisp
 buffer (Point 0 0) :distance 1.0
 ```
 
+The inner expression `(Point 0 0)` evaluates to a Shapely Point instance,
+`buffer` evaluates to `shapely.buffer()`, and `:distance 1.0` assigns a value
+of 1.0 to that method's `distance` keyword argument.
+
+In a fio-planet expression, all coordinates and geometry objects are in the
+`OGC:CRS84` reference system, like GeoJSON. However, function arguments related
+to length or area, such as buffer's distance argument, are understood to have
+units of meters.
+
 fio-filter and fio-map evaluate expressions in the context of a GeoJSON feature
-and its geometry attribute. These are named `f` and `g`. For example, here
-is an expression that tests whether the input feature is within a distance
-`1.0` of a given point.
+and its geometry attribute. These are named `f` and `g`. For example, here is
+an expression that tests whether the input feature is within 50 meters of the
+given point.
 
 ```lisp
-<= (distance g (Point 0 0)) 1.0
+<= (distance g (Point -105.0 39.753056)) 50.0
 ```
 
 fio-reduce evaluates expressions in the context of the sequence of all input
 geometries, which is named `c`. For example, this expression dissolves input
 geometries using Shapely's `unary_union`.
 
 ```lisp
 unary_union c
 ```
 
-fio-filter
-----------
-
-For each feature read from stdin, fio-filter evaluates a pipeline of one or
-more steps described using methods from the Shapely library in Lisp-like
-expressions. If the pipeline expression evaluates to True, the feature passes
-through the filter. Otherwise the feature does not pass.
-
-For example, this pipeline expression
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio filter '< (distance g (Point -109.0 38.5)) 1'
-```
-
-lets through all features that are less than one unit from the given point and
-filters out all other features.
-
-fio-map
--------
-
-For each feature read from stdin, fio-map applies a transformation pipeline and
-writes a copy of the feature, containing the modified geometry, to stdout. For
-example, polygonal features can be "cleaned" by using a `buffer g 0`
-pipeline.
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio map 'buffer g 0'
-```
-
-fio-reduce
-----------
-
-Given a sequence of GeoJSON features (RS-delimited or not) on stdin this prints
-a single value using a provided transformation pipeline.  The set of geometries
-of the input features in the context of these expressions is named "c".
-
-For example, the pipeline expression
-
-```
-$ fio cat zip+https://s3.amazonaws.com/fiona-testing/coutwildrnp.zip \
-| fio reduce 'unary_union c'
-```
-
-dissolves the geometries of input features.
-
 Support
 -------
 
+Documentation is hosted at Read the Docs: https://fio-planet.readthedocs.io/en/latest/.
+
 For usage help, please use the project discussion forum or email
 developers@planet.com.
 
 If you think you've found a bug, please use the project issue tracker.
 
 Roadmap
 -------
@@ -191,8 +126,7 @@
 
 * Sean Gillies <sean.gillies@planet.com>
 
 License
 -------
 
 Apache License, Version 2.0.
-
```

