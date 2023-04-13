# Comparing `tmp/gitarootools-0.1.5.tar.gz` & `tmp/gitarootools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitarootools-0.1.5.tar", max compression
+gzip compressed data, was "gitarootools-0.1.6.tar", max compression
```

## Comparing `gitarootools-0.1.5.tar` & `gitarootools-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,37 @@
--rw-r--r--   0        0        0     1148 2020-04-19 09:51:48.000000 gitarootools-0.1.5/LICENSE
--rw-r--r--   0        0        0     1241 2020-04-30 21:03:55.000000 gitarootools-0.1.5/README.md
--rw-r--r--   0        0        0       86 2021-01-23 03:54:23.709509 gitarootools-0.1.5/gitarootools/__init__.py
--rw-r--r--   0        0        0        0 2020-04-27 00:50:59.000000 gitarootools-0.1.5/gitarootools/archive/__init__.py
--rw-r--r--   0        0        0     3091 2020-04-28 21:03:29.000000 gitarootools-0.1.5/gitarootools/archive/xgmcontainer.py
--rw-r--r--   0        0        0     6801 2020-04-27 20:20:16.000000 gitarootools-0.1.5/gitarootools/archive/xgmitem.py
--rw-r--r--   0        0        0     7856 2020-04-27 20:46:50.000000 gitarootools-0.1.5/gitarootools/archive/xgmtoml.py
--rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.5/gitarootools/audio/__init__.py
--rw-r--r--   0        0        0    10920 2020-04-28 21:03:29.000000 gitarootools-0.1.5/gitarootools/audio/imccontainer.py
--rw-r--r--   0        0        0    18977 2020-04-28 19:26:33.000000 gitarootools-0.1.5/gitarootools/audio/imctoml.py
--rw-r--r--   0        0        0    28916 2020-04-19 11:58:09.000000 gitarootools-0.1.5/gitarootools/audio/subsong.py
--rw-r--r--   0        0        0       63 2020-04-19 09:40:53.000000 gitarootools-0.1.5/gitarootools/cmdline/__init__.py
--rw-r--r--   0        0        0     4156 2020-04-28 19:18:13.000000 gitarootools-0.1.5/gitarootools/cmdline/imcpack.py
--rw-r--r--   0        0        0     4286 2020-04-28 19:26:33.000000 gitarootools-0.1.5/gitarootools/cmdline/imcunpack.py
--rw-r--r--   0        0        0     3362 2022-08-08 05:14:21.786361 gitarootools-0.1.5/gitarootools/cmdline/imx2png.py
--rw-r--r--   0        0        0     4921 2021-01-18 04:02:54.689117 gitarootools-0.1.5/gitarootools/cmdline/png2imx.py
--rw-r--r--   0        0        0     3998 2020-04-28 19:28:46.000000 gitarootools-0.1.5/gitarootools/cmdline/subsong2common.py
--rw-r--r--   0        0        0      408 2020-04-19 09:50:28.000000 gitarootools-0.1.5/gitarootools/cmdline/subsong2subimc.py
--rw-r--r--   0        0        0      398 2020-04-19 09:50:28.000000 gitarootools-0.1.5/gitarootools/cmdline/subsong2wav.py
--rw-r--r--   0        0        0     1539 2020-04-19 09:50:28.000000 gitarootools-0.1.5/gitarootools/cmdline/subsongconv.py
--rw-r--r--   0        0        0     4149 2020-04-28 19:18:13.000000 gitarootools-0.1.5/gitarootools/cmdline/xgmpack.py
--rw-r--r--   0        0        0     4074 2020-04-27 20:20:05.000000 gitarootools-0.1.5/gitarootools/cmdline/xgmunpack.py
--rw-r--r--   0        0        0        0 2020-04-29 19:36:52.000000 gitarootools-0.1.5/gitarootools/image/__init__.py
--rw-r--r--   0        0        0    17724 2021-01-25 04:05:13.859360 gitarootools-0.1.5/gitarootools/image/imximage.py
--rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.5/gitarootools/miscutils/__init__.py
--rw-r--r--   0        0        0     5011 2021-01-25 04:11:23.223912 gitarootools-0.1.5/gitarootools/miscutils/cmdutils.py
--rw-r--r--   0        0        0     6350 2022-08-08 06:12:19.143521 gitarootools-0.1.5/gitarootools/miscutils/datautils.py
--rw-r--r--   0        0        0     4224 2020-05-02 17:22:15.000000 gitarootools-0.1.5/gitarootools/miscutils/extutils.py
--rw-r--r--   0        0        0      981 2022-08-08 06:13:59.841442 gitarootools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2869 2022-08-08 06:38:23.012441 gitarootools-0.1.5/setup.py
--rw-r--r--   0        0        0     1997 2022-08-08 06:38:23.012686 gitarootools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1148 2020-04-19 09:51:48.000000 gitarootools-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1241 2020-04-30 21:03:55.000000 gitarootools-0.1.6/README.md
+-rw-r--r--   0        0        0       86 2022-08-08 06:59:32.010948 gitarootools-0.1.6/gitarootools/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-27 00:50:59.000000 gitarootools-0.1.6/gitarootools/archive/__init__.py
+-rw-r--r--   0        0        0     6238 2023-04-12 05:26:23.575401 gitarootools-0.1.6/gitarootools/archive/pakcontainer.py
+-rw-r--r--   0        0        0     4463 2023-04-12 04:10:21.677616 gitarootools-0.1.6/gitarootools/archive/paktoml.py
+-rw-r--r--   0        0        0     3142 2023-04-12 05:22:28.649251 gitarootools-0.1.6/gitarootools/archive/xgmcontainer.py
+-rw-r--r--   0        0        0     6801 2020-04-27 20:20:16.000000 gitarootools-0.1.6/gitarootools/archive/xgmitem.py
+-rw-r--r--   0        0        0     7894 2023-04-10 04:43:31.018329 gitarootools-0.1.6/gitarootools/archive/xgmtoml.py
+-rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.6/gitarootools/audio/__init__.py
+-rw-r--r--   0        0        0    10947 2023-04-12 05:23:18.615425 gitarootools-0.1.6/gitarootools/audio/imccontainer.py
+-rw-r--r--   0        0        0    18977 2020-04-28 19:26:33.000000 gitarootools-0.1.6/gitarootools/audio/imctoml.py
+-rw-r--r--   0        0        0    28944 2023-04-12 05:30:24.349667 gitarootools-0.1.6/gitarootools/audio/subsong.py
+-rw-r--r--   0        0        0       63 2020-04-19 09:40:53.000000 gitarootools-0.1.6/gitarootools/cmdline/__init__.py
+-rw-r--r--   0        0        0     2986 2023-04-13 05:13:35.976581 gitarootools-0.1.6/gitarootools/cmdline/gmo2animnames.py
+-rw-r--r--   0        0        0     4156 2020-04-28 19:18:13.000000 gitarootools-0.1.6/gitarootools/cmdline/imcpack.py
+-rw-r--r--   0        0        0     4286 2020-04-28 19:26:33.000000 gitarootools-0.1.6/gitarootools/cmdline/imcunpack.py
+-rw-r--r--   0        0        0     3362 2022-08-08 05:14:21.786361 gitarootools-0.1.6/gitarootools/cmdline/imx2png.py
+-rw-r--r--   0        0        0     4132 2023-04-12 03:41:12.325154 gitarootools-0.1.6/gitarootools/cmdline/pakpack.py
+-rw-r--r--   0        0        0     4846 2023-04-12 03:37:25.211594 gitarootools-0.1.6/gitarootools/cmdline/pakunpack.py
+-rw-r--r--   0        0        0     4921 2021-01-18 04:02:54.689117 gitarootools-0.1.6/gitarootools/cmdline/png2imx.py
+-rw-r--r--   0        0        0     3998 2020-04-28 19:28:46.000000 gitarootools-0.1.6/gitarootools/cmdline/subsong2common.py
+-rw-r--r--   0        0        0      408 2020-04-19 09:50:28.000000 gitarootools-0.1.6/gitarootools/cmdline/subsong2subimc.py
+-rw-r--r--   0        0        0      398 2020-04-19 09:50:28.000000 gitarootools-0.1.6/gitarootools/cmdline/subsong2wav.py
+-rw-r--r--   0        0        0     1539 2020-04-19 09:50:28.000000 gitarootools-0.1.6/gitarootools/cmdline/subsongconv.py
+-rw-r--r--   0        0        0     4149 2020-04-28 19:18:13.000000 gitarootools-0.1.6/gitarootools/cmdline/xgmpack.py
+-rw-r--r--   0        0        0     4074 2023-04-12 04:16:46.510728 gitarootools-0.1.6/gitarootools/cmdline/xgmunpack.py
+-rw-r--r--   0        0        0        0 2020-04-29 19:36:52.000000 gitarootools-0.1.6/gitarootools/image/__init__.py
+-rw-r--r--   0        0        0    17764 2023-04-12 04:56:23.341827 gitarootools-0.1.6/gitarootools/image/imximage.py
+-rw-r--r--   0        0        0       63 2020-04-19 09:47:08.000000 gitarootools-0.1.6/gitarootools/miscutils/__init__.py
+-rw-r--r--   0        0        0     5011 2021-01-25 04:11:23.223912 gitarootools-0.1.6/gitarootools/miscutils/cmdutils.py
+-rw-r--r--   0        0        0     6391 2023-04-12 04:45:21.484101 gitarootools-0.1.6/gitarootools/miscutils/datautils.py
+-rw-r--r--   0        0        0     4413 2023-04-12 00:50:22.767259 gitarootools-0.1.6/gitarootools/miscutils/extutils.py
+-rw-r--r--   0        0        0       63 2023-04-13 02:58:32.253643 gitarootools-0.1.6/gitarootools/other/__init__.py
+-rw-r--r--   0        0        0     1826 2023-04-13 05:13:20.716138 gitarootools-0.1.6/gitarootools/other/gmomodel.py
+-rw-r--r--   0        0        0     1143 2023-04-13 05:16:32.873794 gitarootools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 gitarootools-0.1.6/PKG-INFO
```

### Comparing `gitarootools-0.1.5/LICENSE` & `gitarootools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/README.md` & `gitarootools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/archive/xgmcontainer.py` & `gitarootools-0.1.6/gitarootools/archive/xgmcontainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,48 +35,50 @@
         :param imageitems: sequence of xgmitem.XgmImageItem
         :param modelitems: sequence of xgmitem.XgmModelItem
         """
         self.imageitems = imageitems
         self.modelitems = modelitems
 
 
-def read_xgm(file: Union[AnyStr, BinaryIO]) -> XgmContainer:
+def read_xgm(file_or_path: Union[AnyStr, BinaryIO]) -> XgmContainer:
     """read from file and return an XgmContainer
 
