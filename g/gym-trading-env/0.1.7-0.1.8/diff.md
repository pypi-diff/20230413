# Comparing `tmp/gym-trading-env-0.1.7.tar.gz` & `tmp/gym-trading-env-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.1.7.tar", last modified: Wed Apr 12 06:40:44 2023, max compression
+gzip compressed data, was "gym-trading-env-0.1.8.tar", last modified: Thu Apr 13 12:54:04 2023, max compression
```

## Comparing `gym-trading-env-0.1.7.tar` & `gym-trading-env-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.190187 gym-trading-env-0.1.7/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0    14258 2023-04-12 06:40:44.188192 gym-trading-env-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    12396 2023-04-12 06:38:12.000000 gym-trading-env-0.1.7/README.md
--rw-rw-rw-   0        0        0      870 2023-04-12 06:40:24.000000 gym-trading-env-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 06:40:44.190187 gym-trading-env-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.123367 gym-trading-env-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.139323 gym-trading-env-0.1.7/src/gym_trading_env/
--rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.7/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4126 2023-04-12 06:37:36.000000 gym-trading-env-0.1.7/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.7/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.7/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.185201 gym-trading-env-0.1.7/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.7/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-12 06:40:44.175227 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0    14258 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-12 06:40:44.000000 gym-trading-env-0.1.7/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.435812 gym-trading-env-0.1.8/
+-rw-rw-rw-   0        0        0     1088 2023-03-29 17:01:42.000000 gym-trading-env-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    14258 2023-04-13 12:54:04.434810 gym-trading-env-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12396 2023-04-13 12:39:12.000000 gym-trading-env-0.1.8/README.md
+-rw-rw-rw-   0        0        0      870 2023-04-13 12:52:15.000000 gym-trading-env-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 12:54:04.436807 gym-trading-env-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.345824 gym-trading-env-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.367811 gym-trading-env-0.1.8/src/gym_trading_env/
+-rw-rw-rw-   0        0        0      267 2023-04-13 10:54:15.000000 gym-trading-env-0.1.8/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-04-13 12:39:12.000000 gym-trading-env-0.1.8/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0     8871 2023-04-13 11:58:15.000000 gym-trading-env-0.1.8/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2502 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.431806 gym-trading-env-0.1.8/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-13 09:31:51.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-10 08:13:00.000000 gym-trading-env-0.1.8/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:54:04.420809 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0    14258 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 12:54:04.000000 gym-trading-env-0.1.8/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.1.7/LICENSE.txt` & `gym-trading-env-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.7/PKG-INFO` & `gym-trading-env-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.7/README.md` & `gym-trading-env-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.7/pyproject.toml` & `gym-trading-env-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.1.7"
+version = "0.1.8"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env/downloader.py` & `gym-trading-env-0.1.8/src/gym_trading_env/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 async def _ohlcv(exchange, symbol, timeframe, limit, step_since, timedelta):
     result = await exchange.fetch_ohlcv(symbol = symbol, timeframe= timeframe, limit= limit, since=step_since)
     result_df = pd.DataFrame(result, columns=["timestamp_open", "open", "high", "low", "close", "volume"])
     for col in ["open", "high", "low", "close", "volume"]:
         result_df[col] = pd.to_numeric(result_df[col])
     result_df["date_open"] = pd.to_datetime(result_df["timestamp_open"], unit= "ms")
     result_df["date_close"] = pd.to_datetime(result_df["timestamp_open"] + timedelta, unit= "ms")
+
     return result_df
 
 async def _download_symbol(exchange, symbol, timeframe = '5m', since = int(datetime.datetime(year=2020, month= 1, day= 1).timestamp()*1E3), until = int(datetime.datetime.now().timestamp()*1E3), limit = 1000, pause_every = 10, pause = 1):
     timedelta = int(pd.Timedelta(timeframe).to_timedelta64()/1E6)
     tasks = []
     results = []
     for step_since in range(since, until, limit * timedelta):
