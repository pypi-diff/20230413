# Comparing `tmp/etradebot-1.0.0.tar.gz` & `tmp/etradebot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etradebot-1.0.0.tar", last modified: Thu Apr 13 01:39:43 2023, max compression
+gzip compressed data, was "etradebot-1.0.1.tar", last modified: Thu Apr 13 02:02:05 2023, max compression
```

## Comparing `etradebot-1.0.0.tar` & `etradebot-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:43.389000 etradebot-1.0.0/
--rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4986 2023-04-13 01:39:43.372000 etradebot-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4440 2023-04-12 20:42:58.000000 etradebot-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.320000 etradebot-1.0.0/authentication/
--rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.0/authentication/__init__.py
--rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.0/authentication/authentication.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.344000 etradebot-1.0.0/etrade/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/etrade/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.0/etrade/etrade.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.595000 etradebot-1.0.0/etradebot.egg-info/
--rw-rw-rw-   0        0        0     4986 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       46 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      267 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.625000 etradebot-1.0.0/execute/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/execute/__init__.py
--rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.0/execute/execute.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.670000 etradebot-1.0.0/model/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/model/__init__.py
--rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.0/model/investor_views.py
--rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.0/model/model.py
--rw-rw-rw-   0        0        0       42 2023-04-13 01:39:43.387000 etradebot-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1375 2023-04-13 01:38:52.000000 etradebot-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.716000 etradebot-1.0.0/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/strategies/__init__.py
--rw-rw-rw-   0        0        0     2961 2023-04-01 01:26:39.000000 etradebot-1.0.0/strategies/cape_strategy.py
--rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.0/strategies/example_strategy.py
--rw-rw-rw-   0        0        0     1192 2023-04-02 17:50:45.000000 etradebot-1.0.0/strategies/strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.880000 etradebot-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.0/tests/mock_responses.py
--rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.0/tests/test_authentication.py
--rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.0/tests/test_etrade.py
--rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.0/tests/test_execute.py
--rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.0/tests/test_model.py
--rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:39:43.008000 etradebot-1.0.0/utils/
--rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.0/utils/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-04-12 17:27:13.000000 etradebot-1.0.0/utils/credentials.py
--rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.0/utils/fake_data.py
--rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.0/utils/logging_config.py
--rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.0/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.654000 etradebot-1.0.1/
+-rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4799 2023-04-13 02:02:05.647000 etradebot-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4253 2023-04-13 02:00:43.000000 etradebot-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.154000 etradebot-1.0.1/authentication/
+-rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.1/authentication/__init__.py
+-rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.1/authentication/authentication.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.176000 etradebot-1.0.1/etrade/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/etrade/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.1/etrade/etrade.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.236000 etradebot-1.0.1/etradebot.egg-info/
+-rw-rw-rw-   0        0        0     4799 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       46 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       59 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.258000 etradebot-1.0.1/execute/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/execute/__init__.py
+-rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.1/execute/execute.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.293000 etradebot-1.0.1/model/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/model/__init__.py
+-rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.1/model/investor_views.py
+-rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.1/model/model.py
+-rw-rw-rw-   0        0        0       42 2023-04-13 02:02:05.652000 etradebot-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-04-13 02:00:43.000000 etradebot-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.343000 etradebot-1.0.1/strategies/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/strategies/__init__.py
+-rw-rw-rw-   0        0        0     2961 2023-04-01 01:26:39.000000 etradebot-1.0.1/strategies/cape_strategy.py
+-rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.1/strategies/example_strategy.py
+-rw-rw-rw-   0        0        0     1192 2023-04-02 17:50:45.000000 etradebot-1.0.1/strategies/strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.577000 etradebot-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.1/tests/mock_responses.py
+-rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.1/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.1/tests/test_etrade.py
+-rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.1/tests/test_execute.py
+-rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.1/tests/test_model.py
+-rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.637000 etradebot-1.0.1/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.1/utils/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-04-12 17:27:13.000000 etradebot-1.0.1/utils/credentials.py
+-rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.1/utils/fake_data.py
+-rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.1/utils/logging_config.py
+-rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.1/utils/portfolio.py
```

### Comparing `etradebot-1.0.0/LICENSE` & `etradebot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/PKG-INFO` & `etradebot-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etradebot
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python-based trading bot for the E-Trade platform
 Home-page: https://github.com/nathanramoscfa/etradebot
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,18 +17,18 @@
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
 -   Fetches real-time market data from E-Trade API used to execute trades
