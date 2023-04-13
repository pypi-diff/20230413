# Comparing `tmp/tifffile-2023.3.21.tar.gz` & `tmp/tifffile-2023.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifffile-2023.3.21.tar", last modified: Wed Mar 22 00:46:30 2023, max compression
+gzip compressed data, was "tifffile-2023.4.12.tar", last modified: Wed Apr 12 22:27:08 2023, max compression
```

## Comparing `tifffile-2023.3.21.tar` & `tifffile-2023.4.12.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 00:46:30.777109 tifffile-2023.3.21/
--rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2023.3.21/ACKNOWLEDGEMENTS.rst
--rw-rw-rw-   0        0        0    35235 2023-03-22 00:46:24.000000 tifffile-2023.3.21/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2023-03-22 00:46:24.000000 tifffile-2023.3.21/LICENSE
--rw-rw-rw-   0        0        0      540 2023-01-23 07:24:27.000000 tifffile-2023.3.21/MANIFEST.in
--rw-rw-rw-   0        0        0    30541 2023-03-22 00:46:30.777109 tifffile-2023.3.21/PKG-INFO
--rw-rw-rw-   0        0        0    29608 2023-03-22 00:46:24.000000 tifffile-2023.3.21/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-22 00:46:30.752482 tifffile-2023.3.21/docs/
-drwxrwxrwx   0        0        0        0 2023-03-22 00:46:30.752482 tifffile-2023.3.21/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2023.3.21/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1098 2023-01-12 21:14:58.000000 tifffile-2023.3.21/docs/conf.py
--rw-rw-rw-   0        0        0     3629 2023-03-04 01:54:58.000000 tifffile-2023.3.21/docs/make.py
-drwxrwxrwx   0        0        0        0 2023-03-22 00:46:30.752482 tifffile-2023.3.21/examples/
--rw-rw-rw-   0        0        0    15054 2023-02-07 15:45:27.000000 tifffile-2023.3.21/examples/earthbigdata.py
--rw-rw-rw-   0        0        0     2539 2023-01-10 16:09:24.000000 tifffile-2023.3.21/examples/issue125.py
--rw-rw-rw-   0        0        0       42 2023-03-22 00:46:30.779158 tifffile-2023.3.21/setup.cfg
--rw-rw-rw-   0        0        0     3708 2023-01-23 07:09:38.000000 tifffile-2023.3.21/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 00:46:30.757317 tifffile-2023.3.21/tests/
--rw-rw-rw-   0        0        0     1601 2023-03-14 03:16:25.000000 tifffile-2023.3.21/tests/conftest.py
--rw-rw-rw-   0        0        0   694943 2023-03-22 00:17:26.000000 tifffile-2023.3.21/tests/test_tifffile.py
-drwxrwxrwx   0        0        0        0 2023-03-22 00:46:30.769251 tifffile-2023.3.21/tifffile/
--rw-rw-rw-   0        0        0      110 2020-01-01 02:31:34.000000 tifffile-2023.3.21/tifffile/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2023.3.21/tifffile/__main__.py
--rw-rw-rw-   0        0        0    11839 2022-12-29 20:31:08.000000 tifffile-2023.3.21/tifffile/_imagecodecs.py
--rw-rw-rw-   0        0        0    61794 2022-07-28 19:50:49.000000 tifffile-2023.3.21/tifffile/geodb.py
--rw-rw-rw-   0        0        0      680 2022-06-04 00:53:35.000000 tifffile-2023.3.21/tifffile/lsm2bin.py
--rw-rw-rw-   0        0        0     5906 2023-03-10 03:08:14.000000 tifffile-2023.3.21/tifffile/numcodecs.py
--rw-rw-rw-   0        0        0     2410 2022-05-13 03:22:47.000000 tifffile-2023.3.21/tifffile/tiff2fsspec.py
--rw-rw-rw-   0        0        0     1437 2022-06-04 00:53:09.000000 tifffile-2023.3.21/tifffile/tiffcomment.py
--rw-rw-rw-   0        0        0   856311 2023-03-21 23:57:56.000000 tifffile-2023.3.21/tifffile/tifffile.py
-drwxrwxrwx   0        0        0        0 2023-03-22 00:46:30.777109 tifffile-2023.3.21/tifffile.egg-info/
--rw-rw-rw-   0        0        0    30541 2023-03-22 00:46:29.000000 tifffile-2023.3.21/tifffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-03-22 00:46:30.000000 tifffile-2023.3.21/tifffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 00:46:29.000000 tifffile-2023.3.21/tifffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-03-22 00:46:29.000000 tifffile-2023.3.21/tifffile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-03-22 00:46:29.000000 tifffile-2023.3.21/tifffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-22 00:46:29.000000 tifffile-2023.3.21/tifffile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.119431 tifffile-2023.4.12/
+-rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2023.4.12/ACKNOWLEDGEMENTS.rst
+-rw-rw-rw-   0        0        0    35595 2023-04-12 22:27:05.000000 tifffile-2023.4.12/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2023-04-12 22:27:05.000000 tifffile-2023.4.12/LICENSE
+-rw-rw-rw-   0        0        0      540 2023-01-23 07:24:27.000000 tifffile-2023.4.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    30901 2023-04-12 22:27:08.119431 tifffile-2023.4.12/PKG-INFO
+-rw-rw-rw-   0        0        0    29968 2023-04-12 22:27:05.000000 tifffile-2023.4.12/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.091431 tifffile-2023.4.12/docs/
+drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.091431 tifffile-2023.4.12/docs/_static/
+-rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2023.4.12/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1098 2023-01-12 21:14:58.000000 tifffile-2023.4.12/docs/conf.py
+-rw-rw-rw-   0        0        0     3629 2023-03-04 01:54:58.000000 tifffile-2023.4.12/docs/make.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.095431 tifffile-2023.4.12/examples/
+-rw-rw-rw-   0        0        0    15054 2023-02-07 15:45:27.000000 tifffile-2023.4.12/examples/earthbigdata.py
+-rw-rw-rw-   0        0        0     2539 2023-01-10 16:09:24.000000 tifffile-2023.4.12/examples/issue125.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 22:27:08.119431 tifffile-2023.4.12/setup.cfg
+-rw-rw-rw-   0        0        0     3708 2023-01-23 07:09:38.000000 tifffile-2023.4.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.095431 tifffile-2023.4.12/tests/
+-rw-rw-rw-   0        0        0     1601 2023-03-14 03:16:25.000000 tifffile-2023.4.12/tests/conftest.py
+-rw-rw-rw-   0        0        0   700808 2023-04-12 22:24:28.000000 tifffile-2023.4.12/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.107430 tifffile-2023.4.12/tifffile/
+-rw-rw-rw-   0        0        0      110 2020-01-01 02:31:34.000000 tifffile-2023.4.12/tifffile/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2023.4.12/tifffile/__main__.py
+-rw-rw-rw-   0        0        0    11839 2022-12-29 20:31:08.000000 tifffile-2023.4.12/tifffile/_imagecodecs.py
+-rw-rw-rw-   0        0        0    61794 2022-07-28 19:50:49.000000 tifffile-2023.4.12/tifffile/geodb.py
+-rw-rw-rw-   0        0        0      680 2022-06-04 00:53:35.000000 tifffile-2023.4.12/tifffile/lsm2bin.py
+-rw-rw-rw-   0        0        0     5906 2023-03-10 03:08:14.000000 tifffile-2023.4.12/tifffile/numcodecs.py
+-rw-rw-rw-   0        0        0     2410 2022-05-13 03:22:47.000000 tifffile-2023.4.12/tifffile/tiff2fsspec.py
+-rw-rw-rw-   0        0        0     1437 2022-06-04 00:53:09.000000 tifffile-2023.4.12/tifffile/tiffcomment.py
+-rw-rw-rw-   0        0        0   859764 2023-04-12 21:35:37.000000 tifffile-2023.4.12/tifffile/tifffile.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.119431 tifffile-2023.4.12/tifffile.egg-info/
+-rw-rw-rw-   0        0        0    30901 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-04-12 22:27:07.000000 tifffile-2023.4.12/tifffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/top_level.txt
```

### Comparing `tifffile-2023.3.21/CHANGES.rst` & `tifffile-2023.4.12/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Revisions
 ---------
 
