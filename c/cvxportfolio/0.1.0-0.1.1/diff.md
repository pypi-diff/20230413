# Comparing `tmp/cvxportfolio-0.1.0.tar.gz` & `tmp/cvxportfolio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.1.0.tar", max compression
+gzip compressed data, was "cvxportfolio-0.1.1.tar", max compression
```

## Comparing `cvxportfolio-0.1.0.tar` & `cvxportfolio-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      599 2023-04-08 05:48:25.320984 cvxportfolio-0.1.0/LICENSE
--rw-r--r--   0        0        0     1628 2023-04-08 07:25:54.582786 cvxportfolio-0.1.0/README.md
--rw-r--r--   0        0        0     1006 2023-04-08 05:48:25.321868 cvxportfolio-0.1.0/cvxportfolio/__init__.py
--rw-r--r--   0        0        0     7063 2023-04-08 05:48:25.322068 cvxportfolio-0.1.0/cvxportfolio/constraints.py
--rw-r--r--   0        0        0     7168 2023-04-08 05:48:25.322249 cvxportfolio-0.1.0/cvxportfolio/costs.py
--rw-r--r--   0        0        0     1361 2023-04-08 05:48:25.322399 cvxportfolio-0.1.0/cvxportfolio/expression.py
--rw-r--r--   0        0        0    12728 2023-04-08 05:48:25.322805 cvxportfolio-0.1.0/cvxportfolio/policies.py
--rw-r--r--   0        0        0     7810 2023-04-08 05:48:25.323035 cvxportfolio-0.1.0/cvxportfolio/result.py
--rw-r--r--   0        0        0     4400 2023-04-08 05:48:25.323191 cvxportfolio-0.1.0/cvxportfolio/returns.py
--rw-r--r--   0        0        0     7803 2023-04-08 05:48:25.323706 cvxportfolio-0.1.0/cvxportfolio/risks.py
--rw-r--r--   0        0        0     9814 2023-04-08 05:48:25.323924 cvxportfolio-0.1.0/cvxportfolio/simulator.py
--rw-r--r--   0        0        0     2956 2023-04-08 05:48:25.324079 cvxportfolio-0.1.0/cvxportfolio/utils.py
--rw-r--r--   0        0        0      566 2023-04-08 07:43:51.082270 cvxportfolio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 cvxportfolio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-04-08 05:48:25.320984 cvxportfolio-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3681 2023-04-12 17:11:34.075141 cvxportfolio-0.1.1/README.md
+-rw-r--r--   0        0        0     1100 2023-04-13 03:24:52.226520 cvxportfolio-0.1.1/cvxportfolio/__init__.py
+-rw-r--r--   0        0        0     7115 2023-04-12 17:11:34.082324 cvxportfolio-0.1.1/cvxportfolio/constraints.py
+-rw-r--r--   0        0        0     7166 2023-04-12 17:11:34.082677 cvxportfolio-0.1.1/cvxportfolio/costs.py
+-rw-r--r--   0        0        0     6403 2023-04-12 17:11:34.082887 cvxportfolio-0.1.1/cvxportfolio/data.py
+-rw-r--r--   0        0        0     3809 2023-04-12 20:26:08.261760 cvxportfolio-0.1.1/cvxportfolio/estimator.py
+-rw-r--r--   0        0        0     1278 2023-04-12 17:11:34.083203 cvxportfolio-0.1.1/cvxportfolio/expression.py
+-rw-r--r--   0        0        0    12440 2023-04-12 17:11:34.083454 cvxportfolio-0.1.1/cvxportfolio/policies.py
+-rw-r--r--   0        0        0     7758 2023-04-12 17:11:34.083828 cvxportfolio-0.1.1/cvxportfolio/result.py
+-rw-r--r--   0        0        0     4339 2023-04-12 17:11:34.084082 cvxportfolio-0.1.1/cvxportfolio/returns.py
+-rw-r--r--   0        0        0     7696 2023-04-12 17:11:34.084963 cvxportfolio-0.1.1/cvxportfolio/risks.py
+-rw-r--r--   0        0        0     9561 2023-04-12 17:11:34.085683 cvxportfolio-0.1.1/cvxportfolio/simulator.py
+-rw-r--r--   0        0        0     2973 2023-04-12 17:11:34.086422 cvxportfolio-0.1.1/cvxportfolio/utils.py
+-rw-r--r--   0        0        0      673 2023-04-13 03:24:24.847017 cvxportfolio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 cvxportfolio-0.1.1/PKG-INFO
```

### Comparing `cvxportfolio-0.1.0/LICENSE` & `cvxportfolio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.1.0/cvxportfolio/__init__.py` & `cvxportfolio-0.1.1/cvxportfolio/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+# Copyright 2023- The Cvxportfolio Contributors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-__version__ = "0.0.12"
+__version__ = "0.1.1"
+from .data import FredRate, Yfinance
 from .simulator import MarketSimulator
 from .result import SimulationResult
 from .policies import *
 from .constraints import *
 from .utils import *
 from .costs import TcostModel, HcostModel
 from .returns import *
-from .risks import (FullSigma, EmpSigma, SqrtSigma,
-                    FactorModelSigma, RobustFactorModelSigma,
-                    RobustSigma, WorstCaseRisk)
+from .risks import (
+    FullSigma,
+    EmpSigma,
+    SqrtSigma,
+    FactorModelSigma,
+    RobustFactorModelSigma,
+    RobustSigma,
+    WorstCaseRisk,
+)
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/constraints.py` & `cvxportfolio-0.1.1/cvxportfolio/constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-
-from abc import ABCMeta, abstractmethod
 
 import cvxpy as cvx
 import numpy as np
 
 from .utils import values_in_time
 
 
-__all__ = ['LongOnly', 'LeverageLimit', 'LongCash', 'DollarNeutral', 'MaxTrade',
-           'MaxWeights', 'MinWeights', 'FactorMaxLimit', 'FactorMinLimit',
-           'FixedAlpha']
+__all__ = [
+    "LongOnly",
+    "LeverageLimit",
+    "LongCash",
+    "DollarNeutral",
+    "MaxTrade",
+    "MaxWeights",
+    "MinWeights",
+    "FactorMaxLimit",
+    "FactorMinLimit",
+    "FixedAlpha",
+]
 
 
 class BaseConstraint:
-    __metaclass__ = ABCMeta
-
     def __init__(self, **kwargs):
-        self.w_bench = kwargs.pop('w_bench', 0.)
+        self.w_bench = kwargs.pop("w_bench", 0.0)
 
     def weight_expr(self, t, w_plus, z, v):
         """Returns a list of trade constraints.
 
         Args:
           t: time
           w_plus: post-trade weights
           z: trade weights
           v: portfolio value
         """
         if w_plus is None:
             return self._weight_expr(t, None, z, v)
         return self._weight_expr(t, w_plus - self.w_bench, z, v)
 
-    @abstractmethod
     def _weight_expr(self, t, w_plus, z, v):
-        pass
+        raise NotImplementedError
 
 
 class MaxTrade(BaseConstraint):
-    """A limit on maximum trading size.
-    """
+    """A limit on maximum trading size."""
 
     def __init__(self, ADVs, max_fraction=0.05, **kwargs):
         self.ADVs = ADVs
         self.max_fraction = max_fraction
         super(MaxTrade, self).__init__(**kwargs)
 
     def _weight_expr(self, t, w_plus, z, v):
@@ -66,33 +67,34 @@
 
         Args:
           t: time
           w_plus: post-trade weights
           z: trade weights
           v: portfolio value
         """
-        return cvx.abs(z[:-1]) * v <= \
-            np.array(values_in_time(self.ADVs, t)) * self.max_fraction
+        return [
+            cvx.abs(z[:-1]) * v
+            <= np.array(values_in_time(self.ADVs, t)) * self.max_fraction
+        ]
 
 
 class LongOnly(BaseConstraint):
-    """A long only constraint.
-    """
+    """A long only constraint."""
 
     def __init__(self, **kwargs):
         super(LongOnly, self).__init__(**kwargs)
 
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
           t: time
           w_plus: holdings
         """
-        return w_plus >= 0
+        return [w_plus >= 0]
 
 
 class LeverageLimit(BaseConstraint):
     """A limit on leverage.
 
     Attributes:
       limit: A (time) series or scalar giving the leverage limit.
@@ -105,49 +107,47 @@
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
           t: time
           w_plus: holdings
         """
-        return cvx.norm(w_plus[:-1], 1) <= values_in_time(self.limit, t)
+        return [cvx.norm(w_plus[:-1], 1) <= values_in_time(self.limit, t)]
 
 
 class LongCash(BaseConstraint):
