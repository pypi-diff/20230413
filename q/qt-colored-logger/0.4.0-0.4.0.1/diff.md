# Comparing `tmp/qt_colored_logger-0.4.0.tar.gz` & `tmp/qt_colored_logger-0.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt_colored_logger-0.4.0.tar", last modified: Sun Apr  9 16:56:53 2023, max compression
+gzip compressed data, was "qt_colored_logger-0.4.0.1.tar", last modified: Thu Apr 13 17:41:08 2023, max compression
```

## Comparing `qt_colored_logger-0.4.0.tar` & `qt_colored_logger-0.4.0.1.tar`

### file list

```diff
@@ -1,34 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.221768 qt_colored_logger-0.4.0/
--rw-rw-rw-   0        0        0    11357 2023-03-13 14:04:00.000000 qt_colored_logger-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     9691 2023-04-09 16:56:53.221768 qt_colored_logger-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     8898 2023-04-09 10:07:36.000000 qt_colored_logger-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.129109 qt_colored_logger-0.4.0/qt_colored_logger/
--rw-rw-rw-   0        0        0      811 2023-04-09 16:19:08.000000 qt_colored_logger-0.4.0/qt_colored_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.161114 qt_colored_logger-0.4.0/qt_colored_logger/basic/
--rw-rw-rw-   0        0        0      812 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     5893 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1126 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0      848 2023-04-08 15:17:18.000000 qt_colored_logger-0.4.0/qt_colored_logger/basic/patterns.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.178009 qt_colored_logger-0.4.0/qt_colored_logger/logger/
--rw-rw-rw-   0        0        0      739 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0/qt_colored_logger/logger/__init__.py
--rw-rw-rw-   0        0        0    39641 2023-04-09 09:07:44.000000 qt_colored_logger-0.4.0/qt_colored_logger/logger/colored_logger.py
--rw-rw-rw-   0        0        0    37471 2023-04-09 09:14:39.000000 qt_colored_logger-0.4.0/qt_colored_logger/logger/html_colored_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.195121 qt_colored_logger-0.4.0/qt_colored_logger/src/
--rw-rw-rw-   0        0        0      866 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/__init__.py
--rw-rw-rw-   0        0        0     4758 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     8957 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/color_picker.py
--rw-rw-rw-   0        0        0     1677 2023-04-07 12:17:31.000000 qt_colored_logger-0.4.0/qt_colored_logger/src/~log_environment.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.219767 qt_colored_logger-0.4.0/qt_colored_logger/text/
--rw-rw-rw-   0        0        0      720 2023-04-08 16:15:43.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/__init__.py
--rw-rw-rw-   0        0        0     5881 2023-04-09 09:04:41.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/text_buffer.py
--rw-rw-rw-   0        0        0     4822 2023-04-07 12:21:55.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/~animation.py
--rw-rw-rw-   0        0        0     1704 2023-04-07 12:17:31.000000 qt_colored_logger-0.4.0/qt_colored_logger/text/~icon_set.py
--rw-rw-rw-   0        0        0    14432 2021-01-12 12:58:45.000000 qt_colored_logger-0.4.0/qt_colored_logger/~~logger~~.py
--rw-rw-rw-   0        0        0     7482 2021-01-12 12:58:45.000000 qt_colored_logger-0.4.0/qt_colored_logger/~~utils~~.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:56:53.140826 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/
--rw-rw-rw-   0        0        0     9691 2023-04-09 16:56:52.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-09 16:56:53.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:56:52.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-09 16:56:52.000000 qt_colored_logger-0.4.0/qt_colored_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 16:56:53.222767 qt_colored_logger-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2920 2023-04-09 16:39:19.000000 qt_colored_logger-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:41:08.006363 qt_colored_logger-0.4.0.1/
+-rw-rw-rw-   0        0        0    11357 2023-03-13 14:04:00.000000 qt_colored_logger-0.4.0.1/LICENSE
+-rw-rw-rw-   0        0        0     8216 2023-04-13 17:41:08.006363 qt_colored_logger-0.4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7421 2023-04-13 17:39:36.000000 qt_colored_logger-0.4.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:41:07.658621 qt_colored_logger-0.4.0.1/qt_colored_logger/
+-rw-rw-rw-   0        0        0      813 2023-04-13 17:39:36.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:41:07.839087 qt_colored_logger-0.4.0.1/qt_colored_logger/basic/
+-rw-rw-rw-   0        0        0      812 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     5893 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1126 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0      848 2023-04-08 15:17:18.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/basic/patterns.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:41:07.948114 qt_colored_logger-0.4.0.1/qt_colored_logger/logger/
+-rw-rw-rw-   0        0        0      739 2023-04-08 15:53:12.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/logger/__init__.py
+-rw-rw-rw-   0        0        0    39641 2023-04-09 09:07:44.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/logger/colored_logger.py
+-rw-rw-rw-   0        0        0    37471 2023-04-09 09:14:39.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/logger/html_colored_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:41:07.964114 qt_colored_logger-0.4.0.1/qt_colored_logger/src/
+-rw-rw-rw-   0        0        0      866 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     4758 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     8957 2023-04-08 15:58:27.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/src/color_picker.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:41:07.978360 qt_colored_logger-0.4.0.1/qt_colored_logger/text/
+-rw-rw-rw-   0        0        0      720 2023-04-08 16:15:43.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/text/__init__.py
+-rw-rw-rw-   0        0        0     5881 2023-04-09 09:04:41.000000 qt_colored_logger-0.4.0.1/qt_colored_logger/text/text_buffer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:41:07.708992 qt_colored_logger-0.4.0.1/qt_colored_logger.egg-info/
+-rw-rw-rw-   0        0        0     8216 2023-04-13 17:41:07.000000 qt_colored_logger-0.4.0.1/qt_colored_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-13 17:41:07.000000 qt_colored_logger-0.4.0.1/qt_colored_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:41:07.000000 qt_colored_logger-0.4.0.1/qt_colored_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 17:41:07.000000 qt_colored_logger-0.4.0.1/qt_colored_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:41:08.008364 qt_colored_logger-0.4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2922 2023-04-13 17:39:36.000000 qt_colored_logger-0.4.0.1/setup.py
```

### Comparing `qt_colored_logger-0.4.0/LICENSE` & `qt_colored_logger-0.4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/PKG-INFO` & `qt_colored_logger-0.4.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt_colored_logger
-Version: 0.4.0
+Version: 0.4.0.1
 Summary: Powerful functional logger with support for qt programming
 Home-page: https://github.com/Nakama3942/qt_colored_logger
 Author: Kalynovsky 'Nakama3942' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/qt_colored_logger/releases
 Classifier: Development Status :: 3 - Alpha