-    :param file: A file path. Or it can be an already-opened file, in which case:
+    :param file_or_path: A file path. Or an already-opened file, in which case:
         * data will be read starting from the current file position
         * after returning, file position is at the end of the last item's data
         * the caller is responsible for closing the file afterwards
     :return: XgmContainer instance
     """
-    with open_maybe(file, "rb") as file:
+    with open_maybe(file_or_path, "rb") as file:
         num_imageitems, num_modelitems = readstruct(file, "<II")
         imageitems = [read_imageitem(file) for _ in range(num_imageitems)]
         modelitems = [read_modelitem(file) for _ in range(num_modelitems)]
     return XgmContainer(imageitems, modelitems)
 
 
 def write_xgm(
-    xgm: XgmContainer, file: Union[AnyStr, BinaryIO], progressfunc: Callable = None
+    xgm: XgmContainer,
+    file_or_path: Union[AnyStr, BinaryIO],
+    progressfunc: Callable = None,
 ) -> None:
     """write an XgmContainer to file
 
     :param xgm: XgmContainer object
-    :param file: A file path. Or it can be an already-opened file, in which case:
+    :param file_or_path: A file path. Or an already-opened file, in which case:
         * data will be written starting from the current file position
         * after returning, file position is at the end of the last item's data
         * the caller is responsible for closing the file afterwards
     :param progressfunc: function to run whenever an item of the XgmContainer is about
       to be processed. It must accept three arguments: an int item index, an int total
       number of items, and an xgmitem.XgmImageItem/XgmModelItem instance
     """
-    with open_maybe(file, "wb") as file:
+    with open_maybe(file_or_path, "wb") as file:
         num_imageitems, num_modelitems = len(xgm.imageitems), len(xgm.modelitems)
         file.write(struct.pack("<II", num_imageitems, num_modelitems))
         for i, item in enumerate(xgm.imageitems):
             if progressfunc is not None:
                 progressfunc(i, num_imageitems, item)
             write_imageitem(item, file)
-        for item in xgm.modelitems:
+        for i, item in enumerate(xgm.modelitems):
             if progressfunc is not None:
                 progressfunc(i, num_modelitems, item)
             write_modelitem(item, file)
```

### Comparing `gitarootools-0.1.5/gitarootools/archive/xgmitem.py` & `gitarootools-0.1.6/gitarootools/archive/xgmitem.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/archive/xgmtoml.py` & `gitarootools-0.1.6/gitarootools/archive/xgmtoml.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,31 @@
 
 class XgmTomlError(Exception):
     """base class for XGM TOML errors"""
 
     pass
 
 
-# TODO expand help text
 _toml_header = """\
