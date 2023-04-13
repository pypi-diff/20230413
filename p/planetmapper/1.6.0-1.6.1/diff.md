# Comparing `tmp/planetmapper-1.6.0.tar.gz` & `tmp/planetmapper-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.6.0.tar", last modified: Wed Apr  5 09:59:42 2023, max compression
+gzip compressed data, was "planetmapper-1.6.1.tar", last modified: Thu Apr 13 16:41:52 2023, max compression
```

## Comparing `planetmapper-1.6.0.tar` & `planetmapper-1.6.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:59:42.246589 planetmapper-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-05 09:59:42.246589 planetmapper-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-05 09:59:29.000000 planetmapper-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:59:42.246589 planetmapper-1.6.0/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   100081 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:59:42.246589 planetmapper-1.6.0/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   106910 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    42838 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-05 09:59:29.000000 planetmapper-1.6.0/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:59:42.246589 planetmapper-1.6.0/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-05 09:59:42.000000 planetmapper-1.6.0/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-05 09:59:42.000000 planetmapper-1.6.0/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:59:42.000000 planetmapper-1.6.0/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-05 09:59:42.000000 planetmapper-1.6.0/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-05 09:59:42.000000 planetmapper-1.6.0/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 09:59:42.000000 planetmapper-1.6.0/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-05 09:59:29.000000 planetmapper-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:59:42.246589 planetmapper-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-05 09:59:29.000000 planetmapper-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:59:42.246589 planetmapper-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    22098 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    16976 2023-04-05 09:59:29.000000 planetmapper-1.6.0/tests/test_observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.399560 planetmapper-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-13 16:41:52.399560 planetmapper-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-13 16:41:41.000000 planetmapper-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.395560 planetmapper-1.6.1/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.395560 planetmapper-1.6.1/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108552 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42961 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.395560 planetmapper-1.6.1/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 16:41:41.000000 planetmapper-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:41:52.399560 planetmapper-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-13 16:41:41.000000 planetmapper-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.399560 planetmapper-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_utils.py
```

### Comparing `planetmapper-1.6.0/PKG-INFO` & `planetmapper-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
 Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 # PlanetMapper
 