@@ -18,35 +18,18 @@
 License-File: LICENSE
 
 <div align="center">
 
 [![template](https://img.shields.io/badge/Repository-template-darkred)](https://github.com/Nakama3942/template_rep)
 [![GitHub license](https://img.shields.io/github/license/Nakama3942/qt_colored_logger?color=gold&style=flat-square)](https://github.com/Nakama3942/qt_colored_logger/blob/master/LICENSE)
 
-![PyPI](https://img.shields.io/pypi/v/qt-colored-logger?color=yellow&logo=pypi&logoColor=white&style=flat-square)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/Nakama3942/qt_colored_logger?label=latest%20release&logo=github&style=flat-square)
-![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Nakama3942/qt_colored_logger?color=orange&include_prereleases&label=latest%20pre-release&logo=github&style=flat-square)
-![GitHub commits since latest release (by date including pre-releases)](https://img.shields.io/github/commits-since/Nakama3942/qt_colored_logger/v0.3.0?include_prereleases&style=flat-square)
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qt_colored_logger?style=flat-square)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/qt_colored_logger?style=flat-square)
-![PyPI - Format](https://img.shields.io/pypi/format/qt_colored_logger?label=PyPI%20format&style=flat-square)
-![PyPI - Status](https://img.shields.io/pypi/status/qt_colored_logger?label=PyPI%20status&style=flat-square)
-
-![GitHub last commit](https://img.shields.io/github/last-commit/Nakama3942/qt_colored_logger?style=flat-square)
-![GitHub Release Date](https://img.shields.io/github/release-date/Nakama3942/qt_colored_logger?style=flat-square)
-![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Nakama3942/qt_colored_logger?label=%28pre-%29release%20date&style=flat-square)
-
-![GitHub repo size](https://img.shields.io/github/repo-size/Nakama3942/qt_colored_logger?color=darkgreen&style=flat-square)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Nakama3942/qt_colored_logger?color=darkgreen&style=flat-square)
-
-[![CHANGELOG](https://img.shields.io/badge/here-CHANGELOG-yellow)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CHANGELOG.md)
-[![CONTRIBUTING](https://img.shields.io/badge/here-CONTRIBUTING-indigo)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CONTRIBUTING.md)
-[![CODE_OF_CONDUCT](https://img.shields.io/badge/here-CODE_OF_CONDUCT-darkgreen)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CODE_OF_CONDUCT.md)
-[![PULL_REQUEST_TEMPLATE](https://img.shields.io/badge/here-PULL_REQUEST_TEMPLATE-orange)](https://github.com/Nakama3942/qt_colored_logger/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
+!!!ATTENTION!!! In connection with the increase in capabilities and functionality, the library has changed its name! It is now called [Mighty Logger](https://pypi.org/project/mighty-logger/). This repository **is no longer maintained by the author**!
+
+[![NEW PROJECT LIBRARY](https://img.shields.io/badge/NEW-PROJECT_LIBRARY-orange?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/mighty-logger/)
+[![NEW REPOSITORY](https://img.shields.io/badge/NEW-REPOSITORY-darkred?style=for-the-badge&logo=github)](https://github.com/Nakama3942/mighty_logger)
 
 </div>
 
 # Qt_Сolored-logger
 ### Content
 - [Qt_Сolored-logger](#qtсolored-logger)
 	- [Content](#content)
@@ -84,22 +67,17 @@
 ## Important releases
 <details><summary>See the important releases (possible spoilers)</summary>
 
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
-- [ ] v0.5.0 - Unifying update (console and HTML are combined into one class)
-- [ ] v0.6.0 - Symbols update (added hint symbols near log entries types)
-- [ ] v0.7.0 - Progress update (added start of some log entries in threads (process))
-- [ ] v0.8.0 - Animation update (added animations in processes)
-- [ ] v0.9.0 - Search update (added search by log entry types)
-- [ ] v0.9.1 - Extension update (made wheel format and instruction of toml)
-- [ ] v1.0.0 - Completion of logger development (logger development completed)
-- [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
+- [x] v0.5.0 - PROJECT NAME CHANGED
+
+!!!ATTENTION!!! In connection with the increase in capabilities and functionality, the library has changed its name! It is now called [Mighty Logger](https://pypi.org/project/mighty-logger/). This repository **is no longer maintained by the author**!
 
 </details>
 
 - [Content](#content)
 
 ## LICENSE
 The full text of the license can be found at the following [link](https://github.com/Nakama3942/qt_colored_logger/blob/master/LICENSE).
@@ -118,14 +96,16 @@
 > See the License for the specific language governing permissions and
 
 - [Content](#content)
 
 ## Installation
 Despite the fact that the library was originally developed for use in PyQt, it does not require PyQt to be installed, since this framework for outputting to Text fields, which support not only Plain Text, uses HTML and this library simply simplifies the logging process, since the creation process already formatted strings is registered in this library.
 
+!!!ATTENTION!!! In connection with the increase in capabilities and functionality, the library has changed its name! It is now called [Mighty Logger](https://pypi.org/project/mighty-logger/). This repository **is no longer maintained by the author**!
+
 To install the library, enter the command:
 ```sh
 pip install qt-colored-logger
 ```
 
 ## Usage
 This is the simplest example of using the library:
@@ -143,25 +123,27 @@
 > <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span><br>
 > <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-04-09 12:37:07.198496 </span><span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>OK </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Outputting the message</span></span><br>
 
 See the USAGING.md file for more details.
 
 - [Content](#content)
 
-## *Additional functionality*
-*Additional functionality is also planned. Let's keep it a secret for now. Let it be a surprise.*
+## ~~Additional functionality~~
+!!!ATTENTION!!! In connection with the increase in capabilities and functionality, the library has changed its name! It is now called [Mighty Logger](https://pypi.org/project/mighty-logger/). This repository **is no longer maintained by the author**!
 
 - [Content](#content)
 
 ## Data
 See the DATA.md file.
 
 - [Content](#content)
 
 ## Troubleshooting
+!!!ATTENTION!!! In connection with the increase in capabilities and functionality, the library has changed its name! It is now called [Mighty Logger](https://pypi.org/project/mighty-logger/). This repository **is no longer maintained by the author**!
+
 All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/qt_colored_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/qt_colored_logger/blob/master/CODE_OF_CONDUCT.md).
 
 - [Content](#content)
 
 ## Authors
 <table align="center" style="border-width: 10; border-style: ridge">
 	<tr>
```

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/__init__.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 limitations under the License.
 """
 
 # from .colored_logger import Logger
 # from .html_colored_logger import LoggerQ
 
 __authot__ = "Kalynovsky 'Nakama3942' Valentin"
-__version__ = "0.4.0"
+__version__ = "0.4.0.1"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/basic/__init__.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/basic/basic_logger.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/basic/basic_logger.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/basic/exceptions.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/basic/exceptions.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/basic/patterns.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/basic/patterns.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/logger/__init__.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/logger/colored_logger.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/logger/colored_logger.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/logger/html_colored_logger.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/logger/html_colored_logger.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/src/__init__.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/src/__init__.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/src/ansi_format.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/src/ansi_format.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/src/color_picker.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/text/__init__.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/text/__init__.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger/text/text_buffer.py` & `qt_colored_logger-0.4.0.1/qt_colored_logger/text/text_buffer.py`

 * *Files identical despite different names*

### Comparing `qt_colored_logger-0.4.0/qt_colored_logger.egg-info/SOURCES.txt` & `qt_colored_logger-0.4.0.1/qt_colored_logger.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 qt_colored_logger/__init__.py
-qt_colored_logger/~~logger~~.py
-qt_colored_logger/~~utils~~.py
 qt_colored_logger.egg-info/PKG-INFO
 qt_colored_logger.egg-info/SOURCES.txt
 qt_colored_logger.egg-info/dependency_links.txt
 qt_colored_logger.egg-info/top_level.txt
 qt_colored_logger/basic/__init__.py
 qt_colored_logger/basic/basic_logger.py
 qt_colored_logger/basic/exceptions.py
 qt_colored_logger/basic/patterns.py
 qt_colored_logger/logger/__init__.py
 qt_colored_logger/logger/colored_logger.py
 qt_colored_logger/logger/html_colored_logger.py
 qt_colored_logger/src/__init__.py
 qt_colored_logger/src/ansi_format.py
 qt_colored_logger/src/color_picker.py
-qt_colored_logger/src/~log_environment.py
 qt_colored_logger/text/__init__.py
-qt_colored_logger/text/text_buffer.py
-qt_colored_logger/text/~animation.py
-qt_colored_logger/text/~icon_set.py
+qt_colored_logger/text/text_buffer.py
```

### Comparing `qt_colored_logger-0.4.0/setup.py` & `qt_colored_logger-0.4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name="qt_colored_logger",
-    version="0.4.0",
+    version="0.4.0.1",
 
     author="Kalynovsky 'Nakama3942' Valentin",
     author_email="nakama3942@gmail.com",
 
     description="Powerful functional logger with support for qt programming",
     long_description=readme,
     long_description_content_type="text/markdown",
```

