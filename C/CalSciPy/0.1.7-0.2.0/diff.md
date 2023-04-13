# Comparing `tmp/CalSciPy-0.1.7.tar.gz` & `tmp/CalSciPy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.1.7.tar", last modified: Wed Mar 29 21:16:52 2023, max compression
+gzip compressed data, was "CalSciPy-0.2.0.tar", last modified: Thu Apr 13 14:10:37 2023, max compression
```

## Comparing `CalSciPy-0.1.7.tar` & `CalSciPy-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 21:16:52.373063 CalSciPy-0.1.7/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     5009 2023-03-29 21:16:52.371060 CalSciPy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2851 2023-02-20 23:01:38.000000 CalSciPy-0.1.7/README.md
--rw-rw-rw-   0        0        0     2347 2023-03-29 15:46:43.000000 CalSciPy-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 21:16:52.373063 CalSciPy-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-29 21:16:52.294063 CalSciPy-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-03-29 21:16:52.335061 CalSciPy-0.1.7/src/CalSciPy/
--rw-rw-rw-   0        0        0      384 2023-02-20 22:23:21.000000 CalSciPy-0.1.7/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    14953 2023-03-29 16:04:44.000000 CalSciPy-0.1.7/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.1.7/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     4047 2023-02-20 22:16:25.000000 CalSciPy-0.1.7/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     6077 2023-03-29 16:06:43.000000 CalSciPy-0.1.7/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.1.7/src/CalSciPy/interactive_visuals.py
--rw-rw-rw-   0        0        0    10902 2023-02-20 22:21:35.000000 CalSciPy-0.1.7/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.1.7/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.1.7/src/CalSciPy/static_visuals.py
--rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.1.7/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0     2028 2023-03-29 17:18:44.000000 CalSciPy-0.1.7/src/CalSciPy/validators.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.1.7/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:16:52.352061 CalSciPy-0.1.7/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     5009 2023-03-29 21:16:52.000000 CalSciPy-0.1.7/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      678 2023-03-29 21:16:52.000000 CalSciPy-0.1.7/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 21:16:52.000000 CalSciPy-0.1.7/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      453 2023-03-29 21:16:52.000000 CalSciPy-0.1.7/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-29 21:16:52.000000 CalSciPy-0.1.7/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.1.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:16:52.367061 CalSciPy-0.1.7/tests/
--rw-rw-rw-   0        0        0     1949 2023-02-20 22:25:20.000000 CalSciPy-0.1.7/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3073 2023-03-29 17:16:03.000000 CalSciPy-0.1.7/tests/test_bruker.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.1.7/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.1.7/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.306677 CalSciPy-0.2.0/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4998 2023-04-13 14:10:37.305677 CalSciPy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.0/README.md
+-rw-rw-rw-   0        0        0     2315 2023-04-06 15:13:42.000000 CalSciPy-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:10:37.307677 CalSciPy-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.204677 CalSciPy-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.249755 CalSciPy-0.2.0/src/CalSciPy/
+-rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.0/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.0/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.0/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.0/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     2024 2023-04-03 22:21:07.000000 CalSciPy-0.2.0/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     9196 2023-04-05 16:04:42.000000 CalSciPy-0.2.0/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     5129 2023-04-05 15:54:33.000000 CalSciPy-0.2.0/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.0/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.0/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.0/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.268678 CalSciPy-0.2.0/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4998 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      358 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 14:10:37.000000 CalSciPy-0.2.0/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:10:37.300677 CalSciPy-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.0/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.0/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.0/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.0/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.0/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.0/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.0/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.0/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.1.7/LICENSE` & `CalSciPy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.1.7/PKG-INFO` & `CalSciPy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.1.7
+Version: 0.2.0
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
         
