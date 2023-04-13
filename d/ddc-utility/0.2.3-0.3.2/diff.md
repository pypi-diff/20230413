# Comparing `tmp/ddc-utility-0.2.3.tar.gz` & `tmp/ddc-utility-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddc-utility-0.2.3.tar", last modified: Mon Apr  3 14:02:21 2023, max compression
+gzip compressed data, was "ddc-utility-0.3.2.tar", last modified: Thu Apr 13 13:42:04 2023, max compression
```

## Comparing `ddc-utility-0.2.3.tar` & `ddc-utility-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 14:02:21.050906 ddc-utility-0.2.3/
--rw-rw-rw-   0        0        0     1459 2023-04-03 14:02:21.041921 ddc-utility-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 14:02:20.965854 ddc-utility-0.2.3/ddc_cube/
--rw-rw-rw-   0        0        0      126 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/__init__.py
--rw-rw-rw-   0        0        0       19 2023-04-03 12:30:42.000000 ddc-utility-0.2.3/ddc_cube/__version__.py
--rw-rw-rw-   0        0        0     1922 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/auth.py
--rw-rw-rw-   0        0        0    25507 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/chunkstore.py
--rw-rw-rw-   0        0        0    16826 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/config.py
--rw-rw-rw-   0        0        0      188 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/constants.py
--rw-rw-rw-   0        0        0     1789 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/cube.py
--rw-rw-rw-   0        0        0    12164 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/ddc.py
--rw-rw-rw-   0        0        0     3207 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/errors.py
--rw-rw-rw-   0        0        0     6716 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/metadata.py
--rw-rw-rw-   0        0        0     8079 2023-04-03 08:42:27.000000 ddc-utility-0.2.3/ddc_cube/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 14:02:21.020842 ddc-utility-0.2.3/ddc_utility.egg-info/
--rw-rw-rw-   0        0        0     1459 2023-04-03 14:02:20.000000 ddc-utility-0.2.3/ddc_utility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-03 14:02:20.000000 ddc-utility-0.2.3/ddc_utility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 14:02:20.000000 ddc-utility-0.2.3/ddc_utility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-03 14:02:20.000000 ddc-utility-0.2.3/ddc_utility.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-03 14:02:20.000000 ddc-utility-0.2.3/ddc_utility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-04-03 13:07:55.000000 ddc-utility-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-03 14:02:21.050906 ddc-utility-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-03 14:02:21.028123 ddc-utility-0.2.3/test/
--rw-rw-rw-   0        0        0     2582 2022-11-29 08:31:18.000000 ddc-utility-0.2.3/test/test_metadata.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:42:04.169962 ddc-utility-0.3.2/
+-rw-rw-rw-   0        0        0     1110 2023-04-13 13:36:09.000000 ddc-utility-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1491 2023-04-13 13:42:04.150972 ddc-utility-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 13:42:03.994105 ddc-utility-0.3.2/ddc_utility/
+-rw-rw-rw-   0        0        0      159 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/ddc_utility/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-04-13 13:36:09.000000 ddc-utility-0.3.2/ddc_utility/__version__.py
+-rw-rw-rw-   0        0        0     1922 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/ddc_utility/auth.py
+-rw-rw-rw-   0        0        0    26196 2023-04-13 13:36:09.000000 ddc-utility-0.3.2/ddc_utility/chunkstore.py
+-rw-rw-rw-   0        0        0    17691 2023-04-13 13:36:09.000000 ddc-utility-0.3.2/ddc_utility/config.py
+-rw-rw-rw-   0        0        0      188 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/ddc_utility/constants.py
+-rw-rw-rw-   0        0        0     1789 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/ddc_utility/cube.py
+-rw-rw-rw-   0        0        0    12622 2023-04-12 18:48:15.000000 ddc-utility-0.3.2/ddc_utility/ddc.py
+-rw-rw-rw-   0        0        0     3207 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/ddc_utility/errors.py
+-rw-rw-rw-   0        0        0    10627 2023-04-13 13:36:09.000000 ddc-utility-0.3.2/ddc_utility/metadata.py
+-rw-rw-rw-   0        0        0     8079 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/ddc_utility/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:42:04.122037 ddc-utility-0.3.2/ddc_utility.egg-info/
+-rw-rw-rw-   0        0        0     1491 2023-04-13 13:42:03.000000 ddc-utility-0.3.2/ddc_utility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-04-13 13:42:03.000000 ddc-utility-0.3.2/ddc_utility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:42:03.000000 ddc-utility-0.3.2/ddc_utility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2023-04-13 13:42:03.000000 ddc-utility-0.3.2/ddc_utility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 13:42:03.000000 ddc-utility-0.3.2/ddc_utility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      858 2023-04-13 13:36:09.000000 ddc-utility-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:42:04.170957 ddc-utility-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 13:42:04.132954 ddc-utility-0.3.2/test/
+-rw-rw-rw-   0        0        0     2585 2023-04-11 18:31:42.000000 ddc-utility-0.3.2/test/test_metadata.py
```

### Comparing `ddc-utility-0.2.3/PKG-INFO` & `ddc-utility-0.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ddc-utility
-Version: 0.2.3
+Version: 0.3.2
 Summary: Package for retrieving DDC datasests
 Author-email: Balint Alfoldy <alfibalint@gmail.com>, CropOM <marton.tolnai@cropom.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # DDC Utility
 
 This is the Danube Data Cube Utility library, for retrieving data from the Danube Data Cube portal.
 
 ### Installation
 
