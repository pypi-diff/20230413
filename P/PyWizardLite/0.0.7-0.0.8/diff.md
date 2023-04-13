# Comparing `tmp/PyWizardLite-0.0.7.tar.gz` & `tmp/PyWizardLite-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyWizardLite-0.0.7.tar", last modified: Fri Mar 31 07:41:48 2023, max compression
+gzip compressed data, was "dist\PyWizardLite-0.0.8.tar", last modified: Thu Apr 13 07:11:17 2023, max compression
```

## Comparing `PyWizardLite-0.0.7.tar` & `PyWizardLite-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/
--rw-rw-rw-   0        0        0    11558 2023-03-03 06:43:56.000000 PyWizardLite-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2229 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/PyWizardLite/
--rw-rw-rw-   0        0        0       65 2023-03-31 07:39:33.000000 PyWizardLite-0.0.7/PyWizardLite/__init__.py
--rw-rw-rw-   0        0        0    16613 2023-03-31 07:40:22.000000 PyWizardLite-0.0.7/PyWizardLite/pywizardlite.py
-drwxrwxrwx   0        0        0        0 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/PyWizardLite.egg-info/
--rw-rw-rw-   0        0        0     2229 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/PyWizardLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/PyWizardLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/PyWizardLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/PyWizardLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-03 07:46:56.000000 PyWizardLite-0.0.7/PyWizardLite.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1248 2023-03-03 07:35:36.000000 PyWizardLite-0.0.7/README.md
--rw-rw-rw-   0        0        0       86 2023-03-31 07:41:48.000000 PyWizardLite-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1671 2023-03-03 07:20:10.000000 PyWizardLite-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/
+-rw-rw-rw-   0        0        0    35821 2023-04-13 07:09:09.000000 PyWizardLite-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2229 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/PyWizardLite/
+-rw-rw-rw-   0        0        0       65 2023-04-13 07:11:13.000000 PyWizardLite-0.0.8/PyWizardLite/__init__.py
+-rw-rw-rw-   0        0        0    16683 2023-04-03 12:51:54.000000 PyWizardLite-0.0.8/PyWizardLite/pywizardlite.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/PyWizardLite.egg-info/
+-rw-rw-rw-   0        0        0     2229 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/PyWizardLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/PyWizardLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/PyWizardLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/PyWizardLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-03-03 07:46:56.000000 PyWizardLite-0.0.8/PyWizardLite.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1248 2023-03-03 07:35:36.000000 PyWizardLite-0.0.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-13 07:11:17.000000 PyWizardLite-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1671 2023-03-03 07:20:10.000000 PyWizardLite-0.0.8/setup.py
```

### Comparing `PyWizardLite-0.0.7/PKG-INFO` & `PyWizardLite-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWizardLite
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyWizardLite automates downloading the correct Chrome driver and generates XPath expressions for visible elements using their text.
 Home-page: https://github.com/4akhilkumar/PyWizardLite
 Author: Sai Akhil Kumar Reddy N
 Author-email: 4akhilkumar@gmail.com
 License: Apache
 Keywords: Python script,Selenium,ChromeDriver,XPath,Element visibility,Download,Web scraping,Automated testing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyWizardLite-0.0.7/PyWizardLite/pywizardlite.py` & `PyWizardLite-0.0.8/PyWizardLite/pywizardlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-PyWizardLite is a python script that automates the process of downloading the suitable version of
-chrome driver for the chrome version installed on the machine. It also has the functionality
+PyWizardLite is a python script that automates the process of downloading the suitable version
+of chrome driver for the chrome version installed on the machine. It also has the functionality
 to generate the xpath of an element on a webpage using the text of the element and the it
 will wait for the element to be visible.
 
 Information:
     Supports Windows OS Only
 
 Source/Reference:
@@ -17,32 +17,33 @@
 import sys
 import time
 from zipfile import ZipFile
 
 try:
     from selenium.webdriver.common.by import By
     from selenium.webdriver.support.ui import Select
-except ImportError:
-    raise ImportError("Please install selenium package")
+except ImportError as exc:
+    raise ImportError("Please install selenium package") from exc
 
 try:
     import requests
-except ImportError:
-    raise ImportError("Please install requests package")
+except ImportError as exc:
+    raise ImportError("Please install requests package") from exc
+
 
 class ElementNotFound(Exception):
     """
     ElementNotFound is an exception when the element is not found
     """
 
 
 class PyWizardLite:
     """
-    PyWizardLite is a python script that automates the process of downloading the suitable version of
-    chrome driver for the chrome version installed on the machine. It also has the functionality
+    PyWizardLite is a python script that automates the process of downloading the suitable version
+    of chrome driver for the chrome version installed on the machine. It also has the functionality
     to generate the xpath of an element on a webpage using the text of the element and the it
     will wait for the element to be visible.
     """
     __COMMANDS = (
         r'(Get-Item -Path "$env:LOCALAPPDATA\Google\Chrome\Application\chrome.exe").VersionInfo.FileVersion',
         r'(Get-Item -Path "$env:PROGRAMFILES\Google\Chrome\Application\chrome.exe").VersionInfo.FileVersion',
         r'(Get-Item -Path "$env:PROGRAMFILES (x86)\Google\Chrome\Application\chrome.exe").VersionInfo.FileVersion',
@@ -52,14 +53,15 @@
 
     def __init__(self):
         """
         Initialize the PyWizardLite class
         """
         self.__file_response = None
         self.__driver = "chromedriver.exe"
+        self.download_path = None
 
     def system_requirements(self) -> bool:
         """
         Check if the system meets the requirements to run this script
 
         Returns:
             bool: True if the system meets the requirements, False otherwise
@@ -331,15 +333,15 @@
 
             if is_element_found:
                 time.sleep(found_wait_time)
                 break
             time.sleep(1)
 
     def wait_until_css_condition(driver, element_by,
-                                 element: str, css_prop: str, css_value: str, default_time: int = None):
+                            element: str, css_prop: str, css_value: str, default_time: int = None):
         """
         This function waits until the css condition met and default time is 60 seconds
 
         Args:
             element_by (Web Element Object): Set of supported locator strategies
             Acceptable values are ClassName, CSSSelector, ID, LinkText, Name,
             PartialLinkText, TagName, XPath
@@ -370,15 +372,15 @@
         start_time = time.time()
 
         while True:
             condition = False
             end_time = time.time()
             total_time = int(end_time - start_time)
             if total_time >= wait_time:
-                raise Exception(f'The element - {element} not found within the limited time!')
+                raise ElementNotFound(f'The element - {element} not found within the limited time!')
 
             try:
                 is_web_element_found = driver.find_element(element_dict[element_by], element)
                 if is_web_element_found is not None:
                     # Now fetch the inline style of the element
                     inline_style = is_web_element_found.get_attribute('style')
                     # Store the css property and value in a dictionary
```

### Comparing `PyWizardLite-0.0.7/PyWizardLite.egg-info/PKG-INFO` & `PyWizardLite-0.0.8/PyWizardLite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWizardLite
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyWizardLite automates downloading the correct Chrome driver and generates XPath expressions for visible elements using their text.
 Home-page: https://github.com/4akhilkumar/PyWizardLite
 Author: Sai Akhil Kumar Reddy N
 Author-email: 4akhilkumar@gmail.com
 License: Apache
 Keywords: Python script,Selenium,ChromeDriver,XPath,Element visibility,Download,Web scraping,Automated testing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyWizardLite-0.0.7/README.md` & `PyWizardLite-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PyWizardLite-0.0.7/setup.py` & `PyWizardLite-0.0.8/setup.py`

 * *Files identical despite different names*