-# Welcome to the gm-xgmpack repacking file, for all your XGM repacking needs!
+# This is a list of all images and models extracted from the XGM container.
+# Use gm-xgmpack to repack everything back into an XGM file.
 # Try opening this file in a programmer's text editor for handy color highlighting
 # (your editor may need a plugin for TOML support first).
 
-["Item Help/Guide"]
-    # An ImageItem contains just an .IMX image file.
-    # A ModelItem contains both .XG model and .animsep (animation separation) files.
+["Help/Guide"]
+    # An [[ImageItem]] is an .IMX image file.
+    # A [[ModelItem]] is an .XG model and its .animsep (animation separation) file.
 
     name16 = "MODEL.XG"
-    # name16: Unless you use an advanced option below, this is the IMX or XG/animsep
-    # files to use. Also used internally by the game, so it must be 16 ascii characters
-    # or fewer.
+    # name16: The filename of the IMX or XG/animsep file to use. The game uses this name
+    # internally, so it must be 16 ascii characters or fewer.
 
-    # Advanced options: fine control over the file(s) to use.
+    # For 99% of cases, that's all you need to use.
+
+    # Advanced options: finer control over which files to use.
     # By default, name16="MODEL.XG" will use MODEL.XG and MODEL.animsep.
     # Use the following if the real filename is different or is in another directory.
 
     file-path = "models/filename.xg"
     # file-path: path to the actual XG or IMX file, if it's different from <name16>.
     # Also, animsep path will be based on this instead unless you use the option below.