@@ -24,17 +25,17 @@
 Users must have a valid DDC registration.
 
 ### Example
 ```
 $ python
 
 # Importing packages
->>> from ddc_cube.ddc import DanubeDataCube
->>> from ddc_cube.config import DdcCubeConfig, CustomCubeConfig
->>> from ddc_cube.cube import open_cube
+>>> from ddc_utility.ddc import DanubeDataCube
+>>> from ddc_utility.config import DdcCubeConfig, CustomCubeConfig
+>>> from ddc_utility.cube import open_cube
 
 # Setting DDC credentials
 >>> os.environ['DDC_CLIENT_ID'] = ""
 >>> os.environ['DDC_CLIENT_SECRET'] = ""
 
 # Initialize DDC object 
 >>> DDC = DanubeDataCube()
```

### Comparing `ddc-utility-0.2.3/README.md` & `ddc-utility-0.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 Users must have a valid DDC registration.
 
 ### Example
 ```
 $ python
 
 # Importing packages
->>> from ddc_cube.ddc import DanubeDataCube
->>> from ddc_cube.config import DdcCubeConfig, CustomCubeConfig
->>> from ddc_cube.cube import open_cube
+>>> from ddc_utility.ddc import DanubeDataCube
+>>> from ddc_utility.config import DdcCubeConfig, CustomCubeConfig
+>>> from ddc_utility.cube import open_cube
 
 # Setting DDC credentials
 >>> os.environ['DDC_CLIENT_ID'] = ""
 >>> os.environ['DDC_CLIENT_SECRET'] = ""
 
 # Initialize DDC object 
 >>> DDC = DanubeDataCube()
```

### Comparing `ddc-utility-0.2.3/ddc_cube/auth.py` & `ddc-utility-0.3.2/ddc_utility/auth.py`

 * *Files identical despite different names*

### Comparing `ddc-utility-0.2.3/ddc_cube/chunkstore.py` & `ddc-utility-0.3.2/ddc_utility/chunkstore.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from abc import ABCMeta, abstractmethod
 from collections.abc import MutableMapping
 from typing import (Any, Callable, Dict, Iterable, Iterator, KeysView, List,
                     Optional, Tuple)
 
 import numpy as np
 import pandas as pd
-import pyproj
 from numcodecs import Blosc
 
 from .config import CubeConfig, CustomCubeConfig, DdcCubeConfig
 from .errors import DdcException, DdcRequestError
