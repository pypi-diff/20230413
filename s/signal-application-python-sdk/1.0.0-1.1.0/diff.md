# Comparing `tmp/signal-application-python-sdk-1.0.0.tar.gz` & `tmp/signal-application-python-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-application-python-sdk-1.0.0.tar", last modified: Mon Nov 28 14:08:19 2022, max compression
+gzip compressed data, was "signal-application-python-sdk-1.1.0.tar", last modified: Thu Apr 13 18:15:51 2023, max compression
```

## Comparing `signal-application-python-sdk-1.0.0.tar` & `signal-application-python-sdk-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 14:08:18.996638 signal-application-python-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 14:08:18.996638 signal-application-python-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 14:08:18.996638 signal-application-python-sdk-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1719 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 14:08:18.996638 signal-application-python-sdk-1.0.0/signal_application_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 14:08:18.000000 signal-application-python-sdk-1.0.0/signal_application_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      457 2022-11-28 14:08:18.000000 signal-application-python-sdk-1.0.0/signal_application_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 14:08:18.000000 signal-application-python-sdk-1.0.0/signal_application_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2022-11-28 14:08:18.000000 signal-application-python-sdk-1.0.0/signal_application_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-11-28 14:08:18.000000 signal-application-python-sdk-1.0.0/signal_application_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 14:08:18.996638 signal-application-python-sdk-1.0.0/signalsdk/
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/signalsdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/signalsdk/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      291 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/signalsdk/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4913 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/signalsdk/local_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (122)     8058 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/signalsdk/signal_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/signalsdk/signal_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      452 2022-11-28 14:07:20.000000 signal-application-python-sdk-1.0.0/signalsdk/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:51.747072 signal-application-python-sdk-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-13 18:15:51.747072 signal-application-python-sdk-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:15:51.747072 signal-application-python-sdk-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:51.743072 signal-application-python-sdk-1.1.0/signal_application_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-13 18:15:51.000000 signal-application-python-sdk-1.1.0/signal_application_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-13 18:15:51.000000 signal-application-python-sdk-1.1.0/signal_application_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:15:51.000000 signal-application-python-sdk-1.1.0/signal_application_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 18:15:51.000000 signal-application-python-sdk-1.1.0/signal_application_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 18:15:51.000000 signal-application-python-sdk-1.1.0/signal_application_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:51.747072 signal-application-python-sdk-1.1.0/signalsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/signalsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/signalsdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/signalsdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/signalsdk/local_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/signalsdk/signal_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/signalsdk/signal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/signalsdk/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:15:51.747072 signal-application-python-sdk-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/tests/test_local_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-04-13 18:15:22.000000 signal-application-python-sdk-1.1.0/tests/test_signal_app.py
```

### Comparing `signal-application-python-sdk-1.0.0/PKG-INFO` & `signal-application-python-sdk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-application-python-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: signal application services
 Author: Wesley Clover
 Author-email: burak.cakmak@wesleyclover.com
 Description-Content-Type: text/markdown
 
 # signal-application-python-sdk
```

### Comparing `signal-application-python-sdk-1.0.0/README.md` & `signal-application-python-sdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-1.0.0/setup.py` & `signal-application-python-sdk-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from os import path
 from setuptools import setup
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as file:
```

### Comparing `signal-application-python-sdk-1.0.0/signal_application_python_sdk.egg-info/PKG-INFO` & `signal-application-python-sdk-1.1.0/signal_application_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-application-python-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: signal application services
 Author: Wesley Clover
 Author-email: burak.cakmak@wesleyclover.com
 Description-Content-Type: text/markdown
 
 # signal-application-python-sdk
