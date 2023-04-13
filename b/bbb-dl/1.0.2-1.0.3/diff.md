# Comparing `tmp/bbb-dl-1.0.2.tar.gz` & `tmp/bbb-dl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbb-dl-1.0.2.tar", last modified: Fri Mar 17 15:48:32 2023, max compression
+gzip compressed data, was "bbb-dl-1.0.3.tar", last modified: Thu Apr 13 20:16:43 2023, max compression
```

## Comparing `bbb-dl-1.0.2.tar` & `bbb-dl-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:48:32.285592 bbb-dl-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-03-17 15:48:32.281592 bbb-dl-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:48:32.281592 bbb-dl-1.0.2/bbb_dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/bbb_dl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/bbb_dl/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/bbb_dl/ffmpeg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57889 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/bbb_dl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/bbb_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/bbb_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:48:32.281592 bbb-dl-1.0.2/bbb_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-03-17 15:48:32.000000 bbb-dl-1.0.2/bbb_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-17 15:48:32.000000 bbb-dl-1.0.2/bbb_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 15:48:32.000000 bbb-dl-1.0.2/bbb_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-17 15:48:32.000000 bbb-dl-1.0.2/bbb_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 15:48:32.000000 bbb-dl-1.0.2/bbb_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-17 15:48:32.000000 bbb-dl-1.0.2/bbb_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 15:48:32.000000 bbb-dl-1.0.2/bbb_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 15:48:32.285592 bbb-dl-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-17 15:48:22.000000 bbb-dl-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:43.523043 bbb-dl-1.0.3/bbb_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/ffmpeg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58606 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22273 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/bbb_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/setup.py
```

### Comparing `bbb-dl-1.0.2/LICENSE` & `bbb-dl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.2/PKG-INFO` & `bbb-dl-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.2
+Version: 1.0.3
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -140,17 +140,18 @@
 - For AMD CPUs / GPUs, you can try the encoder `h264_amf` (Use the option `--encoder h264_amf`).
 
 > You have to test yourself if it is faster to use your hardware encoder or not. In some cases, hardware encoders are slower than using the CPU directly. 
 
 
 ### Other downloader
 