+from .utils import Bbox
 
 _STATIC_ARRAY_COMPRESSOR_PARAMS = dict(
     cname='zstd',
     clevel=1,
     shuffle=Blosc.SHUFFLE,
     blocksize=0
 )
@@ -81,25 +81,31 @@
         self._trace_store_calls = trace_store_calls
 
         self._time_ranges = self._cube_config.time_lst
         if self._time_ranges.empty:
             raise ValueError('Could not determine any valid time stamps')
 
         self._bbox = self._cube_config.bbox.bbox
+        self._precision = self._cube_config.bbox._precision
 
         width, height = self._cube_config.size.get(
             'x'), self._cube_config.size.get('y')
 
+        spatial_res = self.cube_config.spatial_res
+
         x1, y1, x2, y2 = self._bbox
         x_array = np.linspace(x1, x2, width, dtype=np.float64)
         y_array = np.linspace(y2, y1, height, dtype=np.float64)
+        #x_array = np.round(np.arange(x1, x1 + self._cube_config.spatial_res * width, self._cube_config.spatial_res, dtype=np.float64), self._precision)
+        #y_array = np.round(np.flip(np.arange(y1, y1 + self._cube_config.spatial_res * height, self._cube_config.spatial_res, dtype=np.float64)), self._precision)
+
         self._x_ranges = x_array
         self._y_ranges = y_array
 
-        crs = pyproj.CRS.from_string(self._cube_config.crs)
+        crs = self._cube_config.crs.lower()
 
         def time_stamp_to_str(ts: pd.Timestamp) -> str:
             """
             Convert to ISO string and strip timezone.
             Used to create numpy datetime64 arrays.
             We cannot create directly from pd.Timestamp because Numpy doesn't
             like parsing timezones anymore.
@@ -124,21 +130,25 @@
             history=[
                 dict(
                     program=f'{self._class_name}'
                 )
             ],
             date_created=pd.Timestamp.now().isoformat(),
             time_coverage_start=self._time_ranges[0].isoformat(),
-            time_coverage_end=self._time_ranges[1].isoformat(),
+            time_coverage_end=self._time_ranges[-1].isoformat(),
             time_coverage_duration=(
-                self._time_ranges[1] - self._time_ranges[0]
+                self._time_ranges[-1] - self._time_ranges[0]
             ).isoformat(),
+            crs=crs
         )
 
-        if crs.is_geographic:
+        global_attrs.update(self.get_ds_attrs(self._cube_config.dataset_name))
+
+
+        if crs == "epsg:4326":
             x1, y1, x2, y2 = self._bbox
             global_attrs.update(geospatial_lon_min=x1,
                                 geospatial_lat_min=y1,
                                 geospatial_lon_max=x2,
                                 geospatial_lat_max=y2)
         else:
             x1, y1, x2, y2 = self._bbox
@@ -149,15 +159,15 @@
 
         # setup Virtual File System (vfs)
         self._vfs = {
             '.zgroup': _dict_to_bytes(dict(zarr_format=2)),
             '.zattrs': _dict_to_bytes(global_attrs)
         }
 
-        if crs.is_geographic:
+        if crs == "epsg:4326":
             x_name, y_name = 'lon', 'lat'
             x_attrs, y_attrs = (
                 {
                     "_ARRAY_DIMENSIONS": ['lon'],
                     "units": "decimal_degrees",
                     "long_name": "longitude",
                     "standard_name": "longitude",
@@ -192,21 +202,17 @@
         }
 
         self._add_static_array(x_name, x_array, x_attrs)
         self._add_static_array(y_name, y_array, y_attrs)
         self._add_static_array('time', t_array, time_attrs)
 
         crs_var_attrs = dict()
-        # if not crs.is_geographic:
-        self._add_static_array('crs', np.array(0), dict(
-            _ARRAY_DIMENSIONS=[],
-            **crs.to_cf()))
         crs_var_attrs['grid_mapping'] = 'crs'
 
-        if crs.is_geographic:
+        if crs == "epsg:4326":
             band_array_dimensions = ['time', 'lat', 'lon']
         else:
             band_array_dimensions = ['time', 'y', 'x']
 
         for var_name in self._cube_config.variable_names:
             size = (self._cube_config.size.get('time'),
                     self._cube_config.size.get('y'),
@@ -230,14 +236,21 @@
     def get_var_attrs(self, var_name: str) -> Dict[str, Any]:
         """
         Get any metadata attributes for variable var_name.
         """
         pass
 
     @abstractmethod
+    def get_ds_attrs(self, dataset_name: str) -> Dict[str, Any]:
+        """
+        Get any metadata attributes for a dataset.
+        """
+        pass
+
+    @abstractmethod
     def get_band_encoding(self, var_name: str) -> Dict[str, Any]:
         """
         Get data encoding of a variable.
         """
         pass
 
     @abstractmethod
@@ -251,15 +264,15 @@
         """
         pass
 
     def get_bbox_chunk_info(self,
                             x_chunk_index: int,
                             y_chunk_index: int,
                             x_chunk_size: int,
-                            y_chunk_size: int) -> Tuple[float, float, float, float]:
+                            y_chunk_size: int) -> Bbox:
         """
         Get xy dimension information about a given chunk, based on chunk index
         of the xy dimension.
 
         Args:
             x_chunk_index (int): Start index of the chunk in
                 the x dimension.
@@ -268,29 +281,26 @@
             x_chunk_size (int): Size of the chunk in the x dimension.
             y_chunk_size (int): Size of the chunk in the y dimension.
 
         Returns:
             Tuple[float, float, float, float]: Tuple of bounding box.
         """
 