@@ -54,15 +54,16 @@
 [![Documentation Status](https://readthedocs.org/projects/calscipy/badge/?version=latest)](https://calscipy.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/CalSciPy?)
 ![PyPI - Status](https://img.shields.io/pypi/status/CalSciPy)
 ![GitHub](https://img.shields.io/github/license/darikoneil/CalSciPy)
 [![Contributors](https://img.shields.io/github/contributors-anon/darikoneil/CalSciPy)](https://github.com/darikoneil/CalSciPy/graphs/contributors)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/darikoneil/CalSciPy/calscipy_lint_test_action.yml)
 
-BETA STATUS: This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
+
+This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
 
 #### Highlights
 * Assign unique colormaps to subsets of ROIs to generate rich, informative videos
 * Perona-Malik diffusion for edge-preserving denoising
 * Methods for handling Bruker's PrairieView data
 * Interactive visualization
```

### Comparing `CalSciPy-0.1.7/README.md` & `CalSciPy-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 [![Documentation Status](https://readthedocs.org/projects/calscipy/badge/?version=latest)](https://calscipy.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/CalSciPy?)
 ![PyPI - Status](https://img.shields.io/pypi/status/CalSciPy)
 ![GitHub](https://img.shields.io/github/license/darikoneil/CalSciPy)
 [![Contributors](https://img.shields.io/github/contributors-anon/darikoneil/CalSciPy)](https://github.com/darikoneil/CalSciPy/graphs/contributors)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/darikoneil/CalSciPy/calscipy_lint_test_action.yml)
 
-BETA STATUS: This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
+
+This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
 
 #### Highlights
 * Assign unique colormaps to subsets of ROIs to generate rich, informative videos
 * Perona-Malik diffusion for edge-preserving denoising
 * Methods for handling Bruker's PrairieView data
 * Interactive visualization
```

### Comparing `CalSciPy-0.1.7/pyproject.toml` & `CalSciPy-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.1.7"
+version = "0.2.0"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
@@ -25,28 +25,25 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
-    "imageio[ffmpeg]",
     "matplotlib",
-    "numba",
     "numpy",
-    "pandas",
-    "pillow",
+    "opencv-python",
     "PPVD",
     "prettytable",
+    "pyside2",
     "seaborn",
     "scipy",
-    "scikit-image",
-    "tifffile",
     "tqdm"
 ]
+
 [project.urls]
 documentation = "https://calscipy.readthedocs.io/en/latest/?badge=latest"
 repository = "https://github.com/darikoneil/CalSciPy"
 
 
 [project.optional-dependencies]
 
@@ -57,23 +54,19 @@
     "flake8",
     "flake8-annotations",
     "flake8-bugbear",
     "flake8-class-attributes-order",
     "flake8-comprehensions",
     "flake8-html",
     "flake8-unused-arguments",
-    "pyproject-flake8",
     "pytest",
-    "pytest-datafiles",
+    "pytest-datafiles==2.0.1",
     "pytest-lazy-fixture",
     "pytest-sugar",
     "pytest-clarity",
-    "sphinx",
-    "sphinx-rtd-theme",
-    "sphinx_autodoc_typehints",
     "toml",
     "tomli",
     "twine"
 ]
 
 gpu = [
     "cupy"
@@ -81,32 +74,33 @@
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
     "-s",
     "--color=yes",
     "-vv",
-    "--diff-width=120"
+    "--diff-width=120",
+    "--disable-warnings"
 ]
 testpaths = "tests"
 console_output_style = "progress"
 filterwarnings = [
     "ignore::DeprecationWarning",
-    "ignore::FutureWarning"
+    "ignore::FutureWarning",
 ]
 
 [tool.coverage.run]
 branch = true
 command_line = "-m pytest"
-omit = ["*/tests*", "*tests*", "*tests/*", "tests*", "tests/*", "tests"]
+omit = ["*/tests*", "*tests*", "*tests/*", "tests*", "tests/*", "tests", "scratch", "htmlcov", "flake_report", "docs",
+"dist", "lib", ".pytest_cache", ".idea", ".github"]
 dynamic_context = "test_function"
 
+
 [tool.coverage.report]
 fail_under = 10
 
 [tool.coverage.json]
 pretty_print = true
 
 [tool.coverage.html]
 show_contexts = true
-
-
```

### Comparing `CalSciPy-0.1.7/src/CalSciPy/io_tools.py` & `CalSciPy-0.2.0/src/CalSciPy/io_tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,273 +1,246 @@
 from __future__ import annotations
+from typing import Union, Optional
+from pathlib import Path
+import cv2
 import numpy as np
-import os
-from tqdm.auto import tqdm
-import tifffile
-from typing import Tuple, Optional, Union
-import math
-import pathlib
-from imageio import mimwrite
-
-from PPVD.validation import validate_exists, validate_extension, validate_filename, validate_path
-from PPVD.parsing import convert_permitted_types_to_required, if_dir_append_filename, if_dir_join_filename, \
-    require_full_path
-
-
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=0)
-@validate_path(pos=0)
-@validate_exists(pos=0)
-def load_all_tiffs(folder: Union[str, pathlib.Path]) -> np.ndarray:
-    """
-    Loads all .tif's within a folder into a single numpy array. Assumes .tif files are the standard unsigned 16-bit
-    exported by the majority (all?) of imaging software.
+from json import load, dump
+from PPVD.validation import validate_extension, validate_filename
+from PPVD.parsing import convert_permitted_types_to_required
+from .misc import generate_blocks, calculate_frames_per_file
+
+
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def load_binary(path: Union[str, Path], mapped: bool = False) -> Union[np.ndarray, np.memmap]:
+    if not path.is_file():
+        path = path.joinpath("binary_video")
+
+    # add extensions
+    meta_filename = path.with_suffix(".json")
+    imaging_filename = path.with_suffix(".bin")
+
+    metadata = _Metadata.decode(meta_filename)
+
+    if mapped:
+        return np.memmap(imaging_filename, mode="r+", dtype=metadata.dtype, shape=(metadata.frames, metadata.y,
+                                                                                   metadata.x))
+    else:
+        images = np.fromfile(imaging_filename, dtype=metadata.dtype)
+        images = np.reshape(images, (metadata.frames, metadata.y, metadata.x))
+        return images
 
-    :param folder: folder containing a sequence of tiff stacks
-    :type folder: str or pathlib.Path
-    :return: a numpy array containing the images (frames, y-pixels, x-pixels)
-    :rtype: numpy.ndarray
-    """
-    if isinstance(folder, pathlib.Path):
-        folder = str(folder)
 
-    _filenames = [str(_filename.name) for _filename in pathlib.Path(folder).glob("*") if ".tif" in _filename.suffix]
-    y_pix, x_pix = tifffile.TiffFile(folder + "\\" + _filenames[0]).pages[0].shape
-    _num_frames = []  # initialize
-    [_num_frames.append(len(tifffile.TiffFile(folder + "\\" + _filename).pages)) for _filename in _filenames]
-    _total_frames = sum(_num_frames)
-    complete_image = np.full((_total_frames, y_pix, x_pix), 0, dtype=np.uint16)
-    _last_frame = 0
-
-    for _filename in tqdm(
-            range(len(_filenames)),
-            total=len(_filenames),
-            desc="Loading Images...",
-            disable=False,
-    ):
-        complete_image[_last_frame:_last_frame+_num_frames[_filename], :, :] = \
-            load_single_tiff(folder + "\\" + _filenames[_filename])
-        _last_frame += _num_frames[_filename]
-
-    return complete_image
-
-
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=0)
-@validate_path(pos=0)
-@if_dir_join_filename(default_name="video_meta.txt", flag_pos=0)
-@validate_extension(required_extension=".txt", pos=0)
-@validate_exists(pos=0)
-def load_binary_meta(path: Union[str, pathlib.Path]) -> Tuple[int, int, int, str]:
+@validate_filename(pos=0)
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def load_images(path: Union[str, Path]) -> np.ndarray:
     """
-    Loads the meta file for an associated binary video
+    Load images into a numpy array. If path is a folder, all .tif files found non-recursively in the directory will be
+    compiled to a single array
 
-    :param path: The meta file (.txt ext) or a directory containing metafile
+    :param path: a file containing images or a folder containing several imaging stacks
     :type path: str or pathlib.Path
-    :return: A tuple where (frames, y-pixels, x-pixels, :class:`numpy.dtype`)
-    :rtype: tuple[int, int, int, str]
-    """
-    _num_frames, _y_pixels, _x_pixels, _type = np.genfromtxt(path, delimiter=",", dtype="str")
-    return int(_num_frames), int(_y_pixels), int(_x_pixels), str(_type)
-
-
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=0)
-@validate_filename(pos=0)
-@if_dir_append_filename(default_name="video_meta.txt", flag_pos=0)
-@if_dir_join_filename(default_name="binary_video", flag_pos=0)
-@validate_path(pos=1)
-@validate_exists(pos=0)
-@validate_exists(pos=1)
-def load_mapped_binary(path: Union[str, pathlib.Path], meta_filename: Optional[str] = None, **kwargs: str) -> np.memmap:
+    :return: numpy array (frames, y-pixels, x-pixels)
+    :rtype: numpy.ndarray
     """
-    Loads a raw binary file as numpy array without loading into memory (memmap). Enter a directory to autogenerate the
-    default filenames (binary_video, video_meta.txt)
+    if path.is_file():
+        return _load_single_tif(path)
+    else:
+        return _load_many_tif(path)
+
+
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def save_binary(path: Union[str, Path], images: np.ndarray) -> int:
+    """
+    Save images to language-agnostic binary format. Ideal for optimal read/write speeds and highly-robust to corruption.
+    However, the downside is that the images and their metadata are split into two separate files. Images are saved with
+    the *.bin* extension, while metadata is saved with extension *.json*. If for some reason you lose the metadata, you
+    can still load the binary if you know three of the following: number of frames, y-pixels, x-pixels, and the
+    datatype. The datatype is almost always unsigned 16-bit for all modern imaging systems--even if they are collected
+    at 12 or 13-bit.
 
-    :param path: absolute filepath for binary video or a folder containing a binary video with the default filename
+    :param path: path to save images to. The path stem is considered the filename if it doesn't have any extension.
+    If no filename is provided then the default filename is *binary_video*.
     :type path: str or pathlib.Path
-    :param meta_filename: absolute path to meta file
-    :type meta_filename: Optional[str] = None
-    :keyword mode: mode used in loading numpy.memmap (str, default = "r")
-    :return: memmap (numpy) array (frames, y-pixels, x-pixels)
-    :rtype: numpy.memmap
+    :param images: images to save (frames, y-pixels, x-pixels)
+    :type images: numpy.ndarray
+    :return: 0 if successful
+    :rtype: int
     """
+    # parse the desired path
+    if path.is_file():
+        name = Path.name
+        file_path = Path(path.parents)
+    else:
+        name = "binary_video"
+        file_path = path
+
+    if not file_path.exists():
+        file_path.mkdir(parents=True, exist_ok=True)
+
+    # add extensions
+    imaging_filename = file_path.joinpath(name).with_suffix(".bin")
+    metadata_filename = file_path.joinpath(name).with_suffix(".json")
+
+    # save metadata
+    metadata = _Metadata(images)
+    metadata.encode(metadata_filename)
 
-    _mode = kwargs.get("mode", "r")
-
-    _num_frames, _y_pixels, _x_pixels, _type = load_binary_meta(meta_filename)
+    # save images
+    images.tofile(imaging_filename)
 
-    return np.memmap(path, dtype=_type, shape=(_num_frames, _y_pixels, _x_pixels), mode=_mode)
-# TODO UNIT TEST FOR EXCEPTIONS
 
-
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=0)
 @validate_filename(pos=0)
-@if_dir_append_filename(default_name="video_meta.txt", flag_pos=0)
-@if_dir_join_filename(default_name="binary_video", flag_pos=0)
-@validate_path(pos=1)
-@validate_exists(pos=0)
-@validate_exists(pos=1)
-def load_raw_binary(path: Union[str, pathlib.Path], meta_filename: Optional[str] = None) -> np.ndarray:
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def save_images(path: Union[str, Path], images: np.ndarray, size_cap: float = 3.9) -> int:
     """
-    Loads a raw binary file as a numpy array. Enter a directory to autogenerate the default
-    filenames (binary_video, video_meta.txt)
+    Save a numpy array to a single .tif file. If size > 4GB then saved as a series of files. If path is not a file and
+    already exists the default filename will be *images*.
 
-    :param path: absolute filepath for binary video or directory containing a file named binary video
+    :param path: filename or absolute path
     :type path: str or pathlib.Path
-    :param meta_filename: absolute path to meta file
-    :type meta_filename: Optional[str] = None
-    :return: numpy array (frames, y-pixels, x-pixels)
-    :rtype: numpy.ndarray
-    """
-
-    _num_frames, _y_pixels, _x_pixels, _type = np.genfromtxt(meta_filename, delimiter=",", dtype="str")
-    _num_frames = int(_num_frames)
-    _x_pixels = int(_x_pixels)
-    _y_pixels = int(_y_pixels)
-    return np.reshape(np.fromfile(path, dtype=_type), (_num_frames, _y_pixels, _x_pixels))
-# TODO UNIT TEST FOR EXCEPTIONS
+    :param images: numpy array (frames, y pixels, x pixels)
+    :type images: numpy.ndarray
+    :param size_cap: maximum size per file
+    :type size_cap: float = 3.9
+    :return: returns 0 if successful
+    :rtype: int
+    """
+    # parse desired path
+    if Path.exists(path):
+        if path.is_file():
+            name = path.name
+            file_path = path.parent
+        else:
+            name = "images"
+            file_path = path
+    else:
+        if path.is_file():
+            name = path.name
+            file_path = path.parent
+        else:
+            name = "images"
+            file_path = path
 
+    if not Path.exists(file_path):
+        Path.mkdir(file_path, parents=True, exist_ok=True)
 
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=0)
-@validate_path(pos=0)
-@validate_exists(pos=0)
-def load_single_tiff(path: Union[str, pathlib.Path]) -> np.ndarray:
+    file_size = images.nbytes * 1e-9  # convert to GB
+    if file_size <= size_cap:  # crop at 3.9 to be saved
+        filename = file_path.joinpath(name).with_suffix(".tif")
+        _save_single_tif(filename, images)
+    else:
+        filename = file_path.joinpath(name)
+        _save_many_tif(filename, images, size_cap)
+
+
+@validate_extension(required_extension=".tif", pos=0)
+@convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
+def _load_single_tif(file: Union[str, Path]) -> np.ndarray:
     """
     Load a single .tif as a numpy array
 
-    :param path: absolute filename
-    :type path: str or pathlib.Path
+    :param file: absolute filename
+    :type file: str or pathlib.Path
     :return: numpy array (frames, y-pixels, x-pixels)
     :rtype: numpy.ndarray
     """
-    image = []
-    with tifffile.TiffFile(path) as _file:
-        for _frame in _file.pages:
-            image.append(_frame.asarray())
-
-    return np.array(image)
+    return np.array(cv2.imreadmulti(file, flags=-1)[1])
 
 
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=1)
-@validate_path(pos=1)
-@require_full_path(pos=1)
-@validate_extension(required_extension=".tif", pos=1)
-def save_single_tiff(images: np.ndarray, path: Union[str, pathlib.Path], type_: Optional[np.dtype] = np.uint16) -> None:
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def _load_many_tif(folder: Union[str, Path]) -> np.ndarray:
     """
-    Save a numpy array to a single .tif file. Size must be <4 GB.
+    Loads all .tif's within a folder into a single numpy array.
 
-    :param images: numpy array [frames, y pixels, x pixels]
-    :type images: numpy.ndarray
-    :param path: filename or absolute path
-    :type path: str or pathlib.Path
-    :param type_: type for saving
-    :type type_: Optional[numpy.dtype] = numpy.uint16
-    :rtype: None
+    :param folder: folder containing a sequence of tiff stacks
+    :type folder: str or pathlib.Path
+    :return: a numpy array containing the images (frames, y-pixels, x-pixels)
+    :rtype: numpy.ndarray
     """
+    files = list(folder.glob("*tif"))
+    images = [_load_single_tif(file) for file in files]
 
-    # just save if single frame
-    if len(images.shape) == 2:
-        with tifffile.TiffWriter(path) as tif:
-            tif.save(np.floor(images).astype(type_))
-        return
-
-    with tifffile.TiffWriter(path) as tif:
-        for frame in np.floor(images).astype(type_):
-            tif.save(frame)
+    for image in images:
+        assert (image.shape[1:] == images[0].shape[1:]), "Images don't maintain consistent shape"
 
+    for image in images:
+        assert (image.dtype == images[0].dtype), "Images don't maintain consistent bit depth"
 
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=1)
-@validate_path(pos=1)
-def save_tiff_stack(images: str, output_folder: Union[str, pathlib.Path],
-                    type_: Optional[np.dtype] = np.uint16) -> None:
-    """
-    Save a numpy array to a sequence of .tif stacks
-
-    :param images: numpy array (frames, y-pixels, x-pixels)
-    :type images: numpy.ndarray
-    :param output_folder: folder to save the sequence of .tif stacks
-    :type output_folder: str or pathlib.Path
-    :param type_: type for saving
-    :type type_: Optional[numpy.dtype] = numpy.uint16
-    :rtype: None
-    """
-    _num_frames = images.shape[0]
+    return np.concatenate(images, axis=0)
 
-    _chunks = math.ceil(_num_frames / 7000)
 
-    c_idx = 1
-    for _chunk in range(0, _num_frames, 7000):
+@validate_extension(required_extension=".tif", pos=0)
+@convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
+def _save_single_tif(path: Union[str, Path], images: np.ndarray) -> int:
+    cv2.imwritemulti(path, images)
 
-        _start_idx = _chunk
-        _end_idx = _chunk + 7000
-        if _end_idx > _num_frames:
-            _end_idx = _num_frames + 1
-
-        if c_idx < 10:
-            save_single_tiff(images[_start_idx:_end_idx, :, :],
-                             output_folder + "\\" + "Video_0" + str(c_idx) + "_of_" + str(
-                                       _chunks) + ".tif", type_)
-        else:
-            save_single_tiff(images[_start_idx:_end_idx, :, :],
-                             output_folder + "\\" + "Video_" + str(c_idx) + "_of_" + str(
-                                       _chunks) + ".tif", type_)
-        c_idx += 1
-
-    return print("Finished Saving Tiffs")
-# REFACTOR at some point the CHUNKING
-
-
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=1)
-@validate_path(pos=1)
-@if_dir_append_filename(default_name="video_meta.txt", flag_pos=1)
-@if_dir_join_filename(default_name="binary_video", flag_pos=1)
-@validate_extension(required_extension=".txt", pos=2)
-def save_raw_binary(images: np.ndarray, path: Union[str, pathlib.Path],
-                    meta_filename: Optional[Union[str, pathlib.Path]]) -> None:
-    """
-    Save a numpy array as a binary file with an associated meta .txt file
 
-    :param images: numpy array (frames, y-pixels, x-pixels)
-    :type images: numpy.ndarray
-    :param path:  folder to save in or an absolute filepath for binary video file
-    :type path: str
-    :param meta_filename: absolute filepath for saving meta .txt file
-    :type meta_filename: str
-    :rtype: None
-    """
+@validate_extension(required_extension=".tif", pos=0)
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def _save_many_tif(path: Union[str, Path], images: np.ndarray, size_cap: int = 3.9) -> int:
+    frames_per_file = calculate_frames_per_file(*images.shape[1:], size_cap=size_cap)
+    frames = list(range(images.shape[0]))
+    blocks = generate_blocks(frames, frames_per_file, 0)
+    idx = 0
+    base_filename = path.with_suffix("")
 
     try:
-        pathlib.Path(path).parent.exists()
-    except AssertionError:
-        os.makedirs(str(pathlib.Path(path).parent))
-    finally:
-        with open(meta_filename, 'w') as f:
-            f.writelines([str(images.shape[0]), ",", str(images.shape[1]), ",",
-                          str(images.shape[2]), ",", str(images.dtype)])
-    images.tofile(path)
-    print("Finished saving images as a binary file.")
-# TODO UNIT TEST FOR EXCEPTIONS
-
-
-@convert_permitted_types_to_required(permitted=(str, pathlib.Path), required=str, pos=1)
-@validate_path(pos=1)
-@if_dir_join_filename(default_name="video.mp4", flag_pos=1)
-@validate_extension(required_extension=".mp4", pos=1)
-def save_video(images: np.ndarray, path: Union[str, pathlib.Path], fps: float = 30.0) -> None:
-    """
-    Save numpy array as an .mp4. Will be converted to uint8 if any other datatype.
-
-    :param images: numpy array (frames, y-pixels, x-pixels)
-    :type images: numpy.array
-    :param path: absolute filepath or filename
-    :type path: str or pathlib.Path
-    :param fps: frame rate for saved video
-    :type fps: float = 30.0
-    :rtype: None
-    """
-
-    if images.dtype.type != np.uint8:
-        print("\nForcing to unsigned 8-bit\n")
-        images = images.astype(np.uint8)
-
-    print("\nWriting Images to .mp4...\n")
-    mimwrite(path, images, fps=fps, quality=10, macro_block_size=4)
-    print("\nFinished writing images to .mp4.\n")
-# TODO: NO UNIT TEST
+        for block in blocks:
+            if idx <= 9:
+                filename = base_filename.with_name("".join([base_filename.name, "_0", str(idx)]))
+                filename = filename.with_suffix(".tif")
+            else:
+                filename = path.with_name("".join([base_filename.name, "_", str(idx)]))
+                filename = filename.with_suffix(".tif")
+            _save_single_tif(filename, images[block, :, :])
+            idx += 1
+    except RuntimeError:
+        pass
+    return 0
+
+
+class _Metadata:
+    def __init__(self, images: Optional[np.ndarray] = None):
+        """
+        Metadata object using for saving/loading binary images
+
+        :param images: images in numpy array (frames, y-pixels, x-pixels)
+        :type images: numpy.ndarray
+        """
+        self.frames, self.y, self.x, self.dtype = None, None, None, None
+
+        if images is not None:
+            self.frames, self.y, self.x = images.shape
+            self.dtype = str(images.dtype)
+
+    @classmethod
+    def decode(cls: _Metadata, filename: Path) -> _Metadata:
+
+        with open(str(filename), "r+") as file:
+            attrs = load(file)
+
+        metadata = _Metadata()
+        for key, value in attrs.items():
+            setattr(metadata, key, value)
+
+        if "dtype" not in attrs:
+            raise AttributeError("dtype not found")
+
+        missing_keys = []
+        for key in ["frames", "y", "x"]:
+            if key not in attrs:
+                missing_keys.append(key)
+
+        if len(missing_keys) > 1:
+            raise AttributeError("Require at least 2/3 shape keys")
+
+        if len(missing_keys) == 1:
+            setattr(metadata, missing_keys[0], -1)
+            # set to negative one to let numpy figure it out
+
+        return metadata
+
+    def encode(self, filename: Path) -> int:
+        meta = vars(self)
+        with open(str(filename), "w+") as file:
+            dump(meta, file)
+        return 0
```

### Comparing `CalSciPy-0.1.7/src/CalSciPy/reorganization.py` & `CalSciPy-0.2.0/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.1.7/src/CalSciPy/trace_processing.py` & `CalSciPy-0.2.0/src/CalSciPy/trace_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.1.7/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.2.0/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.1.7
+Version: 0.2.0
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
         
@@ -54,15 +54,16 @@
 [![Documentation Status](https://readthedocs.org/projects/calscipy/badge/?version=latest)](https://calscipy.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/CalSciPy?)
 ![PyPI - Status](https://img.shields.io/pypi/status/CalSciPy)
 ![GitHub](https://img.shields.io/github/license/darikoneil/CalSciPy)
 [![Contributors](https://img.shields.io/github/contributors-anon/darikoneil/CalSciPy)](https://github.com/darikoneil/CalSciPy/graphs/contributors)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/darikoneil/CalSciPy/calscipy_lint_test_action.yml)
 
-BETA STATUS: This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
+
+This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
 
 #### Highlights
 * Assign unique colormaps to subsets of ROIs to generate rich, informative videos
 * Perona-Malik diffusion for edge-preserving denoising
 * Methods for handling Bruker's PrairieView data
 * Interactive visualization
```

### Comparing `CalSciPy-0.1.7/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.2.0/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 pyproject.toml
 src/__init__.py
 src/CalSciPy/__init__.py
 src/CalSciPy/bruker.py
 src/CalSciPy/coloring.py
 src/CalSciPy/event_processing.py
 src/CalSciPy/image_processing.py
-src/CalSciPy/interactive_visuals.py
 src/CalSciPy/io_tools.py
+src/CalSciPy/misc.py
 src/CalSciPy/reorganization.py
-src/CalSciPy/static_visuals.py
 src/CalSciPy/trace_processing.py
-src/CalSciPy/validators.py
 src/CalSciPy/version.py
 src/CalSciPy.egg-info/PKG-INFO
 src/CalSciPy.egg-info/SOURCES.txt
 src/CalSciPy.egg-info/dependency_links.txt
 src/CalSciPy.egg-info/requires.txt
 src/CalSciPy.egg-info/top_level.txt
 tests/test_a_install.py
 tests/test_bruker.py
+tests/test_coloring.py
+tests/test_event_processing.py
+tests/test_io_tools.py
+tests/test_misc.py
 tests/test_reorganization.py
 tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.1.7/tests/test_a_install.py` & `CalSciPy-0.2.0/tests/test_a_install.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 import sys
-from PPVD.style import TerminalStyle
 import pytest
-import os
+from os import chdir
 from pathlib import Path
 import toml
+from PPVD.style import TerminalStyle
 
 
 def retrieve_details(path):
     details = toml.load(path).get("project")
     name = details.get("name")
     version = details.get("version")
     dependencies = details.get("dependencies")
@@ -16,32 +16,32 @@
 
 
 def retrieve_project_directory(path):
     return Path(path).parent
 
 
 def retrieve_project_file():
-    project_file = os.path.join(os.getcwd(), "pyproject.toml")
-    if not os.path.exists(project_file):
-        project_file = os.path.join(Path(os.getcwd()).parent, "pyproject.toml")
-    if not os.path.exists(project_file):
+    project_file = Path.cwd().joinpath("pyproject.toml")
+    if not Path.exists(project_file):
+        project_file = Path.cwd().parent.joinpath("pyproject.toml")
+    if not Path.exists(project_file):
         raise FileNotFoundError("Can't find project file")
     return project_file
 
 
 def collect_project():
     project_file = retrieve_project_file()
     project_directory = retrieve_project_directory(project_file)
     package_name, package_version, package_dependencies = retrieve_details(project_file)
     return project_directory, project_file, package_name, package_version, package_dependencies
 
 
 # get project information and work from correct directory
 proj_dir, proj_file, pkg_name, pkg_version, pkg_dependencies = collect_project()
-os.chdir(proj_dir)
+chdir(proj_dir)
 
 
 print(f"\n{TerminalStyle.YELLOW}Package: {TerminalStyle.BLUE}{pkg_name}{TerminalStyle.RESET}")
 print(f"{TerminalStyle.YELLOW}Version: {TerminalStyle.BLUE}{pkg_version}{TerminalStyle.RESET}")
 print(f"{TerminalStyle.YELLOW}Dependencies: {TerminalStyle.BLUE}{pkg_dependencies}{TerminalStyle.RESET}")
```

### Comparing `CalSciPy-0.1.7/tests/test_bruker.py` & `CalSciPy-0.2.0/tests/test_bruker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import pytest
 import numpy as np
 from pathlib import Path
 from shutil import rmtree
 from tests.helpers import BlockPrinting, read_descriptions
 from tests.conftest import SAMPLES_DATASETS_DIRECTORY
-from CalSciPy.io_tools import load_all_tiffs, load_single_tiff
-from CalSciPy.bruker import determine_imaging_content, load_bruker_tiffs, repackage_bruker_tiffs
+from CalSciPy.io_tools import load_images
+from CalSciPy.bruker import determine_imaging_content, load_bruker_tifs, repackage_bruker_tifs
 
 
 DATASET = pytest.mark.datafiles(
     SAMPLES_DATASETS_DIRECTORY,
     keep_top_dir=False,
     on_duplicate="ignore",
 )
 
 
 @DATASET
 def test_determine_imaging_content(datafiles):
     with BlockPrinting():
         for _dir in datafiles.listdir():
-
-            _input_folder = next(Path(_dir).glob("bruker_folder"))
-            _descriptions = next(Path(_dir).glob("description.txt"))
+            _input_folder = Path(_dir).joinpath("bruker_folder")
+            _descriptions = Path(_dir).joinpath("description.txt")
             _descriptions = read_descriptions(_descriptions)
 
             _contents = determine_imaging_content(_input_folder)
 
             for _test in enumerate(["Channel", "Plane", "Frame", "Height", "Width"]):
                 assert _contents[_test[0]] == _descriptions[_test[0]], f"Description Mismatch: failed on dataset " \
                                                                        f"{Path(_dir).name}: " \
@@ -36,36 +35,37 @@
 
 
 @DATASET
 def test_repackage_bruker_tiffs(datafiles, tmp_path):
     with BlockPrinting():
         for _dir in datafiles.listdir():
             # INGEST
-            _input_folder = next(Path(_dir).glob("bruker_folder"))
-            _descriptions = next(Path(_dir).glob("description.txt"))
+            _input_folder = Path(_dir).joinpath("bruker_folder")
+            _descriptions = Path(_dir).joinpath("description.txt")
             _output_folder = Path(tmp_path).joinpath("".join([Path(_dir).stem, "_output"]))
             # MAKE OUTPUT FOLDER
             _output_folder.mkdir(parents=True, exist_ok=True)
             # RUN FUNCTION
-            repackage_bruker_tiffs(_input_folder, _output_folder, (0, 0))
+            repackage_bruker_tifs(_input_folder, _output_folder, (0, 0))
             # TEST
             _descriptions = read_descriptions(_descriptions)
-            _contents = load_all_tiffs(_output_folder)
+            _contents = load_images(_output_folder)
             assert _contents.shape[0] == np.cumprod(_descriptions[2])[-1], f"Image Mismatch: failed on dataset" \
                                                                            f"{_input_folder.name}"
 
 
 @DATASET
 def test_load_bruker_tiffs(datafiles):
     with BlockPrinting():
         for _dir in datafiles.listdir():
             # INGEST
-            _input_folder = next(Path(_dir).glob("bruker_folder"))
-            _input_image = next(Path(_dir).glob("Video_01_of_1.tif"))
-            _descriptions = next(Path(_dir).glob("description.txt"))
+            _input_folder = Path(_dir).joinpath("bruker_folder")
+            _input_image = Path(_dir).joinpath("multi_page", "images.tif")
+            _descriptions = Path(_dir).joinpath("description.txt")
             # LOAD COMPARISON
             _descriptions = read_descriptions(_descriptions)
-            _image1 = load_single_tiff(_input_image)
+            _image1 = load_images(_input_image)
             # TEST
-            _image2 = load_bruker_tiffs(_input_folder, 1, 0)[0]
-            np.testing.assert_array_equal(_image1, _image2, err_msg=f"Image Mismatch: failed on dataset "
-                                                                    f"{_input_folder.name}")
+            _image2 = load_bruker_tifs(_input_folder, 1, 0)[0]
+            np.testing.assert_array_equal(_image1[0, :, :], _image2[0, :, :],
+                                          err_msg=f"Image Mismatch: failed on dataset "
+                                                  f"{_input_folder.name}")
```

### Comparing `CalSciPy-0.1.7/tests/test_reorganization.py` & `CalSciPy-0.2.0/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.1.7/tests/test_trace_processing.py` & `CalSciPy-0.2.0/tests/test_trace_processing.py`

 * *Files identical despite different names*