```

### Comparing `gitarootools-0.1.5/gitarootools/audio/imccontainer.py` & `gitarootools-0.1.6/gitarootools/audio/imccontainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,24 +167,24 @@
         self.csubsongs = list(containersubsongs)
 
     @property
     def num_subsongs(self):
         return len(self.csubsongs)
 
 
-def read_imc(file):
-    """ read from a IMC audio container file and return an ImcContainer
+def read_imc(file_or_path):
+    """read from a IMC audio container file and return an ImcContainer
 
-    file: A file path. Or it can be an already-opened file, in which case:
+    file_or_path: A file path. Or an already-opened file, in which case:
     - it will read starting from the current file position, with no guarantee of file
       position after returning
     - the caller is responsible for closing the file afterwards
     raises: EOFError if end of file is reached unexpectedly
     """
-    with open_maybe(file, "rb") as file:
+    with open_maybe(file_or_path, "rb") as file:
         start_offset = file.tell()
 
         # read number of subsongs
         num_subsongs = readstruct(file, "<I")
 
         # read raw ssinfo
         fmt, items_per_ssinfo_entry = ("<" + "16s4I" * num_subsongs), 5
@@ -211,27 +211,27 @@
                 subsong_, name, loadmode_raw, rawname, unk1, unk2
             )
             csubsongs.append(csubsong)
 
         return ImcContainer(csubsongs)
 
 
-def write_imc(imccontainer, file, progressfunc=None):
+def write_imc(imccontainer, file_or_path, progressfunc=None):
     """write an ImcContainer to an IMC audio container file
 
     imccontainer: an ImcContainer object