-        x_start_index = x_chunk_index * x_chunk_size
-        y_start_index = y_chunk_index * y_chunk_size
-        x_end_index = x_chunk_index * x_chunk_size + x_chunk_size - 1
-        y_end_index = y_chunk_index * y_chunk_size + y_chunk_size - 1
-
-        x1 = self._x_ranges[x_start_index]
-        x2 = self._x_ranges[x_end_index]
-
-        # The reverse in y direction because of upper-left corner indexing start
-        # i.e. the minimum value of a bounding box in the y direction is the 
-        # x last value of the y coordinate array
-        y1 = self._y_ranges[y_end_index]
-        y2 = self._y_ranges[y_start_index]
+        x_index = x_chunk_index * x_chunk_size
+        y_index = y_chunk_index * y_chunk_size
+
+        x01, _, _, y02 = self._bbox
+        spatial_res = self.cube_config.spatial_res
+
+        x1 = x01 + spatial_res * x_index - spatial_res / 5
+        x2 = x01 + spatial_res * (x_index + x_chunk_size - 1) + spatial_res / 5
+        y1 = y02 - spatial_res * (y_index + y_chunk_size - 1) - spatial_res / 5
+        y2 = y02 - spatial_res * y_index + spatial_res / 5
 
-        return (x1, y1, x2, y2)
+        return Bbox(x1, y1, x2, y2, self._precision)
 
     def get_time_chunk_info(self,
                             time_chunk_index: int,
                             time_chunk_size: int
                             ) -> Tuple[pd.Timestamp, pd.Timestamp, int]:
         """
         Get time dimension information about a given chunk, based on chunk index
@@ -346,15 +356,15 @@
             t_chunk_index, t_chunk_size)
 
         t0 = time.perf_counter()
         try:
             exception = None
             chunk_data = self.fetch_chunk(key,
                                           band_name,
-                                          bbox=request_bbox,
+                                          bbox=request_bbox.bbox,
                                           time_range=(start_time, end_time))
 
             if num_dates < t_chunk_size:
 
                 extend_nan = np.empty(
                     ((t_chunk_size - num_dates)*y_chunk_size * x_chunk_size),
                     dtype='float32')
@@ -557,14 +567,20 @@
             var_name,
             default={}
         )
         if 'fill_value' in band_metadata:
             band_metadata.pop('fill_value')
         return band_metadata
 
+    def get_ds_attrs(self, dataset_name: str) -> Dict[str, Any]:
+        ds_metadata = self._danube_data_cube.dataset(
+            self._cube_config.dataset_name
+        )
+        return ds_metadata
+
     def get_band_encoding(self, var_name: str) -> Dict[str, Any]:
 
         if isinstance(self._cube_config.datatype, dict):
             sample_type = self._cube_config.datatype.get(var_name)
         else:
             sample_type = 'float32'
 
@@ -649,14 +665,17 @@
 
         super().__init__(cube_config=cube_config,
                          observer=observer,
                          trace_store_calls=trace_store_calls)
 
     def get_var_attrs(self, var_name: str) -> Dict[str, Any]:
         return {}
+    
+    def get_ds_attrs(self, dataset_name: str) -> Dict[str, Any]:
+        return {}
 
     def get_band_encoding(self, var_name: str) -> Dict[str, Any]:
 
         if isinstance(self._cube_config.datatype, dict):
             sample_type = self._cube_config.datatype.get(var_name)
         else:
             sample_type = 'float32'
```

### Comparing `ddc-utility-0.2.3/ddc_cube/config.py` & `ddc-utility-0.3.2/ddc_utility/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -287,39 +287,52 @@
         """
         # retrieve source metadata and convert those to correct types
         # improve this with metadata api response
         src_variable_names = list(src_properties.get('datatypes').keys())
 
         src_bbox = Bbox(*src_properties.get('bbox').split(','))
 