```

### Comparing `signal-application-python-sdk-1.0.0/signalsdk/__init__.py` & `signal-application-python-sdk-1.1.0/signalsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-1.0.0/signalsdk/api.py` & `signal-application-python-sdk-1.1.0/signalsdk/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,29 +4,16 @@
 """
 
 import os
 import logging
 import requests
 from signalsdk.signal_exception import SignalAppLocalHttpServerError
 
-API_THING_CONFIG_URL = "http://localhost:{}/api/thing"
 API_APPS_CONFIG_URL = "http://localhost:{}/api/apps"
 
-"""
-# Path: signalsdk/api.py
-# Get app base config from local api server
-# including thing name, account id etc.
-# param: port: local api server port
-# return: app base config dict
-# exception: None
-# """
-def get_local_device_config_api(port=5000):
-    """get thing configuration from local HTTP server
-    """
-    return local_http_api(API_THING_CONFIG_URL, port=port)
 
 def get_app_config_api(appId, port=5000):
     """get app configuration from local HTTP server
     """
     return local_http_api(API_APPS_CONFIG_URL, \
                           query_param={"applicationId": appId}, port=port)
```

### Comparing `signal-application-python-sdk-1.0.0/signalsdk/local_mqtt.py` & `signal-application-python-sdk-1.1.0/signalsdk/local_mqtt.py`

 * *Files identical despite different names*

### Comparing `signal-application-python-sdk-1.0.0/signalsdk/signal_app.py` & `signal-application-python-sdk-1.1.0/signalsdk/signal_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import os
 import logging
 from typing import Callable
 from signalsdk.local_mqtt import LocalMqtt
-from signalsdk.api import get_app_config_api, get_local_device_config_api
+from signalsdk.api import get_app_config_api
 from signalsdk.config import LOCALMQTT_SDK_TOPIC_PREFIX, LOCALMQTT_SDK_APPLICATION_CONFIG_TOPIC
 from signalsdk.signal_exception import SignalAppLocalMqttEventCallBackError, \
-    SignalAppConfigEnvError, SignalAppLocalHttpServerError, \
+    SignalAppConfigEnvError, \
         SignalAppOnConfigChangedCallBackError
 
 from .validator import throw_if_parameter_not_found_in
 
 OnConfigurationChangeRequested=Callable[[dict], None]
 OnEventReceived=Callable[[str], None]
 
 class SignalApp:
     def __init__(self):
         self.localMqtt = None
-        self.baseConfig = {}
         self.app_id = ""
-        self.thing_name = ""
         self.account_id = ""
         self.configurationChangedCallback = None
         self.onEventReceivedCallback = None
         self.local_pub_topic = None
 
     def __get_application_config(self):
         appSettings = get_app_config_api(self.app_id)
@@ -111,28 +109,19 @@
         signal application for configuration change
         :param onEventReceivedCallback: call back function provided by signal
         application for events handling
         """
         logging.info(f"{__name__}: signalsdk::Starting signal app initialize.")
         self.configurationChangedCallback = onConfiguratioChangedCallback
         self.onEventReceivedCallback = onEventReceivedCallback
-        self.baseConfig = get_local_device_config_api()
-        throw_if_parameter_not_found_in(self.baseConfig, 'device config', \
-                                        'local http server', SignalAppLocalHttpServerError)
-        self.thing_name = self.baseConfig['thingName']
-        throw_if_parameter_not_found_in(self.thing_name, 'thing name', \
-                                        'local http server', SignalAppLocalHttpServerError)
-        self.account_id = self.baseConfig['accountId']
-        throw_if_parameter_not_found_in(self.account_id, 'account id', \
-                                        'local http server', SignalAppLocalHttpServerError)
         self.app_id = os.getenv('APPLICATION_ID')
         throw_if_parameter_not_found_in(self.app_id, 'application id', \
                                         'environment variables', SignalAppConfigEnvError)
         #generate local mqtt client id
-        local_mqtt_client_id = self.thing_name + "_" + self.app_id
+        local_mqtt_client_id = "edgesignaSdk_" + self.app_id
         self.localMqtt = LocalMqtt(local_mqtt_client_id)
         self.localMqtt.set_on_connected(self.__start_listening_app_config_updates)
         self.localMqtt.connect()
 
     def next(self, event, next_app_id=''):
         """Publish the event
         :param event: event received on local event bus
```

### Comparing `signal-application-python-sdk-1.0.0/signalsdk/signal_exception.py` & `signal-application-python-sdk-1.1.0/signalsdk/signal_exception.py`

 * *Files identical despite different names*

