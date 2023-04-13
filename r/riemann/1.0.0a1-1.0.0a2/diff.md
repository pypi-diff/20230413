# Comparing `tmp/riemann-1.0.0a1.tar.gz` & `tmp/riemann-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riemann-1.0.0a1.tar", last modified: Tue Apr 11 15:16:46 2023, max compression
+gzip compressed data, was "riemann-1.0.0a2.tar", last modified: Thu Apr 13 03:27:00 2023, max compression
```

## Comparing `riemann-1.0.0a1.tar` & `riemann-1.0.0a2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:16:46.825995 riemann-1.0.0a1/
--rw-rw-rw-   0        0        0     1085 2022-11-19 19:02:44.000000 riemann-1.0.0a1/LICENSE
--rw-rw-rw-   0        0        0     3502 2023-04-11 15:16:46.825995 riemann-1.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2023-01-06 20:40:44.000000 riemann-1.0.0a1/README.md
--rw-rw-rw-   0        0        0     1078 2023-04-11 15:14:54.000000 riemann-1.0.0a1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-11 15:16:46.825995 riemann-1.0.0a1/riemann.egg-info/
--rw-rw-rw-   0        0        0     3502 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 15:16:46.000000 riemann-1.0.0a1/riemann.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8605 2023-04-11 15:10:16.000000 riemann-1.0.0a1/riemann.py
--rw-rw-rw-   0        0        0       42 2023-04-11 15:16:46.825995 riemann-1.0.0a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 03:27:00.351694 riemann-1.0.0a2/
+-rw-rw-rw-   0        0        0     1085 2022-11-19 19:02:44.000000 riemann-1.0.0a2/LICENSE
+-rw-rw-rw-   0        0        0     3494 2023-04-13 03:27:00.351694 riemann-1.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0     2506 2023-04-13 03:23:56.000000 riemann-1.0.0a2/README.md
+-rw-rw-rw-   0        0        0     1078 2023-04-13 03:25:27.000000 riemann-1.0.0a2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-13 03:27:00.351694 riemann-1.0.0a2/riemann.egg-info/
+-rw-rw-rw-   0        0        0     3494 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 03:27:00.000000 riemann-1.0.0a2/riemann.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8190 2023-04-13 01:14:25.000000 riemann-1.0.0a2/riemann.py
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:27:00.351694 riemann-1.0.0a2/setup.cfg
```

### Comparing `riemann-1.0.0a1/LICENSE` & `riemann-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `riemann-1.0.0a1/PKG-INFO` & `riemann-1.0.0a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riemann
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A package for computing Riemann summations in n-dimensional space
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 Project-URL: Homepage, https://github.com/JacobLee23/riemann
 Project-URL: Documentation, https://riemann-py.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/JacobLee23/riemann/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -31,47 +31,46 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/riemann)](https://pypi.org/project/riemann)
 [![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/Jacoblee23/riemann)](https://github.com/JacobLee23/riemann/tags)
 
 ***
 
 ## Basic Usage
 
-**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function over a closed interval. The below code snippet computes the Riemann sum of $f(x) = x^{2}$ over the interval $[0, 1]$ using 10 partitions along the $x$ axis.
+**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function of several real variables over a closed multi-dimensional interval.
+
+The below code snippet computes the Riemann sum of $f(x) = x^{2} + x$ over the interal $[0, 2]$ using 10 partitions using the left rule along the $x$-axis.
 
 ```python
 >>> import riemann
 >>> from riemann import Interval