--   Executes trade types: buy, sell, sell short, and short cover trade types based on user-defined strategies
--   Submits price types: market orders to E-Trade API (limit, stop, and other order types will be added in future releases)
+-   Executes trade types: buy, sell, sell short, and short cover trade types
+-   Submits price type: market orders to E-Trade API
 -   Manages portfolio: tracks positions, balance, and performance
--   Trades: common stocks and ETFs (options, mutual funds, and other security types will be added in future releases)
+-   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
 1. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
 2. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
```

### Comparing `etradebot-1.0.0/README.md` & `etradebot-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
 -   Fetches real-time market data from E-Trade API used to execute trades
--   Executes trade types: buy, sell, sell short, and short cover trade types based on user-defined strategies
--   Submits price types: market orders to E-Trade API (limit, stop, and other order types will be added in future releases)
+-   Executes trade types: buy, sell, sell short, and short cover trade types
+-   Submits price type: market orders to E-Trade API
 -   Manages portfolio: tracks positions, balance, and performance
--   Trades: common stocks and ETFs (options, mutual funds, and other security types will be added in future releases)
+-   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
 1. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
 2. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
```

### Comparing `etradebot-1.0.0/authentication/authentication.py` & `etradebot-1.0.1/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/etrade/etrade.py` & `etradebot-1.0.1/etrade/etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/etradebot.egg-info/PKG-INFO` & `etradebot-1.0.1/etradebot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etradebot
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python-based trading bot for the E-Trade platform
 Home-page: https://github.com/nathanramoscfa/etradebot
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,18 +17,18 @@
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
 -   Fetches real-time market data from E-Trade API used to execute trades
--   Executes trade types: buy, sell, sell short, and short cover trade types based on user-defined strategies
--   Submits price types: market orders to E-Trade API (limit, stop, and other order types will be added in future releases)
+-   Executes trade types: buy, sell, sell short, and short cover trade types
+-   Submits price type: market orders to E-Trade API
 -   Manages portfolio: tracks positions, balance, and performance
--   Trades: common stocks and ETFs (options, mutual funds, and other security types will be added in future releases)
+-   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
 1. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
 2. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
```

### Comparing `etradebot-1.0.0/etradebot.egg-info/SOURCES.txt` & `etradebot-1.0.1/etradebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/execute/execute.py` & `etradebot-1.0.1/execute/execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/model/investor_views.py` & `etradebot-1.0.1/model/investor_views.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/model/model.py` & `etradebot-1.0.1/model/model.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/setup.py` & `etradebot-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='etradebot',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/nathanramoscfa/etradebot',
     license='MIT',
     author='Nathan Ramos, CFA®',
     author_email='info@nrcapitalmanagement.com',
     description='A Python-based trading bot for the E-Trade platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `etradebot-1.0.0/strategies/cape_strategy.py` & `etradebot-1.0.1/strategies/cape_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/strategies/example_strategy.py` & `etradebot-1.0.1/strategies/example_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/strategies/strategy.py` & `etradebot-1.0.1/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/tests/mock_responses.py` & `etradebot-1.0.1/tests/mock_responses.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/tests/test_authentication.py` & `etradebot-1.0.1/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/tests/test_etrade.py` & `etradebot-1.0.1/tests/test_etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/tests/test_execute.py` & `etradebot-1.0.1/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/tests/test_model.py` & `etradebot-1.0.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/utils/credentials.py` & `etradebot-1.0.1/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/utils/fake_data.py` & `etradebot-1.0.1/utils/fake_data.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/utils/logging_config.py` & `etradebot-1.0.1/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.0/utils/portfolio.py` & `etradebot-1.0.1/utils/portfolio.py`

 * *Files identical despite different names*