-    """Requires that cash be non-negative.
-    """
+    """Requires that cash be non-negative."""
 
     def __init__(self, **kwargs):
         super(LongCash, self).__init__(**kwargs)
 
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
           t: time
           w_plus: holdings
         """
-        return w_plus[-1] >= 0
+        return [w_plus[-1] >= 0]
 
 
 class DollarNeutral(BaseConstraint):
-    """Long-short dollar neutral strategy.
-    """
+    """Long-short dollar neutral strategy."""
 
     def __init__(self, **kwargs):
         super(DollarNeutral, self).__init__(**kwargs)
 
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
           t: time
           w_plus: holdings
         """
-        return sum(w_plus[:-1]) == 0
+        return [sum(w_plus[:-1]) == 0]
 
 
 class MaxWeights(BaseConstraint):
     """A max limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
@@ -160,15 +160,15 @@
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
           t: time
           w_plus: holdings
         """
-        return w_plus[:-1] <= values_in_time(self.limit, t)
+        return [w_plus[:-1] <= values_in_time(self.limit, t)]
 
 
 class MinWeights(BaseConstraint):
     """A min limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
@@ -181,15 +181,15 @@
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
           t: time
           w_plus: holdings
         """
-        return w_plus[:-1] >= values_in_time(self.limit, t)
+        return [w_plus[:-1] >= values_in_time(self.limit, t)]
 
 
 class FactorMaxLimit(BaseConstraint):
     """A max limit on portfolio-wide factor (e.g. beta) exposure.
 
     Attributes:
         factor_exposure: An (n * r) matrix giving the factor exposure per asset
@@ -205,16 +205,18 @@
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
             t: time
             w_plus: holdings
         """
-        return values_in_time(self.factor_exposure, t).T @ w_plus[:-1] <= \
-            values_in_time(self.limit, t)
+        return [
+            values_in_time(self.factor_exposure, t).T @ w_plus[:-1]
+            <= values_in_time(self.limit, t)
+        ]
 
 
 class FactorMinLimit(BaseConstraint):
     """A min limit on portfolio-wide factor (e.g. beta) exposure.
 
     Attributes:
         factor_exposure: An (n * r) matrix giving the factor exposure per asset
@@ -230,16 +232,18 @@
     def _weight_expr(self, t, w_plus, z, v):
         """Returns a list of holding constraints.
 
         Args:
             t: time
             w_plus: holdings
         """
-        return values_in_time(self.factor_exposure, t).T @ w_plus[:-1] >= \
-            values_in_time(self.limit, t)
+        return [
+            values_in_time(self.factor_exposure, t).T @ w_plus[:-1]
+            >= values_in_time(self.limit, t)
+        ]
 
 
 class FixedAlpha(BaseConstraint):
     """A constraint to fix portfolio-wide alpha
 
     Attributes:
         forecast_returns: An (n * 1) vector giving the return forecast on each
@@ -249,9 +253,11 @@
 
     def __init__(self, return_forecast, alpha_target, **kwargs):
         super(FixedAlpha, self).__init__(**kwargs)
         self.return_forecast = return_forecast
         self.alpha_target = alpha_target
 
     def _weight_expr(self, t, w_plus, z, v):
-        return values_in_time(self.return_forecast, t).T @ w_plus[:-1] == \
-            values_in_time(self.alpha_target, t)
+        return [
+            values_in_time(self.return_forecast, t).T @ w_plus[:-1]
+            == values_in_time(self.alpha_target, t)
+        ]
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/costs.py` & `cvxportfolio-0.1.1/cvxportfolio/costs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import cvxpy as cvx
 import numpy as np
 import copy
 from .expression import Expression
 from .utils import null_checker, values_in_time
 
 
-__all__ = ['HcostModel', 'TcostModel']
+__all__ = ["HcostModel", "TcostModel"]
 
 
 class BaseCost(Expression):
-
     def __init__(self):
-        self.gamma = 1.  # it is changed by gamma * BaseCost()
+        self.gamma = 1.0  # it is changed by gamma * BaseCost()
 
     def weight_expr(self, t, w_plus, z, value):
         cost, constr = self._estimate(t, w_plus, z, value)
         return self.gamma * cost, constr
 
     def weight_expr_ahead(self, t, tau, w_plus, z, value):
         cost, constr = self._estimate_ahead(t, tau, w_plus, z, value)
@@ -52,15 +49,15 @@
     """A model for holding costs.
 
     Attributes:
       borrow_costs: A dataframe of borrow costs.
       dividends: A dataframe of dividends.
     """
 
-    def __init__(self, borrow_costs, dividends=0.):
+    def __init__(self, borrow_costs, dividends=0.0):
         null_checker(borrow_costs)
         self.borrow_costs = borrow_costs
         null_checker(dividends)
         self.dividends = dividends
         super(HcostModel, self).__init__()
 
     def _estimate(self, t, w_plus, z, value):
@@ -75,33 +72,36 @@
             w_plus = w_plus[w_plus.index != self.cash_key]
             w_plus = w_plus.values
         except AttributeError:
             w_plus = w_plus[:-1]  # TODO fix when cvxpy pandas ready
 
         try:
             self.expression = cvx.multiply(
-                values_in_time(self.borrow_costs, t), cvx.neg(w_plus))
+                values_in_time(self.borrow_costs, t), cvx.neg(w_plus)
+            )
         except TypeError:
-            self.expression = cvx.multiply(values_in_time(
-                self.borrow_costs, t).values, cvx.neg(w_plus))
+            self.expression = cvx.multiply(
+                values_in_time(self.borrow_costs, t).values, cvx.neg(w_plus)
+            )
         try:
-            self.expression -= cvx.multiply(
-                values_in_time(self.dividends, t), w_plus)
+            self.expression -= cvx.multiply(values_in_time(self.dividends, t), w_plus)
         except TypeError:
             self.expression -= cvx.multiply(
-                values_in_time(self.dividends, t).values, w_plus)
+                values_in_time(self.dividends, t).values, w_plus
+            )
 
         return cvx.sum(self.expression), []
 
     def _estimate_ahead(self, t, tau, w_plus, z, value):
         return self._estimate(t, w_plus, z, value)
 
     def value_expr(self, t, h_plus, u):
         self.last_cost = -np.minimum(0, h_plus.iloc[:-1]) * values_in_time(
-            self.borrow_costs, t)
+            self.borrow_costs, t
+        )
         self.last_cost -= h_plus.iloc[:-1] * values_in_time(self.dividends, t)
 
         return sum(self.last_cost)
 
     def optimization_log(self, t):
         return self.expression.value
 
@@ -116,29 +116,28 @@
     https://stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
 
     Attributes:
       volume: A dataframe of volumes.
       sigma: A dataframe of daily volatilities.
       half_spread: A dataframe of bid-ask spreads divided by 2.
       nonlin_coeff: A dataframe of coefficients for the nonlinear cost.
-      power: The nonlinear tcost power.
+      power (float): The nonlinear tcost power.
     """
 
-    def __init__(self, half_spread, nonlin_coeff=0., sigma=0., volume=1.,
-                 power=1.5):
+    def __init__(self, half_spread, nonlin_coeff=0.0, sigma=0.0, volume=1.0, power=1.5):
         null_checker(half_spread)
         self.half_spread = half_spread
         null_checker(sigma)
         self.sigma = sigma
         null_checker(volume)
         self.volume = volume
         null_checker(nonlin_coeff)
         self.nonlin_coeff = nonlin_coeff
         null_checker(power)
-        self.power = power
+        self.power: float = power
         super(TcostModel, self).__init__()
 
     def _estimate(self, t, w_plus, z, value):
         """Estimate tcosts given trades.
 
         Args:
           t: time of estimate
@@ -153,70 +152,73 @@
             z = z[z.index != self.cash_key]
             z = z.values
         except AttributeError:
             z = z[:-1]  # TODO fix when cvxpy pandas ready
 
         constr = []
 
-        second_term = values_in_time(self.nonlin_coeff, t) * values_in_time(
-            self.sigma, t) * (value / values_in_time(self.volume, t)) ** (
-            self.power - 1)
+        second_term = (
+            values_in_time(self.nonlin_coeff, t)
+            * values_in_time(self.sigma, t)
+            * (value / values_in_time(self.volume, t)) ** (self.power - 1)
+        )
 
         # no trade conditions
         if np.isscalar(second_term):
             if np.isnan(second_term):
                 constr += [z == 0]
                 second_term = 0
         else:  # it is a pd series
             no_trade = second_term.index[second_term.isnull()]
             second_term[no_trade] = 0
-            constr += [z[second_term.index.get_loc(tick)] == 0
-                       for tick in no_trade]
+            constr += [z[second_term.index.get_loc(tick)] == 0 for tick in no_trade]
 
         try:
             self.expression = cvx.multiply(
-                values_in_time(self.half_spread, t), cvx.abs(z))
+                values_in_time(self.half_spread, t), cvx.abs(z)
+            )
         except TypeError:
             self.expression = cvx.multiply(
-                values_in_time(self.half_spread, t).values, cvx.abs(z))
+                values_in_time(self.half_spread, t).values, cvx.abs(z)
+            )
         try:
-            self.expression += cvx.multiply(second_term,
-                                            cvx.abs(z) ** self.power)
+            self.expression += cvx.multiply(second_term, cvx.abs(z) ** self.power)
         except TypeError:
             self.expression += cvx.multiply(
-                second_term.values, cvx.abs(z) ** self.power)
+                second_term.values, cvx.abs(z) ** self.power
+            )
 
         return cvx.sum(self.expression), constr
 
     def value_expr(self, t, h_plus, u):
-
         u_nc = u.iloc[:-1]
-        self.tmp_tcosts = (
-            np.abs(u_nc) * values_in_time(self.half_spread, t) +
-            values_in_time(self.nonlin_coeff, t) * values_in_time(self.sigma,
-                                                                  t) *
-            np.abs(u_nc) ** self.power /
-            (values_in_time(self.volume, t) ** (self.power - 1)))
+        self.tmp_tcosts = np.abs(u_nc) * values_in_time(
+            self.half_spread, t
+        ) + values_in_time(self.nonlin_coeff, t) * values_in_time(
+            self.sigma, t
+        ) * np.abs(
+            u_nc
+        ) ** self.power / (
+            values_in_time(self.volume, t) ** (self.power - 1)
+        )
 
         return self.tmp_tcosts.sum()
 
     def optimization_log(self, t):
         try:
             return self.expression.value
         except AttributeError:
             return np.nan
 
     def simulation_log(self, t):
         # TODO find another way
         return self.tmp_tcosts
 
     def _estimate_ahead(self, t, tau, w_plus, z, value):
-        """Returns the estimate at time t of tcost at time tau.
-        """
+        """Returns the estimate at time t of tcost at time tau."""
         return self._estimate(t, w_plus, z, value)
 
     def est_period(self, t, tau_start, tau_end, w_plus, z, value):
-        """Returns the estimate at time t of tcost over given period.
-        """
+        """Returns the estimate at time t of tcost over given period."""
         K = (tau_end - tau_start).days
         tcost, constr = self.weight_expr(t, None, z / K, value)
         return tcost * K, constr
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/expression.py` & `cvxportfolio-0.1.1/cvxportfolio/expression.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,32 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from abc import ABCMeta, abstractmethod
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 
 class Expression:
-    __metaclass__ = ABCMeta
-
-    @abstractmethod
     def weight_expr(self, t, w_plus, z, value):
         """Returns the estimate of cost at time t."""
-        pass
+        raise NotImplementedError
 
     def weight_expr_ahead(self, t, tau, w_plus, z, value):
-        """Returns the estimate at time t of cost at time tau.
-        """
+        """Returns the estimate at time t of cost at time tau."""
         return self.weight_expr(t, w_plus, z, value)
 
     def value_expr(self, t, h_plus, u):
         """Returns the expression at time t, using value representation.
 
         This should be overridden if the term is used in the simulator.
         """
-        return sum(h_plus) * self.weight_expr(t, h_plus / sum(h_plus),
-                                              u / sum(u), sum(h_plus))
+        return sum(h_plus) * self.weight_expr(
+            t, h_plus / sum(h_plus), u / sum(u), sum(h_plus)
+        )
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/policies.py` & `cvxportfolio-0.1.1/cvxportfolio/policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-from abc import ABCMeta, abstractmethod
 import datetime as dt
 import pandas as pd
 import numpy as np
 import logging
 import cvxpy as cvx
 
 from cvxportfolio.costs import BaseCost
 from cvxportfolio.returns import BaseReturnsModel
 from cvxportfolio.constraints import BaseConstraint
 from cvxportfolio.utils import values_in_time, null_checker
 
 
-__all__ = ['Hold', 'FixedTrade', 'PeriodicRebalance', 'AdaptiveRebalance',
-           'SinglePeriodOpt', 'MultiPeriodOpt', 'ProportionalTrade',
-           'RankAndLongShort']
+__all__ = [
+    "Hold",
+    "FixedTrade",
+    "PeriodicRebalance",
+    "AdaptiveRebalance",
+    "SinglePeriodOpt",
+    "MultiPeriodOpt",
+    "ProportionalTrade",
+    "RankAndLongShort",
+]
 
 
 class BasePolicy:
-    """ Base class for a trading policy. """
-    __metaclass__ = ABCMeta
+    """Base class for a trading policy."""
 
     def __init__(self):
         self.costs = []
         self.constraints = []
 
-    @abstractmethod
     def get_trades(self, portfolio, t=dt.datetime.today()):
-        """Trades list given current portfolio and time t.
-        """
-        return NotImplemented
+        """Trades list given current portfolio and time t."""
+        return NotImplementedError
 
     def _nulltrade(self, portfolio):
-        return pd.Series(index=portfolio.index, data=0.)
+        return pd.Series(index=portfolio.index, data=0.0)
 
     def get_rounded_trades(self, portfolio, prices, t):
         """Get trades vector as number of shares, rounded to integers."""
-        return np.round(self.get_trades(portfolio,
-                                        t) / values_in_time(prices, t))[:-1]
+        return np.round(self.get_trades(portfolio, t) / values_in_time(prices, t))[:-1]
 
 
 class Hold(BasePolicy):
-    """Hold initial portfolio.
-    """
+    """Hold initial portfolio."""
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
         return self._nulltrade(portfolio)
 
 
 class RankAndLongShort(BasePolicy):
     """Rank assets, long the best and short the worst (cash neutral)."""
@@ -73,20 +72,20 @@
         self.return_forecast = return_forecast
         super(RankAndLongShort, self).__init__()
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
         prediction = values_in_time(self.return_forecast, t)
         sorted_ret = prediction.sort_values()
 
-        short_trades = sorted_ret.index[:self.num_short]
-        long_trades = sorted_ret.index[-self.num_long:]
+        short_trades = sorted_ret.index[: self.num_short]
+        long_trades = sorted_ret.index[-self.num_long :]
 
-        u = pd.Series(0., index=prediction.index)
-        u[short_trades] = -1.
-        u[long_trades] = 1.
+        u = pd.Series(0.0, index=prediction.index)
+        u[short_trades] = -1.0
+        u[long_trades] = 1.0
         u /= sum(abs(u))
         u = sum(portfolio) * u * self.target_turnover
 
         # import pdb; pdb.set_trace()
         #
         # # ex-post cash neutrality
         # old_cash = portfolio[-1]
@@ -104,95 +103,92 @@
     def __init__(self, targetweight, time_steps):
         self.targetweight = targetweight
         self.time_steps = time_steps
         super(ProportionalTrade, self).__init__()
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
         try:
-            missing_time_steps = len(
-                self.time_steps) - next(i for (i, x)
-                                        in enumerate(self.time_steps)
-                                        if x == t)
+            missing_time_steps = len(self.time_steps) - next(
+                i for (i, x) in enumerate(self.time_steps) if x == t
+            )
         except StopIteration:
-            raise Exception(
-                "ProportionalTrade can only trade on the given time steps")
+            raise Exception("ProportionalTrade can only trade on the given time steps")
         deviation = self.targetweight - portfolio / sum(portfolio)
         return sum(portfolio) * deviation / missing_time_steps
 
 
 class SellAll(BasePolicy):
     """Sell all non-cash assets."""
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
         trade = -pd.Series(portfolio, copy=True)
-        trade.ix[-1] = 0.
+        trade.ix[-1] = 0.0
         return trade
 
 
 class FixedTrade(BasePolicy):
-    """Trade a fixed trade vector.
-    """
+    """Trade a fixed trade vector."""
 
     def __init__(self, tradevec=None, tradeweight=None):
         """Trade the tradevec vector (dollars) or tradeweight weights."""
         if tradevec is not None and tradeweight is not None:
             raise Exception
         if tradevec is None and tradeweight is None:
             raise Exception
         self.tradevec = tradevec
         self.tradeweight = tradeweight
-        assert(self.tradevec is None or sum(self.tradevec) == 0.)
-        assert(self.tradeweight is None or sum(self.tradeweight) == 0.)
+        assert self.tradevec is None or sum(self.tradevec) == 0.0
+        assert self.tradeweight is None or sum(self.tradeweight) == 0.0
         super(FixedTrade, self).__init__()
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
         if self.tradevec is not None:
             return self.tradevec
         return sum(portfolio) * self.tradeweight
 
 
 class BaseRebalance(BasePolicy):
-
     def _rebalance(self, portfolio):
         return sum(portfolio) * self.target - portfolio
 
 
 class PeriodicRebalance(BaseRebalance):
