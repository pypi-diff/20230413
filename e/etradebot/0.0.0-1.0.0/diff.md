# Comparing `tmp/etradebot-0.0.0.tar.gz` & `tmp/etradebot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etradebot-0.0.0.tar", last modified: Sat Apr  1 04:10:49 2023, max compression
+gzip compressed data, was "etradebot-1.0.0.tar", last modified: Thu Apr 13 01:39:43 2023, max compression
```

## Comparing `etradebot-0.0.0.tar` & `etradebot-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.773000 etradebot-0.0.0/
--rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     2290 2023-04-01 04:10:49.770000 etradebot-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-03-22 01:52:19.000000 etradebot-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.344000 etradebot-0.0.0/authentication/
--rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-0.0.0/authentication/__init__.py
--rw-rw-rw-   0        0        0     4691 2023-02-20 07:05:18.000000 etradebot-0.0.0/authentication/authentication.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.359000 etradebot-0.0.0/etrade/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-0.0.0/etrade/__init__.py
--rw-rw-rw-   0        0        0     9571 2023-03-18 07:05:42.000000 etradebot-0.0.0/etrade/etrade.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.621000 etradebot-0.0.0/etradebot.egg-info/
--rw-rw-rw-   0        0        0     2290 2023-04-01 04:10:49.000000 etradebot-0.0.0/etradebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-04-01 04:10:49.000000 etradebot-0.0.0/etradebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 04:10:49.000000 etradebot-0.0.0/etradebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2023-04-01 04:10:49.000000 etradebot-0.0.0/etradebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2023-04-01 04:10:49.000000 etradebot-0.0.0/etradebot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.671000 etradebot-0.0.0/execute/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-0.0.0/execute/__init__.py
--rw-rw-rw-   0        0        0    15484 2023-03-30 14:56:01.000000 etradebot-0.0.0/execute/execute.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.690000 etradebot-0.0.0/model/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-0.0.0/model/__init__.py
--rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-0.0.0/model/investor_views.py
--rw-rw-rw-   0        0        0    30707 2023-03-29 05:54:46.000000 etradebot-0.0.0/model/model.py
--rw-rw-rw-   0        0        0       42 2023-04-01 04:10:49.772000 etradebot-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-01 04:01:49.000000 etradebot-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.710000 etradebot-0.0.0/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-0.0.0/strategies/__init__.py
--rw-rw-rw-   0        0        0     2961 2023-04-01 01:26:39.000000 etradebot-0.0.0/strategies/cape_strategy.py
--rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-0.0.0/strategies/example_strategy.py
--rw-rw-rw-   0        0        0      883 2023-03-30 04:09:50.000000 etradebot-0.0.0/strategies/strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.749000 etradebot-0.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-0.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-0.0.0/tests/mock_responses.py
--rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-0.0.0/tests/test_authentication.py
--rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-0.0.0/tests/test_etrade.py
--rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-0.0.0/tests/test_execute.py
--rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-0.0.0/tests/test_model.py
--rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-0.0.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:10:49.766000 etradebot-0.0.0/utils/
--rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-0.0.0/utils/__init__.py
--rw-rw-rw-   0        0        0     2144 2023-02-18 22:48:29.000000 etradebot-0.0.0/utils/fake_data.py
--rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-0.0.0/utils/logging_config.py
--rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-0.0.0/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:43.389000 etradebot-1.0.0/
+-rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4986 2023-04-13 01:39:43.372000 etradebot-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4440 2023-04-12 20:42:58.000000 etradebot-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.320000 etradebot-1.0.0/authentication/
+-rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.0/authentication/__init__.py
+-rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.0/authentication/authentication.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.344000 etradebot-1.0.0/etrade/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/etrade/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.0/etrade/etrade.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.595000 etradebot-1.0.0/etradebot.egg-info/
+-rw-rw-rw-   0        0        0     4986 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       46 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       59 2023-04-13 01:39:42.000000 etradebot-1.0.0/etradebot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.625000 etradebot-1.0.0/execute/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/execute/__init__.py
+-rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.0/execute/execute.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.670000 etradebot-1.0.0/model/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/model/__init__.py
+-rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.0/model/investor_views.py
+-rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.0/model/model.py
+-rw-rw-rw-   0        0        0       42 2023-04-13 01:39:43.387000 etradebot-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-04-13 01:38:52.000000 etradebot-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.716000 etradebot-1.0.0/strategies/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.0/strategies/__init__.py
+-rw-rw-rw-   0        0        0     2961 2023-04-01 01:26:39.000000 etradebot-1.0.0/strategies/cape_strategy.py
+-rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.0/strategies/example_strategy.py
+-rw-rw-rw-   0        0        0     1192 2023-04-02 17:50:45.000000 etradebot-1.0.0/strategies/strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:42.880000 etradebot-1.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.0/tests/mock_responses.py
+-rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.0/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.0/tests/test_etrade.py
+-rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.0/tests/test_execute.py
+-rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.0/tests/test_model.py
+-rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 01:39:43.008000 etradebot-1.0.0/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.0/utils/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-04-12 17:27:13.000000 etradebot-1.0.0/utils/credentials.py
+-rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.0/utils/fake_data.py
+-rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.0/utils/logging_config.py
+-rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.0/utils/portfolio.py
```

### Comparing `etradebot-0.0.0/LICENSE` & `etradebot-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/authentication/authentication.py` & `etradebot-1.0.0/authentication/authentication.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,54 +48,100 @@
         self.dev = dev
         self.headless = headless
         self.browser = browser
         self.retries = retries
         self.sleep = sleep
 
     def get_oauth(self):