-    file: A file path. Or it can be an already-opened file, in which case:
+    file_or_path: A file path. Or an already-opened file, in which case:
     - it will write starting from the current file position, with no guarantee of file
       position after returning
     - the caller is responsible for closing the file afterwards
     progressfunc: function to run whenever a subsong of the ImcContainer is about to
       be processed. It must accept three arguments: an int subsong index, an int total
       number of subsongs, and an imccontainer.ContainerSubsong instance
     """
-    with open_maybe(file, "wb") as file:
+    with open_maybe(file_or_path, "wb") as file:
         start_offset = file.tell()  # in case we're reading from inside an ISO file, etc
 
         # write num_subsongs
         num_subsongs = imccontainer.num_subsongs
         file.write(struct.pack("<I", num_subsongs))
         if not num_subsongs:
             return
```

### Comparing `gitarootools-0.1.5/gitarootools/audio/imctoml.py` & `gitarootools-0.1.6/gitarootools/audio/imctoml.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/audio/subsong.py` & `gitarootools-0.1.6/gitarootools/audio/subsong.py`

 * *Files 2% similar despite different names*

```diff
@@ -520,30 +520,30 @@
     sstype = subsongtype(filepath)
     if sstype == "subimc":
         return write_subimc(subsong, filepath)
     elif sstype == "wav":
         return write_subwav16(subsong, filepath)
 
 
-def read_subimc(file, knownsize=None):
+def read_subimc(file_or_path, knownsize=None):
     """read from a IMC subsong file and return a Subsong
 
-    file: A file path. Or it can be an already-opened file, in which case:
+    file_or_path: A file path. Or an already-opened file, in which case:
     - it will read starting from the current file position
     - after returning, file position will be right after the subsong file data
     - the caller is responsible for closing the file afterwards
     knownsize: Optional size of the IMC subsong file known in advance. It's only used
       for a quick sanity check (to anticipate reading past end of the subsong). Without
       this, it assumes this subsong ends when the file ends, so it's recommended to pass
       this if reading this subsong from inside a larger container file.
     raises:
     - SubsongError if IMC subsong header is invalid
     - EndOfSubsongError if end of subsong is reached unexpectedly
     """
-    with open_maybe(file, "rb") as file:
+    with open_maybe(file_or_path, "rb") as file:
         # Read imc subsong header
         header = file.read(16)
         if len(header) != 16:
             raise EndOfSubsongError(
                 "Expected 16 bytes for IMC subsong header, only got"
                 f"{len(header)} bytes"
             )
@@ -644,24 +644,24 @@
     channels = list()
     for ch_samples in channels_samples:
         ch = Pcm16Channel(ch_samples)
         channels.append(ch)
     return Subsong(channels, sample_rate)
 
 
-def write_subimc(subsong, file):
+def write_subimc(subsong, file_or_path):
     """write a Subsong to IMC subsong file
 
     subsong: a Subsong instance
-    file: A file path. Or it can be an already-opened file, in which case:
+    file_or_path: A file path. Or an already-opened file, in which case:
     - it will write starting from the current file position. After returning, the file
       position will be at the end of the IMC subsong data it just wrote.
     - the caller is responsible for closing the file afterwards
     """
-    with open_maybe(file, "wb") as file:
+    with open_maybe(file_or_path, "wb") as file:
         file.write(subsong.get_imcdata())
 
 
 def write_subwav16(subsong, file):
     """write a Subsong to WAV file (16-bit signed linear PCM)
 
     subsong: a Subsong object
```

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/imcpack.py` & `gitarootools-0.1.6/gitarootools/cmdline/imcpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/imcunpack.py` & `gitarootools-0.1.6/gitarootools/cmdline/imcunpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/imx2png.py` & `gitarootools-0.1.6/gitarootools/cmdline/imx2png.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/png2imx.py` & `gitarootools-0.1.6/gitarootools/cmdline/png2imx.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/subsong2common.py` & `gitarootools-0.1.6/gitarootools/cmdline/subsong2common.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/subsongconv.py` & `gitarootools-0.1.6/gitarootools/cmdline/subsongconv.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/xgmpack.py` & `gitarootools-0.1.6/gitarootools/cmdline/xgmpack.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/cmdline/xgmunpack.py` & `gitarootools-0.1.6/gitarootools/cmdline/xgmunpack.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 customize the output dir and filenames:
 
   Example 4: Give output dir and file a suffix (e.g. _US results in \
 file_US_XGM{s}file_US{XGMTOML_EXT}
       {parser.prog} -s _US file{XGM_EXT} file2{XGM_EXT}
 
   Example 5: Create unpacked dirs in different outer directory (e.g. unpack to \
-outerdir{s}file_IMC{s})
+outerdir{s}file_XGM{s})
       {parser.prog} -d outerdir file{XGM_EXT}"""
     )
     return parser
 
 
 def main(args=tuple(sys.argv[1:])):
     """args: sequence of command line argument strings"""
```