-    """Track a target portfolio, rebalancing at given times.
-    """
+    """Track a target portfolio, rebalancing at given times."""
 
     def __init__(self, target, period, **kwargs):
         """
         Args:
             target: target weights, n+1 vector
             period: supported options are "day", "week", "month", "quarter",
                 "year".
                 rebalance on the first day of each new period
         """
         self.target = target
         self.period = period
         super(PeriodicRebalance, self).__init__()
 
     def is_start_period(self, t):
-        result = not getattr(t, self.period) == getattr(self.last_t,
-                                                        self.period) if \
-            hasattr(self,
-                    'last_t')\
+        result = (
+            not getattr(t, self.period) == getattr(self.last_t, self.period)
+            if hasattr(self, "last_t")
             else True
+        )
         self.last_t = t
         return result
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
-        return self._rebalance(portfolio) if self.is_start_period(t) else \
-            self._nulltrade(portfolio)
+        return (
+            self._rebalance(portfolio)
+            if self.is_start_period(t)
+            else self._nulltrade(portfolio)
+        )
 
 
 class AdaptiveRebalance(BaseRebalance):
-    """ Rebalance portfolio when deviates too far from target.
-    """
+    """Rebalance portfolio when deviates too far from target."""
 
     def __init__(self, target, tracking_error):
         self.target = target
         self.tracking_error = tracking_error
         super(AdaptiveRebalance, self).__init__()
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
@@ -208,17 +204,17 @@
 class SinglePeriodOpt(BasePolicy):
     """Single-period optimization policy.
 
     Implements the model developed in chapter 4 of our paper
     https://stanford.edu/~boyd/papers/cvx_portfolio.html
     """
 
-    def __init__(self, return_forecast, costs, constraints, solver=None,
-                 solver_opts=None):
-
+    def __init__(
+        self, return_forecast, costs, constraints, solver=None, solver_opts=None
+    ):
         if not isinstance(return_forecast, BaseReturnsModel):
             null_checker(return_forecast)
         self.return_forecast = return_forecast
 
         super(SinglePeriodOpt, self).__init__()
 
         for cost in costs:
@@ -251,58 +247,56 @@
         w = portfolio / value
         z = cvx.Variable(w.size)  # TODO pass index
         wplus = w.values + z
 
         if isinstance(self.return_forecast, BaseReturnsModel):
             alpha_term = self.return_forecast.weight_expr(t, wplus)
         else:
-            alpha_term = cvx.sum(cvx.multiply(
-                values_in_time(self.return_forecast, t).values,
-                wplus))
+            alpha_term = cvx.sum(
+                cvx.multiply(values_in_time(self.return_forecast, t).values, wplus)
+            )
 
-        assert(alpha_term.is_concave())
+        assert alpha_term.is_concave()
 
         costs, constraints = [], []
 
         for cost in self.costs:
             cost_expr, const_expr = cost.weight_expr(t, wplus, z, value)
             costs.append(cost_expr)
             constraints += const_expr
 
-        constraints += [item for item in (con.weight_expr(t, wplus, z, value)
-                                          for con in self.constraints)]
+        for constr in self.constraints:
+            constraints += constr.weight_expr(t, wplus, z, value)
 
         for el in costs:
-            assert (el.is_convex())
+            assert el.is_convex()
 
         for el in constraints:
-            assert (el.is_dcp())
+            assert el.is_dcp()
 
         self.prob = cvx.Problem(
-            cvx.Maximize(alpha_term - sum(costs)),
-            [cvx.sum(z) == 0] + constraints)
+            cvx.Maximize(alpha_term - sum(costs)), [cvx.sum(z) == 0] + constraints
+        )
         try:
             self.prob.solve(solver=self.solver, **self.solver_opts)
 
-            if self.prob.status == 'unbounded':
-                logging.error(
-                    'The problem is unbounded. Defaulting to no trades')
+            if self.prob.status == "unbounded":
+                logging.error("The problem is unbounded. Defaulting to no trades")
                 return self._nulltrade(portfolio)
 
-            if self.prob.status == 'infeasible':
-                logging.error(
-                    'The problem is infeasible. Defaulting to no trades')
+            if self.prob.status == "infeasible":
+                logging.error("The problem is infeasible. Defaulting to no trades")
                 return self._nulltrade(portfolio)
 
             return pd.Series(index=portfolio.index, data=(z.value * value))
         except (cvx.SolverError, TypeError):
-            logging.error(
-                'The solver %s failed. Defaulting to no trades' % self.solver)
+            logging.error("The solver %s failed. Defaulting to no trades" % self.solver)
             return self._nulltrade(portfolio)
 
+
 # class LookaheadModel():
 #     """Returns the planning periods for multi-period.
 #     """
 #     def __init__(self, trading_times, period_lens):
 #         self.trading_times = trading_times
 #         self.period_lens = period_lens
 #
@@ -315,67 +309,67 @@
 #             incr = length*pd.Timedelta('1 days')
 #             periods.append((tau, tau + incr))
 #             tau += incr
 #         return periods
 
 
 class MultiPeriodOpt(SinglePeriodOpt):
-
-    def __init__(self, trading_times,
-                 terminal_weights, lookahead_periods=None, *args, **kwargs):
+    def __init__(
+        self, trading_times, terminal_weights, lookahead_periods=None, *args, **kwargs
+    ):
         """
         trading_times: list, all times at which get_trades will be called
         lookahead_periods: int or None. if None uses all remaining periods
         """
         # Number of periods to look ahead.
         self.lookahead_periods = lookahead_periods
         self.trading_times = trading_times
         # Should there be a constraint that the final portfolio is the bmark?
         self.terminal_weights = terminal_weights
         super(MultiPeriodOpt, self).__init__(*args, **kwargs)
 
     def get_trades(self, portfolio, t=dt.datetime.today()):
-
         value = sum(portfolio)
-        assert (value > 0.)
+        assert value > 0.0
         w = cvx.Constant(portfolio.values / value)
 
         prob_arr = []
         z_vars = []
 
         # planning_periods = self.lookahead_model.get_periods(t)
-        for tau in \
-                self.trading_times[self.trading_times.index(t):
-                                   self.trading_times.index(t) +
-                                   self.lookahead_periods]:
+        for tau in self.trading_times[
+            self.trading_times.get_loc(t) : self.trading_times.get_loc(t)
+            + self.lookahead_periods
+        ]:
             # delta_t in [pd.Timedelta('%d days' % i) for i in
             # range(self.lookahead_periods)]:
 
             #            tau = t + delta_t
             z = cvx.Variable(*w.shape)
             wplus = w + z
             obj = self.return_forecast.weight_expr_ahead(t, tau, wplus)
 
             costs, constr = [], []
             for cost in self.costs:
-                cost_expr, const_expr = cost.weight_expr_ahead(
-                    t, tau, wplus, z, value)
+                cost_expr, const_expr = cost.weight_expr_ahead(t, tau, wplus, z, value)
                 costs.append(cost_expr)
                 constr += const_expr
 
             obj -= sum(costs)
             constr += [cvx.sum(z) == 0]
-            constr += [con.weight_expr(t, wplus, z, value)
-                       for con in self.constraints]
+            for single_constr in self.constraints:
+                constr += single_constr.weight_expr(t, wplus, z, value)
 
             prob = cvx.Problem(cvx.Maximize(obj), constr)
             prob_arr.append(prob)
             z_vars.append(z)
             w = wplus
 
         # Terminal constraint.
         if self.terminal_weights is not None:
-            prob_arr[-1].constraints += [wplus == self.terminal_weights.values]
+            # prob_arr[-1].constraints += [wplus == self.terminal_weights.values]
+            prob_arr[-1] = cvx.Problem(
+                cvx.Maximize(obj), constr + [wplus == self.terminal_weights.values]
+            )
 
         sum(prob_arr).solve(solver=self.solver)
-        return pd.Series(index=portfolio.index,
-                         data=(z_vars[0].value * value))
+        return pd.Series(index=portfolio.index, data=(z_vars[0].value * value))
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/result.py` & `cvxportfolio-0.1.1/cvxportfolio/result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from __future__ import print_function
 import collections
 import numpy as np
 import pandas as pd
 import copy
 from .policies import MultiPeriodOpt
 
 
 def getFiscalQuarter(dt):
-    """Convert a time to a fiscal quarter.
-    """
+    """Convert a time to a fiscal quarter."""
     year = dt.year
     quarter = (dt.month - 1) // 3 + 1
     return "Q%i %s" % (quarter, year)
 
 
 class SimulationResult:
     """A container for the result of a simulation.
@@ -36,17 +33,24 @@
     Attributes:
         h_next: A dataframe of holdings over time.
         u: A dataframe of trades over time.
         tcosts: A series of transaction costs over time.
         borrow_costs: A series of borrow costs over time.
     """
 
