# Comparing `tmp/selene-2.0.0rc1.tar.gz` & `tmp/selene-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selene-2.0.0rc1.tar", max compression
+gzip compressed data, was "selene-2.0.0rc2.tar", max compression
```

## Comparing `selene-2.0.0rc1.tar` & `selene-2.0.0rc2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0    16589 2023-04-10 12:28:03.426931 selene-2.0.0rc1/README.md
--rw-r--r--   0        0        0     7951 2023-04-10 11:04:48.138046 selene-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6045 2023-04-01 13:26:39.498825 selene-2.0.0rc1/selene/__init__.py
--rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc1/selene/_managed.py
--rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc1/selene/api/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc1/selene/api/base/__init__.py
--rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc1/selene/api/shared/__init__.py
--rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc1/selene/common/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc1/selene/common/data_structures/__init__.py
--rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc1/selene/common/data_structures/persistent.py
--rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc1/selene/common/fp.py
--rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc1/selene/common/helpers.py
--rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc1/selene/common/none_object.py
--rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc1/selene/common/predicate.py
--rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc1/selene/core/__init__.py
--rw-r--r--   0        0        0     7107 2023-04-10 11:06:23.401462 selene-2.0.0rc1/selene/core/command.py
--rw-r--r--   0        0        0     6608 2023-04-10 11:06:23.381272 selene-2.0.0rc1/selene/core/condition.py
--rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc1/selene/core/conditions.py
--rw-r--r--   0        0        0    50433 2023-04-11 00:26:18.593662 selene-2.0.0rc1/selene/core/configuration.py
--rw-r--r--   0        0        0     9224 2023-04-11 01:37:57.353410 selene-2.0.0rc1/selene/core/configuration.pyi
--rw-r--r--   0        0        0    44329 2023-04-11 01:51:05.070968 selene-2.0.0rc1/selene/core/entity.py
--rw-r--r--   0        0        0    11983 2023-04-11 01:51:05.074766 selene-2.0.0rc1/selene/core/entity.pyi
--rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc1/selene/core/exceptions.py
--rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc1/selene/core/locator.py
--rw-r--r--   0        0        0    17245 2023-04-10 11:06:23.584719 selene-2.0.0rc1/selene/core/match.py
--rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc1/selene/core/query.py
--rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc1/selene/core/wait.py
--rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc1/selene/py.typed
--rw-r--r--   0        0        0      107 2023-04-01 17:58:51.579568 selene-2.0.0rc1/selene/support/__init__.py
--rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc1/selene/support/_logging.py
--rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc1/selene/support/by.py
--rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc1/selene/support/conditions/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc1/selene/support/conditions/be.py
--rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc1/selene/support/conditions/have.py
--rw-r--r--   0        0        0     8989 2023-04-10 11:06:23.509416 selene-2.0.0rc1/selene/support/conditions/not_.py
--rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc1/selene/support/shared/__init__.py
--rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc1/selene/support/shared/browser.py
--rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc1/selene/support/shared/config.py
--rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc1/selene/support/shared/jquery_style.py
--rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc1/selene/support/webdriver.py
--rw-r--r--   0        0        0    18274 1970-01-01 00:00:00.000000 selene-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    16589 2023-04-10 12:28:03.426931 selene-2.0.0rc2/README.md
+-rw-r--r--   0        0        0     7937 2023-04-12 20:12:16.143699 selene-2.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6045 2023-04-12 19:26:33.211787 selene-2.0.0rc2/selene/__init__.py
+-rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc2/selene/_managed.py
+-rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc2/selene/api/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc2/selene/api/base/__init__.py
+-rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc2/selene/api/shared/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc2/selene/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc2/selene/common/data_structures/__init__.py
+-rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc2/selene/common/data_structures/persistent.py
+-rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc2/selene/common/fp.py
+-rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc2/selene/common/helpers.py
+-rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc2/selene/common/none_object.py
+-rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc2/selene/common/predicate.py
+-rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc2/selene/core/__init__.py
+-rw-r--r--   0        0        0     8731 2023-04-13 16:15:03.548744 selene-2.0.0rc2/selene/core/command.py
+-rw-r--r--   0        0        0     6608 2023-04-10 11:06:23.381272 selene-2.0.0rc2/selene/core/condition.py
+-rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc2/selene/core/conditions.py
+-rw-r--r--   0        0        0    61013 2023-04-13 13:34:08.396102 selene-2.0.0rc2/selene/core/configuration.py
+-rw-r--r--   0        0        0     9441 2023-04-12 19:41:51.757408 selene-2.0.0rc2/selene/core/configuration.pyi
+-rw-r--r--   0        0        0    44335 2023-04-13 13:44:05.445570 selene-2.0.0rc2/selene/core/entity.py
+-rw-r--r--   0        0        0    12087 2023-04-12 19:44:29.895473 selene-2.0.0rc2/selene/core/entity.pyi
+-rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc2/selene/core/exceptions.py
+-rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc2/selene/core/locator.py
+-rw-r--r--   0        0        0    17245 2023-04-10 11:06:23.584719 selene-2.0.0rc2/selene/core/match.py
+-rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc2/selene/core/query.py
+-rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc2/selene/core/wait.py
+-rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc2/selene/py.typed
+-rw-r--r--   0        0        0      107 2023-04-01 17:58:51.579568 selene-2.0.0rc2/selene/support/__init__.py
+-rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc2/selene/support/_logging.py
+-rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc2/selene/support/by.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc2/selene/support/conditions/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc2/selene/support/conditions/be.py
+-rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc2/selene/support/conditions/have.py
+-rw-r--r--   0        0        0     8989 2023-04-10 11:06:23.509416 selene-2.0.0rc2/selene/support/conditions/not_.py
+-rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc2/selene/support/shared/__init__.py
+-rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc2/selene/support/shared/browser.py
+-rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc2/selene/support/shared/config.py
+-rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc2/selene/support/shared/jquery_style.py
+-rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc2/selene/support/webdriver.py
+-rw-r--r--   0        0        0    18274 1970-01-01 00:00:00.000000 selene-2.0.0rc2/PKG-INFO
```

### Comparing `selene-2.0.0rc1/LICENSE` & `selene-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/README.md` & `selene-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/pyproject.toml` & `selene-2.0.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selene"
-version = "2.0.0rc1"
+version = "2.0.0rc2"
 description = "User-oriented browser tests in Python (Selenide port)"
 authors = ["Iakiv Kramarenko <yashaka@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
 	"testing",
 	"selenium",
@@ -54,15 +54,14 @@
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pycodestyle = "*"
 pylint = "^2.7.2"
 pytest = "*"
 pytest-cov = "*"
-codecov = "*"
 mypy = "*"
 pydantic = "^1.10.7"
 python-dotenv = "0.21.1"
 Appium-Python-Client = "^2.9.0"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `selene-2.0.0rc1/selene/__init__.py` & `selene-2.0.0rc2/selene/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,8 +223,8 @@
 """
 
 # """
 # Just types...
 # """
 from selene.core.entity import Element, Collection  # noqa
 
-__version__ = '2.0.0rc1'
+__version__ = '2.0.0rc2'
```

### Comparing `selene-2.0.0rc1/selene/api/__init__.py` & `selene-2.0.0rc2/selene/api/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/api/base/__init__.py` & `selene-2.0.0rc2/selene/api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/api/shared/__init__.py` & `selene-2.0.0rc2/selene/api/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/common/data_structures/persistent.py` & `selene-2.0.0rc2/selene/common/data_structures/persistent.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/common/fp.py` & `selene-2.0.0rc2/selene/common/fp.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/common/helpers.py` & `selene-2.0.0rc2/selene/common/helpers.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/common/none_object.py` & `selene-2.0.0rc2/selene/common/none_object.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/common/predicate.py` & `selene-2.0.0rc2/selene/common/predicate.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/__init__.py` & `selene-2.0.0rc2/selene/core/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/command.py` & `selene-2.0.0rc2/selene/core/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,18 +15,26 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+import sys
 from typing import Union, Optional
 
+import typing
+from selenium.webdriver import Keys
+
 from selene.core.entity import Element, Collection, Browser
 from selene.core.wait import Command
+from selenium.webdriver import ActionChains
+from selenium.webdriver.common.actions import interaction
+from selenium.webdriver.common.actions.action_builder import ActionBuilder
+from selenium.webdriver.common.actions.pointer_input import PointerInput
 
 
 def save_screenshot(path: Optional[str] = None) -> Command[Browser]:
     command: Command[Browser] = Command(
         'save screenshot',
         lambda browser: browser.config._save_screenshot_strategy(browser.config, path),
     )
@@ -51,14 +59,55 @@
         # not as `.perform(command.save_screenshot())`
         browser = path
         command.__call__(browser)
 
     return command
 
 
+select_all: Command[Element] = Command(
+    'select all by ctrl+a or cmd+a for mac',
+    lambda element: typing.cast(Element, element)
+    .locate()
+    .send_keys(
+        (Keys.COMMAND if sys.platform == 'darwin' else Keys.CONTROL) + 'a' + Keys.NULL,
+    ),
+)
+
+
+# TODO: can we make it work for both mobile and web?
+#       should we selectively choose proper interaction.POINTER_TOUCH below?
+def _long_press(duration=1.0):
+    def func(element: Element):
+        located_element = element.locate()
+        driver = element.config.driver
+        actions: ActionChains = ActionChains(driver)
+
+        actions.w3c_actions = ActionBuilder(
+            driver, mouse=PointerInput(interaction.POINTER_TOUCH, 'touch')
+        )
+        (
+            actions.w3c_actions.pointer_action.move_to(located_element)
+            .pointer_down()
+            .pause(duration)
+            .release()
+        )
+        actions.perform()
+
+    command = Command(f'long press with duration={duration}', func)
+
+    if isinstance(duration, Element):
+        # somebody passed command as `.perform(command.long_press)`
+        # not as `.perform(command.long_press())`
+        # TODO: refactor to really allow such use case without conflicts on types
+        element = duration
+        command.__call__(element)
+
+    return command
+
+
 class js:  # pylint: disable=invalid-name
     @staticmethod
     def set_value(value: Union[str, int]) -> Command[Element]:
         def func(element: Element):
             element.execute_script(
                 """
                 var text = arguments[0];
```

### Comparing `selene-2.0.0rc1/selene/core/condition.py` & `selene-2.0.0rc2/selene/core/condition.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/conditions.py` & `selene-2.0.0rc2/selene/core/conditions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/configuration.py` & `selene-2.0.0rc2/selene/core/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 import os
 import time
 import typing
 import warnings
 from typing import Callable, Optional, Any
 
 from selenium.webdriver.common.options import BaseOptions
-from selenium.webdriver.remote.command import Command
+from selenium.webdriver.common.service import Service
 
 from selene.common import fp, helpers
 from selene.common.data_structures import persistent
-from selene.common.fp import F, pipe, thread
+from selene.common.fp import F
 from selene.common.helpers import on_error_return_false
 
 from selene.core.exceptions import TimeoutException
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from selene.core.wait import Wait, E
 
@@ -65,62 +65,68 @@
     from webdriver_manager.chrome import ChromeDriverManager  # type: ignore
     from webdriver_manager.firefox import GeckoDriverManager  # type: ignore
     from webdriver_manager.microsoft import EdgeChromiumDriverManager  # type: ignore
 
     from webdriver_manager.core.utils import ChromeType  # type: ignore
 
     def install_and_build_chrome():
+        # TODO: consider simplifying the logic... to much of ifs
+        #       probably all ifs were already before calling this function
+        #       see example of simplification in install_and_build_firefox
         if config.driver_options:
             if isinstance(config.driver_options, ChromeOptions):
                 return Chrome(
-                    service=ChromeService(
+                    service=config.driver_service
+                    or ChromeService(
                         ChromeDriverManager(chrome_type=ChromeType.GOOGLE).install()
                     ),
                     options=config.driver_options,
                 )
             else:
                 raise ValueError(
                     f'Default config.build_driver_strategy («driver factory»), '
-                    f'if config.name is set to "chrome", – '
-                    f'expects only instance of ChromeOptions or None in config.driver_options,'
+                    f'if config.driver_name is set to "chrome", - '
+                    f'expects only instance of ChromeOptions or None'
+                    f'in config.driver_options,'
                     f'but got: {config.driver_options}'
                 )
         else:
             return Chrome(
-                service=ChromeService(
+                service=config.driver_service
+                or ChromeService(
                     ChromeDriverManager(chrome_type=ChromeType.GOOGLE).install()
                 )
             )
 
     def install_and_build_firefox():
-        return (
-            Firefox(
-                service=FirefoxService(GeckoDriverManager().install()),
-                options=config.driver_options,
-            )
-            if config.driver_options
-            else Firefox(service=FirefoxService(GeckoDriverManager().install()))
+        return Firefox(
+            service=config.driver_service
+            or FirefoxService(GeckoDriverManager().install()),
+            options=config.driver_options,
         )
 
     def install_and_build_edge():
         if config.driver_options:
             if isinstance(config.driver_options, EdgeOptions):
                 return Edge(
-                    service=EdgeService(EdgeChromiumDriverManager().install()),
+                    service=config.driver_service
+                    or EdgeService(EdgeChromiumDriverManager().install()),
                     options=config.driver_options,
                 )
             else:
                 raise ValueError(
                     f'Default config.build_driver_strategy, '
-                    f'if config.name is set to "edge", – '
+                    f'if config.driver_name is set to "edge", - '
                     f'expects only instance of EdgeOptions or None in config.driver_options,'
                     f'but got: {config.driver_options}'
                 )
         else:
-            return Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
+            return Edge(
+                service=config.driver_service or (EdgeChromiumDriverManager().install())
+            )
 
     def build_remote_driver():
         from selenium.webdriver import Remote
 
         # TODO: consider guessing browserstack remote url
         #       if noticed 'bstack:options' in config.driver_options
 
@@ -177,19 +183,27 @@
             or (
                 config.driver_options
                 and 'platformName' in config.driver_options.capabilities
                 and config.driver_options.capabilities['platformName'].lower()
                 in ['android', 'ios']
             )
         )
+        else 'remote'
+        if (config.driver_remote_url or config.driver_name == 'remote')
         # TODO: consider automatically detect installed browser if driver_name not set
-        else (config.driver_name or 'chrome')
-        if not config.driver_remote_url
-        else 'remote',
-        'chrome',
+        else (
+            config.driver_name
+            if config.driver_name
+            else config.driver_options.capabilities['browserName']
+            if (
+                config.driver_options
+                and 'browserName' in config.driver_options.capabilities
+            )
+            else 'chrome'
+        )
     )()
 
 
 def _maybe_reset_driver_then_tune_window_and_get_with_base_url(config: Config):
     def get(url: Optional[str] = None) -> None:
         if (
             config._reset_not_alive_driver_on_get_url
@@ -411,99 +425,110 @@
     For example, `config.timeout` is used in all "waiting" logic
     of Selene commands. And `config.base_url` is used
     in `browser.open(relative_url)` command.
 
     As option, the driver instance is also considered. Moreover, this config
     is not just config, but fully manages the driver lifecycle.
     Actually, the "driver manager" is a part of this config.
-    Here's how you can build a driver with the instance of this config:
 
-    >>> from selene import Config
-    >>> config = Config()
-    >>> driver = config.driver  # new instance, built on 1st access to `driver`
-    >>> assert driver.name == 'chrome'
-
-    Or pre-configuring the firefox driver:
-
-    >>> from selene import Config
-    >>> config = Config(driver_name='firefox')
-    >>> driver = config.driver
-    >>> assert driver.name == 'firefox'
-
-    Or post-configuring the firefox driver:
-
-    >>> from selene import Config
-    >>> config = Config()
-    >>> config.driver_name = 'firefox'
-    >>> driver = config.driver
-    >>> assert driver.name == 'firefox'
-
-    Selene has already predefined shared instance of Config,
-    so you can economize on lines of code;)...
-
-    >>> from selene.support.shared import config
-    >>> config.driver_name = 'firefox'
-    >>> driver = config.driver
-    >>> assert driver.name == 'firefox'
-
-    Same shared Config instance is available as browser.config:
-
-    >>> from selene import browser
-    >>> browser.config.driver_name = 'firefox'
-    >>> driver = browser.config.driver
-    >>> assert driver.name == 'firefox'
-
-    There is an alternative style of customizing config.
-    The `config.option_name = value` is known in programming
-    as "imperative programming" style. When you are creating
-    a new Config from scratch, you are actually using
-    a "declarative programming" style:
-
-    >>> from selene import Config
-    >>> my_config = Config(driver_name='firefox')
-    >>> driver = my_config.driver
-    >>> assert driver.name == 'firefox'
-
-    Here is an alternative declarative style of
-    customizing new config by copying existing:
-
-    >>> from selene import browser
-    >>> my_config = browser.config.with_(driver_name='firefox')
-    >>> driver = my_config.driver
-    >>> assert driver.name == 'firefox'
-    >>> # AND...
-    >>> assert driver is not browser.config.driver  # ;)
-    >>> assert browser.config.driver.name == 'chrome'
-
-    As you can see Selene config is closely related to the browser.
-    Moreover, the same type of "declarative config copying" happens implicitely,
-    when you apply "copying" to browser:
-
-    >>> from selene import browser
-    >>> second_browser = browser.with_(driver_name='firefox')
-    >>> assert second_browser.config.driver.name == 'firefox'
-    >>> # AND...
-    >>> assert second_browser.config.driver is not browser.config.driver  # ;)
-    >>> assert browser.config.driver.name == 'chrome'
-
-    Moreover, if you need only a driver, you can have it
-    via `browser.driver` shortcut, thus, completely hiding the config:
-
-    >>> from selene import browser
-    >>> second_browser = browser.with_(driver_name='firefox')
-    >>> assert second_browser.driver.name == 'firefox'
-    >>> # AND...
-    >>> assert second_browser.driver is not browser.driver  # ;)
-    >>> assert browser.driver.name == 'chrome'
-
-    – such shortcut exists only for the `driver` option of config,
-    not for other options like `timeout` or `base_url`.
-    More nuances of `browser` behavior find in its docs;).
+    While surfing through all avaialable options, pay attention to terminology:
+
+    - all options that have a `driver` word in their name
+      are related to driver management, and they are connected in a specific way:)
+      - read more on this under `config.with_` doc section;)
+    - all options that have a `strategy` word in their name directly influence
+      the driver lifecycle in context of driver management.
+    - all options that are prefixed with `_` are considered "experimental"
+        - their naming can be changed in the future, or even an option can be removed
 
     Examples:
+        Here's how you can build a driver with the instance of this config:
+
+        >>> from selene import Config
+        >>> config = Config()
+        >>> driver = config.driver  # new instance, built on 1st access to `driver`
+        >>> assert driver.name == 'chrome'
+
+        Or pre-configuring the firefox driver:
+
+        >>> from selene import Config
+        >>> config = Config(driver_name='firefox')
+        >>> driver = config.driver
+        >>> assert driver.name == 'firefox'
+
+        Or post-configuring the firefox driver:
+
+        >>> from selene import Config
+        >>> config = Config()
+        >>> config.driver_name = 'firefox'
+        >>> driver = config.driver
+        >>> assert driver.name == 'firefox'
+
+        Selene has already predefined shared instance of Config,
+        so you can economize on lines of code;)...
+
+        >>> from selene.support.shared import config
+        >>> config.driver_name = 'firefox'
+        >>> driver = config.driver
+        >>> assert driver.name == 'firefox'
+
+        Same shared Config instance is available as browser.config:
+
+        >>> from selene import browser
+        >>> browser.config.driver_name = 'firefox'
+        >>> driver = browser.config.driver
+        >>> assert driver.name == 'firefox'
+
+        There is an alternative style of customizing config.
+        The `config.option_name = value` is known in programming
+        as "imperative programming" style. When you are creating
+        a new Config from scratch, you are actually using
+        a "declarative programming" style:
+
+        >>> from selene import Config
+        >>> my_config = Config(driver_name='firefox')
+        >>> driver = my_config.driver
+        >>> assert driver.name == 'firefox'
+
+        Here is an alternative declarative style of
+        customizing new config by copying existing:
+
+        >>> from selene import browser
+        >>> my_config = browser.config.with_(driver_name='firefox')
+        >>> driver = my_config.driver
+        >>> assert driver.name == 'firefox'
+        >>> # AND...
+        >>> assert driver is not browser.config.driver  # ;)
+        >>> assert browser.config.driver.name == 'chrome'
+
+        As you can see Selene config is closely related to the browser.
+        Moreover, the same type of "declarative config copying" happens implicitely,
+        when you apply "copying" to browser:
+
+        >>> from selene import browser
+        >>> second_browser = browser.with_(driver_name='firefox')
+        >>> assert second_browser.config.driver.name == 'firefox'
+        >>> # AND...
+        >>> assert second_browser.config.driver is not browser.config.driver  # ;)
+        >>> assert browser.config.driver.name == 'chrome'
+
+        Moreover, if you need only a driver, you can have it
+        via `browser.driver` shortcut, thus, completely hiding the config:
+
+        >>> from selene import browser
+        >>> second_browser = browser.with_(driver_name='firefox')
+        >>> assert second_browser.driver.name == 'firefox'
+        >>> # AND...
+        >>> assert second_browser.driver is not browser.driver  # ;)
+        >>> assert browser.driver.name == 'chrome'
+
+        - such shortcut exists only for the `driver` option of config,
+        not for other options like `timeout` or `base_url`.
+        More nuances of `browser` behavior find in its docs;).
+
         And here are some more examples of customizing config
         for common test automation use cases...
 
         Scenario: "Run locally in headless Chrome"
 
         >>> from selene import browser
         >>> from selenium import webdriver
@@ -607,19 +632,19 @@
         >>>     },
         >>> )
         >>> browser.config.driver_options = options
         >>> browser.config.driver_remote_url = 'http://hub.browserstack.com/wd/hub'
 
     By having config options that influences Selene behavior,
     like `config.timeout` and `config.base_url`,
-    – together with complete "driver management",
+    - together with complete "driver management",
     we definitely break SRP principle... In the name of Good:D. Kind of;).
 
     All this makes it far from being a simple options data class...
-    – yet kept as one «class for everything» to keep things easier to use,
+    - yet kept as one «class for everything» to keep things easier to use,
     especially taking into account some historical reasons of Selenes design,
     that was influenced a lot by the Selenide from Java world.
     As a result sometimes options are not consistent with each other,
     when we speak about different contexts of their usage.
     For example, this same config,
     once customized with `config.driver_options = UiAutomator2Options()`,
     will result in mobile driver built, but then all other web-related options,
@@ -654,17 +679,19 @@
     """
     A factory to build a driver instance based on this config instance.
     The driver built with this factory will be available via `config.driver`.
     Hence, you can't use `config.driver` directly inside this factory,
     because it may lead to recursion.
 
     The default factory builds:
-    * either a local driver by value specified in `config.driver_name`
-    * or remote driver by value specified in `config.driver_remote_url`.
-    * or mobile driver according to `config.driver_options` capabilities.
+
+    - either a local driver by value specified in `config.driver_name`
+    - or a local driver by browserName capability specified in `config.driver_options`
+    - or remote driver by value specified in `config.driver_remote_url`.
+    - or mobile driver according to `config.driver_options` capabilities.
     """
 
     # TODO: isn't this option too much?
     #       having it, we have to keep driver descriptor definition
     #       after this option definition,
     #       that is pretty tightly coupled...
     #       heh, but maybe we definitely have to keep it defined
@@ -674,41 +701,94 @@
     # Should we simplify things? Or keep it as is with get_driver?
     _schedule_driver_teardown_strategy: Callable[
         [Config, Callable[[], WebDriver]],
         typing.Union[None, typing.Any],
     ] = lambda config, get_driver: atexit.register(
         lambda: config._teardown_driver_strategy(config)(get_driver())
     )
+    """
+    Defines when drier will be teardown.
+    Is supposed to use config._teardown_driver_strategy under the hood.
+
+    By default, it's registered as an atexit handler.
+    """
 
     # TODO: since it's curried, shouldn't we rename it driver_teardown_strategy?
     _teardown_driver_strategy: Callable[
         [Config], Callable[[WebDriver], None]
     ] = lambda config: lambda driver: (
         driver.quit()
         if not config.hold_driver_at_exit
         and config._is_driver_set_strategy(driver)
         and config._is_driver_alive_strategy(driver)
         else None
     )
+    """
+    Defines how driver will be teardown.
+
+    By default it quits the driver if it's alive and not asked to be held at exit
+    via `config.hold_driver_at_exit`.
+    """
 
     # TODO: should we make it private so far?
     # TODO: shouldn't it be config-based?
     _is_driver_set_strategy: Callable[[Optional[WebDriver]], bool] = lambda driver: (
         driver is not ... and driver is not None
     )
+    """
+    Defines how to check if driver is set, and so defines how to "unset" or "reset" it.
+    """
 
     # TODO: should we make it private so far?
     _is_driver_alive_strategy: Callable[[WebDriver], bool] = lambda driver: (
         # on_error_return_false(lambda: driver.title is not None)
         (driver.service.process is not None and driver.service.process.poll() is None)
         if hasattr(driver, 'service')
         else on_error_return_false(lambda: driver.window_handles is not None)
     )
+    """
+    Defines the logic of checking driver for being alive.
+
+    Is supposed to be used in context of triggering automatic driver rebuild,
+    depending on context.
+    """
 
     driver_options: Optional[BaseOptions] = None
+    """
+    Individual browser options to be used on building a driver.
+
+    Examples:
+        Can be used instead of `config.driver_name` to tell Selene
+        which driver to build, e.g. just specifying
+
+        >>> from selene import browser
+        >>> from selenium import webdriver
+        >>>
+        >>> browser.config.driver_options = webdriver.FirefoxOptions()`
+
+        - will tell Selene to build a Firefox driver.
+
+        But usually you want something more specific,
+        like specifying to run a browser in headless more:
+
+        >>> from selene import browser
+        >>> from selenium import webdriver
+        >>>
+        >>> options = webdriver.ChromeOptions()
+        >>> options.add_argument('--headless')
+        >>> browser.config.driver_options = options
+    """
+
+    driver_service: Optional[Service] = None
+    """
+    Service instance for managing the starting and stopping of the driver.
+    Might be useful, for example, for customizing driver executable path,
+    if you want to use a custom driver executable instead of the one,
+    downloaded by Selene automatically via WDM.
+    """
 
     # Probably, more precise and technically correct name and signature would be:
     #     driver_remote_connection: Optional[Union[str, RemoteConnection]] = None
     # But we decided to keep it more simple and user-friendly
     # in context of the majority of use cases when we just need to pass a URL:
     # for appium and remote cases
     driver_remote_url: Optional[str] = None
@@ -719,27 +799,48 @@
     Also known as `command_executor`,
     when passing on init: `driver = remote.WebDriver(command_executor=HERE)`.
     Currently we name it and type hint as URL,
     but if you pass a RemoteConnection object,
     it will work same way as in Selenium WebDriver.
     """
 
+    # TODO: consider typing as Optional[Literal['chrome', 'firefox', 'edge', 'appium']]
     # TODO: consider setting to None or ... by default,
     #       and pick up by factory any installed browser in a system
-    driver_name: str = 'chrome'
+    driver_name: Optional[str] = None
     """
     A desired name of the driver to build by `config.build_driver_strategy`.
+
+    If not set (i.e. set to None, that is a current default value),
+    the 'chrome' driver will be used by default.
+
     It is ignored by default `config.build_driver_strategy`
     if `config.driver_remote_url` is set.
 
-    GIVEN set to any of: 'chrome', 'firefox', 'edge',
-    AND config.driver is left unset (default value is ...),
-    THEN default config.build_driver_strategy will automatically install drivers
-    AND build webdriver instance for you
-    AND this config will store the instance in config.driver
+    If you are going to provide your desired driver options
+    via `config.driver_options`,
+    then Selene will try to guess the corresponding driver name
+    based on the options you provided. I.e. no need to provide both:
+
+    ```python
+    config.driver_name = 'chrome'
+    config.driver_options = ChromeOptions()
+    ```
+
+    It's enough to provide only the options:
+
+    ```python
+    config.driver_options = ChromeOptions()
+    ```
+
+    GIVEN set to any of: 'chrome', 'firefox', 'edge',<br>
+    AND config.driver is left unset (default value is ...),<br>
+    THEN default config.build_driver_strategy will automatically install drivers<br>
+    AND build webdriver instance for you<br>
+    AND this config will store the instance in config.driver<br>
     """
 
     # TODO: finalize the name of this option and consider making public
     _override_driver_with_all_driver_like_options: bool = True
     """
     Controls whether driver will be deep copied
     with `config.driver_name`, `config.driver_remote_url`,
@@ -797,15 +898,15 @@
         >>> firefox_config = chrome_config.with_(name='firefox')
         >>> firefox = firefox_config.driver
         >>> assert firefox is chrome  # o_O ;)
     """
 
     # TODO: consider to deprecate because might confuse in case of Appium usage
     @property
-    def browser_name(self) -> str:
+    def browser_name(self) -> Optional[str]:
         return self.driver_name
 
     # TODO: consider to deprecate because might confuse in case of Appium usage
     @browser_name.setter
     def browser_name(self, value: str):
         self.driver_name = value
 
@@ -848,14 +949,20 @@
     #       or should we implement same "decorator-like" style
     #       for other config-based strategies too?
     # TODO: refactor to inline definition with lambda style
     _driver_get_url_strategy: Callable[
         [Config],
         Callable[[Optional[str]], None],
     ] = _maybe_reset_driver_then_tune_window_and_get_with_base_url
+    """
+    Defines how to get url with driver depending on other options, like config.base_url.
+
+    Is used inside `browser.open(relative_or_absolute_url)`,
+    and defines its behavior correspondingly.
+    """
 
     # TODO: should we use `rebuild` term instead of `reset`?
     #       to be consistent with `rebuild_not_alive_driver`...
     #       Technically, we are not explicitely rebuilding it with this option,
     #       we do reset it by setting to `...`. But then in same `get_url`,
     #       on first access it will be rebuilt automatically.
     _reset_not_alive_driver_on_get_url: bool = True
@@ -918,107 +1025,242 @@
     #       But since we have another object named as _managed_driver,
     #       it might be confusing... so maybe DriverManagerDescriptor?
     #       or DriverLifeCycleDescriptor?
     #       or is it ok to have similar names? We still have a Descriptor suffix...
     driver: WebDriver = _ManagedDriverDescriptor(default=...)  # type: ignore
     """
     A driver instance with lifecycle managed by this config special options
-    (TODO: specify these options...),
     depending on their values and customization of this attribute.
 
-    GIVEN unset, i.e. equals to default `...` or `None`,
-    WHEN accessed first time (e.g. via config.driver)
-    THEN it will be set to the instance built by `config.build_driver_strategy`.
-
-    GIVEN set manually to an existing driver instance,
-          like: `config.driver = Chrome()`
-    THEN it will be reused as it is on any next access
-    WHEN reset to `...` OR `None`
-    THEN will be rebuilt by `config.build_driver_strategy`
-
-    GIVEN set manually to an existing driver instance (not callable),
-          like: `config.driver = Chrome()`
-    AND at some point of time the driver is not alive
-        like crashed or quit
-    AND `config._reset_not_alive_driver_on_get_url` is set to `True`,
-        that is default
-    WHEN driver.get(url) is requested under the hood
-         like at `browser.open(url)`
-    THEN config.driver will be reset to `...`
-    AND thus will be rebuilt by `config.build_driver_strategy`
-
-    GIVEN set manually to a callable that returns WebDriver instance
-          (currently marked with FutureWarning, so might be deprecated)
-    WHEN accessed fist time
-    AND any next time
-    THEN will call the callable and return the result
-
-    GIVEN unset or set manually to not callable
-    AND `config.hold_driver_at_exit` is set to `False` (that is default)
-    WHEN the process exits
-    THEN driver will be quit.
+    Once driver-definition-related options are set
+    (like `config.driver_options`, `config.driver_remote_url`),
+    the driver will be built on first access to this attribute.
+    Thus, to build the driver with Selene,
+    you simply call `config.driver` for the first time,
+    and usually the simplest way to access it
+    - is through either `browser.config.driver` or even `browser.driver` shortcut.
+    Moreover, usually you don't do this explicitly,
+    but rather use `browser.open(url)` to build a driver and open a page.
+
+    Scenarios:
+        GIVEN unset, i.e. equals to default `...` or `None`,<br>
+        WHEN accessed first time (e.g. via config.driver)<br>
+        THEN it will be set to the instance built by `config.build_driver_strategy`.<br>
+
+        GIVEN set manually to an existing driver instance,
+              like: `config.driver = Chrome()`<br>
+        THEN it will be reused as it is on any next access<br>
+        WHEN reset to `...` OR `None`<br>
+        THEN will be rebuilt by `config.build_driver_strategy`<br>
+
+        GIVEN set manually to an existing driver instance (not callable),
+              like: `config.driver = Chrome()`<br>
+        AND at some point of time the driver is not alive
+            like crashed or quit<br>
+        AND `config._reset_not_alive_driver_on_get_url` is set to `True`,
+            that is default<br>
+        WHEN driver.get(url) is requested under the hood
+             like at `browser.open(url)`<br>
+        THEN config.driver will be reset to `...`<br>
+        AND thus will be rebuilt by `config.build_driver_strategy`<br>
+
+        GIVEN set manually to a callable that returns WebDriver instance
+              (currently marked with FutureWarning, so might be deprecated)<br>
+        WHEN accessed fist time<br>
+        AND any next time<br>
+        THEN will call the callable and return the result<br>
+
+        GIVEN unset or set manually to not callable<br>
+        AND `config.hold_driver_at_exit` is set to `False` (that is default)<br>
+        WHEN the process exits<br>
+        THEN driver will be quit.<br>
     """
 
     timeout: float = 4
+    """
+    A default timeout for all Selene waiting that happens under the hood
+    of the majority of Selene commands and assertions.
+    """
+
     poll_during_waits: int = 100
     """
     A fake option, not currently used in Selene waiting:)
     """
 
     # --- Web-specific options ---
     # TODO: should we pass here None?
     #       and use "not None" as _get_base_url_on_open_with_no_args=True?
     # TODO: should we rename it to app_url? or even just app?
     #       and use it as app capability for mobile?
     #       if not set in driver_options...
     base_url: str = ''
+    """
+    A base url to be used when opening a page with relative url.
+
+    Examples:
+        Instead of duplicating the same base url in all your tests:
+
+        >>> from selene import browser
+        >>> browser.open('https://mywebapp.xyz/signin')
+        >>> ...
+        >>> browser.open('https://mywebapp.xyz/signup')
+        >>> ...
+        >>> browser.open('https://mywebapp.xyz/profile')
+        >>> ...
+
+        You can set it once in your config and then just use relative urls:
+
+        >>> from selene import browser
+        >>> browser.config.base_url = 'https://mywebapp.xyz'
+        >>> browser.open('/signin')
+        >>> ...
+        >>> browser.open('/signup')
+        >>> ...
+        >>> browser.open('/profile')
+        >>> ...
+    """
     # TODO: when adding driver_get_url_strategy
     #       should we rename it to get_base_url_when_relative_url_is_missed?
     #       should we use driver term in the name?
     _get_base_url_on_open_with_no_args: bool = False
+    """
+    A flag to indicate whether to use `config.base_url`
+    when opening a page with `browser.open()` command without arguments.
+
+    If you call `browser.open()` without arguments,
+    it will just force the driver to be built and real browser to be opened.
+
+    Even if you have set `config.base_url`, to reuse it in your tests on `browser.open`,
+    you have to specify the url explicitly, like `browser.open('/')`
+    or at least `browser.open('')`.
+
+    But there are cases where you would like to load base url on `browser.open()`,
+    for example in context of cross-platform testing. Then you use this option;)
+    See example at
+    https://github.com/yashaka/selene/blob/master/examples/run_cross_platform
+    """
     window_width: Optional[int] = None
+    """
+    If set, will be used to set the window width on next call to `browser.open(url)`.
+    """
     window_height: Optional[int] = None
+    """
+    If set, will be used to set the window height on next call to `browser.open(url)`.
+    """
     log_outer_html_on_failure: bool = False
+    """
+    If set to True, will log outer html of the element on failure of any Selene command.
+
+    Is disabled by default, because:
+
+    - it might add too much of noise to the logs
+    - will not work on mobile app tests because under the hood - uses JavaScript
+    """
     set_value_by_js: bool = False
+    """
+    A flag to indicate whether to use JavaScript to set value of an element
+    on `element.set_value(value)` for purposes of speeding up the test execution,
+    or as a workaround when default selenium-based implementation does not work.
+    """
     type_by_js: bool = False
+    """
+    A flag to indicate whether to use JavaScript to type text to an element
+    on `element.type(text)` for purposes of speeding up the test execution,
+    or as a workaround when default selenium-based implementation does not work.
+    """
     click_by_js: bool = False
+    """
+    A flag to indicate whether to use JavaScript to click on element
+    via `element.click()`, usually, as a workaround,
+    when default selenium-based implementation does not work.
+    """
     wait_for_no_overlap_found_by_js: bool = False
+    """
+    A flag to indicate whether to use JavaScript to detect overlapping elements
+    and wait for them to disappear, when calling commands like `element.type(text)`.
+    It is needed because Selenium does not support overlapping elements detection
+    on any command except `click`. Hence, when you call `click` on an element,
+    and there is some overlay on top of it
+    (e.g. for the sake of indicating "loading in progress"),
+    that is going to disappear after some time,
+    then Selenium will detect such overlap,
+    that tells Selene to wait for it to disappear.
+    But for any other command (double_click, context_click, type, etc.)
+    Selenium will not and so Selene will not wait.
+    Hence, if you want to wait in such cases, turn on this option.
+    Just keep in mind, that it will work only for web tests, not mobile.
+    """
 
     # TODO: better name? now technically it's not a decorator but decorator_builder...
     # or decorator_factory...
     # yet in python they call it just «decorator with args» or «decorator with params»
     # so technically we are correct naming it simply _wait_decorator
     # by type hint end users yet will see the real signature
     # and hence guess its «builder-like» nature
     # yet... should we for verbosity distinguish options
     # that a decorator factories from options that are simple decorators?
     # maybe better time to decide on this will be once we have more such options :p
     _wait_decorator: Callable[[Wait[E]], Callable[[F], F]] = lambda w: lambda f: f
+    """
+    Is used when performing any element command and assertion (i.e. should)
+    Hence, can be used to log corresponding commands with waits,
+    and integrate with something like allure reporting;)
+
+    Yet prefixed with underscore, indicating that method is experimental,
+    and so can be renamed or change its type signature, etc.
+
+    The default value of this option just does nothing.
+
+    See example of implementing and setting a custom wait decorator
+    at https://github.com/yashaka/selene/blob/master/examples/log_all_selene_commands_with_wait.py
+
+    Examples:
+        And here is how you can use some predefined wait decorators in Selene,
+        for example, to configure logging Selene commands to Allure report:
+
+        >>> from selene.support.shared import browser
+        >>> from selene import support
+        >>> import allure_commons
+        >>>
+        >>> browser.config._wait_decorator = support._logging.wait_with(
+        >>>   context=allure_commons._allure.StepContext
+        >>> )
+    """
 
+    # TODO: why we name it as hook_* why not handle_* ?
+    #       what would be proper style?
     hook_wait_failure: Optional[Callable[[TimeoutException], Exception]] = None
     '''
     A handler for all exceptions, thrown on failed waiting for timeout.
     Should process the original exception and rethrow it or the modified one.
-
-    TODO: why we name it as hook_* why not handle_* ?
-          what would be proper style?
     '''
 
     reports_folder: str = os.path.join(
         os.path.expanduser('~'),
         '.selene',
         'screenshots',
         str(round(time.time() * 1000)),
     )
+    """
+    A folder to save screenshots and page sources on failure.
+    """
     save_screenshot_on_failure: bool = True
+    """
+    A flag to indicate whether to save screenshot on failure or not.
+    If saved, will be also logged to the console on failure.
+    """
     save_page_source_on_failure: bool = True
+    """
+    A flag to indicate whether to save page source on failure or not.
+    If saved, will be also logged to the console on failure.
+    """
     # TODO: consider making public
     _counter: itertools.count = itertools.count(start=int(round(time.time() * 1000)))
     """
-    A counter, currently used for incrementing screenshot names
+    A counter, currently used for incrementing screenshot and page source names
     """
     last_screenshot: Optional[str] = None
     last_page_source: Optional[str] = None
     # TODO: is a _strategy suffix a good naming convention in this context?
     #       maybe yes, because we yet accept config in it...
     #       so we expect it to be a Strategy of some bigger Context
     _save_screenshot_strategy: Callable[
@@ -1058,14 +1300,20 @@
         fp.do(
             lambda path: setattr(config, 'last_screenshot', path)
         ),  # On refactor>rename, we may miss it here :( better would be like:
         #  setattr(config, config.__class__.last_screenshot.name, path)
         #  but currently .name will return '__boxed_last_screenshot' :(
         #  think on how we can resolve this...
     )
+    """
+    Defines a strategy for saving a screenshot.
+
+    The default strategy saves a screenshot to a file,
+    and stores the path to `config.last_screenshot`.
+    """
 
     _save_page_source_strategy: Callable[
         [Config, Optional[str]], Any
     ] = lambda config, path=None: fp.thread(
         path,
         lambda path: (
             config._generate_filename(suffix='.html') if path is None else path
@@ -1102,21 +1350,36 @@
         fp.do(
             lambda path: setattr(config, 'last_page_source', path)
         ),  # On refactor>rename, we may miss it here :( better would be like:
         #  setattr(config, config.__class__.last_screenshot.name, path)
         #  but currently .name will return '__boxed_last_screenshot' :(
         #  think on how we can resolve this...
     )
+    """
+    Defines a strategy for saving a page source on failure.
+
+    The default strategy saves a page_source to a file,
+    and stores the path to `config.last_page_source`.
+    """
 
     # TODO: consider adding option to disable persistence of all not-overridden options
     #       or marking some of them as not persistent
     #       (i.e. unbind some of them keeping the previous value set)
     def with_(self, **options_to_override) -> Config:
         """
 
+        Returns:
+            A new config with overridden options that were specified as arguments.
+
+                All other config options will be shallow-copied
+                from the current config.
+                Those other options that are of immutable types,
+                like `int` - will be also copied by reference,
+                i.e. in a truly shallow way.
+
         Parameters:
             **options_to_override:
                 options to override in the new config.
 
                 Technically "override" here means:
                 "deep copy option storage and update its value to the specified one".
                 All other option storages will be:
@@ -1127,32 +1390,27 @@
                 and `self._override_driver_with_all_driver_like_options` is True,
                 then `driver` will be implicitly added to the options to override,
                 i.e. `with_(driver_name='firefox')` will be equivalent
                 to `with_(driver_name='firefox', driver=...)`.
                 The latter gives a readable and concise shortcut
                 to spawn more than one browser:
 
-                >>> config = Config(timeout=10.0, base_url='https://autotest.how')
-                >>> chrome = config.driver  # chrome is default browser
-                >>> firefox_config = config.with_(driver_name='firefox')
-                >>> firefox = firefox_config.driver
-                >>> edge_config = config.with_(driver_name='edge')
-                >>> edge = edge_config.driver
+                ```python
+                from selene import Config
+
+                config = Config(timeout=10.0, base_url='https://autotest.how')
+                chrome = config.driver  # chrome is default browser
+                firefox_config = config.with_(driver_name='firefox')
+                firefox = firefox_config.driver
+                edge_config = config.with_(driver_name='edge')
+                edge = edge_config.driver
+                ```
 
                 Same logic applies to `remote_url`,
                 and all other config.*driver* options.
-
-        Returns:
-            a new config with overridden options that were specified as arguments.
-
-            All other config options will be shallow-copied
-            from the current config.
-            Those other options that are of immutable types,
-            like `int` – will be also copied by reference,
-            i.e. in a truly shallow way.
         """
         options = (
             {'driver': ..., **options_to_override}
             if (
                 self._override_driver_with_all_driver_like_options
                 and 'driver' not in options_to_override
                 and any('driver' in key for key in options_to_override)
@@ -1213,14 +1471,18 @@
         entity,
         at_most=config.timeout,
         or_fail_with=config._inject_screenshot_and_page_source_pre_hooks(
             config.hook_wait_failure
         ),
         _decorator=config._wait_decorator,
     )
+    """
+    A strategy for building a Wait object based on other config options
+    like `config.timeout`, `config.hook_wait_failure`, `config._wait_decorator`, etc.
+    """
 
     # TODO: we definitely not need it inside something called Config,
     #       especially "base interface like config
     #       consider refactor to wait_factory as configurable config property
     # TODO: should we move it config._executor.wait(entity) ?
     def wait(self, entity: E) -> Wait[E]:
         return self._build_wait_strategy(self)(entity)
```

### Comparing `selene-2.0.0rc1/selene/core/configuration.pyi` & `selene-2.0.0rc2/selene/core/configuration.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import itertools
 from typing import Callable, Optional, Any, Union
 
 from selenium.webdriver.common.options import BaseOptions
+from selenium.webdriver.common.service import Service
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from selene.common.fp import F
 from selene.core.wait import Wait, E
 
 class _DriverStrategiesExecutor:
     def __init__(self, config: Config): ...
@@ -48,16 +49,17 @@
 
 class Config:
     """
     all options prefixed with _ are so marked as experimental and may change in future
     """
 
     # Options to customize default driver lifecycle
-    driver_name: str = 'chrome'
+    driver_name: Optional[str] = None
     driver_options: Optional[BaseOptions] = None
+    driver_service: Optional[Service] = None
     driver_remote_url: Optional[str] = None
     hold_driver_at_exit: bool = False
     _reset_not_alive_driver_on_get_url: bool = True
     rebuild_not_alive_driver: bool = False
     _driver_get_url_strategy: Callable[[Config], Callable[[Optional[str]], None]] = ...
     # Options to customize driver management
     build_driver_strategy: Callable[[Config], WebDriver] = ...
@@ -98,16 +100,17 @@
     _build_wait_strategy: Callable[[Config], Callable[[E], Wait[E]]] = ...
     _executor: _DriverStrategiesExecutor = ...
 
     def __init__(
         self,
         *,
         # Options to customize default driver lifecycle
-        driver_name: str = 'chrome',
+        driver_name: Optional[str] = None,
         driver_options: Optional[BaseOptions] = None,
+        driver_service: Optional[Service] = None,
         driver_remote_url: Optional[str] = None,
         hold_driver_at_exit: bool = False,
         _reset_not_alive_driver_on_get_url: bool = True,
         rebuild_not_alive_driver: bool = False,
         _driver_get_url_strategy: Callable[
             [Config], Callable[[Optional[str]], None]
         ] = ...,
@@ -149,16 +152,17 @@
         # Etc.
         _build_wait_strategy: Callable[[Config], Callable[[E], Wait[E]]] = ...,
     ): ...
     def with_(
         self,
         *,
         # Options to customize default driver lifecycle
-        driver_name: str = 'chrome',
+        driver_name: Optional[str] = None,
         driver_options: Optional[BaseOptions] = None,
+        driver_service: Optional[Service] = None,
         driver_remote_url: Optional[str] = None,
         hold_driver_at_exit: bool = False,
         _reset_not_alive_driver_on_get_url: bool = True,
         rebuild_not_alive_driver: bool = False,
         _driver_get_url_strategy: Callable[
             [Config], Callable[[Optional[str]], None]
         ] = ...,
```

### Comparing `selene-2.0.0rc1/selene/core/entity.py` & `selene-2.0.0rc2/selene/core/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,15 +463,16 @@
         )
 
         return self
 
     def send_keys(self, *value) -> Element:
         """
         To be used for more low level operations like «uploading files», etc.
-        To simulate normal input of keys by user when typing – use Element.type(self, text).
+        To simulate normal input of keys by user when typing
+        - use Element.type(self, text).
         """
         self.wait.command('send keys', lambda element: element().send_keys(*value))
         return self
 
     def press(self, *keys) -> Element:
         def fn(element: Element):
             webelement = (
```

### Comparing `selene-2.0.0rc1/selene/core/entity.pyi` & `selene-2.0.0rc2/selene/core/entity.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import itertools
 import typing
 from abc import ABC, abstractmethod
 
 from selenium.webdriver.common.options import BaseOptions
+from selenium.webdriver.common.service import Service
 
 from selene.common.fp import pipe as pipe, F
 from selene.common.helpers import (
     flatten as flatten,
     is_absolute_url as is_absolute_url,
     to_by as to_by,
 )
@@ -203,14 +204,15 @@
     def with_(
         self,
         config: Optional[Config] = None,
         *,
         # Options to customize default driver lifecycle
         driver_name: str = 'chrome',
         driver_options: Optional[BaseOptions] = None,
+        driver_service: Optional[Service] = None,
         driver_remote_url: Optional[str] = None,
         hold_driver_at_exit: bool = False,
         _reset_not_alive_driver_on_get_url: bool = True,
         rebuild_not_alive_driver: bool = False,
         _driver_get_url_strategy: Callable[
             [Config], Callable[[Optional[str]], None]
         ] = ...,
```

### Comparing `selene-2.0.0rc1/selene/core/exceptions.py` & `selene-2.0.0rc2/selene/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/locator.py` & `selene-2.0.0rc2/selene/core/locator.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/match.py` & `selene-2.0.0rc2/selene/core/match.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/query.py` & `selene-2.0.0rc2/selene/core/query.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/core/wait.py` & `selene-2.0.0rc2/selene/core/wait.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/_logging.py` & `selene-2.0.0rc2/selene/support/_logging.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/by.py` & `selene-2.0.0rc2/selene/support/by.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/conditions/be.py` & `selene-2.0.0rc2/selene/support/conditions/be.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/conditions/have.py` & `selene-2.0.0rc2/selene/support/conditions/have.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/conditions/not_.py` & `selene-2.0.0rc2/selene/support/conditions/not_.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/shared/__init__.py` & `selene-2.0.0rc2/selene/support/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/shared/browser.py` & `selene-2.0.0rc2/selene/support/shared/browser.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/shared/config.py` & `selene-2.0.0rc2/selene/support/shared/config.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/shared/jquery_style.py` & `selene-2.0.0rc2/selene/support/shared/jquery_style.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/selene/support/webdriver.py` & `selene-2.0.0rc2/selene/support/webdriver.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc1/PKG-INFO` & `selene-2.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selene
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: User-oriented browser tests in Python (Selenide port)
 Home-page: https://yashaka.github.io/selene/
 License: MIT
 Keywords: testing,selenium,selenide,browser,pageobject,widget,wrapper
 Author: Iakiv Kramarenko
 Author-email: yashaka@gmail.com
 Requires-Python: >=3.7,<4.0
```

