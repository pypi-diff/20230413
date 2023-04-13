# Comparing `tmp/Termighty-3.0.2.tar.gz` & `tmp/Termighty-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Termighty-3.0.2.tar", last modified: Wed Apr 12 21:08:09 2023, max compression
+gzip compressed data, was "Termighty-3.0.3.tar", last modified: Thu Apr 13 17:18:56 2023, max compression
```

## Comparing `Termighty-3.0.2.tar` & `Termighty-3.0.3.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.591605 Termighty-3.0.2/
--rw-rw-rw-   0        0        0    35823 2022-09-11 20:43:48.000000 Termighty-3.0.2/LICENSE
--rw-rw-rw-   0        0        0      596 2023-04-12 21:08:09.591605 Termighty-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       78 2022-09-11 20:43:48.000000 Termighty-3.0.2/README.md
--rw-rw-rw-   0        0        0      105 2022-09-18 20:12:03.000000 Termighty-3.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-04-12 21:08:09.593606 Termighty-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-04-12 21:06:13.000000 Termighty-3.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.526106 Termighty-3.0.2/source/
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.545607 Termighty-3.0.2/source/Termighty.egg-info/
--rw-rw-rw-   0        0        0      596 2023-04-12 21:08:09.000000 Termighty-3.0.2/source/Termighty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-04-12 21:08:09.000000 Termighty-3.0.2/source/Termighty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:08:09.000000 Termighty-3.0.2/source/Termighty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 21:08:09.000000 Termighty-3.0.2/source/Termighty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-12 21:08:09.000000 Termighty-3.0.2/source/Termighty.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.549106 Termighty-3.0.2/source/termighty/
--rw-rw-rw-   0        0        0      115 2022-09-11 20:43:48.000000 Termighty-3.0.2/source/termighty/__init__.py
--rw-rw-rw-   0        0        0      403 2022-09-17 22:33:08.000000 Termighty-3.0.2/source/termighty/config.ini
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.557106 Termighty-3.0.2/source/termighty/data/
--rw-rw-rw-   0        0        0     7971 2022-09-17 14:02:53.000000 Termighty-3.0.2/source/termighty/data/keymaps.json
--rw-rw-rw-   0        0        0    66090 2022-09-11 20:43:48.000000 Termighty-3.0.2/source/termighty/data/rgb.json
--rw-rw-rw-   0        0        0      216 2022-09-11 20:43:48.000000 Termighty-3.0.2/source/termighty/data/styles.json
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.563105 Termighty-3.0.2/source/termighty/obj/
--rw-rw-rw-   0        0        0       54 2022-09-11 20:43:48.000000 Termighty-3.0.2/source/termighty/obj/__init__.py
--rw-rw-rw-   0        0        0    15095 2022-09-18 18:49:31.000000 Termighty-3.0.2/source/termighty/obj/color.py
--rw-rw-rw-   0        0        0    17757 2022-09-18 14:21:27.000000 Termighty-3.0.2/source/termighty/obj/string.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.571106 Termighty-3.0.2/source/termighty/settings/
--rw-rw-rw-   0        0        0       80 2022-09-11 20:43:48.000000 Termighty-3.0.2/source/termighty/settings/__init__.py
--rw-rw-rw-   0        0        0     1737 2022-09-17 22:33:43.000000 Termighty-3.0.2/source/termighty/settings/config.py
--rw-rw-rw-   0        0        0     1010 2022-09-18 14:22:15.000000 Termighty-3.0.2/source/termighty/settings/data.py
--rw-rw-rw-   0        0        0     1469 2022-09-11 20:43:48.000000 Termighty-3.0.2/source/termighty/settings/system.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.581606 Termighty-3.0.2/source/termighty/utils/
--rw-rw-rw-   0        0        0       97 2022-09-18 19:41:57.000000 Termighty-3.0.2/source/termighty/utils/__init__.py
--rw-rw-rw-   0        0        0    44886 2022-09-18 18:29:32.000000 Termighty-3.0.2/source/termighty/utils/key_processor.py
--rw-rw-rw-   0        0        0    10167 2022-09-18 18:29:32.000000 Termighty-3.0.2/source/termighty/utils/listener.py
--rw-rw-rw-   0        0        0     6754 2022-09-17 20:42:16.000000 Termighty-3.0.2/source/termighty/utils/term.py
--rw-rw-rw-   0        0        0     5787 2022-09-17 13:34:43.000000 Termighty-3.0.2/source/termighty/utils/term_old.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:08:09.588107 Termighty-3.0.2/source/termighty/widgets/
--rw-rw-rw-   0        0        0       68 2022-09-12 19:41:55.000000 Termighty-3.0.2/source/termighty/widgets/__init__.py
--rw-rw-rw-   0        0        0    16825 2023-04-12 20:57:24.000000 Termighty-3.0.2/source/termighty/widgets/text_box.py
--rw-rw-rw-   0        0        0    15908 2023-04-12 21:02:58.000000 Termighty-3.0.2/source/termighty/widgets/text_editor.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.151046 Termighty-3.0.3/
+-rw-rw-rw-   0        0        0    35823 2022-09-11 20:43:48.000000 Termighty-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0      634 2023-04-13 17:18:56.151546 Termighty-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2022-09-11 20:43:48.000000 Termighty-3.0.3/README.md
+-rw-rw-rw-   0        0        0      105 2022-09-18 20:12:03.000000 Termighty-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      130 2023-04-13 17:18:56.153046 Termighty-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-04-13 17:18:35.000000 Termighty-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.087046 Termighty-3.0.3/source/
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.107546 Termighty-3.0.3/source/Termighty.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      900 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 17:18:56.000000 Termighty-3.0.3/source/Termighty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.111046 Termighty-3.0.3/source/termighty/
+-rw-rw-rw-   0        0        0      115 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/__init__.py
+-rw-rw-rw-   0        0        0      403 2022-09-17 22:33:08.000000 Termighty-3.0.3/source/termighty/config.ini
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.118546 Termighty-3.0.3/source/termighty/data/
+-rw-rw-rw-   0        0        0     7971 2022-09-17 14:02:53.000000 Termighty-3.0.3/source/termighty/data/keymaps.json
+-rw-rw-rw-   0        0        0    66090 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/data/rgb.json
+-rw-rw-rw-   0        0        0      216 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/data/styles.json
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.124546 Termighty-3.0.3/source/termighty/obj/
+-rw-rw-rw-   0        0        0       54 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/obj/__init__.py
+-rw-rw-rw-   0        0        0    15095 2022-09-18 18:49:31.000000 Termighty-3.0.3/source/termighty/obj/color.py
+-rw-rw-rw-   0        0        0    17757 2022-09-18 14:21:27.000000 Termighty-3.0.3/source/termighty/obj/string.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.133047 Termighty-3.0.3/source/termighty/settings/
+-rw-rw-rw-   0        0        0       80 2022-09-11 20:43:48.000000 Termighty-3.0.3/source/termighty/settings/__init__.py
+-rw-rw-rw-   0        0        0     1737 2022-09-17 22:33:43.000000 Termighty-3.0.3/source/termighty/settings/config.py
+-rw-rw-rw-   0        0        0     1010 2022-09-18 14:22:15.000000 Termighty-3.0.3/source/termighty/settings/data.py
+-rw-rw-rw-   0        0        0     1458 2023-04-13 13:51:49.000000 Termighty-3.0.3/source/termighty/settings/system.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.141546 Termighty-3.0.3/source/termighty/utils/
+-rw-rw-rw-   0        0        0       97 2022-09-18 19:41:57.000000 Termighty-3.0.3/source/termighty/utils/__init__.py
+-rw-rw-rw-   0        0        0    45163 2023-04-13 14:59:33.000000 Termighty-3.0.3/source/termighty/utils/key_processor.py
+-rw-rw-rw-   0        0        0    10100 2023-04-13 14:40:44.000000 Termighty-3.0.3/source/termighty/utils/listener.py
+-rw-rw-rw-   0        0        0     5463 2023-04-13 14:00:48.000000 Termighty-3.0.3/source/termighty/utils/term.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:18:56.148046 Termighty-3.0.3/source/termighty/widgets/
+-rw-rw-rw-   0        0        0       68 2022-09-12 19:41:55.000000 Termighty-3.0.3/source/termighty/widgets/__init__.py
+-rw-rw-rw-   0        0        0    16902 2023-04-13 14:19:25.000000 Termighty-3.0.3/source/termighty/widgets/text_box.py
+-rw-rw-rw-   0        0        0    15848 2023-04-13 15:25:28.000000 Termighty-3.0.3/source/termighty/widgets/text_editor.py
```

### Comparing `Termighty-3.0.2/LICENSE` & `Termighty-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.2/PKG-INFO` & `Termighty-3.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Termighty
-Version: 3.0.2
+Version: 3.0.3
 Summary: Cross-Platform Terminal Coloring, Formatting, and Management Utilities.
 Home-page: https://github.com/GabrielSCabrera/Termighty
-Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.2.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.3.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: terminal,xterm,gui,windows,linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # Termighty
 
 High-level utilities for cross-platform terminal interaction.
```

### Comparing `Termighty-3.0.2/setup.py` & `Termighty-3.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 setup(
     name="Termighty",
     packages=find_packages(where="source"),
     package_dir={"": "source"},
     include_package_data=True,
     package_data={"": ["data/*.json", "config.ini"]},
-    version="3.0.2",
+    version="3.0.3",
     description="Cross-Platform Terminal Coloring, Formatting, and Management Utilities.",
     long_description=long_description,
     author="Gabriel S. Cabrera",
     author_email="gabriel.sigurd.cabrera@gmail.com",
     url=url,
-    download_url=url + "archive/v3.0.2.tar.gz",
+    download_url=url + "archive/v3.0.3.tar.gz",
     keywords=["terminal", "xterm", "gui", "windows", "linux"],
     install_requires=dependencies,
     # ext_modules=cythonize(["source/termighty/utils/key_processor.pyx"]),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.10",
     ],
```

### Comparing `Termighty-3.0.2/source/Termighty.egg-info/PKG-INFO` & `Termighty-3.0.3/source/Termighty.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Termighty
-Version: 3.0.2
+Version: 3.0.3
 Summary: Cross-Platform Terminal Coloring, Formatting, and Management Utilities.
 Home-page: https://github.com/GabrielSCabrera/Termighty
-Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.2.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/Termightyarchive/v3.0.3.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: terminal,xterm,gui,windows,linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # Termighty
 
 High-level utilities for cross-platform terminal interaction.
```

### Comparing `Termighty-3.0.2/source/Termighty.egg-info/SOURCES.txt` & `Termighty-3.0.3/source/Termighty.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,10 @@
 source/termighty/settings/config.py
 source/termighty/settings/data.py
 source/termighty/settings/system.py
 source/termighty/utils/__init__.py
 source/termighty/utils/key_processor.py
 source/termighty/utils/listener.py
 source/termighty/utils/term.py
-source/termighty/utils/term_old.py
 source/termighty/widgets/__init__.py
 source/termighty/widgets/text_box.py
 source/termighty/widgets/text_editor.py
```

### Comparing `Termighty-3.0.2/source/termighty/data/keymaps.json` & `Termighty-3.0.3/source/termighty/data/keymaps.json`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.2/source/termighty/data/rgb.json` & `Termighty-3.0.3/source/termighty/data/rgb.json`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.2/source/termighty/obj/color.py` & `Termighty-3.0.3/source/termighty/obj/color.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.2/source/termighty/obj/string.py` & `Termighty-3.0.3/source/termighty/obj/string.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.2/source/termighty/settings/config.py` & `Termighty-3.0.3/source/termighty/settings/config.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.2/source/termighty/settings/data.py` & `Termighty-3.0.3/source/termighty/settings/data.py`

 * *Files identical despite different names*

### Comparing `Termighty-3.0.2/source/termighty/settings/system.py` & `Termighty-3.0.3/source/termighty/settings/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import platform
 import shutil
 import threading
 import time
 import warnings
```

### Comparing `Termighty-3.0.2/source/termighty/utils/key_processor.py` & `Termighty-3.0.3/source/termighty/utils/key_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from termighty.settings.config import Config
+from typing import Optional, Union
 
 
 class KeyProcessor:
     """
     Performs all text processing operations given rows of text, a cursor position, and a key input.
     """
 
