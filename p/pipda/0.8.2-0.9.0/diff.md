# Comparing `tmp/pipda-0.8.2.tar.gz` & `tmp/pipda-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipda-0.8.2.tar", max compression
+gzip compressed data, was "pipda-0.9.0.tar", max compression
```

## Comparing `pipda-0.8.2.tar` & `pipda-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2022-10-17 02:55:45.855784 pipda-0.8.2/LICENSE
--rw-r--r--   0        0        0     5166 2022-10-17 02:55:45.855784 pipda-0.8.2/README.md
--rw-r--r--   0        0        0      441 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/__init__.py
--rw-r--r--   0        0        0     3434 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/context.py
--rw-r--r--   0        0        0     6636 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/expression.py
--rw-r--r--   0        0        0     6328 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/function.py
--rw-r--r--   0        0        0     2452 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/operator.py
--rw-r--r--   0        0        0     4802 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/piping.py
--rw-r--r--   0        0        0     3233 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/reference.py
--rw-r--r--   0        0        0      831 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/symbolic.py
--rw-r--r--   0        0        0     4354 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/utils.py
--rw-r--r--   0        0        0     9936 2022-10-17 02:55:45.855784 pipda-0.8.2/pipda/verb.py
--rw-r--r--   0        0        0      984 2022-10-17 02:55:45.855784 pipda-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 pipda-0.8.2/setup.py
--rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 pipda-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-10-28 22:39:34.031527 pipda-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5166 2022-10-28 22:39:34.031527 pipda-0.9.0/README.md
+-rw-r--r--   0        0        0      467 2022-10-28 22:39:34.031527 pipda-0.9.0/pipda/__init__.py
+-rw-r--r--   0        0        0     3434 2022-10-28 22:39:34.031527 pipda-0.9.0/pipda/context.py
+-rw-r--r--   0        0        0     7019 2022-10-28 22:39:34.031527 pipda-0.9.0/pipda/expression.py
+-rw-r--r--   0        0        0     6328 2022-10-28 22:39:34.031527 pipda-0.9.0/pipda/function.py
+-rw-r--r--   0        0        0     2452 2022-10-28 22:39:34.031527 pipda-0.9.0/pipda/operator.py
+-rw-r--r--   0        0        0     4802 2022-10-28 22:39:34.031527 pipda-0.9.0/pipda/piping.py
+-rw-r--r--   0        0        0     3233 2022-10-28 22:39:34.035527 pipda-0.9.0/pipda/reference.py
+-rw-r--r--   0        0        0      831 2022-10-28 22:39:34.035527 pipda-0.9.0/pipda/symbolic.py
+-rw-r--r--   0        0        0     4354 2022-10-28 22:39:34.035527 pipda-0.9.0/pipda/utils.py
+-rw-r--r--   0        0        0     9936 2022-10-28 22:39:34.035527 pipda-0.9.0/pipda/verb.py
+-rw-r--r--   0        0        0      984 2022-10-28 22:39:34.035527 pipda-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 pipda-0.9.0/setup.py
+-rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 pipda-0.9.0/PKG-INFO
```

### Comparing `pipda-0.8.2/LICENSE` & `pipda-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/README.md` & `pipda-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/context.py` & `pipda-0.9.0/pipda/context.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/expression.py` & `pipda-0.9.0/pipda/expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,30 @@
 
 
 class Expression(ABC):
     """The abstract Expression class"""
 
     _pipda_operator = None
 
+    def _pipda_array_func(
+        self,
+        ufunc: Callable,
+        method: str,
+        *inputs: Any,
+        **kwargs: Any,
+    ) -> FunctionCall:
+        """Allow numpy array function to work on Expression objects"""
+        from .function import Function, FunctionCall
+
+        if method != "__call__":
+            ufunc = getattr(ufunc, method)
+
+        fun = Function(ufunc, None, {})
+        return FunctionCall(fun, *inputs, **kwargs)
+
     def __array_ufunc__(
         self,
         ufunc: Callable,
         method: str,
         *inputs: Any,
         **kwargs: Any,
     ) -> FunctionCall:
@@ -71,33 +87,21 @@
 
         if (
             ufunc.__name__ == PIPING_OPS[VerbCall.PIPING][2]
             and isinstance(inputs[1], VerbCall)
             and len(inputs) == 2
             and method == "__call__"
         ):