->>> f = lambda x: x ** 2
->>> intervals = [Interval(0, 1, 10)]
->>> methods = [riemann.LEFT]
->>> riemann.rsum(f, intervals, methods)
-Decimal('0.285')
+>>> f = lambda x: x ** 2 + x
+>>> intervals = [Interval(0, 2, 10)]
+>>> rules = [riemann.Left]
+>>> riemann.riemann_sum(f, intervals, rules)
+Decimal('2.28')
 ```
 
-However, **Riemann** is not restricted to computing Riemann sums only over one dimension. A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensional interval. The below code snippet computes the Riemann sum of $f(x, y) = x^{2} + y^{2}$ over the interval $x \in [0, 1], y \in [0, 1]$ using 10 partitions along the $x$ axis and 10 partitions along the $y$ axis.
+However, **riemann** is not restricted to computing Riemann sums only over one dimension.
+A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensionl interval.
+Additionally, different combinations of rules can be used to compute the Riemann sum.
+
+See [Quickstart](https://riemann-py.readthedocs.io/en/latest/user/quickstart.html) for additional example usage of the **riemann** module.
 
-```python
->>> import riemann
->>> from riemann import Interval
->>> f = lambda x, y: x ** 2 + y ** 2
->>> intervals = [Interval(0, 1, 10), Interval(0, 1, 10)]
->>> methods = [riemann.LEFT, riemann.LEFT]
->>> riemann.rsum(f, intervals, methods)
-Decimal('0.57')
-```
 
 ## Features
 
-- Fast computation of Riemann sum.
-- Support for computation of multi-dimensional Riemann sum.
-- Built-in support for left, middle, and right Riemann sum methods.
+- Fast computation of Riemann sums.
+- Supports the computation of multi-dimensional Riemann sums.
+- Supports the computation of the left, middle, and right Riemann sums.
+- Supports the computation of the trapezoidal Riemann sum.
+- Supports the computation of the upper and lower Darboux sums. (Under Development)
 
 ## Requirements
 
-**Riemann** requires Python 3.5+. This project does not require any additional dependencies.
+**Riemann** requires **Python 3.8+**. This project does not require any additional dependencies.
 
 ## Installation
 
 ```console
 $ pip install riemann
 ```
```