@@ -717,21 +718,26 @@
     def process_key(
         cls,
         raw_text: list[str, ...],
         cursor_position: tuple[int, int],
         selected: list[tuple[int, int], ...],
         shape: tuple[int, int],
         key: str,
+        ignore_keys: Optional[Union[str, tuple[str,...]]] = None,
     ) -> tuple[bool, list[str, ...], tuple[int, int], list[tuple[int, int], ...]]:
         """
         Take the current text and cursor position, and modify them using the given key input.
         """
         # By default, the text will be updated.  Is set to False if a key without a binding is detected.
         call = True
 
+        if ignore_keys is not None and (key == ignore_keys or key in ignore_keys):
+            call = False
+            return call, raw_text, cursor_position, selected
+
         # Keybindings map to classmethods
         match key:
 
             # Arrow Keys (To move the cursor).
 
             case "Left" | "Keypad-Left":
                 cursor_position = cls.key_arrow_left(
```

### Comparing `Termighty-3.0.2/source/termighty/utils/listener.py` & `Termighty-3.0.3/source/termighty/utils/listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import os
-import re
 import sys
 
-from termighty.settings.config import Config
 from termighty.settings.data import Data
 from termighty.settings.system import System
 from termighty.utils.term import Term
 
 import threading
 import time
 
-from typing import Callable, Optional, Union
+from typing import Optional, Union
 
 # If the OS is Windows, uses msvcrt to read inputs from the terminal.
 if System.os == "Windows":
     import msvcrt
 
 # If the OS is Linux-based, uses termios and tty to read inputs from the terminal.
 else:
```

### Comparing `Termighty-3.0.2/source/termighty/utils/term.py` & `Termighty-3.0.3/source/termighty/utils/term.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,45 +47,26 @@
             self.flush_string(string)
 
     def _compile_buffer(self, text_buffer_grid):
         """
         Prepares the buffer for flushing -- improves efficiency by avoiding printing over a specific position more than
         once.
         """
-
-    # def cursor_down(self, N: int = 1, flush: bool = False) -> None:
-    #     """
-    #     Move the cursor down by the designated number of rows `N`.
-    #     """
-    #     string = f"\033[{N}B"
-    #     if not flush:
-    #         self._text_buffer.append(string)
-    #     else:
-    #         self.flush_string(string)
+        # TODO
 
     def cursor_hide(self, flush: bool = False) -> None:
         """
         Make the cursor invisible (appends to the buffer).
         """
         string = "\033[?25l"
         if not flush:
             self._text_buffer.append(string)
         else:
             self.flush_string(string)
 
-    # def cursor_left(self, N: int = 1, flush: bool = False) -> None:
-    #     """
-    #     Move the cursor left by the designated number of columns `N`.
-    #     """
-    #     string = f"\033[{N}D"
-    #     if not flush:
-    #         self._text_buffer.append(string)
-    #     else:
-    #         self.flush_string(string)
-
     def cursor_load(self, flush: bool = False) -> None:
         """
         Load the cursor position (appends to the buffer) -- save it first by calling `cursor_save`.
         """
         string = "\0338"
         if not flush:
             self._text_buffer.append(string)
@@ -98,24 +79,14 @@
         """
         string = f"\033[{line+1};{column+1}H"
         if not flush:
             self._text_buffer.append(string)
         else:
             self.flush_string(string)
 
-    # def cursor_right(self, N: int = 1, flush: bool = False) -> None:
-    #     """
-    #     Move the cursor right by the designated number of columns `N`.
-    #     """
-    #     string = f"\033[{N}C"
-    #     if not flush:
-    #         self._text_buffer.append(string)
-    #     else:
-    #         self.flush_string(string)
-
     def cursor_save(self, flush: bool = False) -> None:
         """
         Save the cursor position (appends to the buffer) -- reload it by calling `cursor_load`.
         """
         string = "\0337"
         if not flush:
             self._text_buffer.append(string)
@@ -128,24 +99,14 @@
         """
         string = "\033[?25h"
         if not flush:
             self._text_buffer.append(string)
         else:
             self.flush_string(string)
 
-    # def cursor_up(self, N: int = 1, flush: bool = False) -> None:
-    #     """
-    #     Move the cursor up by the designated number of rows `N`.
-    #     """
-    #     string = f"\033[{N}A"
-    #     if not flush:
-    #         self._text_buffer.append(string)
-    #     else:
-    #         self.flush_string(string)
-
     def flush(self) -> None:
         """
         Flush the entire buffer to the terminal. Remove whatever is flushed from the buffer; if something is appended
         to the buffer while the flushing occurs, does not remove that element from the buffer.
         """
         with self.__class__._flush_lock:
             current_buffer_state = self._text_buffer.copy()
@@ -161,14 +122,15 @@
         """
         with self.__class__._flush_lock:
             sys.stdout.write(string)
             sys.stdout.flush()
 
     # def write(self, string: str, flush: bool = False) -> None:
     #     """
+    #     TODO: Rewrite for buffer compiler
     #     Write the given `string` wherever the cursor is currently positioned to the buffer (appends to the buffer).
     #     """
     #     if not flush:
     #         self._text_buffer.append(f"{string}")
     #     else:
     #         self.flush_string(string)
```

### Comparing `Termighty-3.0.2/source/termighty/widgets/text_box.py` & `Termighty-3.0.3/source/termighty/widgets/text_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import collections.abc
 import numpy as np
-import string
 
 from termighty.obj.color import Color
 from termighty.settings.config import Config
 from termighty.settings.data import Data
 from termighty.settings.system import System
 from termighty.utils.term import Term
 
@@ -64,14 +63,15 @@
             argnames=("background", "foreground", "style"),
         )
 
         self._init_color_attributes(background=background, foreground=foreground, style=style)
 
         self._active = False
         self._view_changed = False