+        src_dimensions = src_properties.get('dimensions')
+
+        src_depth = src_dimensions.get('time')
+        src_width = src_dimensions.get('x') or src_dimensions.get('lon')
+        src_height = src_dimensions.get('y') or src_dimensions.get('lat')
+
         src_datatype = src_properties.get('datatypes')
 
         src_spatial_res = float(src_properties.get('spatial_res'))
 
         src_time_lst = pd.to_datetime(src_properties.get('time_lst'))
 
         # Adjust user defined input arguments with the source parameters
         variable_names = self._get_variable_names(src_variable_names, self.variable_names)
 
         datatype = {k: np.dtype(src_datatype.get(k)) for k in variable_names}
 
-        bbox = self._get_bbox(src_bbox, self.bbox, src_spatial_res)
+        x_lst, y_lst = self._get_xy_lst(src_bbox, src_width, src_height, self.bbox)
+
+        precision = len(str(src_spatial_res).split('.')[-1]) + 1
 
         time_lst = self._get_time_lst(src_time_lst, self.time_range, self.time_period) 
 
         depth = self._get_t_size(time_lst)
-        width, height = self._get_xy_size(bbox, src_spatial_res)
+        width, height = self._get_xy_size(x_lst, y_lst)
 
         base_dt = max(datatype.values())
         width, height, chunk_w, chunk_h = self._get_xy_chunk_size(width, height, base_dt)
-
         time_freq = self.time_period or 'original'
-        # readjust bbox based on new size
-        bbox.maxx = bbox.minx + (width-1) * src_spatial_res
-        bbox.maxy = bbox.miny + (height-1) * src_spatial_res
+
+        x_lst = x_lst[0:width]
+        y_lst = y_lst[0:height]
+
+        x1 = x_lst[0]# - src_spatial_res / 5
+        x2 = x_lst[-1]# + src_spatial_res / 5
+        y1 = y_lst[0]# - src_spatial_res / 5
+        y2 = y_lst[-1]# + src_spatial_res / 5
+        bbox = Bbox(x1, y1, x2, y2, precision)
 
         chunk_size = {}
         num_chunks = {}
 
         # get chunksize in time dim. Size of the chunks can be varied on the
         # time dimension based on the variable's datatype
         for var in variable_names:
@@ -354,30 +367,46 @@
                            ) -> List[str]:
         if not variable_names:
             variable_names = src_variable_names
         else:
             variable_names = list(set(variable_names) & set(src_variable_names))
         return variable_names
 