### Comparing `riemann-1.0.0a1/README.md` & `riemann-1.0.0a2/riemann.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: riemann
+Version: 1.0.0a2
+Summary: A package for computing Riemann summations in n-dimensional space
+Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
+Project-URL: Homepage, https://github.com/JacobLee23/riemann
+Project-URL: Documentation, https://riemann-py.readthedocs.io/en/latest/
+Project-URL: Issue Tracker, https://github.com/JacobLee23/riemann/issues/
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # riemann
 
 ![Repository Logo](docs/_static/riemann-logo.png)
 
 **Riemann**, a pure-Python package for computing Riemann sums of functions of several real variables.
 
 [![GitHub](https://img.shields.io/github/license/JacobLee23/riemann)](https://github.com/JacobLee23/riemann/blob/master/LICENSE)
@@ -9,47 +31,46 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/riemann)](https://pypi.org/project/riemann)
 [![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/Jacoblee23/riemann)](https://github.com/JacobLee23/riemann/tags)
 
 ***
 
 ## Basic Usage
 
-**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function over a closed interval. The below code snippet computes the Riemann sum of $f(x) = x^{2}$ over the interval $[0, 1]$ using 10 partitions along the $x$ axis.
+**Riemann** provides an intuitive syntax for calculating the Riemann sum of a function of several real variables over a closed multi-dimensional interval.
+
+The below code snippet computes the Riemann sum of $f(x) = x^{2} + x$ over the interal $[0, 2]$ using 10 partitions using the left rule along the $x$-axis.
 
 ```python
 >>> import riemann
 >>> from riemann import Interval
->>> f = lambda x: x ** 2
->>> intervals = [Interval(0, 1, 10)]
->>> methods = [riemann.LEFT]
->>> riemann.rsum(f, intervals, methods)
-Decimal('0.285')
+>>> f = lambda x: x ** 2 + x
+>>> intervals = [Interval(0, 2, 10)]
+>>> rules = [riemann.Left]
+>>> riemann.riemann_sum(f, intervals, rules)
+Decimal('2.28')
 ```
 
-However, **Riemann** is not restricted to computing Riemann sums only over one dimension. A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensional interval. The below code snippet computes the Riemann sum of $f(x, y) = x^{2} + y^{2}$ over the interval $x \in [0, 1], y \in [0, 1]$ using 10 partitions along the $x$ axis and 10 partitions along the $y$ axis.
+However, **riemann** is not restricted to computing Riemann sums only over one dimension.
+A similar syntax can be used to calculate the Riemann sum of a function of several real variables over a closed multi-dimensionl interval.
+Additionally, different combinations of rules can be used to compute the Riemann sum.
+
+See [Quickstart](https://riemann-py.readthedocs.io/en/latest/user/quickstart.html) for additional example usage of the **riemann** module.
 
-```python
->>> import riemann
->>> from riemann import Interval
->>> f = lambda x, y: x ** 2 + y ** 2
->>> intervals = [Interval(0, 1, 10), Interval(0, 1, 10)]
->>> methods = [riemann.LEFT, riemann.LEFT]
->>> riemann.rsum(f, intervals, methods)
-Decimal('0.57')
-```
 
 ## Features
 
-- Fast computation of Riemann sum.
-- Support for computation of multi-dimensional Riemann sum.
-- Built-in support for left, middle, and right Riemann sum methods.
+- Fast computation of Riemann sums.
+- Supports the computation of multi-dimensional Riemann sums.
+- Supports the computation of the left, middle, and right Riemann sums.
+- Supports the computation of the trapezoidal Riemann sum.
+- Supports the computation of the upper and lower Darboux sums. (Under Development)
 
 ## Requirements
 
-**Riemann** requires Python 3.5+. This project does not require any additional dependencies.
+**Riemann** requires **Python 3.8+**. This project does not require any additional dependencies.
 
 ## Installation
 
 ```console
 $ pip install riemann
 ```
```

### Comparing `riemann-1.0.0a1/pyproject.toml` & `riemann-1.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel >= 0.29.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "riemann"
-version = "1.0.0-a.1"
+version = "1.0.0-a.2"
 authors = [
   { name="Jacob Lee", email="Jacob.J.Lee@outlook.com" },
 ]
 description = "A package for computing Riemann summations in n-dimensional space"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `riemann-1.0.0a1/riemann.py` & `riemann-1.0.0a2/riemann.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,138 @@
 r"""
-A pure-Python package for computing :math:`n`-dimensional Riemann sums.
-
------
-
-Let :math:`f: [a,b] \rightarrow \mathbb{R}` be a function defined on a closed interval
-:math:`[a, b]` of the real numbers, :math:`\mathbb(R)`, and
-
-.. math::
-
-    P = ([x_{0}, x_{1}], [x_{1}, x_{2}], \dots , [x_{n-1}, x_{n}]),
-
-a partition of :math:`[a, b]`, that is
-
-.. math::
-
-    a = x_{0} < x_{1} < x_{2} < \dots < x_{n} = b.
-
-A Riemann sum of :math:`S` of :math:`f` over :math:`[a, b]` with partition :math:`P` is defined as
-
-.. math::
-
-    S = \sum_{i=1}^{n} f(x_{i}^{*}) \Delta x_{i},
-
-where :math:`\Delta x_{i} = x_{i} - x_{i-1}` and :math:`x_{i}^{*} \in [x_{i-1}, x_{i}]`. One might
-produce different Riemann sum depending on which :math:`x_{i}^{*}`'s are chosen.
-
-Higher dimensional Riemann sums follow a similar pattern. An :math:`n`-dimensional Riemann sum is
-
-.. math::
-
-    S = \sum_{i=1}^{n} f(P_{i}^{*}) \Delta V_{i}
-
-where :math:`P_{i}^{*} \in V_{i}`, that is, it is a point in the :math:`n`-dimensional cell
-:math:`V_{i}` with :math:`n`-dimensional volume :math:`\Delta V_{i}`.
-
-`Source <https://en.wikipedia.org/wiki/Riemann_sum>`_
+**Riemann**, a pure-Python package for computing :math:`n`-dimensional Riemann sums.
 """
 
 from decimal import Decimal
 import functools
 import inspect
 import itertools
 from numbers import Number
 import operator
 import typing
 
 
 @typing.runtime_checkable
 class FunctionSRV(typing.Protocol):
     r"""
-    Callable type that represents a function of several real variables. Inherits from
-    :class:`typing.Protocol`.
+    Callable type that represents a function of several real variables.
+    Inherits from :class:`typing.Protocol`.
 
     .. math::
 
         f: \mathbb{R}^{n} \rightarrow \mathbb{R}
 
     Instances of this class are analagous to the following function:
 
     .. code-block:: python
 
+        >>> from numbers import Number
         >>> def function(*x: Number) -> Number: ...
 
     The callable object takes any number of :class:`numbers.Number` objects and returns a single
     :class:`numbers.Number` object.
 
     This class uses the :func:`typing.runtime_checkable` decorator, so :func:`isinstance` can be
     to determine whether a callable object is an instance of this class:
 
-    .. code-block:: python
+    .. doctest:: python
 
+        >>> from numbers import Number
         >>> from riemann import FunctionSRV
-        >>> isinstance(lambda: 0, FunctionSRV)
+        >>> def function(*x: Number) -> Number: ...
+        >>> isinstance(function, FunctionSRV)
+        True
+        >>> def f():
+        ...     return 0
+        >>> isinstance(f, FunctionSRV)
         True
-        >>> isinstance(lambda x: x, FunctionSRV)
+        >>> def g(x):
+        ...     return x
+        >>> isinstance(g, FunctionSRV)
         True
-        >>> isinstance(lambda x, y: x * y, FunctionSRV)
+        >>> def h(x, y):
+        ...     return x * y
+        >>> isinstance(h, FunctionSRV)
         True
-        >>> isinstance(lambda x, y, z: (x ** 2) * (y ** 2) * (z ** 2), FunctionSRV)
+        >>> def i(x, y, z):
+        ...     return x ** 2 + y ** 2 + z ** 2
+        >>> isinstance(i, FunctionSRV)
         True
     """
     def __call__(self, *args: Number) -> Number: ...
 
 
-class RSumMethod:
+class RSumRule:
     r"""
-    .. math::
-
-        \Delta x = \frac{b-a}{n}, i \in \{0, 1, \dots, n-1\}
-
-    :param lower: The lower bound of the interval of summation
-    :param length: The length of each partition of the interval of summation
-    :return: The value of :math:`x_{i}^{*}`
+    Specifies that a particular Riemann sum rule should be used over an interval.
     """
-    def __call__(self, lower: Decimal, length: Decimal) -> Decimal:
+    @classmethod
+    def value(cls, lower: Decimal, length: Decimal) -> Decimal:
+        r"""
+        :param lower: The lower bound of the interval of summation
+        :param length: The length of each partition of the interval of summation
+        :return: The value of :math:`x_{i}^{*}`
+        """
         raise NotImplementedError
 
 
-class Left(RSumMethod):
+class Left(RSumRule):
     r"""
-    Specifies that the Left Riemann Sum method should be used over the corresponding dimension.
-    Inherits from :py:class:`RSumMethod`.
+    Specifies that the left rule should be used to compute the Riemann sum over an interval.
+    """
+    @classmethod
+    def value(cls, lower: Decimal, length: Decimal) -> Decimal:
+        r"""
+        .. math::
 
-    .. math::
+            x_{i}^{*} = x_{i-1} = a + i \Delta x
 
-        x_{i}^{*} = x_{i-1} = a + i \Delta x
-    """
-    def __call__(self, lower: Decimal, length: Decimal) -> Decimal:
+        :param lower: The lower bound of the interval of summation
+        :param length: The length of each partition of the interval of summation
+        :return: The value of :math:`x_{i}^{*}`
+        """
         return lower
 
 
-class Middle(RSumMethod):
+class Middle(RSumRule):
     r"""
-    Specifies that the Middle Riemann Sum method should be used over the corresponding dimension.
-    Inherits from :py:class:`RSumMethod`.
-
-    .. math::
-
-        x_{i}^{*} = \frac{x_{i-1} + x_{i}}{2} = a + \frac{1}{2} i \Delta x
+    Specifies that the midpoint rule should be used to compute the Riemann sum over an interval.
     """
-    def __call__(self, lower: Decimal, length: Decimal) -> Decimal:
+    @classmethod
+    def value(cls, lower: Decimal, length: Decimal) -> Decimal:
+        r"""
+        .. math::
+        
+            x_{i}^{*} = \frac{x_{i-1} + x_{i}}{2} = a + (i + \frac{1}{2}) \Delta x
+            
+        :param lower: The lower bound of the interval of summation
+        :param length: The length of each partition of the interval of summation
+        :return: The value of :math:`x_{i}^{*}`
+        """
         return lower + length / 2
 
 
-class Right(RSumMethod):
+class Right(RSumRule):
     r"""
-    Specifies that the Right Riemann Sum method should be used over the corresponding dimension.
-    Inherits from :py:class:`RSumMethod`.
-
-    .. math::
-
-        x_{i}^{*} = x_{i} = a + (i + 1) \Delta x
+    Specifies that the right rule should be used to compute the Riemann sum over an interval.
     """
-    def __call__(self, lower: Decimal, length: Decimal) -> Decimal:
+    @classmethod
+    def value(cls, lower: Decimal, length: Decimal) -> Decimal:
+        r"""
+        .. math::
+        
+            x_{i}^{*} = x_{i} = a + (i + 1) \Delta x
+            
+        :param lower: The lower bound of the interval of summation
+        :param length: The length of each partition of the interval of summation
+        :return: The value of :math:`x_{i}^{*}`
+        """
         return lower + length
 
 
-LEFT, MIDDLE, RIGHT = Left(), Middle(), Right()
-
-
 class Interval:
     """
     Represents the closed interval over which a Riemann sum is computed.
 
     :param lower: The lower bound of the interval
     :param upper: The upper bound of the interval
     :return: The number of partitions dividing the interval
@@ -158,91 +148,84 @@
         return "{}(lower={}, upper={}, npartitions={})".format(
             type(self).__name__,
             self.lower,
             self.upper,
             self.npartitions
         )
 
-    def partitions(self, method: RSumMethod) -> typing.Generator[Decimal, None, None]:
+    def partitions(self, rule: RSumRule) -> typing.Generator[Decimal, None, None]:
         """
-        :param method: The method to use for calculating the Riemann sum
+        :param rule: The rule to use for compute the Riemann sum
         :return: A generator of the values of each partition of the interval
         """
         lower, length = self.lower, self.length
 
         for _ in range(self.npartitions):
-            yield method(lower, length)
+            yield rule.value(lower, length)
 
             lower += length
 
 
 def riemann_sum(
-    function: FunctionSRV, intervals: typing.Sequence[Interval], methods: typing.Sequence[RSumMethod]
+    function: FunctionSRV,
+    intervals: typing.Sequence[Interval],
+    rules: typing.Sequence[typing.Type[RSumRule]]
 ):
     r"""
-    Computes the Riemann Sum of a function of several variables over a closed multidimensional
-    interval using indicated Riemann sum methods.
-
-    The number of parameters of ``function``, the number of elements in ``intervals``, and the
-    number of elements in ``methods`` all must be equal. In other words, every parameter in
-    ``function`` must correspond to exactly one element in ``intervals`` and one element in
-    ``methods``.
-
-    .. note::
+    Computes the Riemann sum of a function of several variables over a closed multidimensional
+    interval using specified Riemann sum rules.
 
-        The order of ``intervals`` and ``methods`` are significant.
+    The following must all be equal:
 
-        The first parameter of ``function`` corresponds to ``intervals[0]`` and ``methods[0]``, the
-        second to ``intervals[1]`` and ``methods[1]``, the third to ``intervals[2]`` and
-        ``methods[2]``, etc.
+    - The number of parameters of ``function``
+    - The number of elements in ``intervals``
+    - The number of elements in ``rules``.
+    
+    In other words, every parameter in ``function`` must correspond to exactly one element in
+    ``intervals`` and one element in ``rules``.
+
+    The order of ``intervals`` and ``rules`` is significant.
+    During computation, each parameter of ``function`` is mapped to its corresponding element in
+    ``intervals`` and its corresponding element in ``rules``.
+    That is, the first parameter of ``function`` corresopnds to ``intervals[0]`` and ``rules[0]``,
+    the second to ``intervals[1]`` and ``rules[1]``, etc.
 
     :param function: A callable object representing function of several real variables
     :param intervals: The closed intervals over which the Riemann sum is calculated
-    :param methods: The methods to use for calculating the Riemann sum
-    :return: The value of the Riemann Sum over the indicated intervals using the indicated methods
-    :raise ValueError: Length of the ``function`` parameter list, ``intervals``, and ``methods`` are unequal
+    :param rules: The rules to use for calculating the Riemann sum
+    :return: The value of the Riemann sum over the indicated intervals using the indicated rules
+    :raise ValueError: The ``function`` parameter list, ``intervals``, and ``rules`` are not equal in length
     """
     ndimensions = len(inspect.signature(function).parameters)
 
-    intervals = [x if isinstance(x, Interval) else Interval(*x) for x in intervals]
     if len(intervals) != ndimensions:
         raise ValueError(
-            "The length of 'intervals' and the 'function' parameter list must be equal"
+            "The length of 'intervals' must equal the length of the parameter list of 'funcion'"
         )
-
-    if len(methods) != ndimensions:
+    if len(rules) != ndimensions:
         raise ValueError(
-            "The length of 'methods' and the 'function' parameter list must be equal"
+            "The length of 'rules' must equal the length of the parameter list of 'function'"
         )
 
     delta = functools.reduce(operator.mul, (x.length for x in intervals))
-    values = (x.partitions(m) for x, m in zip(intervals, methods))
+    values = (x.partitions(r) for x, r in zip(intervals, rules))
 
     return (sum(function(*v) for v in itertools.product(*values)) * delta).normalize()
 
 
 def trapezoidal_rule(
     function: FunctionSRV, intervals: typing.Sequence[Interval]
 ):
     r"""
-    Computes the Riemann Sum of a function of several variables over a closed multidimensional
-    interval using the trapezoidal rule.
-
-    The number of parameters of ``function`` and the number of elements in ``intervals`` must be
-    equal. In other words, every parameter in ``function`` must correspond to exactly one element
-    in ``intervals``.
-
-    .. note::
-
-        The order of ``intervals`` is significant.
-
-        The first parameter of ``function`` corresponds to ``intervals[0]``, the second to
-        ``intervals[1]``, the third to ``intervals[2]``, etc.
+    Computes the Riemann sum of a function of several variables over a closed multidimensional
+    interval using the trapezoidal.
 
+    This function utilizes the functionality of :py:func:`riemann_sum` to compute the Riemann sum.
+    
     :param function: A callable object representing function of several real variables
     :param intervals: The closed intervals over which the Riemann sum is calculated
     :return: The value of the Riemann sum over the indicated intervals using the trapezoidal rule
     """
-    methods = itertools.product((Left, Right), repeat=len(intervals))
+    rules = itertools.product((Left, Right), repeat=len(intervals))
     ncombinations = Decimal(2) ** len(intervals)
 
-    return (sum(riemann_sum(function, intervals, m) for m in methods) / ncombinations).normalize()
+    return (sum(riemann_sum(function, intervals, r) for r in rules) / ncombinations).normalize()
```