+        self._text = None
 
     """MAGIC METHODS"""
 
     def __call__(self, text: Union[str, list[str, ...]]) -> None:
         """
         Modify the current state of the TextBox by replacing its contents with the given text. Accepts a single string,
         or a list of strings -- if a list is given, will place each element in its own row within the TextBox.
@@ -323,14 +323,16 @@
 
         self._alignment = mode
 
     def start(self, dt: float = 0.005):
         """
         Activate a thread that runs the method self._run_thread.
         """
+        if self._text is None:
+            self.__call__([""])
         self._thread = threading.Thread(target=self._run_thread, args=(dt,), daemon=False)
         self._thread.start()
 
     def stop(self) -> None:
         """
         Kill the active thread.
         """
```

### Comparing `Termighty-3.0.2/source/termighty/widgets/text_editor.py` & `Termighty-3.0.3/source/termighty/widgets/text_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import numpy as np
 
 from termighty.obj.color import Color
 from termighty.settings.config import Config
 from termighty.settings.data import Data
-from termighty.settings.system import System
 from termighty.utils.listener import Listener
 from termighty.utils import KeyProcessor
-from termighty.utils.term import Term
 from termighty.widgets.text_box import TextBox
 
 import textwrap
 import threading
-import time
 
 from typing import Optional, Union
 
 
 class TextEditor(TextBox):
     """
     A subclass of `TextBox` that uses class `Listener` to detect keyboard inputs, and emulate a fully-functional word
@@ -236,25 +233,26 @@
             w = max(self._line_numbers_width, int(np.log10(len(self._text))) + 2)
         else:
             w = 0
 
         if self._wrap_text:
             pass
         else:
+
             # Vertically scrolls the view of the text based on the cursor position.
             if (diff := cursor_position[0] - self._shape[0] + self._scroll_buffer[0]) >= 0:
                 self._origin = (self._origin[0] + diff, self._origin[1])
             elif (diff := cursor_position[0] - self._scroll_buffer[0]) < 0:
-                self._origin = (max(0, self._origin[0] + diff), self._origin[1])
+                self._origin = (max(0, self._origin[0] + diff - self._row_start), self._origin[1])
 
             # Horizontally scrolls the view of the text based on the cursor position.
             if (diff := cursor_position[1] - self._shape[1] + self._scroll_buffer[1]) >= 0:
                 self._origin = (self._origin[0], self._origin[1] + diff)
             elif (diff := cursor_position[1] - self._scroll_buffer[1]) < 0:
-                self._origin = (self._origin[0], max(0, self._origin[1] + diff))
+                self._origin = (self._origin[0], max(0, self._origin[1] + diff - self._col_start))
 
             cursor_position = (
                 row + self._row_start - self._origin[0],
                 col + self._col_start - self._origin[1] + w,
             )
 
         self._selected_processed = [
```