-    def _get_bbox(self,
+    def _get_xy_lst(self,
                  src_bbox: Bbox,
-                 bbox: Optional[Bbox] = None,
-                 spatial_res: Optional[float] = None) -> Bbox:
+                 dim_x: int,
+                 dim_y: int,
+                 bbox: Optional[Bbox] = None
+                 ) -> Tuple[np.array, np.array]:
+
+        src_x_array = np.linspace(src_bbox.minx, src_bbox.maxx, dim_x) #np.arange(src_bbox.minx, src_bbox.maxx + spatial_res, spatial_res)
+        src_y_array = np.linspace(src_bbox.miny, src_bbox.maxy, dim_y) #np.arange(src_bbox.miny, src_bbox.maxy + spatial_res, spatial_res)
 
         if not bbox:
-            bbox = src_bbox
+            x_array = src_x_array
+            y_array = src_y_array
         else:
-            x1 = bbox.minx if bbox.minx >= src_bbox.minx else src_bbox.minx
-            y1 = bbox.miny if bbox.miny >= src_bbox.miny else src_bbox.miny
-            x2 = bbox.maxx if bbox.maxx <= src_bbox.maxx else src_bbox.maxx
-            y2 = bbox.maxy if bbox.maxy <= src_bbox.maxy else src_bbox.maxy
-            precision = len(str(spatial_res).split('.')[-1])
-            bbox = Bbox(x1, y1, x2, y2, precision)
+            x_array = src_x_array[
+                (src_x_array >= bbox.minx) &
+                (src_x_array <= bbox.maxx)
+                ]
+
+            y_array = src_y_array[
+                (src_y_array >= bbox.miny) &
+                (src_y_array <= bbox.maxy)
+                ]
+           
+            if len(x_array) == 0:
+                raise ValueError(f'Invalid bbox {bbox.bbox} '
+                                 '-- results in an empty x range list')
+            if len(y_array) == 0:
+                raise ValueError(f'Invalid bbox {bbox.bbox} '
+                                 '-- results in an empty y range list')
 
-        return bbox
+        return x_array, y_array
 
     def _get_time_lst(self,
                      src_time_lst: pd.DatetimeIndex,
                      time_range: Optional[TimeRange] = None,
                      time_period: Optional[str] = None) -> pd.DatetimeIndex:
 
         if not time_range:
@@ -398,22 +427,17 @@
 
         return time_lst
 
     def _get_t_size(self, time_lst: pd.DatetimeIndex) -> int:
         return len(time_lst)
 
     def _get_xy_size(self,
-                    bbox: Bbox,
-                    spatial_res: float) -> Tuple[int, int]:
-
-        x1, y1, x2, y2 = bbox.bbox
-        x_array = np.arange(x1, x2, spatial_res, dtype=np.float64)
-        y_array = np.arange(y1, y2, spatial_res, dtype=np.float64)
-        width, height = x_array.size, y_array.size
-        return width, height
+                     x_lst: np.array, 
+                     y_lst: np.array) -> Tuple[int, int]:
+        return len(x_lst), len(y_lst)
 
     def _get_xy_chunk_size(self,
                           width: int,
                           height: int,
                           datatype: np.dtype) -> Tuple[int, int, int, int]:
 
         item_size = datatype.itemsize
```

### Comparing `ddc-utility-0.2.3/ddc_cube/cube.py` & `ddc-utility-0.3.2/ddc_utility/cube.py`

 * *Files identical despite different names*

### Comparing `ddc-utility-0.2.3/ddc_cube/ddc.py` & `ddc-utility-0.3.2/ddc_utility/ddc.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,20 +83,30 @@
             )
 
         with self.session.request(
                 method, url, params=params, json=json_data, headers=headers,
                 auth=auth) as response:
 
             if self._trace_store_calls:
-                print(
-                    "Received API response: "
-                    f"{response.status_code} {response.reason}\n"
-                    f"Headers: {response.headers}\n"
-                    f"Content: {response.content}"
-                )
+
+                if isinstance(response.content, bytes):
+                    print(
+                        "Received API response: "
+                        f"{response.status_code} {response.reason}\n"
+                        f"Headers: {response.headers}\n"
+                        f"Content: 'bytes content'"
+                    )               
+                
+                else:
+                    print(
+                        "Received API response: "
+                        f"{response.status_code} {response.reason}\n"
+                        f"Headers: {response.headers}\n"
+                        f"Content: {response.content}"
+                    )
 
             if response.status_code == 400:
                 raise BadRequest(response)
             if response.status_code == 401:
                 raise Unauthorized(response)
             if response.status_code == 403:
                 raise Forbidden(response)
@@ -132,19 +142,20 @@
                              'client_secret': self.client_secret}
 
                 token = fetch_token(auth_data, headers, token_url)
                 auth = OAuth2Handler(
                     token.get('bearer_token'), token.get('expires_at'))
 
                 if self._trace_store_calls:
+                    body = {'client_id': self.client_id, 'client_secret': '*****'}
                     print(
                         f"Making API request: 'POST' {token_url}\n"
                         f"Parameters: {None}\n"
                         f"Headers: {headers}\n"
-                        f"Body: {'client_id': self.client_id, 'client_secret': '*****'}"
+                        f"Body: {body}"
                     )
                     print("Token is not provided or expired, made a request to fetch token.")
             else:
                 auth = self.auth
 
                 if self._trace_store_calls:
                     print(
```

### Comparing `ddc-utility-0.2.3/ddc_cube/errors.py` & `ddc-utility-0.3.2/ddc_utility/errors.py`

 * *Files identical despite different names*

### Comparing `ddc-utility-0.2.3/ddc_cube/utils.py` & `ddc-utility-0.3.2/ddc_utility/utils.py`

 * *Files identical despite different names*

### Comparing `ddc-utility-0.2.3/ddc_utility.egg-info/PKG-INFO` & `ddc-utility-0.3.2/ddc_utility.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ddc-utility
-Version: 0.2.3
+Version: 0.3.2
 Summary: Package for retrieving DDC datasests
 Author-email: Balint Alfoldy <alfibalint@gmail.com>, CropOM <marton.tolnai@cropom.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # DDC Utility
 
 This is the Danube Data Cube Utility library, for retrieving data from the Danube Data Cube portal.
 
 ### Installation
 
@@ -24,17 +25,17 @@
 Users must have a valid DDC registration.
 
 ### Example
 ```
 $ python
 
 # Importing packages
->>> from ddc_cube.ddc import DanubeDataCube
->>> from ddc_cube.config import DdcCubeConfig, CustomCubeConfig
->>> from ddc_cube.cube import open_cube
+>>> from ddc_utility.ddc import DanubeDataCube
+>>> from ddc_utility.config import DdcCubeConfig, CustomCubeConfig
+>>> from ddc_utility.cube import open_cube
 
 # Setting DDC credentials
 >>> os.environ['DDC_CLIENT_ID'] = ""
 >>> os.environ['DDC_CLIENT_SECRET'] = ""
 
 # Initialize DDC object 
 >>> DDC = DanubeDataCube()
```

### Comparing `ddc-utility-0.2.3/pyproject.toml` & `ddc-utility-0.3.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ddc-utility"
-version = "0.2.3"
+version = "0.3.2"
 description = "Package for retrieving DDC datasests"
 authors = [
     {name = "Balint Alfoldy", email = "alfibalint@gmail.com"},
     {name = "CropOM", email = "marton.tolnai@cropom.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.8"
@@ -22,12 +22,12 @@
     "pyproj >= 3.4.1",
     "requests >= 2.28.2",
     "xarray >= 2023.1.0",
     "zarr >= 2.13.6",
 ]
 
 [tool.setuptools.packages.find]
-include = ["ddc_cube*"]
+include = ["ddc_utility*"]
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `ddc-utility-0.2.3/test/test_metadata.py` & `ddc-utility-0.3.2/test/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from ddc_cube.metadata import DanubeDataCubeMetadata
+from ddc_utility.metadata import DanubeDataCubeMetadata
 
 
 @pytest.fixture
 def meta():
     return DanubeDataCubeMetadata()
```