+        """
+        :description: Get OAuth object
+
+        :return: OAuth object
+        :rtype: pyetrade.ETradeOAuth
+        """
         return pyetrade.ETradeOAuth(
             self.sandbox_key if self.dev else self.consumer_key,
             self.sandbox_secret if self.dev else self.consumer_secret,
             self.web_username,
             self.web_password,
             self.etrade_cookie
         )
 
     @staticmethod
     def get_access_tokens(oauth, verifier_code):
+        """
+        :description: Get access tokens
+
+        :param oauth: OAuth object
+        :type oauth: pyetrade.ETradeOAuth
+        :param verifier_code: Verifier code
+        :type verifier_code: str
+        :return: Access tokens
+        :rtype: dict
+        """
         return oauth.get_access_token(verifier_code)
 
     def get_accounts_api(self, tokens):
+        """
+        :description: Get accounts API object
+
+        :param tokens: Access tokens
+        :type tokens: dict
+        :return: Accounts API object
+        :rtype: pyetrade.ETradeAccounts
+        """
         return pyetrade.ETradeAccounts(
             self.sandbox_key if self.dev else self.consumer_key,
             self.sandbox_secret if self.dev else self.consumer_secret,
             tokens['oauth_token'],
             tokens['oauth_token_secret'],
             self.dev
         )
 
     def get_orders_api(self, tokens):
+        """
+        :description: Get orders API object
+
+        :param tokens: Access tokens
+        :type tokens: dict
+        :return: Orders API object
+        :rtype: pyetrade.ETradeOrder
+        """
         return pyetrade.ETradeOrder(
             self.sandbox_key if self.dev else self.consumer_key,
             self.sandbox_secret if self.dev else self.consumer_secret,
             tokens['oauth_token'],
             tokens['oauth_token_secret'],
             self.dev
         )
 
     def get_market_api(self, tokens):
+        """
+        :description: Get market API object
+
+        :param tokens: Access tokens
+        :type tokens: dict
+        :return: Market API object
+        :rtype: pyetrade.ETradeMarket
+        """
         return pyetrade.ETradeMarket(
             self.sandbox_key if self.dev else self.consumer_key,
             self.sandbox_secret if self.dev else self.consumer_secret,
             tokens['oauth_token'],
             tokens['oauth_token_secret'],
             self.dev
         )
 
     def access_api(self):
+        """
+        :description: Access Etrade API
+
+        :return: Etrade API objects
+        :rtype: tuple
+        """
         oauth = self.get_oauth()
         verifier_code = oauth.get_verification_code(self.dev, self.headless, self.browser)
         tokens = self.get_access_tokens(oauth, verifier_code)
 
         return (
             self.get_accounts_api(tokens),
             self.get_orders_api(tokens),
```

### Comparing `etradebot-0.0.0/etrade/etrade.py` & `etradebot-1.0.0/etrade/etrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             sandbox_key, sandbox_secret, dev, headless, browser, retries, sleep
         )
         self.accounts, self.orders, self.market = self.auth.etrade_login()
         self.dev = dev
 
     def get_account_list(self, prints=False):
         """
-        Get a list of all accounts
+        :description: Get a list of all accounts
 
         :param prints: Print the accounts
         :type prints: bool
         :return: DataFrame of accounts
         :rtype: pandas.DataFrame
         """
         list_accounts = self.accounts.list_accounts(resp_format='json')