@@ -45,14 +46,15 @@
             results.extend(await asyncio.gather(*tasks))
             await asyncio.sleep(pause)
             tasks = []
     if len(tasks) > 0 :
         results.extend(await asyncio.gather(*tasks))
     final_df = pd.concat(results, ignore_index= True)
     final_df = final_df.loc[(since < final_df["timestamp_open"]) & (final_df["timestamp_open"] < until), :]
+    del final_df["timestamp_open"]
     final_df.set_index('date_open', drop=True, inplace=True)
     final_df.sort_index(inplace= True)
     final_df.dropna(inplace=True)
     final_df.drop_duplicates(inplace=True)
     return final_df
 
 async def _download_symbols(exchange_name, symbols, dir, timeframe,  **kwargs):
```

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env/environments.py` & `gym-trading-env-0.1.8/src/gym_trading_env/environments.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,84 +9,92 @@
 from collections import Counter
 from .utils.history import History
 from .utils.portfolio import Portfolio, TargetPortfolio
 
 import tempfile, os
 import warnings
 warnings.filterwarnings("error")
+def basic_reward_function(history : History):
+    return np.log(history["portfolio_valuation", -1] / history["portfolio_valuation", -2])
 
 class TradingEnv(gym.Env):
     """A trading environment for OpenAI gym"""
-    metadata = {'render.modes': ['human']}
+    metadata = {'render_modes': ['human']}
     def __init__(self,
                 df : pd.DataFrame,
                 positions : list = [0, 1],
-                reward_function = lambda history : np.log(history["portfolio_valuation", -1] / history["portfolio_valuation", -2]),
+                reward_function = basic_reward_function,
                 windows = None,
                 trading_fees = 0,
                 borrow_interest_rate = 0,
                 max_leverage = None,
                 portfolio_initial_value = 1000,
                 initial_position = 0,
+                include_position_in_features = True,
                 name = "Stock",
                 ):
         self.name = name
-        self._set_df(df)
+
         self.positions = positions
         self.reward_function = reward_function
         self.windows = windows
         self.trading_fees = trading_fees
         self.borrow_interest_rate = borrow_interest_rate
         self.max_leverage =max_leverage
         self.portfolio_initial_value = float(portfolio_initial_value)
         self.initial_position = initial_position
+        assert self.initial_position in self.positions, "The 'initial_position' parameter must one position mentionned in the 'position' (default is [0, 1]) parameter."
+        self.include_position_in_features = include_position_in_features
+        self._set_df(df)
 
         self.action_space = spaces.Discrete(len(positions))
-        self.observation_space = spaces.Dict(
-            {
-                "features": spaces.Box(
-                    self._obs_array.min() if self._nb_features > 0 else 0,
-                    self._obs_array.max() if self._nb_features > 0 else 1,
-                    shape = (self._nb_features, self.windows) if self.windows is not None else (self._nb_features, )
-                ),
-                "position": spaces.Box(-1, 1)
-            }
-        )
+        self.observation_space = spaces.Box(
+            -np.inf,
+            np.inf,
+            shape = [self._nb_features]
+        )
+        if self.windows is not None:
+            self.observation_space = spaces.Box(
+                -np.inf,
+                np.inf,
+                shape = [self.windows, self._nb_features]
+            )
+
 
     def _set_df(self, df):
+        df = df.copy()
         self._features_columns = [col for col in df.columns if "feature" in col]
         self._info_columns = list(set(list(df.columns) + ["close"]) - set(self._features_columns))
         self._nb_features = len(self._features_columns)
 
+        if self.include_position_in_features:
+            df["feature_position"] = self.initial_position
+            self._features_columns.append("feature_position")
+            self._nb_features += 1
         self.df = df
-        self._obs_array = np.array(self.df[self._features_columns])
+        self._obs_array = np.array(self.df[self._features_columns], dtype= np.float32)
         self._info_array = np.array(self.df[self._info_columns])
         self._price_array = np.array(self.df["close"])
 
     
     def _get_ticker(self, delta = 0):
         return self.df.iloc[self._step + delta]
     def _get_price(self, delta = 0):
         return self._price_array[self._step + delta]
-
-    def _leverage_check(self, portfolio_distribution, price):
-        if (portfolio_distribution["borrowed_asset"] * price + portfolio_distribution["borrowed_fiat"]) > 0.95*self.max_leverage * (portfolio_distribution["asset"] * price + portfolio_distribution["fiat"]):
-            return True
-        return False
     
-
     def _get_obs(self):
-        if self.windows is None: _step_index = self._step
-        else: _step_index = np.arange(self._step + 1 - self.windows , self._step + 1)
-        return {
-            "features" : self._obs_array[_step_index],
-            "position" : self._position
-            }
+        if self.include_position_in_features: self._obs_array[self._step, -1] = self._position
+        if self.windows is None:
+            _step_index = self._step
+        else: 
+            _step_index = np.arange(self._step + 1 - self.windows , self._step + 1)
+        return self._obs_array[_step_index]
+
     
-    def reset(self, seed = None):
+    def reset(self, seed = None, options=None):
         super().reset(seed = seed)
         self._step = 0
         self._limit_orders = {}
         if self.windows is not None: self._step = self.windows
 
         self._portfolio  = TargetPortfolio(
             position=self.initial_position,
@@ -94,30 +102,32 @@
             price = self._get_price()
         )
         self._position = self.initial_position
         self.historical_info = History(max_size= len(self.df))
         self.historical_info.set(
             step = self._step,
             date = self.df.index.values[self._step],
-            action = None,
+            action = self.positions.index(self.initial_position),
             position = self._position,
             data =  dict(zip(self._info_columns, self._info_array[self._step])),
             portfolio_valuation = self.portfolio_initial_value,
             portfolio_distribution = self._portfolio.get_portfolio_distribution(),
             reward = 0,
         )
+
         return self._get_obs(), self.historical_info[0]
 
     def _trade(self, position, price = None):
         self._portfolio.trade_to_position(
             position, 
             price = self._get_price() if price is None else price, 
             trading_fees = self.trading_fees
         )
         self._position = position
+        return
 
     def _take_action(self, position):
         if position != self._position:
             self._trade(position)
     
     def _take_action_order_limit(self):
         if len(self._limit_orders) > 0:
@@ -141,32 +151,33 @@
 
         self._take_action_order_limit()
         price = self._get_price()
         self._portfolio.update_interest(borrow_interest_rate= self.borrow_interest_rate)
         portfolio_value = self._portfolio.valorisation(price)
         portfolio_distribution = self._portfolio.get_portfolio_distribution()
         done, truncated = False, False
-        if self.max_leverage is not None:
-            done = self._leverage_check(portfolio_distribution, price)
+        if portfolio_value <= 0: done = True
         if self._step >= len(self.df) - 1:
             truncated = True
         
         self.historical_info.add(
             step = self._step,
             date = self.df.index.values[self._step],
             action = position_index,
             position = self._position,
             data =  dict(zip(self._info_columns, self._info_array[self._step])),
             portfolio_valuation = portfolio_value,
             portfolio_distribution = portfolio_distribution, 
             reward = 0
         )
-        reward = self.reward_function(self.historical_info)
-        self.historical_info["reward", -1] = reward
-        return self._get_obs(),  self.reward_function(self.historical_info), done, truncated, self.historical_info[-1]
+        if not done:
+            reward = self.reward_function(self.historical_info)
+            self.historical_info["reward", -1] = reward
+
+        return self._get_obs(),  self.historical_info["reward", -1], done, truncated, self.historical_info[-1]
     
     def save_for_render(self, dir = "render_logs"):
         assert "open" in self.df and "high" in self.df and "low" in self.df and "close" in self.df, "Your DataFrame needs to contain columns : open, high, low, close to render !"
         columns = list(set(self.historical_info.columns) - set([f"date_{col}" for col in self._info_columns]))
         history_df = pd.DataFrame(
             self.historical_info[columns], columns= columns
         )
```

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env/renderer.py` & `gym-trading-env-0.1.8/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.1.8/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.1.8/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.1.8/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.1.8/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.7/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.1.8/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