-            # We can't patch numpy.ndarray
+            # We can't patch numpy.
+            # So make
+            # np.ndarray([1, 2]) >> verb()
+            # work
             return inputs[1]._pipda_eval(inputs[0])
 
-        from .function import Function, FunctionCall
-
-        if method == "reduce":
-            ufunc = ufunc.reduce
-
-        elif method == "accumulate":
-            ufunc = ufunc.accumulate
-
-        elif method == "reduceat":
-            ufunc = ufunc.reduceat
-
-        elif method == "outer":
-            ufunc = ufunc.outer
-
-        fun = Function(ufunc, None, {})
-        return FunctionCall(fun, *inputs, **kwargs)
+        return self._pipda_array_func(ufunc, method, *inputs, **kwargs)
 
     def __hash__(self) -> int:
         """Make it hashable"""
         return hash(id(self))
 
     def __getattr__(self, name: str) -> ReferenceAttr:
         """Whenever `expr.attr` is encountered,
@@ -199,7 +203,13 @@
     @abstractmethod
     def _pipda_eval(
         self,
         data: Any,
         context: ContextBase = None,
     ) -> Any:
         """Evaluate the expression using given data"""
+
+
+def register_expr_array_func(func: Callable) -> Callable:
+    """Register a function to be used as __array_ufunc__ on Expression"""
+    Expression._pipda_array_func = func  # type: ignore
+    return func
```

### Comparing `pipda-0.8.2/pipda/function.py` & `pipda-0.9.0/pipda/function.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/operator.py` & `pipda-0.9.0/pipda/operator.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/piping.py` & `pipda-0.9.0/pipda/piping.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/reference.py` & `pipda-0.9.0/pipda/reference.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/symbolic.py` & `pipda-0.9.0/pipda/symbolic.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/utils.py` & `pipda-0.9.0/pipda/utils.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pipda/verb.py` & `pipda-0.9.0/pipda/verb.py`

 * *Files identical despite different names*

### Comparing `pipda-0.8.2/pyproject.toml` & `pipda-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pipda"
-version = "0.8.2"
+version = "0.9.0"
 readme = "README.md"
 description = "A framework for data piping in python"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 executing = "^1.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
-pytest-cov = "^3"
+pytest-cov = "^4"
 numpy = "^1.20"
 pandas = "^1.3"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pipda-0.8.2/setup.py` & `pipda-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['executing>=1.1.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'pipda',
-    'version': '0.8.2',
+    'version': '0.9.0',
     'description': 'A framework for data piping in python',
     'long_description': "# pipda\n\n[![Pypi][7]][8] [![Github][9]][10] [![PythonVers][11]][8] [![Codacy][16]][14] [![Codacy coverage][15]][14] ![Docs building][13] ![Building][12]\n\nA framework for data piping in python\n\nInspired by [siuba][1], [dfply][2], [plydata][3] and [dplython][4], but with simple yet powerful APIs to mimic the `dplyr` and `tidyr` packages in python\n\n[API][17] | [Change Log][18] | [Documentation][19]\n\n## Installation\n\n```shell\npip install -U pipda\n```\n\n## Usage\n\n### Verbs\n\nVerbs are functions next to the piping sign (`>>`) receiving the data directly.\n\n```python\nimport pandas as pd\nfrom pipda import (\n    register_verb,\n    register_func,\n    register_operator,\n    evaluate_expr,\n    Operator,\n    Symbolic,\n    Context\n)\n\nf = Symbolic()\n\ndf = pd.DataFrame({\n    'x': [0, 1, 2, 3],\n    'y': ['zero', 'one', 'two', 'three']\n})\n\ndf\n\n#      x    y\n# 0    0    zero\n# 1    1    one\n# 2    2    two\n# 3    3    three\n\n@register_verb(pd.DataFrame)\ndef head(data, n=5):\n    return data.head(n)\n\ndf >> head(2)\n#      x    y\n# 0    0    zero\n# 1    1    one\n\n@register_verb(pd.DataFrame, context=Context.EVAL)\ndef mutate(data, **kwargs):\n    data = data.copy()\n    for key, val in kwargs.items():\n        data[key] = val\n    return data\n\ndf >> mutate(z=1)\n#    x      y  z\n# 0  0   zero  1\n# 1  1    one  1\n# 2  2    two  1\n# 3  3  three  1\n\ndf >> mutate(z=f.x)\n#    x      y  z\n# 0  0   zero  0\n# 1  1    one  1\n# 2  2    two  2\n# 3  3  three  3\n```\n\n### Functions used as verb arguments\n\n```python\n# verb can be used as an argument passed to another verb\n# dep=True make `data` argument invisible while calling\n@register_verb(pd.DataFrame, context=Context.EVAL, dep=True)\ndef if_else(data, cond, true, false):\n    cond.loc[cond.isin([True]), ] = true\n    cond.loc[cond.isin([False]), ] = false\n    return cond\n\n# The function is then also a singledispatch generic function\n\ndf >> mutate(z=if_else(f.x>1, 20, 10))\n#    x      y   z\n# 0  0   zero  10\n# 1  1    one  10\n# 2  2    two  20\n# 3  3  three  20\n```\n\n```python\n# function without data argument\n@register_func\ndef length(strings):\n    return [len(s) for s in strings]\n\ndf >> mutate(z=length(f.y))\n\n#    x     y    z\n# 0  0  zero    4\n# 1  1   one    3\n# 2  2   two    3\n# 3  3 three    5\n```\n\n### Context\n\nThe context defines how a reference (`f.A`, `f['A']`, `f.A.B` is evaluated)\n\n```python\n@register_verb(pd.DataFrame, context=Context.SELECT)\ndef select(df, *columns):\n    return df[list(columns)]\n\ndf >> select(f.x, f.y)\n#    x     y\n# 0  0  zero\n# 1  1   one\n# 2  2   two\n# 3  3 three\n```\n\n## How it works\n\n```R\ndata %>% verb(arg1, ..., key1=kwarg1, ...)\n```\n\nThe above is a typical `dplyr`/`tidyr` data piping syntax.\n\nThe counterpart python syntax we expect is:\n\n```python\ndata >> verb(arg1, ..., key1=kwarg1, ...)\n```\n\nTo implement that, we need to defer the execution of the `verb` by turning it into a `Verb` object, which holds all information of the function to be executed later. The `Verb` object won't be executed until the `data` is piped in. It all thanks to the [`executing`][5] package to let us determine the ast nodes where the function is called. So that we are able to determine whether the function is called in a piping mode.\n\nIf an argument is referring to a column of the data and the column will be involved in the later computation, the it also needs to be deferred. For example, with `dplyr` in `R`:\n\n```R\ndata %>% mutate(z=a)\n```\n\nis trying add a column named `z` with the data from column `a`.\n\nIn python, we want to do the same with:\n\n```python\ndata >> mutate(z=f.a)\n```\n\nwhere `f.a` is a `Reference` object that carries the column information without fetching the data while python sees it immmediately.\n\nHere the trick is `f`. Like other packages, we introduced the `Symbolic` object, which will connect the parts in the argument and make the whole argument an `Expression` object. This object is holding the execution information, which we could use later when the piping is detected.\n\n## Documentation\n\n[https://pwwang.github.io/pipda/][19]\n\nSee also [datar][6] for realcase usages.\n\n[1]: https://github.com/machow/siuba\n[2]: https://github.com/kieferk/dfply\n[3]: https://github.com/has2k1/plydata\n[4]: https://github.com/dodger487/dplython\n[5]: https://github.com/alexmojaki/executing\n[6]: https://github.com/pwwang/datar\n[7]: https://img.shields.io/pypi/v/pipda?style=flat-square\n[8]: https://pypi.org/project/pipda/\n[9]: https://img.shields.io/github/v/tag/pwwang/pipda?style=flat-square\n[10]: https://github.com/pwwang/pipda\n[11]: https://img.shields.io/pypi/pyversions/pipda?style=flat-square\n[12]: https://img.shields.io/github/workflow/status/pwwang/pipda/Build%20and%20Deploy?style=flat-square\n[13]: https://img.shields.io/github/workflow/status/pwwang/pipda/Build%20Docs?style=flat-square\n[14]: https://app.codacy.com/gh/pwwang/pipda/dashboard\n[15]: https://img.shields.io/codacy/coverage/75d312da24c94bdda5923627fc311a99?style=flat-square\n[16]: https://img.shields.io/codacy/grade/75d312da24c94bdda5923627fc311a99?style=flat-square\n[17]: https://pwwang.github.io/pipda/api/pipda/\n[18]: https://pwwang.github.io/pipda/CHANGELOG/\n[19]: https://pwwang.github.io/pipda/\n",
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipda-0.8.2/PKG-INFO` & `pipda-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipda
-Version: 0.8.2
+Version: 0.9.0
 Summary: A framework for data piping in python
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