@@ -92,15 +92,15 @@
         if prints:
             print(df)
 
         return df
 
     def get_orders_list(self, account_id_key, prints=False):
         """
-        Get a list of all orders for a given account
+        :description: Get a list of all orders for a given account
 
         :param account_id_key: Account ID
         :type account_id_key: str
         :param prints: Print the orders
         :type prints: bool
         :return: DataFrame of orders
         :rtype: pandas.DataFrame
@@ -143,14 +143,24 @@
 
         if prints:
             print(df)
 
         return df
 
     def get_market_quote(self, symbols, prints=False):
+        """
+        :description: Get market quote for a list of symbols
+
+        :param symbols: List of symbols
+        :type symbols: list
+        :param prints: Print the quote
+        :type prints: bool
+        :return: DataFrame of quote
+        :rtype: pandas.DataFrame
+        """
         json_dict = self.market.get_quote(symbols, resp_format='json')
         quote_data = json_dict['QuoteResponse']['QuoteData']
         data = []
         headers = []
         for quote in quote_data:
             symbol = quote['Product']['symbol']
             headers.append(symbol)
@@ -197,15 +207,15 @@
             print('')
             print(f'Buying Power: ${buying_power:,.2f}')
 
         return float(buying_power)
 
     def get_portfolio_data(self, account_id_key, sort_by='totalGainPct', ascending=False):
         """
-        Get portfolio data
+        :description: Get portfolio data
 
         :param account_id_key: Account ID key
         :type account_id_key: str
         :param sort_by: Sort by column
         :type sort_by: str
         :param ascending: Sort ascending
         :type ascending: bool
```

### Comparing `etradebot-0.0.0/etradebot.egg-info/SOURCES.txt` & `etradebot-1.0.0/etradebot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 tests/mock_responses.py
 tests/test_authentication.py
 tests/test_etrade.py
 tests/test_execute.py
 tests/test_model.py
 tests/test_utils.py
 utils/__init__.py
+utils/credentials.py
 utils/fake_data.py
 utils/logging_config.py
 utils/portfolio.py
```

### Comparing `etradebot-0.0.0/execute/execute.py` & `etradebot-1.0.0/execute/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,29 @@
 import random
 import pandas as pd
 import xml.etree.ElementTree as ET
 from pypfopt import DiscreteAllocation
 
 
 class Execute:
+    """
+    :description: Execute trades
+
+    :param etrade: Etrade API object
+    :type etrade: pyetrade.ETradeAccounts, required
+    """
     def __init__(
             self, etrade
     ):
+        """
+        :description: Initialize class
+
+        :return: None
+        :rtype: None
+        """
         self.etrade = etrade
 
     def calculate_shares(
             self, weights, buying_power, reinvest=True, prints=False
     ):
         """
         :description: Calculate shares to buy or sell
@@ -61,26 +73,25 @@
         return shares_to_buy
 
     def generate_trades(
             self, account_id_key, symbol, order_action, quantity, price_type='MARKET', order_term='GOOD_FOR_DAY',
             market_session='REGULAR', preview=True, prints=False
     ):
         """
-        :description: Generate trades. If preview is True, trades will be previewed. If preview is False, trades will be
-        executed.
+        :description: Generate trades. If preview is True, trades will be previewed. If False, trades will be executed.
 
         :param account_id_key: Account ID key
         :type account_id_key: str, required
         :param symbol: Ticker
         :type symbol: str, required
         :param order_action: Order action
         :type order_action: str, required
         :param quantity: Quantity
         :type quantity: int, required
-        :param price_type: Price type, default is 'MARKET'
+        :param price_type: Price type, default is 'MARKET'.
         :type price_type: str, optional
         :param order_term: Order term, default is 'GOOD_FOR_DAY'
         :type order_term: str, optional
         :param market_session: Market session, default is 'REGULAR'
         :type market_session: str, optional
         :param preview: Preview trades, default is True. If False, trades will be executed.
         :type preview: bool, optional