### Comparing `gitarootools-0.1.5/gitarootools/image/imximage.py` & `gitarootools-0.1.6/gitarootools/image/imximage.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,26 +193,26 @@
                 ]
             elif self.alpha255:
                 return self.pixels
         else:  # RGB or indexed
             return self.pixels
 
 
-def read_imx(fp: BinaryFp) -> ImxImage:
+def read_imx(file_or_path: BinaryFp) -> ImxImage:
     """read from an IMX image file and return an ImxImage
 
-    :param fp: A file path. Or it can be an already-opened file, in which case:
+    :param file_or_path: A file path. Or an already-opened file, in which case:
         - it will read starting from the current file position
         - after returning, file position will be right after the IMX file data
         - the caller is responsible for closing the file afterwards
     :raises ImxImageError if IMX header is invalid
     :raises EndOfImxImageError if end of IMX data is reached unexpectedly
     :return: ImxImage instance
     """
-    with open_maybe(fp, "rb") as file:
+    with open_maybe(file_or_path, "rb") as file:
         try:
             magic = readdata(file, 4)
             if magic != b"IMX\0":
                 raise ImxImageError(f"Not an IMX file, unknown magic {magic!r}")
             width, height, pixfmtdata = readstruct(file, "<16x2I8s")
             pixfmt = _pixfmtdata_pixfmt.get(pixfmtdata)
             if pixfmt is None:
@@ -251,24 +251,24 @@
 
         except EOFError as e:
             raise EndOfImxImageError(str(e))
 
     return ImxImage(width, height, pixels, palette, pixfmt=pixfmt, alpha128=True)
 
 
-def write_imx(imximage: ImxImage, fp: BinaryFp) -> None:
+def write_imx(imximage: ImxImage, file_or_path: BinaryFp) -> None:
     """write imximage to file
 
     :param imximage: an ImxImage instance
-    :param fp: A file path. Or it can be an already-opened file, in which case:
+    :param file_or_path: A file path. Or an already-opened file, in which case:
         - it will write starting from the current file position
         - after returning, file position will be right after the written IMX data
         - the caller is responsible for closing the file afterwards
     """
-    with open_maybe(fp, "wb") as file:
+    with open_maybe(file_or_path, "wb") as file:
         # header
         file.write(b"IMX\0")
         pixfmtdata = _pixfmt_pixfmtdata[imximage.pixfmt]
         writestruct(file, "<16x2I8s", *imximage.size, pixfmtdata)
 
         # palette
         if imximage.pixfmt in ("i4", "i8"):
```

### Comparing `gitarootools-0.1.5/gitarootools/miscutils/cmdutils.py` & `gitarootools-0.1.6/gitarootools/miscutils/cmdutils.py`

 * *Files identical despite different names*

### Comparing `gitarootools-0.1.5/gitarootools/miscutils/datautils.py` & `gitarootools-0.1.6/gitarootools/miscutils/datautils.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,37 +119,37 @@
         )
     return data
 
 
 def writestruct(file: BinaryIO, fmt: AnyStr, *values: Any) -> None:
     """write values to file according to struct fmt
 
-    :param file: file object with read(bytes) method
+    :param file: file object with write(bytes) method
     :param fmt: string struct format (see documentation for builtin struct module)
     :param values: values to write to file, must match fmt
     :return:
     """
     file.write(struct.pack(fmt, *values))
 
 
-def open_maybe(file, mode="r", **kwargs):
+def open_maybe(file_or_path, mode="r", **kwargs):
     """a drop-in replacement for open() that can also take an already-opened file
 
     Like open(), open_maybe() can be used in a with statement.
     Differences from builtin open():
     - First argument can be an already-opened file object instead of a path.
     - If given an already-opened file, it will not be closed when the context manager/
       with statement ends.
     """
     # check if it's already a file