-[![PyPI](https://img.shields.io/pypi/v/planetmapper?logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
+[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
 [![Upload Python Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
 [![Black](https://github.com/ortk95/planetmapper/actions/workflows/black.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/black.yml)
 [![Tests](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `planetmapper-1.6.0/README.md` & `planetmapper-1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PlanetMapper
 
-[![PyPI](https://img.shields.io/pypi/v/planetmapper?logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
+[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
 [![Upload Python Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
 [![Black](https://github.com/ortk95/planetmapper/actions/workflows/black.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/black.yml)
 [![Tests](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `planetmapper-1.6.0/planetmapper/__init__.py` & `planetmapper-1.6.1/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper/base.py` & `planetmapper-1.6.1/planetmapper/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return self._get_equality_tuple() == other._get_equality_tuple()
 
     def _get_equality_tuple(self) -> tuple:
-        return (self._optimize_speed,)
+        return (self._optimize_speed, repr(self))
 
     def standardise_body_name(self, name: str | int) -> str:
         """
         Return a standardised version of the name of a SPICE body.
 
         This converts the provided `name` into the SPICE ID code with `spice.bods2c`,
         then back into a string with `spice.bodc2s`. This standardises to the version of
```

### Comparing `planetmapper-1.6.0/planetmapper/basic_body.py` & `planetmapper-1.6.1/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper/body.py` & `planetmapper-1.6.1/planetmapper/body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper/body_xy.py` & `planetmapper-1.6.1/planetmapper/body_xy.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,39 +34,15 @@
 from .progress import progress_decorator
 
 T = TypeVar('T')
 S = TypeVar('S')
 P = ParamSpec('P')
 
 
-def _cache_clearable_result(fn: Callable[[S], T]) -> Callable[[S], T]:
-    """
-    Decorator to cache the output of a method call.
-
-    This requires that the class has a `self._cache` dict which can be used to store
-    the cached result. The dictionary key is derived from the name of the decorated
-    function.
-
-    The results cached by this decorator can be cleared using `self._cache.clear()`, so
-    this is useful for results which need to be invalidated (i.e. backplane images
-    which are invalidated the moment the disc params are changed). If the result is
-    stable (i.e. backplane maps) then use `_cache_stable_result` instead.
-    """
-
-    @functools.wraps(fn)
-    def decorated(self):
-        k = fn.__name__
-        if k not in self._cache:
-            self._cache[k] = fn(self)
-        return self._cache[k]
-
-    return decorated
-
-
-def _cache_clearable_result_with_args(
+def _cache_clearable_result(
     fn: Callable[Concatenate[S, P], T]
 ) -> Callable[Concatenate[S, P], T]:
     """
     Decorator to cache the output of a method call with variable arguments.
 
     This requires that the class has a `self._cache` dict which can be used to store
     the cached result. The dictionary key is derived from the name of the decorated
@@ -96,15 +72,15 @@
 ) -> Callable[Concatenate[S, P], T]:
     """
     Decorator to cache stable result
 
     Very roughly, this is a type-hinted version of `functools.lru_cache` that doesn't
     cache self.
 
-    See _cache_clearable_result_with_args for more details.
+    See _cache_clearable_result for more details.
     """
 
     @functools.wraps(fn)
     def decorated(self, *args_in: P.args, **kwargs_in: P.kwargs):
         args, kwargs = _replace_np_arrr_args_with_tuples(args_in, kwargs_in)
         k = (fn.__name__, args, frozenset(kwargs.items()))
         if k not in self._stable_cache:
@@ -1947,15 +1923,15 @@
 
         Returns:
             Array containing cylindrical map of declination values as viewed by the
             observer. Locations which are not visible have a value of NaN.
         """
         return self._get_radec_map(**map_kwargs)[:, :, 1]
 
-    @_cache_clearable_result_with_args
+    @_cache_clearable_result
     @progress_decorator
     def _get_xy_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         out = self._make_empty_map(2, **map_kwargs)
         radec_map = self._get_radec_map(**map_kwargs)
         for a, b in self._iterate_image(out.shape, progress=True):
             ra, dec = radec_map[a, b]
             if not math.isnan(ra):
```

### Comparing `planetmapper-1.6.0/planetmapper/data/rings.json` & `planetmapper-1.6.1/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper/data_loader.py` & `planetmapper-1.6.1/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper/gui.py` & `planetmapper-1.6.1/planetmapper/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,31 +63,35 @@
     'rings': dict(zorder=3.4, color='w', linewidth=0.5, linestyle='solid'),
     'poles': dict(zorder=3.5, color='k', outline_color='w'),
     'coordinates_lonlat': dict(zorder=3.6, marker='x', color='k', s=36),
     'coordinates_radec': dict(zorder=3.7, marker='+', color='k', s=36),
     'other_bodies': dict(zorder=3.8, marker='+', color='w', s=36),
     'other_bodies_labels': dict(zorder=3.81, color='grey'),
     'marked_coord': dict(zorder=4, color='cyan', linewidth=0.5, linestyle='dotted'),
-    'image': dict(zorder=0.9, cmap='inferno', vmin=0, vmax=100),
+    'image': dict(zorder=0.9, cmap='inferno'),
     '_': dict(
         grid_interval=30,
         image_mode='single',
         image_idx_single=0,
         image_idx_r=0,
         image_idx_g=1,
         image_idx_b=2,
         image_gamma=1,
+        image_vmin=0,
+        image_vmax=100,
+        image_limit_type='absolute',
     ),
 }
 
 
 LINESTYLES = ['solid', 'dashed', 'dotted', 'dashdot']
 MARKERS = ['x', '+', 'o', '.', '*', 'v', '^', '<', '>', ',', 'D', 'd', '|', '_']
 GRID_INTERVALS = ['10', '30', '45', '90']
 CMAPS = ['gray', 'viridis', 'plasma', 'inferno', 'magma', 'cividis']
+LIMIT_TYPES = ['absolute', 'percentile']
 
 MAP_INTERPOLATIONS = ('nearest', 'linear', 'quadratic', 'cubic')
 MAP_PROJECTIONS = ('rectangular', 'orthographic', 'azimuthal')
 
 DEFAULT_HINT = (
     'Use the various options in "Find disc" to automatically adjust the disc position'
 )
@@ -1005,20 +1009,30 @@
         self.ax.set_facecolor('0.1')
         self.ax.set_axisbelow(True)
 
     def replot_image(self):
         self.remove_artists('image')
 
         mode = self.plot_settings['_'].setdefault('image_mode', 'single')
+        vmin = self.plot_settings['_'].setdefault('image_vmin', 0)
+        vmax = self.plot_settings['_'].setdefault('image_vmax', 1)
+        limit_type = self.plot_settings['_'].setdefault('image_limit_type', 'absolute')
+
         image = self.image_modes[mode][0]()  # type: ignore
 
+        if limit_type == 'percentile':
+            vmin = np.nanpercentile(image, vmin)
+            vmax = np.nanpercentile(image, vmax)
+
         self.plot_handles['image'].append(
             self.ax.imshow(
                 image,
                 origin='lower',
+                vmin=vmin,
+                vmax=vmax,
                 **self.plot_settings['image'],
             )
         )
 
     def replot_limb(self):
         self.remove_artists('limb')
         self.remove_artists('limb_dayside')
@@ -2309,16 +2323,24 @@
 
 class PlotImageSetting(ArtistSetting):
     def make_menu(self) -> None:
         settings = self.gui.plot_settings[self.key]
         general_settings = self.gui.plot_settings['_']
 
         self.cmap = tk.StringVar(value=settings.setdefault('cmap', 'gray'))
-        self.image_vmin = tk.StringVar(value=str(settings.setdefault('vmin', 0)))
-        self.image_vmax = tk.StringVar(value=str(settings.setdefault('vmax', 100)))
+
+        self.image_vmin = tk.StringVar(
+            value=str(general_settings.setdefault('image_vmin', 0))
+        )
+        self.image_vmax = tk.StringVar(
+            value=str(general_settings.setdefault('image_vmax', 100))
+        )
+        self.image_limit_type = tk.StringVar(
+            value=str(general_settings.setdefault('image_limit_type', 'absolute'))
+        )
 
         self.image_mode = tk.StringVar(
             value=general_settings.setdefault('image_mode', 'single')
         )
         self.image_idx_single = tk.StringVar(
             value=str(general_settings.setdefault('image_idx_single', 0))
         )
@@ -2360,15 +2382,15 @@
                     textvariable=textvariable,
                     from_=0,
                     to=idx_max,
                     increment=1,
                     width=10,
                 )
 
-        self.grid: list[tuple[tk.Widget, tk.Widget, set[IMAGE_MODE]]] = [
+        self.grid: list[tuple[tk.Widget, tk.Widget, set[IMAGE_MODE|Literal['_readonly']]]] = [
             (
                 ttk.Label(frame, text='Wavelength index (single): '),
                 IndexInput(self.image_idx_single),
                 {'single'},
             ),
             (
                 ttk.Label(frame, text='Wavelength index (red): '),
@@ -2427,34 +2449,52 @@
                     from_=0,
                     to=100,
                     increment=5,
                     width=10,
                 ),
                 {'single', 'sum'},
             ),
+            (
+                ttk.Label(frame, text='vmin/vmax type: '),
+                ttk.Combobox(
+                    frame,
+                    textvariable=self.image_limit_type,
+                    values=LIMIT_TYPES,
+                    width=10,
+                    state='readonly',
+                ),
+                {'single', 'sum', '_readonly'},
+            ),
         ]
         self.add_to_menu_grid([(a, b) for a, b, c in self.grid], frame=frame)
 
         msg = '\n'.join(
             [
+                '',
                 'Images are scaled to vary from 0 to 100,',
                 'so set vmin=0 and vmax=100 to show the',
                 'entire dynamic range.',
+                '',
+                'Set vmin/vmax type to "percentile" to',
+                'calculate the limits as percentiles of the',
+                'data in the image. This can be useful if',
+                'your data has extreme outliers (e.g. try',
+                'vmin=1, vmax=99, type=percentile).',
             ]
         )
         ttk.Label(self.grid_frame, text=msg).pack()
 
         self.image_mode.trace_add('write', self.change_image_mode_radio)
         self.change_image_mode_radio()  # run initial setup
 
     def change_image_mode_radio(self, *_) -> None:
         mode = self.image_mode.get()
         for l, widget, modes in self.grid:
             if mode in modes:
-                widget['state'] = 'normal'
+                widget['state'] = 'readonly' if '_readonly' in modes else 'normal'
             else:
                 widget['state'] = 'disable'
 
     def get_idx(self, stirng_variable: tk.StringVar, name: str) -> int:
         sz = self.gui.get_observation().data.shape[0]
         return self.get_int(
             stirng_variable, name=name, positive=False, minimum=-sz, maximum=sz - 1
@@ -2481,21 +2521,22 @@
                     self.image_idx_b, 'wavelength index (blue)'
                 )
 
             general_settings['image_gamma'] = self.get_float(
                 self.image_gamma, 'gamma', positive=False
             )
             if image_mode in {'single', 'sum'}:
-                settings['vmin'] = self.get_float(
+                general_settings['image_limit_type'] = self.image_limit_type.get()
+                general_settings['image_vmin'] = self.get_float(
                     self.image_vmin, 'vmin', positive=False
                 )
-                settings['vmax'] = self.get_float(
+                general_settings['image_vmax'] = self.get_float(
                     self.image_vmax, 'vmax', positive=False
                 )
-                if settings['vmin'] >= settings['vmax']:
+                if general_settings['image_vmin'] >= general_settings['image_vmax']:
                     tkinter.messagebox.showwarning(
                         title='Error parsing limits',
                         message=f'vmin must be less than vmax',
                     )
                     return False
         except ValueError:
             return False
```

### Comparing `planetmapper-1.6.0/planetmapper/kernel_downloader.py` & `planetmapper-1.6.1/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper/observation.py` & `planetmapper-1.6.1/planetmapper/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import photutils.aperture
 import PIL.Image
 import scipy.ndimage
 from astropy.io import fits
 from astropy.utils.exceptions import AstropyWarning
 
 from . import common, utils
-from .body_xy import BodyXY, _MapKwargs, Unpack, _cache_clearable_result_with_args
+from .body_xy import BodyXY, _MapKwargs, Unpack, _cache_clearable_result
 from .progress import progress_decorator, SaveMapProgressHookCLI, SaveNavProgressHookCLI
 
 T = TypeVar('T')
 S = TypeVar('S')
 P = ParamSpec('P')
 
 
@@ -115,14 +115,17 @@
                 raise ValueError('`path` and `data` are mutually exclusive')
             if header is not None:
                 raise ValueError('`path` and `header` are mutually exclusive')
             self._load_data_from_path()
 
         # TODO validate/standardise shape of data here (cube etc.)
         self.data = np.asarray(self.data)
+        if len(self.data.shape) == 2:
+            # Turn data into cube for consistency
+            self.data = self.data[np.newaxis, ...]
         if self.header is not None:
             # use values from header to fill in arguments (e.g. target) which aren't
             # specified by the user
             self._add_kw_from_header(kwargs, self.header)
         super().__init__(nx=self.data.shape[-1], ny=self.data.shape[-2], **kwargs)
 
         if self.header is None:
@@ -143,15 +146,15 @@
 
     def __repr__(self) -> str:
         return f'Observation({self.path!r})'
 
     def _get_equality_tuple(self) -> tuple:
         return (
             self.path,
-            self.data.tolist(),
+            self.data.data,
             self.header,
             super()._get_equality_tuple(),
         )
 
     def _load_data_from_path(self):
         assert self.path is not None
         if any(self.path.endswith(ext) for ext in self.FITS_FILE_EXTENSIONS):
@@ -268,16 +271,17 @@
         be the same as the previous run.
 
         Raises:
             ValueError: if the header does not contain appropriate metadata values. This
                 is likely because the file was not created by `planetmapper`.
         """
         if (
-            self._make_fits_kw('MAP PROJECTION') in self.header or 
-            self._make_fits_kw('DEGREE-INTERVAL') in self.header):
+            self._make_fits_kw('MAP PROJECTION') in self.header
+            or self._make_fits_kw('DEGREE-INTERVAL') in self.header
+        ):
             raise ValueError('FITS header refers to mapped data')
         try:
             self.set_disc_params(
                 x0=self.header[self._make_fits_kw('DISC X0')],  # type: ignore
                 y0=self.header[self._make_fits_kw('DISC Y0')],  # type: ignore
                 r0=self.header[self._make_fits_kw('DISC R0')],  # type: ignore
                 rotation=self.header[self._make_fits_kw('DISC ROT')],  # type: ignore
@@ -518,15 +522,15 @@
             Array containing cube of maped of the values in `img` at each location on
             the surface of the target body. Locations which are not visible or outside
             the projection domain have a value of NaN.
         """
         # Return a copy so that the cached value isn't tainted by any modifications
         return self._get_mapped_data(interpolation=interpolation, **map_kwargs).copy()
 
-    @_cache_clearable_result_with_args
+    @_cache_clearable_result
     @progress_decorator
     def _get_mapped_data(
         self,
         interpolation: Literal['nearest', 'linear', 'quadratic', 'cubic'] = 'linear',
         **map_kwargs: Unpack[_MapKwargs],
     ):
         projected = []
```

### Comparing `planetmapper-1.6.0/planetmapper/progress.py` & `planetmapper-1.6.1/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper/utils.py` & `planetmapper-1.6.1/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.6.1/planetmapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
 Keywords: planetmapper,astronomy,space,science,spice,ephemeris,planetary-science
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
 # PlanetMapper
 
-[![PyPI](https://img.shields.io/pypi/v/planetmapper?logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
+[![PyPI](https://img.shields.io/pypi/v/planetmapper?label=PyPi&logo=python&logoColor=silver)](https://pypi.org/project/planetmapper/)
 [![Upload Python Package](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/python-publish.yml)
 [![Pylint](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/pylint.yml)
 [![Black](https://github.com/ortk95/planetmapper/actions/workflows/black.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/black.yml)
 [![Tests](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml/badge.svg)](https://github.com/ortk95/planetmapper/actions/workflows/unittest.yml)
 [![Documentation Status](https://readthedocs.org/projects/planetmapper/badge/?version=latest)](https://planetmapper.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `planetmapper-1.6.0/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.6.1/planetmapper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 tests/test_base.py
 tests/test_basic_body.py
 tests/test_body.py
 tests/test_body_xy.py
 tests/test_common.py
 tests/test_gui.py
 tests/test_init.py
-tests/test_observation.py
+tests/test_observation.py
+tests/test_utils.py
```

### Comparing `planetmapper-1.6.0/setup.py` & `planetmapper-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/tests/test_base.py` & `planetmapper-1.6.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/tests/test_basic_body.py` & `planetmapper-1.6.1/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/tests/test_body.py` & `planetmapper-1.6.1/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/tests/test_body_xy.py` & `planetmapper-1.6.1/tests/test_body_xy.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import numpy as np
 from numpy import array, nan
 
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
 from planetmapper import BodyXY
-from planetmapper.body_xy import BackplaneNotFoundError, Backplane
+from planetmapper.body_xy import (
+    BackplaneNotFoundError,
+    Backplane,
+    _cache_clearable_result,
+    _cache_stable_result,
+)
 
 
 class TestBodyXY(unittest.TestCase):
     def setUp(self):
         planetmapper.set_kernel_path(common_testing.KERNEL_PATH)
         self.body = BodyXY(
             'Jupiter', observer='HST', utc='2005-01-01T00:00:00', nx=15, ny=10
@@ -82,15 +87,14 @@
                 fn(np.random.rand())
                 self.assertEqual(len(self.body._cache), 0)
 
         self.body._stable_cache.clear()
         self.body.get_emission_angle_map(degree_interval=90)
         self.assertGreater(len(self.body._stable_cache), 0)
 
-
     def test_xy_conversions(self):
         # xy, radec, lonlat, km
         coordinates = [
             [
                 (0, 0),
                 (196.3684350770821, -5.581107015413806),
                 (nan, nan),
@@ -573,7 +577,78 @@
 
     def test_plot_map(self):
         fig, ax = plt.subplots()
         self.body.plot_map(np.ones((180, 360)), ax=ax)
         plt.close(fig)
 
     # Backplane contents tested against FITS reference in test_observation
+
+
+class TestCache(unittest.TestCase):
+    def setUp(self):
+        self._cache = {}
+        self._stable_cache = {}
+        self.functions_called = []
+
+    @_cache_clearable_result
+    def f_clearable(self, a, b=1):
+        self.functions_called.append('f_clearable')
+        return ('f_clearable', a * b)
+
+    @_cache_stable_result
+    def f_stable(self, a, b=1):
+        self.functions_called.append('f_stable')
+        return ('f_stable', a * b)
+
+    def test_clearable_cache(self):
+        self.functions_called = []
+        for attempt in range(3):
+            with self.subTest(attempt=attempt):
+                self._cache.clear()
+                self.functions_called = []
+
+                self.assertEqual(self.f_clearable(1), ('f_clearable', 1))
+                self.assertEqual(self.functions_called, ['f_clearable'])
+                self.assertEqual(self.f_clearable(1), ('f_clearable', 1))
+                self.assertEqual(self.functions_called, ['f_clearable'])
+
+                self.assertEqual(self.f_clearable(2), ('f_clearable', 2))
+                self.assertEqual(self.functions_called, ['f_clearable'] * 2)
+                self.assertEqual(self.f_clearable(2), ('f_clearable', 2))
+                self.assertEqual(self.functions_called, ['f_clearable'] * 2)
+
+                self.assertEqual(self.f_clearable(2, b=2), ('f_clearable', 4))
+                self.assertEqual(self.functions_called, ['f_clearable'] * 3)
+                self.assertEqual(self.f_clearable(2, b=2), ('f_clearable', 4))
+                self.assertEqual(self.functions_called, ['f_clearable'] * 3)
+
+                self.assertEqual(self.f_clearable(1), ('f_clearable', 1))
+                self.assertEqual(self.f_clearable(2), ('f_clearable', 2))
+                self.assertEqual(self.f_clearable(2, b=2), ('f_clearable', 4))
+                self.assertEqual(self.functions_called, ['f_clearable'] * 3)
+
+                self.assertEqual(len(self._cache), 3)
+
+    def test_stable_cache(self):
+        self.functions_called = []
+
+        self.assertEqual(self.f_stable(1), ('f_stable', 1))
+        self.assertEqual(self.functions_called, ['f_stable'])
+        self.assertEqual(self.f_stable(1), ('f_stable', 1))
+        self.assertEqual(self.functions_called, ['f_stable'])
+
+        self.assertEqual(self.f_stable(2), ('f_stable', 2))
+        self.assertEqual(self.functions_called, ['f_stable'] * 2)
+        self.assertEqual(self.f_stable(2), ('f_stable', 2))
+        self.assertEqual(self.functions_called, ['f_stable'] * 2)
+
+        self.assertEqual(self.f_stable(2, b=2), ('f_stable', 4))
+        self.assertEqual(self.functions_called, ['f_stable'] * 3)
+        self.assertEqual(self.f_stable(2, b=2), ('f_stable', 4))
+        self.assertEqual(self.functions_called, ['f_stable'] * 3)
+
+        self.assertEqual(self.f_stable(1), ('f_stable', 1))
+        self.assertEqual(self.f_stable(2), ('f_stable', 2))
+        self.assertEqual(self.f_stable(2, b=2), ('f_stable', 4))
+        self.assertEqual(self.functions_called, ['f_stable'] * 3)
+
+        self.assertEqual(len(self._stable_cache), 3)
```

### Comparing `planetmapper-1.6.0/tests/test_init.py` & `planetmapper-1.6.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.0/tests/test_observation.py` & `planetmapper-1.6.1/tests/test_observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,29 +106,29 @@
                 np.array_equal(
                     obs.data,
                     np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]]),
                 )
             )
 
         with self.subTest('data+target+observer+utc'):
-            data = np.ones((5, 6))
+            data = np.ones((5, 6, 7))
             obs = Observation(
                 data=data,
                 target='Jupiter',
                 observer='hst',
                 utc='2005-01-01T00:00:00',
             )
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertTrue(np.array_equal(obs.data, data))
 
         with self.subTest('data+header+target+observer+utc'):
-            data = np.ones((5, 6))
+            data = np.ones((5, 6, 7))
             header = fits.Header({'key': 'value'})
             obs = Observation(
                 data=data,
                 header=header,
                 target='Jupiter',
                 observer='hst',
                 utc='2005-01-01T00:00:00',
@@ -136,47 +136,65 @@
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
-        with self.subTest('data+header'):
+
+        with self.subTest('image+header'):
             data = np.ones((5, 6))
             header = fits.Header(
                 {'OBJECT': 'jupiter', 'TELESCOP': 'HST', 'DATE-OBS': '2005-01-01'}
             )
             obs = Observation(
                 data=data,
                 header=header,
             )
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
+            data_expected = data[np.newaxis, :, :]
+            self.assertTrue(np.array_equal(obs.data, data_expected))
+
+        with self.subTest('data+header'):
+            data = np.ones((5, 6, 7))
+            header = fits.Header(
+                {'OBJECT': 'jupiter', 'TELESCOP': 'HST', 'DATE-OBS': '2005-01-01'}
+            )
+            obs = Observation(
+                data=data,
+                header=header,
+            )
+            self.assertIsNone(obs.path)
+            self.assertEqual(obs.target, 'JUPITER')
+            self.assertEqual(obs.observer, 'HST')
+            self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
+            self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
         with self.subTest('data+header+mix'):
-            data = np.ones((5, 6))
+            data = np.ones((5, 6, 7))
             header = fits.Header({'OBJECT': 'jupiter', 'DATE-OBS': '2005-01-01'})
             obs = Observation(
                 data=data,
                 header=header,
                 observer='HST',
             )
             self.assertIsNone(obs.path)
             self.assertEqual(obs.target, 'JUPITER')
             self.assertEqual(obs.observer, 'HST')
             self.assertEqual(obs.utc, '2005-01-01T00:00:00.000000')
             self.assertEqual(obs.header, header)
             self.assertTrue(np.array_equal(obs.data, data))
 
         with self.subTest('data+header+override'):
-            data = np.ones((5, 6))
+            data = np.ones((5, 6, 7))
             header = fits.Header(
                 {'OBJECT': 'mars', 'TELESCOP': 'HST', 'DATE-OBS': '2005-01-01'}
             )
             obs = Observation(
                 data=data,
                 header=header,
                 target='jupiter',
```