```

### Comparing `etradebot-0.0.0/model/investor_views.py` & `etradebot-1.0.0/model/investor_views.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/model/model.py` & `etradebot-1.0.0/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,20 @@
             symbol[:-len(' US Equity')] if api_source == 'yahoo' and symbol.endswith(' US Equity') else symbol
             for symbol in symbols
         ]
 
         return symbols
 
     def get_historical_prices(self):
+        """
+        :description: Get historical prices
+
+        :return: Historical prices
+        :rtype: pandas.DataFrame
+        """
         if self.api_source == 'yahoo':
             if self.period is None:
                 start_date_obj = datetime.strptime(self.start_date, '%m-%d-%Y')
                 end_date_obj = datetime.strptime(self.end_date, '%m-%d-%Y')
                 start_date_formatted = datetime.strftime(start_date_obj, '%Y-%m-%d')
                 end_date_formatted = datetime.strftime(end_date_obj, '%Y-%m-%d')
                 try:
@@ -320,17 +326,17 @@
                 'PX_LAST',
                 start=prices[symbols].index[0],
                 end=prices[symbols].index[-1]
             ).squeeze().round(2)
             market_prices.name = market_name
 
         if prints:
-            print('Market Symbol:', self.market_symbol)
+            print('\nMarket Symbol:', self.market_symbol)
             print('Market Name:', market_name)
-            print('\nMarket Prices:')
+            print('Market Prices:')
             print(market_prices.apply(lambda x: '${:,.2f}'.format(round(x, 2))))
 
         return self.market_symbol, market_name, market_prices
 
     def market_implied_risk_aversion(self, market_prices, risk_free_rate, prints=False):
         """
         :description: Market implied risk aversion
```

### Comparing `etradebot-0.0.0/setup.py` & `etradebot-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='etradebot',
-    version='0.0.0',
+    version='1.0.0',
     url='https://github.com/nathanramoscfa/etradebot',
     license='MIT',
     author='Nathan Ramos, CFA®',
     author_email='info@nrcapitalmanagement.com',
     description='A Python-based trading bot for the E-Trade platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -18,23 +18,28 @@
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.11",
     install_requires=[
+        'blpapi==3.19.1',
         'cvxpy==1.3.0',
         'jupyterlab==3.6.1',
         'keyring==23.13.1',
         'matplotlib==3.7.1',
         'numpy==1.24.2',
         'pandas==1.5.3',
+        'pyportfolioopt==1.5.2',
         'scikit-learn==1.2.2',
         'scipy==1.10.1',
         'selenium==4.8.2',
         'statsmodels==0.13.5',
         'tqdm==4.65.0',
         'xmltodict==0.13.0',
         'yahooquery==2.3.0',
         'yfinance==0.2.12'
+    ],
+    dependency_links=[
+        'https://bcms.bloomberg.com/pip/simple/blpapi/'
     ]
 )
```

### Comparing `etradebot-0.0.0/strategies/cape_strategy.py` & `etradebot-1.0.0/strategies/cape_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/strategies/example_strategy.py` & `etradebot-1.0.0/strategies/example_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/tests/mock_responses.py` & `etradebot-1.0.0/tests/mock_responses.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/tests/test_authentication.py` & `etradebot-1.0.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/tests/test_etrade.py` & `etradebot-1.0.0/tests/test_etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/tests/test_execute.py` & `etradebot-1.0.0/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/tests/test_model.py` & `etradebot-1.0.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/utils/fake_data.py` & `etradebot-1.0.0/utils/fake_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
     :description: Create fake portfolio for testing purposes
     :param buying_power: Buying power
     :type buying_power: float, required
     :param prints: Prints, default is False
     :type prints: bool, optional
     :return: Fake portfolio
+    :rtype: pandas.core.frame.DataFrame
     """
     tickers = ['SPY', 'AGG', 'PSCD', 'QQQ', 'SPSM', 'OIH']
     weights = [0.80, 0.40, 0.10, -0.10, -0.10, -0.10]
     prices = pd.Series(data=[round(random.uniform(10, 100), 2) for i in range(len(tickers))], index=tickers)
     quantity = [x * buying_power for x in weights] / prices
     df = pd.DataFrame(data={
         'symbolDescription': tickers,
```

### Comparing `etradebot-0.0.0/utils/logging_config.py` & `etradebot-1.0.0/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `etradebot-0.0.0/utils/portfolio.py` & `etradebot-1.0.0/utils/portfolio.py`

 * *Files identical despite different names*