+2023.4.12
+
+- Pass 4988 tests.
+- Do not write duplicate ImageDescription tags from extratags (breaking).
+- Support multifocal SVS files (#193).
+- Log warning when filtering out extratags.
+- Fix writing OME-TIFF with image description in extratags.
+- Ignore invalid predictor tag value if prediction is not used.
+- Raise KeyError if ZarrStore is missing requested chunk.
+
 2023.3.21
 
-- Pass 4981 tests.
 - Fix reading MMstack with missing data (#187).
 
 2023.3.15
 
 - Fix corruption using tile generators with prediction/compression (#185).
 - Add parser for Micro-Manager MMStack series (breaking).
 - Return micromanager_metadata IndexMap as numpy array (breaking).
```

### Comparing `tifffile-2023.3.21/LICENSE` & `tifffile-2023.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/MANIFEST.in` & `tifffile-2023.4.12/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/PKG-INFO` & `tifffile-2023.4.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2023.3.21
+Version: 2023.4.12
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -51,15 +51,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.3.21
+:Version: 2023.4.12
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -87,33 +87,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.10, 3.11.2, 64-bit
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.3.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.4.12
+
+- Pass 4988 tests.
+- Do not write duplicate ImageDescription tags from extratags (breaking).
+- Support multifocal SVS files (#193).
+- Log warning when filtering out extratags.
+- Fix writing OME-TIFF with image description in extratags.
+- Ignore invalid predictor tag value if prediction is not used.
+- Raise KeyError if ZarrStore is missing requested chunk.
+
 2023.3.21
 
-- Pass 4981 tests.
 - Fix reading MMstack with missing data (#187).
 
 2023.3.15
 
 - Fix corruption using tile generators with prediction/compression (#185).
 - Add parser for Micro-Manager MMStack series (breaking).
 - Return micromanager_metadata IndexMap as numpy array (breaking).
```

### Comparing `tifffile-2023.3.21/README.rst` & `tifffile-2023.4.12/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.3.21
+:Version: 2023.4.12
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -62,33 +62,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.10, 3.11.2, 64-bit
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.3.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.4.12
+
+- Pass 4988 tests.
+- Do not write duplicate ImageDescription tags from extratags (breaking).
+- Support multifocal SVS files (#193).
+- Log warning when filtering out extratags.
+- Fix writing OME-TIFF with image description in extratags.
+- Ignore invalid predictor tag value if prediction is not used.
+- Raise KeyError if ZarrStore is missing requested chunk.
+
 2023.3.21
 
-- Pass 4981 tests.
 - Fix reading MMstack with missing data (#187).
 
 2023.3.15
 
 - Fix corruption using tile generators with prediction/compression (#185).
 - Add parser for Micro-Manager MMStack series (breaking).
 - Return micromanager_metadata IndexMap as numpy array (breaking).
```

### Comparing `tifffile-2023.3.21/docs/conf.py` & `tifffile-2023.4.12/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/docs/make.py` & `tifffile-2023.4.12/docs/make.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/examples/earthbigdata.py` & `tifffile-2023.4.12/examples/earthbigdata.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/examples/issue125.py` & `tifffile-2023.4.12/examples/issue125.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/setup.py` & `tifffile-2023.4.12/setup.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tests/conftest.py` & `tifffile-2023.4.12/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tests/test_tifffile.py` & `tifffile-2023.4.12/tests/test_tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # mypy: check-untyped-defs=False
 
 """Unittests for the tifffile package.
 
 Public data files can be requested from the author.
 Private data files are not available due to size and copyright restrictions.
 
-:Version: 2023.3.21
+:Version: 2023.4.12
 
 """
 
 import binascii
 import datetime
 import glob
 import json
@@ -1720,16 +1720,16 @@
     # https://github.com/cgohlke/tifffile/issues/112
     with TempFileName('issue_description_bytes') as fname:
         imwrite(
             fname,
             [[0]],
             description='1st description',
             extratags=[
-                (270, 1, None, b'\1\128\0', True),
-                (270, 1, None, b'\2\128\0', True),
+                ('ImageDescription', 1, None, b'\1\128\0', True),
+                ('ImageDescription', 1, None, b'\2\128\0', True),
             ],
             metadata=False,
         )
         with TiffFile(fname) as tif:
             page = tif.pages.first
             assert page.description == '1st description'
             assert page.description1 == ''
@@ -2512,14 +2512,51 @@
             or not imagecodecs.TIFF
             or (compression == 'packbits' and predictor == 'horizontal')
         ):
             return
         assert_array_equal(imagecodecs.imread(fname), data.squeeze())
 
 
+def test_issue_extratags_filter(caplog):
+    """Test filtering extratags."""
+    # https://github.com/cgohlke/tifffile/pull/188
+    with TempFileName('extratags_filter') as fname:
+        imwrite(
+            fname,
+            shape=(10, 10),
+            dtype='u1',
+            extratags=[
+                (322, 3, 1, 2, False),  # TileWidth is filtered
+                (34665, 13, 1, 0, False),  # ExifIFD is filtered
+                (270, 2, 0, 'second description', True),  # filtered
+                ('FillOrder', 3, 1, 1, True),  # by name should go through
+            ],
+        )
+        assert 'extratag 322' in caplog.text
+        assert 'extratag 34665' in caplog.text
+        with TiffFile(fname) as tif:
+            tags = tif.pages.first.tags
+            assert 322 not in tags
+            assert 34665 not in tags
+            assert tags.get(270, index=1) is None
+            assert tags[266].value == 1
+
+
+def test_issue_invalid_predictor(caplog):
+    """Test decoding JPEG compression with invalid predictor tag."""
+    fname = private_file('issues/invalid_predictor.tiff')
+    with TiffFile(fname) as tif:
+        page = tif.pages.first
+        assert page.predictor == 58240
+        assert page.compression == 7
+        data = page.asarray()
+        assert 'ignoring predictor' in caplog.text
+        assert data.shape == (1275, 1650, 4)
+
+
 class TestExceptions:
     """Test various Exceptions and Warnings."""
 
     data = random_data(numpy.uint16, (5, 13, 17))
 
     @pytest.fixture(scope='class')
     def fname(self):
@@ -11922,26 +11959,34 @@
         assert meta['Summary']['MicroManagerVersion'] == '1.4.16 20140128'
         assert meta['Summary']['Prefix'] == 'movie_9'
         assert meta['IndexMap'].shape == (125, 5)
         assert meta['Comments'] == {'Summary': ''}
         assert meta['DisplaySettings'][0]['Name'] == 'Dual-GFP'
         # assert series properties
         series = tif.series[0]
+        assert series[-1] is None  # missing page
         assert len(series) == 126
         assert series.shape == (63, 2, 264, 320)
         assert series.axes == 'TCYX'
         assert series.kind == 'mmstack'
         assert not series.is_multifile
         # assert data
         data = tif.asarray()
         assert isinstance(data, numpy.ndarray)
         assert data.shape == (63, 2, 264, 320)
         assert data.dtype == numpy.uint16
         assert data[59, 1, 151, 186] == 599
-        assert_aszarr_method(series, data)
+        # assert zarr
+        if not SKIP_ZARR and zarr is not None:
+            with series.aszarr(fillvalue=100) as store:
+                assert '1.1.0.0' in store
+                assert '62.1.0.0' not in store  # missing page
+                z = zarr.open(store, mode='r')
+                assert z[62, 1, 0, 0] == 100
+                assert_array_equal(data[:62], z[:62])
         # test OME and ImageJ
         assert_array_equal(data, imread(fname, is_mmstack=False))
         assert_array_equal(data, imread(fname, is_mmstack=False, is_ome=False))
         assert__str__(tif)
 
 
 @pytest.mark.skipif(SKIP_PRIVATE or SKIP_LARGE, reason=REASON)
@@ -13440,15 +13485,15 @@
 
 def test_write_extratags():
     """Test write extratags."""
     data = random_data(numpy.uint8, (2, 219, 301))
     description = 'Created by TestTiffWriter\nLorem ipsum dolor...'
     pagename = 'Page name'
     extratags = [
-        (270, 's', 0, description, True),
+        ('ImageDescription', 's', 0, description, True),
         ('PageName', 's', 0, pagename, False),
         (50001, 'b', 1, b'1', True),
         (50002, 'b', 2, b'12', True),
         (50004, 'b', 4, b'1234', True),
         (50008, 'B', 8, b'12345678', True),
     ]
     with TempFileName('extratags') as fname:
@@ -13579,14 +13624,28 @@
                 assert page.tags['DateTime'].value == dt
                 assert page.datetime == datetime.datetime.strptime(
                     dt, '%Y:%m:%d %H:%M:%S'
                 )
             assert__str__(tif)
 
 
+def test_write_software_tag():
+    """Test write Software tag."""
+    data = random_data(numpy.uint8, (2, 219, 301))
+    software = 'test_tifffile.py'
+    with TempFileName('software_tag') as fname:
+        imwrite(fname, data, software=software)
+        assert_valid_tiff(fname)
+        with TiffFile(fname) as tif:
+            assert len(tif.pages) == 2
+            assert tif.pages.first.software == software
+            assert 'Software' not in tif.pages[1].tags
+            assert__str__(tif)
+
+
 def test_write_description_tag():
     """Test write two description tags."""
     data = random_data(numpy.uint8, (2, 219, 301))
     description = 'Created by TestTiffWriter\nLorem ipsum dolor...'
     with TempFileName('description_tag') as fname:
         imwrite(fname, data, description=description)
         assert_valid_tiff(fname)
@@ -13630,26 +13689,115 @@
             assert (
                 tif.pages.first.tags.get('ImageDescription', index=1) is None
             )
             assert tif.series[0].kind == 'generic'
             assert__str__(tif)
 
 
-def test_write_software_tag():
-    """Test write Software tag."""
-    data = random_data(numpy.uint8, (2, 219, 301))
-    software = 'test_tifffile.py'
-    with TempFileName('software_tag') as fname:
-        imwrite(fname, data, software=software)
-        assert_valid_tiff(fname)
+def test_write_description_ome():
+    """Test write multiple imagedescription tags to OME."""
+    # https://forum.image.sc/t/79471
+    with TempFileName('description_ome') as fname:
+        with pytest.warns(UserWarning):
+            imwrite(
+                fname,
+                shape=(2, 32, 32),
+                dtype='uint8',
+                ome=True,
+                description='description',  # not written
+                extratags=[('ImageDescription', 2, None, 'extratags', False)],
+            )
         with TiffFile(fname) as tif:
-            assert len(tif.pages) == 2
-            assert tif.pages.first.software == software
-            assert 'Software' not in tif.pages[1].tags
-            assert__str__(tif)
+            assert tif.is_ome
+            page = tif.pages.first
+            assert page.description.startswith('<?xml')
+            assert page.description1 == 'extratags'
+            assert tif.pages[1].description == 'extratags'
+
+
+def test_write_description_imagej():
+    """Test write multiple imagedescription tags."""
+    with TempFileName('description_imagej') as fname:
+        with pytest.warns(UserWarning):
+            imwrite(
+                fname,
+                shape=(2, 32, 32),
+                dtype='uint8',
+                imagej=True,
+                description='description',  # not written
+                extratags=[('ImageDescription', 2, None, 'extratags', False)],
+            )
+        with TiffFile(fname) as tif:
+            assert tif.is_imagej
+            page = tif.pages.first
+            assert page.description.startswith('ImageJ=')
+            assert page.description1 == 'extratags'
+            assert tif.pages[1].description == 'extratags'
+
+
+def test_write_description_shaped():
+    """Test write multiple imagedescription tags to shaped."""
+    with TempFileName('description_shaped') as fname:
+        imwrite(
+            fname,
+            shape=(2, 32, 32),
+            dtype='uint8',
+            description='description',  # written
+            extratags=[('ImageDescription', 2, None, 'extratags', False)],
+        )
+        with TiffFile(fname) as tif:
+            assert tif.is_shaped
+            page = tif.pages.first
+            assert page.description == 'description'
+            assert page.description1.startswith('{')
+            assert page.tags.getall(270)[2].value == 'extratags'
+            assert tif.pages[1].description == 'extratags'
+
+
+def test_write_description_overwrite():
+    """Test overwrite imagedescription tag."""
+    with TempFileName('description_overwrite') as fname:
+        with TiffWriter(fname) as tif:
+            tif.write(
+                shape=(2, 32, 32),
+                dtype='uint8',
+                description='description',  # overwritten
+                extratags=[('ImageDescription', 2, None, 'extratags', False)],
+                metadata=None,
+            )
+            tif.overwrite_description('overwritten description')
+        with TiffFile(fname) as tif:
+            assert not tif.is_shaped
+            page = tif.pages.first
+            assert page.description == 'overwritten description'
+            assert page.description1 == 'extratags'
+            assert tif.pages[1].description == 'extratags'
+
+
+def test_write_description_extratags():
+    """Test write imagedescription tags using extratag."""
+    with TempFileName('description_extratags') as fname:
+        with TiffWriter(fname) as tif:
+            tif.write(
+                shape=(2, 32, 32),
+                dtype='uint8',
+                extratags=[
+                    (270, 2, None, 'description 0', False),
+                    ('ImageDescription', 2, None, 'description 1', False),
+                ],
+                metadata=None,
+            )
+        with TiffFile(fname) as tif:
+            assert not tif.is_shaped
+            page = tif.pages.first
+            assert page.description == 'description 0'
+            assert page.description1 == 'description 1'
+            page = tif.pages[1]
+            assert page.description == 'description 0'
+            assert page.description1 == 'description 1'
 
 
 def test_write_resolution_float():
     """Test write float Resolution tag."""
     data = random_data(numpy.uint8, (2, 219, 301))
     resolution = (92.0, 92.0)
     with TempFileName('resolution_float') as fname:
@@ -18295,15 +18443,15 @@
     """Test opentile package."""
     # https://github.com/imi-bigpicture/opentile
     try:
         from hashlib import md5
 
         import turbojpeg
         from opentile.geometry import Point
-        from opentile.ndpi_tiler import NdpiTiler
+        from opentile.formats import NdpiTiler
     except ImportError:
         pytest.skip('opentile missing')
 
     fname = private_file('HamamatsuNDPI/CMU-1.ndpi')
 
     turbo_path = os.path.join(
         os.path.dirname(turbojpeg.__file__), 'turbojpeg.dll'
```

### Comparing `tifffile-2023.3.21/tifffile/_imagecodecs.py` & `tifffile-2023.4.12/tifffile/_imagecodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tifffile/geodb.py` & `tifffile-2023.4.12/tifffile/geodb.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tifffile/lsm2bin.py` & `tifffile-2023.4.12/tifffile/lsm2bin.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tifffile/numcodecs.py` & `tifffile-2023.4.12/tifffile/numcodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tifffile/tiff2fsspec.py` & `tifffile-2023.4.12/tifffile/tiff2fsspec.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tifffile/tiffcomment.py` & `tifffile-2023.4.12/tifffile/tiffcomment.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.3.21/tifffile/tifffile.py` & `tifffile-2023.4.12/tifffile/tifffile.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.3.21
+:Version: 2023.4.12
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -92,33 +92,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.10, 3.11.2, 64-bit
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.3.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.4.12
+
+- Pass 4988 tests.
+- Do not write duplicate ImageDescription tags from extratags (breaking).
+- Support multifocal SVS files (#193).
+- Log warning when filtering out extratags.
+- Fix writing OME-TIFF with image description in extratags.
+- Ignore invalid predictor tag value if prediction is not used.
+- Raise KeyError if ZarrStore is missing requested chunk.
+
 2023.3.21
 
-- Pass 4981 tests.
 - Fix reading MMstack with missing data (#187).
 
 2023.3.15
 
 - Fix corruption using tile generators with prediction/compression (#185).
 - Add parser for Micro-Manager MMStack series (breaking).
 - Return micromanager_metadata IndexMap as numpy array (breaking).
@@ -793,15 +802,15 @@
 
     $ python -m tifffile temp.ome.tif
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.3.21'
+__version__ = '2023.4.12'
 
 __all__ = [
     'TiffFile',
     'TiffFileError',
     'TiffFrame',
     'TiffPage',
     'TiffPages',
@@ -1827,15 +1836,17 @@
                    Not used for string or bytes values.
                 3. value (Sequence[Any]): `count` values compatible with
                    `dtype`. Bytes must contain count values of dtype packed
                    as binary data.
                 4. writeonce (bool): If *True*, write tag to first page
                    of a series only.
 
-                Duplicate and select tags in TIFF.TAG_FILTERED are not written.
+                Duplicate and select tags in TIFF.TAG_FILTERED are not written
+                if the extratag is specified by integer code.
+                Extratags cannot be used to write IFD type tags.
 
             contiguous:
                 If *False* (default), write data to a new series.
                 If *True* and the data and arguments are compatible with
                 previous written ones (same shape, no compression, etc.),
                 the image data are stored contiguously after the previous one.
                 In that case, `photometric`, `planarconfig`, and
@@ -2584,15 +2595,16 @@
             # ImageDescription: user provided description
             addtag(tags, 270, 2, 0, description, True)
 
         # write shape and metadata to ImageDescription
         self._metadata = {} if not metadata else metadata.copy()
         if self._omexml is not None:
             if len(self._omexml.images) == 0:
-                description = ''  # rewritten later at end of file
+                # rewritten later at end of file
+                description = '\x00\x00\x00\x00'
             else:
                 description = None
         elif self._imagej:
             ijmetadata = parse_kwargs(
                 self._metadata,
                 'Info',
                 'Labels',
@@ -2624,23 +2636,31 @@
         elif self._tifffile and (metadata or metadata == {}):
             if self._truncate:
                 self._metadata.update(truncated=True)
             description = shaped_description(inputshape, **self._metadata)
             description += '\x00' * 16  # add buffer for in-place update
         # elif metadata is None and self._truncate:
         #     raise ValueError('cannot truncate without writing metadata')
-        else:
+        elif description is not None:
+            if not isinstance(description, bytes):
+                description = description.encode('ascii')
+            self._descriptiontag = TiffTag(
+                self, 0, 270, 2, len(description), description, 0
+            )
             description = None
 
         if description is None:
             # disable shaped format if user disabled metadata
             self._tifffile = False
         else:
             description = description.encode('ascii')
             addtag(tags, 270, 2, 0, description, True)
+            self._descriptiontag = TiffTag(
+                self, 0, 270, 2, len(description), description, 0
+            )
         del description
 
         if software is None:
             software = 'tifffile.py'
         if software:
             addtag(tags, 305, 2, 0, software, True)
         if datetime:
@@ -2972,19 +2992,18 @@
         if dataiter is None and not contiguous:
             raise ValueError('cannot write non-contiguous empty file')
 
         # add extra tags from user; filter duplicate and select tags
         extratag: TagTuple
         tagset = {t[0] for t in tags}
         tagset.update(TIFF.TAG_FILTERED)
-        if 270 in tagset:
-            # allow duplicate ImageDescription
-            tagset.remove(270)
         for extratag in extratags:
-            if extratag[0] not in tagset:
+            if extratag[0] in tagset:
+                log_warning(f'{self!r} not writing extratag {extratag[0]}')
+            else:
                 addtag(tags, *extratag)
         del tagset
         del extratags
 
         # TODO: check TIFFReadDirectoryCheckOrder warning in files containing
         #   multiple tags of same code
         # the entries in an IFD must be sorted in ascending order by tag code
@@ -3143,33 +3162,43 @@
                         ifd.seek(pos)
                         ifd.write(value)
                         if code == tagoffsets:
                             dataoffsetsoffset = offset, pos
                         elif code == tagbytecounts:
                             databytecountsoffset = offset, pos
                         elif code == 270:
-                            assert self._descriptiontag is not None
-                            self._descriptiontag.offset = (
-                                ifdpos + tagoffset + tagindex * tagsize
-                            )
-                            self._descriptiontag.valueoffset = ifdpos + pos
+                            if (
+                                self._descriptiontag is not None
+                                and self._descriptiontag.offset == 0
+                                and value.startswith(
+                                    self._descriptiontag.value
+                                )
+                            ):
+                                self._descriptiontag.offset = (
+                                    ifdpos + tagoffset + tagindex * tagsize
+                                )
+                                self._descriptiontag.valueoffset = ifdpos + pos
                         elif code == 330:
                             subifdsoffsets = offset, pos
                     elif code == tagoffsets:
                         dataoffsetsoffset = offset, None
                     elif code == tagbytecounts:
                         databytecountsoffset = offset, None
                     elif code == 270:
-                        assert self._descriptiontag is not None
-                        self._descriptiontag.offset = (
-                            ifdpos + tagoffset + tagindex * tagsize
-                        )
-                        self._descriptiontag.valueoffset = (
-                            self._descriptiontag.offset + offsetsize + 4
-                        )
+                        if (
+                            self._descriptiontag is not None
+                            and self._descriptiontag.offset == 0
+                            and self._descriptiontag.value in tag[1][-4:]
+                        ):
+                            self._descriptiontag.offset = (
+                                ifdpos + tagoffset + tagindex * tagsize
+                            )
+                            self._descriptiontag.valueoffset = (
+                                self._descriptiontag.offset + offsetsize + 4
+                            )
                     elif code == 330:
                         subifdsoffsets = offset, None
                 ifdsize = ifd.tell()
                 if ifdsize % 2:
                     ifd.write(b'\x00')
                     ifdsize += 1
 
@@ -3706,19 +3735,18 @@
                 except UnicodeEncodeError as exc:
                     raise ValueError(
                         'TIFF strings must be 7-bit ASCII'
                     ) from exc
             elif not isinstance(value, bytes):
                 raise ValueError('TIFF strings must be 7-bit ASCII')
 
-            if len(value) == 0 or value[-1] != b'\x00':
+            if len(value) == 0 or value[-1:] != b'\x00':
                 value += b'\x00'
             count = len(value)
             if code == 270:
-                self._descriptiontag = TiffTag(self, 0, 270, 2, count, None, 0)
                 rawcount = int(value.find(b'\x00\x00'))
                 if rawcount < 0:
                     rawcount = count
                 else:
                     # length of string without buffer
                     rawcount = max(self.tiff.offsetsize + 1, rawcount + 1)
                     rawcount = min(count, rawcount)
@@ -5065,61 +5093,82 @@
 
         series = []
         self.pages.cache = True
         self.pages.useframes = False
         self.pages.set_keyframe(0)
         self.pages._load()
 
-        # Baseline
-        index = 0
-        page = self.pages[index]
-        series.append(
-            TiffPageSeries(
-                [page],
-                page.shape,
-                page.dtype,
-                page.axes,
-                name='Baseline',
-                kind='svs',
-            )
-        )
-        # Thumbnail
-        index += 1
-        if index == len(self.pages):
+        # baseline
+        firstpage = self.pages.first
+        if len(self.pages) == 1:
             self.is_uniform = False
-            return series
-        page = self.pages[index]
-        series.append(
-            TiffPageSeries(
-                [page],
-                page.shape,
-                page.dtype,
-                page.axes,
-                name='Thumbnail',
-                kind='svs',
-            )
+            return [
+                TiffPageSeries(
+                    [firstpage],
+                    firstpage.shape,
+                    firstpage.dtype,
+                    firstpage.axes,
+                    name='Baseline',
+                    kind='svs',
+                )
+            ]
+
+        # thumbnail
+        page = self.pages[1]
+        thumnail = TiffPageSeries(
+            [page],
+            page.shape,
+            page.dtype,
+            page.axes,
+            name='Thumbnail',
+            kind='svs',
         )
-        # Resolutions
-        # TODO: resolutions not by two
-        index += 1
+
+        # resolutions and focal planes
+        levels = {firstpage.shape: [firstpage]}
+        index = 2
         while index < len(self.pages):
             page = cast(TiffPage, self.pages[index])
             if not page.is_tiled or page.is_reduced:
                 break
-            series[0].levels.append(
+            if page.shape in levels:
+                levels[page.shape].append(page)
+            else:
+                levels[page.shape] = [page]
+            index += 1
+
+        zsize = len(levels[firstpage.shape])
+        if not all(len(level) == zsize for level in levels.values()):
+            log_warning(f'{self!r} SVS series focal planes do not match')
+            zsize = 1
+        baseline = TiffPageSeries(
+            levels[firstpage.shape],
+            (zsize,) + firstpage.shape,
+            firstpage.dtype,
+            'Z' + firstpage.axes,
+            name='Baseline',
+            kind='svs',
+        )
+        for shape, level in levels.items():
+            if shape == firstpage.shape:
+                continue
+            page = level[0]
+            baseline.levels.append(
                 TiffPageSeries(
-                    [page],
-                    page.shape,
+                    level,
+                    (zsize,) + page.shape,
                     page.dtype,
-                    page.axes,
+                    'Z' + page.axes,
                     name='Resolution',
                     kind='svs',
                 )
             )
-            index += 1
+        series.append(baseline)
+        series.append(thumnail)
+
         # Label, Macro; subfiletype 1, 9
         for _ in range(2):
             if index == len(self.pages):
                 break
             page = self.pages[index]
             if page.subfiletype == 9:  # type: ignore
                 name = 'Macro'
@@ -5658,28 +5707,39 @@
                     f'{self!r} OME series cannot read multi-file pyramids'
                 )
                 break
             for level in range(len(keyframe.subifds)):
                 found_keyframe = False
                 ifds = []
                 for page in aseries.pages:
-                    if page is None or page.subifds is None:
+                    if (
+                        page is None
+                        or page.subifds is None
+                        or page.subifds[level] < 8
+                    ):
                         ifds.append(None)
                         continue
                     page.parent.filehandle.seek(page.subifds[level])
                     if page.keyframe == page:
-                        ifd = keyframe = TiffPage(self, (page.index, level))
+                        ifd = keyframe = TiffPage(
+                            self, (page.index, level + 1)
+                        )
                         found_keyframe = True
                     elif not found_keyframe:
                         raise RuntimeError('no keyframe found')
                     else:
                         ifd = TiffFrame(
-                            self, (page.index, level), keyframe=keyframe
+                            self, (page.index, level + 1), keyframe=keyframe
                         )
                     ifds.append(ifd)
+                if all(ifd_or_none is None for ifd_or_none in ifds):
+                    log_warning(
+                        f'{self!r} OME series level {level + 1} is empty'
+                    )
+                    break
                 # fix shape
                 shape = list(aseries.get_shape(False))
                 axes = aseries.get_axes(False)
                 for i, ax in enumerate(axes):
                     if ax == 'X':
                         shape[i] = keyframe.imagewidth
                     elif ax == 'Y':
@@ -8133,19 +8193,25 @@
 
         try:
             if self.predictor == 1:
                 unpredict = None
             else:
                 unpredict = TIFF.UNPREDICTORS[self.predictor]
         except KeyError as exc:
+            if self.compression not in TIFF.IMAGE_COMPRESSIONS:
 
-            def decode_raise_predictor(*args, exc=str(exc)[1:-1], **kwargs):
-                raise ValueError(f'{exc}')
+                def decode_raise_predictor(
+                    *args, exc=str(exc)[1:-1], **kwargs
+                ):
+                    raise ValueError(f'{exc}')
 
-            return cache(decode_raise_predictor)
+                return cache(decode_raise_predictor)
+
+            log_warning(f'{self!r} ignoring predictor {self.predictor}')
+            unpredict = None
 
         if self.tags.get(339) is not None:
             tag = self.tags[339]  # SampleFormat
             if tag.count != 1 and any(i - tag.value[0] for i in tag.value):
 
                 def decode_raise_sampleformat(*args, **kwargs):
                     raise ValueError(
@@ -10894,15 +10960,15 @@
                     value = value.encode('ascii')
                 except UnicodeEncodeError as exc:
                     raise ValueError(
                         'TIFF strings must be 7-bit ASCII'
                     ) from exc
             elif not isinstance(value, bytes):
                 raise ValueError('TIFF strings must be 7-bit ASCII')
-            if len(value) == 0 or value[-1] != b'\x00':
+            if len(value) == 0 or value[-1:] != b'\x00':
                 value += b'\x00'
             count = len(value)
             value = (value,)
 
         elif isinstance(value, bytes):
             # pre-packed binary data
             dtsize = struct.calcsize(dataformat)
@@ -12022,15 +12088,22 @@
     def __iter__(self) -> Iterator[str]:
         return iter(self._store)
 
     def __len__(self) -> int:
         return len(self._store)
 
     def __contains__(self, key: object, /) -> bool:
-        return key in self._store
+        if key in self._store:
+            return True
+        assert isinstance(key, str)
+        return self._contains(key)
+
+    def _contains(self, key: str, /) -> bool:
+        """Return if key is in store."""
+        raise NotImplementedError
 
     def __delitem__(self, key: object, /) -> None:
         raise PermissionError('ZarrStore is read-only')
 
     def __getitem__(self, key: str, /) -> Any:
         if key in self._store:
             return self._store[key]
@@ -12658,31 +12731,34 @@
             fh.write('\n }\n}')
         elif _close:
             fh.write('\n}')
 
         if not hasattr(jsonfile, 'write'):
             fh.close()
 
+    def _contains(self, key: str, /) -> bool:
+        """Return if key is in store."""
+        try:
+            _, page, _, offset, bytecount = self._parse_key(key)
+        except KeyError:
+            return False
+        return (
+            page is not None
+            and offset is not None
+            and bytecount is not None
+            and offset > 0
+            and bytecount > 0
+        )
+
     def _getitem(self, key: str, /) -> NDArray[Any]:
         """Return chunk from file."""
         keyframe, page, chunkindex, offset, bytecount = self._parse_key(key)
 
-        if self._chunkmode:
-            chunks = keyframe.shape
-        else:
-            chunks = keyframe.chunks
-
         if page is None or offset == 0 or bytecount == 0:
-            assert keyframe.dtype is not None
-            chunk = ZarrStore._empty_chunk(
-                chunks, keyframe.dtype, self._fillvalue
-            )
-            if self._transform is not None:
-                chunk = self._transform(chunk)
-            return chunk
+            raise KeyError(key)
 
         fh = page.parent.filehandle
 
         if self._chunkmode and offset is None:
             self._filecache.open(fh)
             chunk = page.asarray(
                 lock=self._filecache.lock, maxworkers=self._maxworkers
@@ -12705,14 +12781,18 @@
         chunk = keyframe.decode(
             chunk_bytes, chunkindex, **decodeargs  # type: ignore
         )[0]
         assert chunk is not None
         if self._transform is not None:
             chunk = self._transform(chunk)
 
+        if self._chunkmode:
+            chunks = keyframe.shape
+        else:
+            chunks = keyframe.chunks
         if chunk.size != product(chunks):
             raise RuntimeError(f'{chunk.size} != {product(chunks)}')
         return chunk  # .tobytes()
 
     def _setitem(self, key: str, value: bytes, /) -> None:
         """Write chunk to file."""
         if not self._writable:
@@ -12992,25 +13072,29 @@
                 'compressor': None,
                 'fill_value': ZarrStore._value(fillvalue, self._dtype),
                 'order': 'C',
                 'filters': None,
             }
         )
 
+    def _contains(self, key: str, /) -> bool:
+        """Return if key is in store."""
+        try:
+            indices = tuple(int(i) for i in key.split('.'))
+        except Exception:
+            return False
+        return indices in self._lookup
+
     def _getitem(self, key: str, /) -> NDArray[Any]:
         """Return chunk from file."""
         indices = tuple(int(i) for i in key.split('.'))
         filename = self._lookup.get(indices, None)
         if filename is None:
-            chunk = ZarrStore._empty_chunk(
-                self._chunks, self._dtype, self._fillvalue
-            )
-        else:
-            chunk = self._imread(filename, **self._kwargs)
-        return chunk
+            raise KeyError(key)
+        return self._imread(filename, **self._kwargs)
 
     def _setitem(self, key: str, value: bytes, /) -> None:
         raise PermissionError('ZarrStore is read-only')
 
     def write_fsspec(
         self,
         jsonfile: str | os.PathLike[Any] | TextIO,
@@ -17184,16 +17268,20 @@
                 322,  # TileWidth
                 323,  # TileLength
                 324,  # TileOffsets
                 325,  # TileByteCounts
                 330,  # SubIFDs,
                 338,  # ExtraSamples
                 339,  # SampleFormat
+                400,  # GlobalParametersIFD
                 32997,  # ImageDepth
                 32998,  # TileDepth
+                34665,  # ExifTag
+                34853,  # GPSTag
+                40965,  # InteroperabilityTag
             )
         )
 
     @cached_property
     def TAG_TUPLE(self) -> frozenset[int]:
         # tags whose values must be stored as tuples
         return frozenset(
```

### Comparing `tifffile-2023.3.21/tifffile.egg-info/PKG-INFO` & `tifffile-2023.4.12/tifffile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2023.3.21
+Version: 2023.4.12
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -51,15 +51,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.3.21
+:Version: 2023.4.12
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -87,33 +87,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.10, 3.11.2, 64-bit
+- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.3.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.4.12
+
+- Pass 4988 tests.
+- Do not write duplicate ImageDescription tags from extratags (breaking).
+- Support multifocal SVS files (#193).
+- Log warning when filtering out extratags.
+- Fix writing OME-TIFF with image description in extratags.
+- Ignore invalid predictor tag value if prediction is not used.
+- Raise KeyError if ZarrStore is missing requested chunk.
+
 2023.3.21
 
-- Pass 4981 tests.
 - Fix reading MMstack with missing data (#187).
 
 2023.3.15
 
 - Fix corruption using tile generators with prediction/compression (#185).
 - Add parser for Micro-Manager MMStack series (breaking).
 - Return micromanager_metadata IndexMap as numpy array (breaking).
```

### Comparing `tifffile-2023.3.21/tifffile.egg-info/SOURCES.txt` & `tifffile-2023.4.12/tifffile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