-    if hasattr(file, "read") or hasattr(file, "write"):
-        return nullcontext(file)
+    if hasattr(file_or_path, "read") or hasattr(file_or_path, "write"):
+        return nullcontext(file_or_path)
     else:
         # it's not already a file, so open one
-        return open(file, mode, **kwargs)
+        return open(file_or_path, mode, **kwargs)
 
 
 def clamp(val, min_, max_):
     """clamp val to between min_ and max_ inclusive"""
     if val < min_:
         return min_
     if val > max_:
```

### Comparing `gitarootools-0.1.5/gitarootools/miscutils/extutils.py` & `gitarootools-0.1.6/gitarootools/miscutils/extutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
 # === Archive: XGM container extensions ===
 XGM_EXT = f"{_d}XGM"
 XGMTOML_EXT = f"{_d}XGM{_d}toml"
 # *.XGM.TOML case insensitive:
 XGMTOML_EXT_GLOB = f"*{_d}[xX][gG][mM]{_d}[tT][oO][mM][lL]"
 ANIMSEP_EXT = f"{_d}animsep"
+# === Archive: PAK container extensions ===
+PAK_EXT = f"{_d}PAK"
+PAKTOML_EXT = f"{_d}PAK{_d}toml"
+# *.XGM.TOML case insensitive:
+PAKTOML_EXT_GLOB = f"*{_d}[pP][aA][kK]{_d}[tT][oO][mM][lL]"
 
 # === Image: IMX image extension ===
 IMX_EXT = f"{_d}IMX"
 
 # == Image: PNG image extension and pixel format pseudo-extensions ===
 PNG_EXT = f"{_d}png"
 PIXFMT_EXAMPLE = "rgb24"
```

### Comparing `gitarootools-0.1.5/pyproject.toml` & `gitarootools-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "gitarootools"
-version = "0.1.5"
+version = "0.1.6"
 description = "command line tools to work with Gitaroo Man game data"
 license = "MIT"
 authors = ["boringhexi <boringhexi@pm.me>"]
 readme = "README.md"
 repository = "https://github.com/boringhexi/gitarootools"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-tomlkit = "^0.11.2 "
-pillow = "^9.2.0"
+tomlkit = "^0.11.7 "
+pillow = "^9.5.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.3.0"
 
 [tool.poetry.scripts]
+gm-gmo2animnames = "gitarootools.cmdline.gmo2animnames:main"
 gm-imcpack = "gitarootools.cmdline.imcpack:main"
 gm-imcunpack = "gitarootools.cmdline.imcunpack:main"
+gm-pakpack = "gitarootools.cmdline.pakpack:main"
+gm-pakunpack = "gitarootools.cmdline.pakunpack:main"
 gm-subsongconv = "gitarootools.cmdline.subsongconv:main"
 gm-subsong2subimc = "gitarootools.cmdline.subsong2subimc:main"
 gm-subsong2wav = "gitarootools.cmdline.subsong2wav:main"
 gm-xgmpack = "gitarootools.cmdline.xgmpack:main"
 gm-xgmunpack = "gitarootools.cmdline.xgmunpack:main"
 gm-imx2png = "gitarootools.cmdline.imx2png:main"
 gm-png2imx = "gitarootools.cmdline.png2imx:main"
 
 [build-system]
-requires = ["poetry>=1.1.14"]
+requires = ["poetry>=1.4.2"]
 build-backend = "poetry.masonry.api"
```

### Comparing `gitarootools-0.1.5/PKG-INFO` & `gitarootools-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gitarootools
-Version: 0.1.5
+Version: 0.1.6
 Summary: command line tools to work with Gitaroo Man game data
 Home-page: https://github.com/boringhexi/gitarootools
 License: MIT
 Author: boringhexi
 Author-email: boringhexi@pm.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pillow (>=9.2.0,<10.0.0)
-Requires-Dist: tomlkit (>=0.11.2,<0.12.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: tomlkit (>=0.11.7,<0.12.0)
 Project-URL: Repository, https://github.com/boringhexi/gitarootools
 Description-Content-Type: text/markdown
 
 # gitarootools — command line tools to work with Gitaroo Man game data
  
 *Gitaroo Man* is a rhythm action video game for PlayStation 2. This set of tools allows
 you to work with data from the game, converting game files to more viewable formats. In
```