-    def __init__(self, initial_portfolio, policy, cash_key, simulator,
-                 simulation_times=None, PPY=252,
-                 timedelta=pd.Timedelta("1 days")):
+    def __init__(
+        self,
+        initial_portfolio,
+        policy,
+        cash_key,
+        simulator,
+        simulation_times=None,
+        PPY=252,
+        timedelta=pd.Timedelta("1 days"),
+    ):
         """
         Initialize the result object.
 
         Args:
             initial_portfolio:
             policy:
             simulator:
@@ -61,85 +65,80 @@
         self.simulator = simulator
         self.policy = policy
 
     def summary(self):
         print(self._summary_string())
 
     def _summary_string(self):
-        data = collections.OrderedDict({
-            'Number of periods':
-                self.u.shape[0],
-            'Initial timestamp':
-                self.h.index[0],
-            'Final timestamp':
-                self.h.index[-1],
-            'Portfolio return (%)':
-                self.returns.mean() * 100 * self.PPY,
-            'Excess return (%)':
-                self.excess_returns.mean() * 100 * self.PPY,
-            'Excess risk (%)':
-                self.excess_returns.std() * 100 * np.sqrt(self.PPY),
-            'Sharpe ratio':
-                self.sharpe_ratio,
-            'Max. drawdown':
-                self.max_drawdown,
-            'Turnover (%)':
-                self.turnover.mean() * 100 * self.PPY,
-            'Average policy time (sec)':
-                self.policy_time.mean(),
-            'Average simulator time (sec)':
-                self.simulation_time.mean(),
-        })
+        data = collections.OrderedDict(
+            {
+                "Number of periods": self.u.shape[0],
+                "Initial timestamp": self.h.index[0],
+                "Final timestamp": self.h.index[-1],
+                "Portfolio return (%)": self.returns.mean() * 100 * self.PPY,
+                "Excess return (%)": self.excess_returns.mean() * 100 * self.PPY,
+                "Excess risk (%)": self.excess_returns.std() * 100 * np.sqrt(self.PPY),
+                "Sharpe ratio": self.sharpe_ratio,
+                "Max. drawdown": self.max_drawdown,
+                "Turnover (%)": self.turnover.mean() * 100 * self.PPY,
+                "Average policy time (sec)": self.policy_time.mean(),
+                "Average simulator time (sec)": self.simulation_time.mean(),
+            }
+        )
 
-        return (pd.Series(data=data).
-                to_string(float_format='{:,.3f}'.format))
+        return pd.Series(data=data).to_string(float_format="{:,.3f}".format)
 
     def log_data(self, name, t, entry):
         try:
             getattr(self, name).loc[t] = entry
         except AttributeError:
-            setattr(self, name,
-                    (pd.Series if np.isscalar(entry) else
-                     pd.DataFrame)(index=[t], data=[entry]))
+            setattr(
+                self,
+                name,
+                (pd.Series if np.isscalar(entry) else pd.DataFrame)(
+                    index=[t], data=[entry]
+                ),
+            )
 
     def log_policy(self, t, exec_time):
         self.log_data("policy_time", t, exec_time)
         # TODO mpo policy requires changes in the optimization_log methods
         if not isinstance(self.policy, MultiPeriodOpt):
             for cost in self.policy.costs:
-                self.log_data("policy_" + cost.__class__.__name__,
-                              t, cost.optimization_log(t))
+                self.log_data(
+                    "policy_" + cost.__class__.__name__, t, cost.optimization_log(t)
+                )
 
     def log_simulation(self, t, u, h_next, risk_free_return, exec_time):
         self.log_data("simulation_time", t, exec_time)
         self.log_data("u", t, u)
         self.log_data("h_next", t, h_next)
         self.log_data("risk_free_returns", t, risk_free_return)
         for cost in self.simulator.costs:
-            self.log_data("simulator_" + cost.__class__.__name__,
-                          t, cost.simulation_log(t))
+            self.log_data(
+                "simulator_" + cost.__class__.__name__, t, cost.simulation_log(t)
+            )
 
     @property
     def h(self):
         """
         Concatenate initial portfolio and h_next dataframe.
 
         """
         tmp = self.h_next.copy()
-        tmp.loc['last'] = np.nan
+        tmp.loc["last"] = np.nan
         tmp = self.h_next.shift(1)
         tmp.iloc[0] = self.initial_portfolio
         # TODO fix ?
         # tmp.loc[self.h_next.index[-1] + self.timedelta]=self.h_next.iloc[-1]
         return tmp
 
     @property
     def v(self):
-        """The value of the portfolio over time.
-        """
+        """The value of the portfolio over time."""
         return self.h.sum(axis=1)
 
     @property
     def profit(self):
         """The profit made, in dollars."""
         return self.v[-1] - self.v[0]
 
@@ -161,46 +160,42 @@
     @property
     def mean_return(self):
         """The annualized mean portfolio return."""
         return self.PPY * np.mean(self.returns)
 
     @property
     def returns(self):
-        """The returns R_t = (v_{t+1}-v_t)/v_t
-        """
+        """The returns R_t = (v_{t+1}-v_t)/v_t"""
         val = self.v
-        return pd.Series(data=val.values[1:] / val.values[:-1] - 1,
-                         index=val.index[:-1])
+        return pd.Series(
+            data=val.values[1:] / val.values[:-1] - 1, index=val.index[:-1]
+        )
 
     @property
     def growth_rates(self):
         """The growth rate log(v_{t+1}/v_t)"""
         return np.log(self.returns + 1)
 
     @property
     def annual_growth_rate(self):
-        """The annualized growth rate PPY/T sum_{t=1}^T log(v_{t+1}/v_t)
-        """
+        """The annualized growth rate PPY/T sum_{t=1}^T log(v_{t+1}/v_t)"""
         return self.growth_rates.sum() * self.PPY / self.growth_rates.size
 
     @property
     def annual_return(self):
-        """The annualized return in percent.
-        """
+        """The annualized return in percent."""
         ret = self.growth_rates
         return self._growth_to_return(ret.mean())
 
     def _growth_to_return(self, growth):
-        """Convert growth to annualized percentage return.
-        """
+        """Convert growth to annualized percentage return."""
         return 100 * (np.exp(self.PPY * growth) - 1)
 
     def get_quarterly_returns(self, benchmark=None):
-        """The annualized returns for each fiscal quarter.
-        """
+        """The annualized returns for each fiscal quarter."""
         ret = self.growth_rates
         quarters = ret.groupby(getFiscalQuarter).aggregate(np.mean)
         return self._growth_to_return(quarters)
 
     def get_best_quarter(self, benchmark=None):
         ret = self.get_quarterly_returns(benchmark)
         return (ret.argmax(), ret.max())
@@ -211,34 +206,34 @@
 
     @property
     def excess_returns(self):
         return self.returns - self.risk_free_returns
 
     @property
     def sharpe_ratio(self):
-        return np.sqrt(self.PPY) * np.mean(self.excess_returns) / \
-            np.std(self.excess_returns)
+        return (
+            np.sqrt(self.PPY)
+            * np.mean(self.excess_returns)
+            / np.std(self.excess_returns)
+        )
 
     @property
     def turnover(self):
-        """Turnover ||u_t||_1/v_t
-        """
+        """Turnover ||u_t||_1/v_t"""
         noncash_trades = self.u.drop(self.cash_key, axis=1)
         return np.abs(noncash_trades).sum(axis=1) / self.v
 
     @property
     def trading_days(self):
-        """The fraction of days with nonzero turnover.
-        """
+        """The fraction of days with nonzero turnover."""
         return (self.turnover.values > 0).sum() / self.turnover.size
 
     @property
     def max_drawdown(self):
-        """The maximum peak to trough drawdown in percent.
-        """
+        """The maximum peak to trough drawdown in percent."""
         val_arr = self.v.values
         max_dd_so_far = 0
         cur_max = val_arr[0]
         for val in val_arr[1:]:
             if val >= cur_max:
                 cur_max = val
             elif 100 * (cur_max - val) / cur_max > max_dd_so_far:
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/returns.py` & `cvxportfolio-0.1.1/cvxportfolio/returns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 
 import cvxpy as cvx
 from cvxportfolio.expression import Expression
 from .utils import values_in_time, null_checker
 
-__all__ = ['ReturnsForecast', 'MPOReturnsForecast',
-           'MultipleReturnsForecasts']
+__all__ = ["ReturnsForecast", "MPOReturnsForecast", "MultipleReturnsForecasts"]
 
 
 class BaseReturnsModel(Expression):
     pass
 
 
 class ReturnsForecast(BaseReturnsModel):
@@ -32,15 +29,15 @@
 
     Attributes:
       alpha_data: A dataframe of return estimates.
       delta_data: A confidence interval around the estimates.
       half_life: Number of days for alpha auto-correlation to halve.
     """
 
-    def __init__(self, returns, delta=0., gamma_decay=None, name=None):
+    def __init__(self, returns, delta=0.0, gamma_decay=None, name=None):
         null_checker(returns)
         self.returns = returns
         null_checker(delta)
         self.delta = delta
         self.gamma_decay = gamma_decay
         self.name = name
 