-[bbb-video-download](https://github.com/tilmanmoser/bbb-video-download) 
+[bbb-video-download](https://github.com/tilmanmoser/bbb-video-download)
 - It uses a clever approach written in Node.js that can be easily integrated into a bbb server
 - You can use the `--backup` option to feed `bbb-video-download`.
+- A multi-threaded port in go-lang can be found here: [bbb-video-converter](https://github.com/cli-ish/bbb-video-converter)
 
 [bbb-download](https://github.com/fossasia/bbb-download)
 - Takes advantage of the fact that you can use the bbb-player to play the session data offline.
 - Instead of creating a video file, this downloader downloads only the necessary files from the server, so you can use the bbb-player to play the session offline. The player is provided to you via shortcut.
 
 If someone wants to link another downloader here, which offers e.g. functions that bbb-dl does not offer, feel free to open an issue.
```

### Comparing `bbb-dl-1.0.2/README.md` & `bbb-dl-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,18 @@
 - For AMD CPUs / GPUs, you can try the encoder `h264_amf` (Use the option `--encoder h264_amf`).
 
 > You have to test yourself if it is faster to use your hardware encoder or not. In some cases, hardware encoders are slower than using the CPU directly. 
 
 
 ### Other downloader
 
-[bbb-video-download](https://github.com/tilmanmoser/bbb-video-download) 
+[bbb-video-download](https://github.com/tilmanmoser/bbb-video-download)
 - It uses a clever approach written in Node.js that can be easily integrated into a bbb server
 - You can use the `--backup` option to feed `bbb-video-download`.
+- A multi-threaded port in go-lang can be found here: [bbb-video-converter](https://github.com/cli-ish/bbb-video-converter)
 
 [bbb-download](https://github.com/fossasia/bbb-download)
 - Takes advantage of the fact that you can use the bbb-player to play the session data offline.
 - Instead of creating a video file, this downloader downloads only the necessary files from the server, so you can use the bbb-player to play the session offline. The player is provided to you via shortcut.
 
 If someone wants to link another downloader here, which offers e.g. functions that bbb-dl does not offer, feel free to open an issue.
```

### Comparing `bbb-dl-1.0.2/bbb_dl/batch.py` & `bbb-dl-1.0.3/bbb_dl/batch.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.2/bbb_dl/ffmpeg.py` & `bbb-dl-1.0.3/bbb_dl/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.2/bbb_dl/main.py` & `bbb-dl-1.0.3/bbb_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,48 +4,47 @@
 import asyncio
 import hashlib
 import math
 import os
 import re
 import shutil
 import traceback
-
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from functools import partial
 from http.server import ThreadingHTTPServer
+from io import StringIO
 from itertools import cycle
 from pathlib import Path
 from threading import Thread
-from typing import List, Dict, Any, Tuple
+from typing import Any, Dict, List, Tuple
 from xml.etree import ElementTree as ET
-from xml.etree.ElementTree import ParseError, Element
+from xml.etree.ElementTree import Element, ParseError
 
-import aiohttp
 import aiofiles
-
+import aiohttp
 from aiohttp.client_exceptions import ClientError, ClientResponseError
+from colorama import just_fix_windows_console
 from playwright.async_api import async_playwright
 from playwright.async_api._generated import Page
-from colorama import just_fix_windows_console
 
 from bbb_dl.ffmpeg import FFMPEG
+from bbb_dl.utils import KNOWN_VIDEO_AUDIO_EXTENSIONS, BBBDLCookieJar, Log
+from bbb_dl.utils import PathTools as PT
 from bbb_dl.utils import (
+    QuietRequestHandler,
+    Timer,
     _s,
     _x,
     append_get_idx,
+    convert_to_aiohttp_cookie_jar,
     format_bytes,
     formatSeconds,
     get_free_port,
-    KNOWN_VIDEO_AUDIO_EXTENSIONS,
-    Log,
-    PathTools as PT,
-    QuietRequestHandler,
-    Timer,
     xpath_text,
 )
 from bbb_dl.version import __version__
 
 
 class ActionType(Enum):
     show_image = 1
@@ -158,14 +157,20 @@
         self.filename = filename
         self.output_dir = self.get_output_dir(output_dir)
         self.slideshow_width = int(force_width) if force_width is not None else None
         self.slideshow_height = int(force_height) if force_height is not None else None
 
         self.ffmpeg = FFMPEG(verbose, ffmpeg_location, encoder, audiocodec, preset, crf)
 
+        self.cookies_path = PT.make_path(self.working_dir, "cookies.txt")
+        self.cookies_text = None
+        if os.path.isfile(self.cookies_path):
+            with open(self.cookies_path, 'r', encoding='utf-8') as cookie_file:
+                self.cookies_text = cookie_file.read()
+
         # Check DL-URL
         m_obj = re.match(self.VALID_URL_RE, self.dl_url)
 
         if m_obj is None:
             Log.error(
                 f'Error: Your URL {self.dl_url} does not match the bbb session pattern.'
                 + ' If you think this URL should work, please open an issue on https://github.com/C0D3D3V/bbb-dl/issues'
@@ -174,14 +179,21 @@
 
         self.video_id = m_obj.group('id')
         self.video_website = m_obj.group('website')
         self.presentation_base_url = self.video_website + '/presentation/' + self.video_id
         self.tmp_dir = self.get_tmp_dir(self.video_id)
         self.frames_dir = self.get_frames_dir()
 
+    def get_cookie_jar(self) -> aiohttp.CookieJar:
+        if self.cookies_text is not None:
+            cookie_jar = BBBDLCookieJar(StringIO(self.cookies_text))
+            cookie_jar.load(ignore_discard=True, ignore_expires=True)
+            return convert_to_aiohttp_cookie_jar(cookie_jar)
+        return None
+
     def run(self):
         if not self.backup:
             Log.yellow(f'Output directory for the final video is: {self.output_dir}')
             Log.yellow(f'Directory for the temporary files is: {self.tmp_dir}')
         else:
             Log.yellow(f'Output directory for backup is: {self.tmp_dir}')
 
@@ -851,27 +863,30 @@
                 self.filename += '.mp3'
             return str(Path(self.output_dir) / PT.to_valid_name(self.filename))
         else:
             return str(
                 Path(self.output_dir) / PT.to_valid_name(metadata.date_formatted + '_' + metadata.title + '.mp3')
             )
 
+    @classmethod
     def get_output_dir(
-        self,
+        cls,
         output_dir: str,
     ):
-        return self.check_directory(output_dir, os.getcwd(), 'output', '--output-dir')
+        return cls.check_directory(output_dir, os.getcwd(), 'output', '--output-dir')
 
+    @classmethod
     def get_working_dir(
-        self,
+        cls,
         working_dir: str,
     ):
-        return self.check_directory(working_dir, PT.get_project_data_directory(), 'temporary', '--working-dir')
+        return cls.check_directory(working_dir, PT.get_project_data_directory(), 'temporary', '--working-dir')
 
-    def check_directory(self, path: str, default_path: str, file_type: str, option_name: str):
+    @staticmethod
+    def check_directory(path: str, default_path: str, file_type: str, option_name: str):
         if path is None:
             path = default_path
         else:
             path = PT.sanitize_path(path)
 
         path = PT.get_abs_path(path)
         try:
@@ -980,15 +995,15 @@
             total = 0
             tries_num = 0
             file_obj = None
             can_continue_on_fail = False
             headers = self.headers.copy()
             finished_successfully = False
             async with semaphore, aiohttp.ClientSession(
-                conn_timeout=conn_timeout, read_timeout=read_timeout
+                cookie_jar=self.get_cookie_jar(), conn_timeout=conn_timeout, read_timeout=read_timeout
             ) as session:
                 while tries_num < self.max_dl_retries:
                     try:
                         if tries_num > 0 and can_continue_on_fail:
                             headers["Range"] = f"bytes={received}-"
                         elif not can_continue_on_fail and 'Range' in headers:
                             del headers['Range']
@@ -1240,17 +1255,14 @@
         with Timer() as t:
             asyncio.run(self.ffmpeg.extract_audio(webcams_path, result_path))
         Log.info(f'Extracting audio finished and took: {formatSeconds(t.duration)}')
         return result_path
 
 
 def get_parser():
-    """
-    Creates a new argument parser.
-    """
     parser = argparse.ArgumentParser(
         description=('Big Blue Button Downloader that downloads a BBB lesson as MP4 video')
     )
 
     parser.add_argument('URL', type=str, help='URL of a BBB lesson')
 
     parser.add_argument(
@@ -1427,16 +1439,15 @@
 
     return parser
 
 
 # --- called at the program invocation: -------------------------------------
 def main(args=None):
     just_fix_windows_console()
-    parser = get_parser()
-    args = parser.parse_args(args)
+    args = get_parser().parse_args(args)
 
     with Timer() as final_t:
         bbb_dl = BBBDL(
             args.URL,
             args.filename,
             args.output_dir,
             args.verbose,
```

### Comparing `bbb-dl-1.0.2/bbb_dl.egg-info/PKG-INFO` & `bbb-dl-1.0.3/bbb_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.2
+Version: 1.0.3
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
@@ -140,17 +140,18 @@
 - For AMD CPUs / GPUs, you can try the encoder `h264_amf` (Use the option `--encoder h264_amf`).
 
 > You have to test yourself if it is faster to use your hardware encoder or not. In some cases, hardware encoders are slower than using the CPU directly. 
 
 
 ### Other downloader
 
-[bbb-video-download](https://github.com/tilmanmoser/bbb-video-download) 
+[bbb-video-download](https://github.com/tilmanmoser/bbb-video-download)
 - It uses a clever approach written in Node.js that can be easily integrated into a bbb server
 - You can use the `--backup` option to feed `bbb-video-download`.
+- A multi-threaded port in go-lang can be found here: [bbb-video-converter](https://github.com/cli-ish/bbb-video-converter)
 
 [bbb-download](https://github.com/fossasia/bbb-download)
 - Takes advantage of the fact that you can use the bbb-player to play the session data offline.
 - Instead of creating a video file, this downloader downloads only the necessary files from the server, so you can use the bbb-player to play the session offline. The player is provided to you via shortcut.
 
 If someone wants to link another downloader here, which offers e.g. functions that bbb-dl does not offer, feel free to open an issue.
```

### Comparing `bbb-dl-1.0.2/setup.py` & `bbb-dl-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     license='GPL-2.0',
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'bbb-dl = bbb_dl.main:main',
             'bbb-dl-batch = bbb_dl.batch:main',
+            'bbb-dl-browser = bbb_dl.browser:main',
         ],
     },
     python_requires='>=3.7',
     install_requires=[
         'aiofiles>=22.1.0',
         'aiohttp>=3.8.3',
         'playwright>=1.29.0',
```