@@ -51,18 +48,16 @@
           t: time estimate is made.
           wplus: An expression for holdings.
           tau: time of alpha being estimated.
 
         Returns:
           An expression for the alpha.
         """
-        alpha = cvx.multiply(
-            values_in_time(self.returns, t), wplus)
-        alpha -= cvx.multiply(
-            values_in_time(self.delta, t), cvx.abs(wplus))
+        alpha = cvx.multiply(values_in_time(self.returns, t), wplus)
+        alpha -= cvx.multiply(values_in_time(self.delta, t), cvx.abs(wplus))
         return cvx.sum(alpha)
 
     def weight_expr_ahead(self, t, tau, wplus):
         """Returns the estimate at time t of alpha at time tau.
 
         Args:
           t: time estimate is made.
@@ -71,15 +66,15 @@
 
         Returns:
           An expression for the alpha.
         """
 
         alpha = self.weight_expr(t, wplus)
         if tau > t and self.gamma_decay is not None:
-            alpha *= (tau - t).days**(-self.gamma_decay)
+            alpha *= (tau - t).days ** (-self.gamma_decay)
         return alpha
 
 
 class MPOReturnsForecast(BaseReturnsModel):
     """A single alpha estimation.
 
     Attributes:
@@ -140,10 +135,9 @@
           tau: time of alpha being estimated.
 
         Returns:
           An expression for the alpha.
         """
         alpha = 0
         for idx, source in enumerate(self.alpha_sources):
-            alpha += source.weight_expr_ahead(t,
-                                              tau, wplus) * self.weights[idx]
+            alpha += source.weight_expr_ahead(t, tau, wplus) * self.weights[idx]
         return alpha
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/risks.py` & `cvxportfolio-0.1.1/cvxportfolio/risks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from abc import abstractmethod
 import logging
 
 import cvxpy as cvx
 import numpy as np
 import pandas as pd
 
 from .costs import BaseCost
 from .utils import values_in_time
+
 logger = logging.getLogger(__name__)
 
 
-__all__ = ['FullSigma', 'EmpSigma', 'SqrtSigma', 'WorstCaseRisk',
-           'RobustFactorModelSigma', 'RobustSigma',  'FactorModelSigma']
+__all__ = [
+    "FullSigma",
+    "EmpSigma",
+    "SqrtSigma",
+    "WorstCaseRisk",
+    "RobustFactorModelSigma",
+    "RobustSigma",
+    "FactorModelSigma",
+]
 
 
 # def locator(obj, t):
 #     """Picks last element before t."""
 #     try:
 #         if isinstance(obj, pd.Panel):
 #             return obj.iloc[obj.axes[0].get_loc(t, method='pad')]
@@ -44,38 +49,35 @@
 #         return obj.loc[prev_t, :]
 
 #     except AttributeError:  # obj not pandas
 #         return obj
 
 
 class BaseRiskModel(BaseCost):
-
     def __init__(self, **kwargs):
-        self.w_bench = kwargs.pop('w_bench', 0.)
+        self.w_bench = kwargs.pop("w_bench", 0.0)
         super(BaseRiskModel, self).__init__()
-        self.gamma_half_life = kwargs.pop('gamma_half_life', np.inf)
+        self.gamma_half_life = kwargs.pop("gamma_half_life", np.inf)
 
     def weight_expr(self, t, w_plus, z, value):
         self.expression = self._estimate(t, w_plus - self.w_bench, z, value)
         return self.gamma * self.expression, []
 
-    @abstractmethod
     def _estimate(self, t, w_plus, z, value):
         pass
 
     def weight_expr_ahead(self, t, tau, w_plus, z, value):
         """Estimate risk model at time tau in the future."""
         if self.gamma_half_life == np.inf:
-            gamma_multiplier = 1.
+            gamma_multiplier = 1.0
         else:
             decay_factor = 2 ** (-1 / self.gamma_half_life)
             # TODO not dependent on days
             gamma_init = decay_factor ** ((tau - t).days)
-            gamma_multiplier = gamma_init * \
-                (1 - decay_factor) / (1 - decay_factor)
+            gamma_multiplier = gamma_init * (1 - decay_factor) / (1 - decay_factor)
 
         return gamma_multiplier * self.weight_expr(t, w_plus, z, value)[0], []
 
     def optimization_log(self, t):
         if self.expression.value:
             return self.expression.value
         else:
@@ -90,135 +92,134 @@
             or single matrix.
 
     """
 
     def __init__(self, Sigma, **kwargs):
         self.Sigma = Sigma  # Sigma is either a matrix or a pd.Panel
         try:
-            assert(not pd.isnull(Sigma).values.any())
+            assert not pd.isnull(Sigma).values.any()
         except AttributeError:
-            assert (not pd.isnull(Sigma).any())
+            assert not pd.isnull(Sigma).any()
         super(FullSigma, self).__init__(**kwargs)
 
     def _estimate(self, t, wplus, z, value):
         try:
-            self.expression = cvx.quad_form(
-                wplus, values_in_time(self.Sigma, t))
+            self.expression = cvx.quad_form(wplus, values_in_time(self.Sigma, t))
         except TypeError:
-            self.expression = cvx.quad_form(
-                wplus, values_in_time(self.Sigma, t).values)
+            self.expression = cvx.quad_form(wplus, values_in_time(self.Sigma, t).values)
         return self.expression
 
 
 class EmpSigma(BaseRiskModel):
     """Empirical Sigma matrix, built looking at *lookback* past returns."""
 
     def __init__(self, returns, lookback, **kwargs):
         """returns is dataframe, lookback is int"""
         self.returns = returns
         self.lookback = lookback
-        assert(not np.any(pd.isnull(returns)))
+        assert not np.any(pd.isnull(returns))
         super(EmpSigma, self).__init__(**kwargs)
 
     def _estimate(self, t, wplus, z, value):
         idx = self.returns.index.get_loc(t)
         # TODO make sure pandas + cvxpy works
-        R = self.returns.iloc[max(idx - 1 - self.lookback, 0):idx - 1]
-        assert (R.shape[0] > 0)
+        R = self.returns.iloc[max(idx - 1 - self.lookback, 0) : idx - 1]
+        assert R.shape[0] > 0
         self.expression = cvx.sum_squares(R.values * wplus) / self.lookback
         return self.expression
 
 
 class SqrtSigma(BaseRiskModel):
-
     def __init__(self, sigma_sqrt, **kwargs):
         """returns is dataframe, lookback is int"""
         self.sigma_sqrt = sigma_sqrt
-        assert(not np.any(pd.isnull(sigma_sqrt)))
+        assert not np.any(pd.isnull(sigma_sqrt))
         super(SqrtSigma, self).__init__(**kwargs)
 
     def _estimate(self, t, wplus, z, value):
         # TODO make sure pandas + cvxpy works
         self.expression = cvx.sum_squares(wplus.T * self.sigma_sqrt.values)
         return self.expression
 
 
 class FactorModelSigma(BaseRiskModel):
-
     def __init__(self, exposures, factor_Sigma, idiosync, **kwargs):
         """Each is a pd.Panel (or ) or a vector/matrix"""
         self.exposures = exposures
-        assert (not exposures.isnull().values.any())
+        assert not exposures.isnull().values.any()
         self.factor_Sigma = factor_Sigma
-        assert (not factor_Sigma.isnull().values.any())
+        assert not factor_Sigma.isnull().values.any()
         self.idiosync = idiosync
-        assert(not idiosync.isnull().values.any())
+        assert not idiosync.isnull().values.any()
         super(FactorModelSigma, self).__init__(**kwargs)
 
     def _estimate(self, t, wplus, z, value):
-        self.expression = cvx.sum_squares(cvx.multiply(
-            np.sqrt(values_in_time(self.idiosync, t)), wplus)) + \
-            cvx.quad_form((wplus.T @ values_in_time(self.exposures, t).values.T).T,
-                          values_in_time(self.factor_Sigma, t).values)
+        self.expression = cvx.sum_squares(
+            cvx.multiply(np.sqrt(values_in_time(self.idiosync, t)), wplus)
+        ) + cvx.quad_form(
+            (wplus.T @ values_in_time(self.exposures, t).values.T).T,
+            values_in_time(self.factor_Sigma, t).values,
+        )
         return self.expression
 
 
 class RobustSigma(BaseRiskModel):
     """Implements covariance forecast error risk."""
 
     def __init__(self, Sigma, epsilon, **kwargs):
         self.Sigma = Sigma  # pd.Panel or matrix
         self.epsilon = epsilon  # pd.Series or scalar
         super(RobustSigma, self).__init__(**kwargs)
 
     def _estimate(self, t, wplus, z, value):
-        self.expression = cvx.quad_form(wplus, values_in_time(self.Sigma, t)) + \
-            values_in_time(self.epsilon, t) * \
-            (cvx.abs(wplus).T * np.diag(values_in_time(
-                self.Sigma, t)))**2
+        self.expression = (
+            cvx.quad_form(wplus, values_in_time(self.Sigma, t))
+            + values_in_time(self.epsilon, t)
+            * (cvx.abs(wplus).T * np.diag(values_in_time(self.Sigma, t))) ** 2
+        )
 
         return self.expression
 
 
 class RobustFactorModelSigma(BaseRiskModel):
     """Implements covariance forecast error risk."""
 
     def __init__(self, exposures, factor_Sigma, idiosync, epsilon, **kwargs):
         """Each is a pd.Panel (or ) or a vector/matrix"""
         self.exposures = exposures
-        assert (not exposures.isnull().values.any())
+        assert not exposures.isnull().values.any()
         self.factor_Sigma = factor_Sigma
-        assert (not factor_Sigma.isnull().values.any())
+        assert not factor_Sigma.isnull().values.any()
         self.idiosync = idiosync
-        assert(not idiosync.isnull().values.any())
+        assert not idiosync.isnull().values.any()
         self.epsilon = epsilon
         super(RobustFactorModelSigma, self).__init__(**kwargs)
 
     def _estimate(self, t, wplus, z, value):
         F = values_in_time(self.exposures, t)
         f = (wplus.T * F.T).T
         Sigma_F = values_in_time(self.factor_Sigma, t)
         D = values_in_time(self.idiosync, t)
-        self.expression = cvx.sum_squares(
-            cvx.multiply(np.sqrt(D), wplus)) + \
-            cvx.quad_form(f, Sigma_F) + \
-            self.epsilon * (cvx.abs(f).T * np.sqrt(np.diag(Sigma_F)))**2
+        self.expression = (
+            cvx.sum_squares(cvx.multiply(np.sqrt(D), wplus))
+            + cvx.quad_form(f, Sigma_F)
+            + self.epsilon * (cvx.abs(f).T * np.sqrt(np.diag(Sigma_F))) ** 2
+        )
 
         return self.expression
 
 
 class WorstCaseRisk(BaseRiskModel):
-
     def __init__(self, riskmodels, **kwargs):
         self.riskmodels = riskmodels
         super(WorstCaseRisk, self).__init__(**kwargs)
 
     def _estimate(self, t, wplus, z, value):
-        self.risks = [risk.weight_expr(t, wplus, z, value)
-                      for risk in self.riskmodels]
+        self.risks = [risk.weight_expr(t, wplus, z, value) for risk in self.riskmodels]
         return cvx.max_elemwise(*self.risks)
 
     def optimization_log(self, t):
         """Return data to log in the result object."""
-        return pd.Series(index=[model.__class__.__name__ for
-                                model in self.riskmodels],
-                         data=[risk.value[0, 0] for risk in self.risks])
+        return pd.Series(
+            index=[model.__class__.__name__ for model in self.riskmodels],
+            data=[risk.value[0, 0] for risk in self.risks],
+        )
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/simulator.py` & `cvxportfolio-0.1.1/cvxportfolio/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-"""
-Copyright 2016 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import copy
 import logging
 import time
 
 import multiprocess
 import numpy as np
@@ -31,27 +29,27 @@
 # TODO update benchmark weights (?)
 # Also could try jitting with numba.
 
 
 class MarketSimulator:
     logger = None
 
-    def __init__(self, market_returns, costs,
-                 market_volumes=None, cash_key='cash'):
+    def __init__(self, market_returns, costs, market_volumes=None, cash_key="cash"):
         """Provide market returns object and cost objects."""
         self.market_returns = market_returns
         if market_volumes is not None:
             self.market_volumes = market_volumes[
-                market_volumes.columns.difference([cash_key])]
+                market_volumes.columns.difference([cash_key])
+            ]
         else:
             self.market_volumes = None
 
         self.costs = costs
         for cost in self.costs:
-            assert (isinstance(cost, BaseCost))
+            assert isinstance(cost, BaseCost)
 
         self.cash_key = cash_key
 
     def propagate(self, h, u, t):
         """Propagates the portfolio forward over time period t, given trades u.
 
         Args:
@@ -59,192 +57,211 @@
             u: n vector with the stock trades (not cash)
             t: current time
 
         Returns:
             h_next: portfolio after returns propagation
             u: trades vector with simulated cash balance
         """
-        assert (u.index.equals(h.index))
+        assert u.index.equals(h.index)
 
         if self.market_volumes is not None:
             # don't trade if volume is null
-            null_trades = self.market_volumes.columns[
-                self.market_volumes.loc[t] == 0]
+            null_trades = self.market_volumes.columns[self.market_volumes.loc[t] == 0]
             if len(null_trades):
-                logging.info('No trade condition for stocks %s on %s' %
-                             (null_trades, t))
-                u.loc[null_trades] = 0.
+                logging.info(
+                    "No trade condition for stocks %s on %s" % (null_trades, t)
+                )
+                u.loc[null_trades] = 0.0
 
         hplus = h + u
         costs = [cost.value_expr(t, h_plus=hplus, u=u) for cost in self.costs]
         for cost in costs:
-            assert(not pd.isnull(cost))
-            assert(not np.isinf(cost))
+            assert not pd.isnull(cost)
+            assert not np.isinf(cost)
 
-        u[self.cash_key] = - sum(u[u.index != self.cash_key]) - sum(costs)
+        u[self.cash_key] = -sum(u[u.index != self.cash_key]) - sum(costs)
         hplus[self.cash_key] = h[self.cash_key] + u[self.cash_key]
 
-        assert (hplus.index.sort_values().equals(
-            self.market_returns.columns.sort_values()))
+        assert hplus.index.sort_values().equals(
+            self.market_returns.columns.sort_values()
+        )
         h_next = self.market_returns.loc[t] * hplus + hplus
 
-        assert (not h_next.isnull().values.any())
-        assert (not u.isnull().values.any())
+        assert not h_next.isnull().values.any()
+        assert not u.isnull().values.any()
         return h_next, u
 
-    def run_backtest(self, initial_portfolio, start_time, end_time,
-                     policy, loglevel=logging.WARNING):
-        """Backtest a single policy.
-        """
+    def run_backtest(
+        self, initial_portfolio, start_time, end_time, policy, loglevel=logging.WARNING
+    ):
+        """Backtest a single policy."""
         logging.basicConfig(level=loglevel)
 
-        results = SimulationResult(initial_portfolio=copy.copy(
-            initial_portfolio),
-            policy=policy, cash_key=self.cash_key,
-            simulator=self)
+        results = SimulationResult(
+            initial_portfolio=copy.copy(initial_portfolio),
+            policy=policy,
+            cash_key=self.cash_key,
+            simulator=self,
+        )
         h = initial_portfolio
 
         simulation_times = self.market_returns.index[
-            (self.market_returns.index >= start_time) &
-            (self.market_returns.index <= end_time)]
-        logging.info('Backtest started, from %s to %s' %
-                     (simulation_times[0], simulation_times[-1]))
+            (self.market_returns.index >= start_time)
+            & (self.market_returns.index <= end_time)
+        ]
+        logging.info(
+            "Backtest started, from %s to %s"
+            % (simulation_times[0], simulation_times[-1])
+        )
 
         for t in simulation_times:
-            logging.info('Getting trades at time %s' % t)
+            logging.info("Getting trades at time %s" % t)
             start = time.time()
             try:
                 u = policy.get_trades(h, t)
             except cvx.SolverError:
                 logging.warning(
-                    'Solver failed on timestamp %s. Default to no trades.' % t)
-                u = pd.Series(index=h.index, data=0.)
+                    "Solver failed on timestamp %s. Default to no trades." % t
+                )
+                u = pd.Series(index=h.index, data=0.0)
             end = time.time()
-            assert (not pd.isnull(u).any())
+            assert not pd.isnull(u).any()
             results.log_policy(t, end - start)
 
-            logging.info('Propagating portfolio at time %s' % t)
+            logging.info("Propagating portfolio at time %s" % t)
             start = time.time()
             h, u = self.propagate(h, u, t)
             end = time.time()
-            assert (not h.isnull().values.any())
-            results.log_simulation(t=t, u=u, h_next=h,
-                                   risk_free_return=self.market_returns.loc[
-                                       t, self.cash_key],
-                                   exec_time=end - start)
-
-        logging.info('Backtest ended, from %s to %s' %
-                     (simulation_times[0], simulation_times[-1]))
+            assert not h.isnull().values.any()
+            results.log_simulation(
+                t=t,
+                u=u,
+                h_next=h,
+                risk_free_return=self.market_returns.loc[t, self.cash_key],
+                exec_time=end - start,
+            )
+
+        logging.info(
+            "Backtest ended, from %s to %s"
+            % (simulation_times[0], simulation_times[-1])
+        )
         return results
 
-    def run_multiple_backtest(self, initial_portf, start_time,
-                              end_time, policies,
-                              loglevel=logging.WARNING, parallel=True):
-        """Backtest multiple policies.
-        """
+    def run_multiple_backtest(
+        self,
+        initial_portf,
+        start_time,
+        end_time,
+        policies,
+        loglevel=logging.WARNING,
+        parallel=True,
+    ):
+        """Backtest multiple policies."""
 
         def _run_backtest(policy):
-            return self.run_backtest(initial_portf, start_time, end_time,
-                                     policy, loglevel=loglevel)
+            return self.run_backtest(
+                initial_portf, start_time, end_time, policy, loglevel=loglevel
+            )
 
         num_workers = min(multiprocess.cpu_count(), len(policies))
         if parallel:
             workers = multiprocess.Pool(num_workers)
             results = workers.map(_run_backtest, policies)
             workers.close()
             return results
         else:
             return list(map(_run_backtest, policies))
 
     def what_if(self, time, results, alt_policies, parallel=True):
-        """Run alternative policies starting from given time.
-        """
+        """Run alternative policies starting from given time."""
         # TODO fix
         initial_portf = copy.copy(results.h.loc[time])
         all_times = results.h.index
-        alt_results = self.run_multiple_backtest(initial_portf,
-                                                 time,
-                                                 all_times[-1],
-                                                 alt_policies, parallel)
+        alt_results = self.run_multiple_backtest(
+            initial_portf, time, all_times[-1], alt_policies, parallel
+        )
         for idx, alt_result in enumerate(alt_results):
             alt_result.h.loc[time] = results.h.loc[time]
             alt_result.h.sort_index(axis=0, inplace=True)
         return alt_results
 
     @staticmethod
     def reduce_signal_perturb(initial_weights, delta):
         """Compute matrix of perturbed weights given initial weights."""
-        perturb_weights_matrix = \
-            np.zeros((len(initial_weights), len(initial_weights)))
+        perturb_weights_matrix = np.zeros((len(initial_weights), len(initial_weights)))
         for i in range(len(initial_weights)):
-            perturb_weights_matrix[i, :] = initial_weights / \
-                (1 - delta * initial_weights[i])
+            perturb_weights_matrix[i, :] = initial_weights / (
+                1 - delta * initial_weights[i]
+            )
             perturb_weights_matrix[i, i] = (1 - delta) * initial_weights[i]
         return perturb_weights_matrix
 
-    def attribute(self, true_results, policy,
-                  selector=None,
-                  delta=1,
-                  fit="linear",
-                  parallel=True):
+    def attribute(
+        self, true_results, policy, selector=None, delta=1, fit="linear", parallel=True
+    ):
         """Attributes returns over a period to individual alpha sources.
 
         Args:
             true_results: observed results.
             policy: the policy that achieved the returns.
                     Alpha model must be a stream.
             selector: A map from SimulationResult to time series.
             delta: the fractional deviation.
             fit: the type of fit to perform.
         Returns:
             A dict of alpha source to return series.
         """
         # Default selector looks at profits.
         if selector is None:
+
             def selector(result):
                 return result.v - sum(result.initial_portfolio)
 
         alpha_stream = policy.return_forecast
         assert isinstance(alpha_stream, MultipleReturnsForecasts)
         times = true_results.h.index
         weights = alpha_stream.weights
         assert np.sum(weights) == 1
         alpha_sources = alpha_stream.alpha_sources
         num_sources = len(alpha_sources)
         Wmat = self.reduce_signal_perturb(weights, delta)
         perturb_pols = []
         for idx in range(len(alpha_sources)):
             new_pol = copy.copy(policy)
-            new_pol.return_forecast = MultipleReturnsForecasts(alpha_sources,
-                                                               Wmat[idx, :])
+            new_pol.return_forecast = MultipleReturnsForecasts(
+                alpha_sources, Wmat[idx, :]
+            )
             perturb_pols.append(new_pol)
         # Simulate
         p0 = true_results.initial_portfolio
-        alt_results = self.run_multiple_backtest(p0, times[0], times[-1],
-                                                 perturb_pols, parallel=parallel)
+        alt_results = self.run_multiple_backtest(
+            p0, times[0], times[-1], perturb_pols, parallel=parallel
+        )
         # Attribute.
         true_arr = selector(true_results).values
         attr_times = selector(true_results).index
         Rmat = np.zeros((num_sources, len(attr_times)))
         for idx, result in enumerate(alt_results):
             Rmat[idx, :] = selector(result).values
         Pmat = cvx.Variable((num_sources, len(attr_times)))
         if fit == "linear":
             prob = cvx.Problem(cvx.Minimize(0), [Wmat @ Pmat == Rmat])
             prob.solve()
         elif fit == "least-squares":
             error = cvx.sum_squares(Wmat @ Pmat - Rmat)
-            prob = cvx.Problem(cvx.Minimize(error),
-                               [Pmat.T @ weights == true_arr])
+            prob = cvx.Problem(cvx.Minimize(error), [Pmat.T @ weights == true_arr])
             prob.solve()
         else:
             raise Exception("Unknown fitting method.")
         # Dict of results.
         wmask = np.tile(weights[:, np.newaxis], (1, len(attr_times))).T
-        data = pd.DataFrame(columns=[s.name for s in alpha_sources],
-                            index=attr_times,
-                            data=Pmat.value.T * wmask)
-        data['residual'] = true_arr - np.asarray((weights @ Pmat).value).ravel()
-        data['RMS error'] = np.asarray(
-            cvx.norm(Wmat @ Pmat - Rmat, 2, axis=0).value).ravel()
-        data['RMS error'] /= np.sqrt(num_sources)
+        data = pd.DataFrame(
+            columns=[s.name for s in alpha_sources],
+            index=attr_times,
+            data=Pmat.value.T * wmask,
+        )
+        data["residual"] = true_arr - np.asarray((weights @ Pmat).value).ravel()
+        data["RMS error"] = np.asarray(
+            cvx.norm(Wmat @ Pmat - Rmat, 2, axis=0).value
+        ).ravel()
+        data["RMS error"] /= np.sqrt(num_sources)
         return data
```

### Comparing `cvxportfolio-0.1.0/cvxportfolio/utils.py` & `cvxportfolio-0.1.1/cvxportfolio/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-"""
-Copyright 2017 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import logging
 
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 
 logger = logging.getLogger(__name__)
 
-__all__ = ['null_checker', 'non_null_data_args',
-           'values_in_time', 'plot_what_if']
+__all__ = ["null_checker", "non_null_data_args", "values_in_time", "plot_what_if"]
 
 
 def values_in_time(obj, t, tau=None):
     """Obtain value(s) of object at time t, or right before.
 
     Optionally specify time tau>=t for which we want a prediction,
     otherwise it is assumed tau = t.
@@ -51,20 +48,20 @@
     tau: np.Timestamp (or similar), or None. Time tau >= t
         of the prediction,  e.g., tau could be tomorrow, t
         today, and we ask for prediction of market volume tomorrow,
         made today. If None, then it is assumed tau = t.
 
     """
 
-    if hasattr(obj, '__call__'):
+    if hasattr(obj, "__call__"):
         return obj(t, tau)
 
     if isinstance(obj, pd.Series) or isinstance(obj, pd.DataFrame):
         try:
-            if isinstance(obj.index, pd.MultiIndex):
+            if not (tau is None) and isinstance(obj.index, pd.MultiIndex):
                 return obj.loc[(t, tau)]
             else:
                 return obj.loc[t]
         except KeyError:
             return obj
 
     return obj
@@ -75,26 +72,26 @@
     for result in alt_results:
         result.value.plot(label=result.pol_name, linestyle="--")
     plt.axvline(x=time, linestyle=":")
 
 
 def null_checker(obj):
     """Check if obj contains NaN."""
-    if (isinstance(obj, pd.DataFrame) or
-            isinstance(obj, pd.Series)):
+    if isinstance(obj, pd.DataFrame) or isinstance(obj, pd.Series):
         if np.any(pd.isnull(obj)):
-            raise ValueError('Data object contains NaN values', obj)
+            raise ValueError("Data object contains NaN values", obj)
     elif np.isscalar(obj):
         if np.isnan(obj):
-            raise ValueError('Data object contains NaN values', obj)
+            raise ValueError("Data object contains NaN values", obj)
     else:
-        raise TypeError('Data object can only be scalar or Pandas.')
+        raise TypeError("Data object can only be scalar or Pandas.")
 
 
 def non_null_data_args(f):
     def new_f(*args, **kwds):
         for el in args:
             null_checker(el)
         for el in kwds.values():
             null_checker(el)
         return f(*args, **kwds)
+
     return new_f
```

