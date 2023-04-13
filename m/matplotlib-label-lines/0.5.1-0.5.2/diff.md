# Comparing `tmp/matplotlib_label_lines-0.5.1.tar.gz` & `tmp/matplotlib_label_lines-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_label_lines-0.5.1.tar", last modified: Fri Feb 25 14:22:26 2022, max compression
+gzip compressed data, was "matplotlib_label_lines-0.5.2.tar", last modified: Thu Apr 13 09:12:25 2023, max compression
```

## Comparing `matplotlib_label_lines-0.5.1.tar` & `matplotlib_label_lines-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ccc       (1000) ccc       (1000)        0 2022-02-25 14:22:26.838056 matplotlib_label_lines-0.5.1/
--rw-r--r--   0 ccc       (1000) ccc       (1000)     1072 2017-12-31 16:20:51.000000 matplotlib_label_lines-0.5.1/LICENSE
--rw-r--r--   0 ccc       (1000) ccc       (1000)       26 2021-01-15 10:44:15.000000 matplotlib_label_lines-0.5.1/MANIFEST.in
--rw-r--r--   0 ccc       (1000) ccc       (1000)     3755 2022-02-25 14:22:26.838056 matplotlib_label_lines-0.5.1/PKG-INFO
--rw-r--r--   0 ccc       (1000) ccc       (1000)     2725 2022-02-25 14:22:11.000000 matplotlib_label_lines-0.5.1/Readme.md
-drwxr-xr-x   0 ccc       (1000) ccc       (1000)        0 2022-02-25 14:22:26.838056 matplotlib_label_lines-0.5.1/labellines/
--rw-r--r--   0 ccc       (1000) ccc       (1000)       97 2022-02-25 14:22:11.000000 matplotlib_label_lines-0.5.1/labellines/__init__.py
--rw-r--r--   0 ccc       (1000) ccc       (1000)     7835 2022-02-24 15:31:25.000000 matplotlib_label_lines-0.5.1/labellines/core.py
--rw-r--r--   0 ccc       (1000) ccc       (1000)     6809 2022-02-24 09:27:39.000000 matplotlib_label_lines-0.5.1/labellines/line_label.py
--rw-r--r--   0 ccc       (1000) ccc       (1000)     9778 2022-02-24 15:31:25.000000 matplotlib_label_lines-0.5.1/labellines/test.py
--rw-r--r--   0 ccc       (1000) ccc       (1000)     3290 2022-02-24 15:16:14.000000 matplotlib_label_lines-0.5.1/labellines/utils.py
-drwxr-xr-x   0 ccc       (1000) ccc       (1000)        0 2022-02-25 14:22:26.838056 matplotlib_label_lines-0.5.1/matplotlib_label_lines.egg-info/
--rw-r--r--   0 ccc       (1000) ccc       (1000)     3755 2022-02-25 14:22:26.000000 matplotlib_label_lines-0.5.1/matplotlib_label_lines.egg-info/PKG-INFO
--rw-r--r--   0 ccc       (1000) ccc       (1000)      398 2022-02-25 14:22:26.000000 matplotlib_label_lines-0.5.1/matplotlib_label_lines.egg-info/SOURCES.txt
--rw-r--r--   0 ccc       (1000) ccc       (1000)        1 2022-02-25 14:22:26.000000 matplotlib_label_lines-0.5.1/matplotlib_label_lines.egg-info/dependency_links.txt
--rw-r--r--   0 ccc       (1000) ccc       (1000)      177 2022-02-25 14:22:26.000000 matplotlib_label_lines-0.5.1/matplotlib_label_lines.egg-info/requires.txt
--rw-r--r--   0 ccc       (1000) ccc       (1000)       11 2022-02-25 14:22:26.000000 matplotlib_label_lines-0.5.1/matplotlib_label_lines.egg-info/top_level.txt
--rw-r--r--   0 ccc       (1000) ccc       (1000)      916 2022-02-21 14:18:28.000000 matplotlib_label_lines-0.5.1/pyproject.toml
--rw-r--r--   0 ccc       (1000) ccc       (1000)     1780 2022-02-25 14:22:26.838056 matplotlib_label_lines-0.5.1/setup.cfg
--rw-r--r--   0 ccc       (1000) ccc       (1000)       38 2021-09-07 10:58:27.000000 matplotlib_label_lines-0.5.1/setup.py
+drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     1072 2017-12-31 16:20:51.000000 matplotlib_label_lines-0.5.2/LICENSE
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)       26 2021-01-15 10:44:15.000000 matplotlib_label_lines-0.5.2/MANIFEST.in
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3703 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/PKG-INFO
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     2894 2023-04-13 09:05:24.000000 matplotlib_label_lines-0.5.2/Readme.md
+drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/labellines/
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      101 2023-04-13 09:04:11.000000 matplotlib_label_lines-0.5.2/labellines/__init__.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     7929 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/core.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     6777 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/line_label.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     9763 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/test.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3714 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/utils.py
+drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3703 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/PKG-INFO
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      398 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/SOURCES.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)        1 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/dependency_links.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      120 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/requires.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)       11 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/top_level.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      645 2023-02-22 17:22:22.000000 matplotlib_label_lines-0.5.2/pyproject.toml
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      997 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/setup.cfg
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)       38 2021-09-07 10:58:27.000000 matplotlib_label_lines-0.5.2/setup.py
```

### Comparing `matplotlib_label_lines-0.5.1/LICENSE` & `matplotlib_label_lines-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_label_lines-0.5.1/PKG-INFO` & `matplotlib_label_lines-0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 Metadata-Version: 2.1
 Name: matplotlib_label_lines
-Version: 0.5.1
+Version: 0.5.2
 Summary: Label lines in matplotlib.
 Home-page: https://github.com/cphyc/matplotlib-label-lines
 Author: Corentin Cadiou
 Author-email: contact@cphyc.me
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: AIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # matplotlib-label-lines
 [![Build status](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml/badge.svg)](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.1)](https://pypi.org/project/matplotlib-label-lines/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.2)](https://pypi.org/project/matplotlib-label-lines/)
 [![PyPI](https://img.shields.io/pypi/v/matplotlib-label-lines)](https://pypi.org/project/matplotlib-label-lines)
 [![codecov](https://codecov.io/gh/cphyc/matplotlib-label-lines/branch/master/graph/badge.svg)](https://codecov.io/gh/cphyc/matplotlib-label-lines)
 
 Easily label line(s) using matplotlib.
 
 The code is heavily based on http://stackoverflow.com/questions/16992038/inline-labels-in-matplotlib (original code from NauticalMile).
 
@@ -107,8 +102,9 @@
 
 labelLines(ax.get_lines(), xvals=(0.1, 1), zorder=2.5)
 
 fig.show()
 ```
 ![Example](https://raw.githubusercontent.com/cphyc/matplotlib-label-lines/master/example.png)
 
-
+# Citing
+If you're using this package for research purposes, consider citing the [Zenodo entry (https://zenodo.org/record/7428071)](https://zenodo.org/record/7428071).
```

### Comparing `matplotlib_label_lines-0.5.1/Readme.md` & `matplotlib_label_lines-0.5.2/Readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # matplotlib-label-lines
 [![Build status](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml/badge.svg)](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.1)](https://pypi.org/project/matplotlib-label-lines/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.2)](https://pypi.org/project/matplotlib-label-lines/)
 [![PyPI](https://img.shields.io/pypi/v/matplotlib-label-lines)](https://pypi.org/project/matplotlib-label-lines)
 [![codecov](https://codecov.io/gh/cphyc/matplotlib-label-lines/branch/master/graph/badge.svg)](https://codecov.io/gh/cphyc/matplotlib-label-lines)
 
 Easily label line(s) using matplotlib.
 
 The code is heavily based on http://stackoverflow.com/questions/16992038/inline-labels-in-matplotlib (original code from NauticalMile).
 
@@ -78,7 +78,10 @@
     ax.semilogx(X, chi2(5).pdf(a * X), label=str(a))
 
 labelLines(ax.get_lines(), xvals=(0.1, 1), zorder=2.5)
 
 fig.show()
 ```
 ![Example](https://raw.githubusercontent.com/cphyc/matplotlib-label-lines/master/example.png)
+
+# Citing
+If you're using this package for research purposes, consider citing the [Zenodo entry (https://zenodo.org/record/7428071)](https://zenodo.org/record/7428071).
```

### Comparing `matplotlib_label_lines-0.5.1/labellines/core.py` & `matplotlib_label_lines-0.5.2/labellines/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.container import ErrorbarContainer
 from matplotlib.dates import DateConverter, num2date
 from more_itertools import always_iterable
 
 from .line_label import LineLabel
-from .utils import ensure_float, maximum_bipartite_matching
+from .utils import maximum_bipartite_matching, normalize_xydata
 
 
 # Label line with line2D label data
 def labelLine(
     line,
     x,
     label=None,
@@ -19,15 +19,16 @@
     drop_label=False,
     yoffset=0,
     yoffset_logspace=False,
     outline_color="auto",
     outline_width=8,
     **kwargs,
 ):
-    """Label a single matplotlib line at position x
+    """
+    Label a single matplotlib line at position x
 
     Parameters
     ----------
     line : matplotlib.lines.Line
        The line holding the label
     x : number
        The location in data unit of the label
@@ -67,14 +68,15 @@
             warnings.warn(
                 (
                     "%s could not be annotated due to `nans` values. "
                     "Consider using another location via the `x` argument."
                 )
                 % line,
                 UserWarning,
+                stacklevel=1,
             )
             return
         raise err
 
     if drop_label:
         line.set_label(None)
 
@@ -121,15 +123,15 @@
        Optional arguments passed to ax.text
     """
     if lines:
         ax = lines[0].axes
     else:
         ax = plt.gca()
 
-    handles, allLabels = ax.get_legend_handles_labels()
+    handles, all_labels = ax.get_legend_handles_labels()
 
     all_lines = []
     for h in handles:
         if isinstance(h, ErrorbarContainer):
             line = h.lines[0]
         else:
             line = h
@@ -144,14 +146,15 @@
         for line in lines:
             if line in all_lines:
                 continue
 
             warnings.warn(
                 "Tried to label line %s, but could not find a label for it." % line,
                 UserWarning,
+                stacklevel=1,
             )
 
     # In case no x location was provided, we need to use some heuristics
     # to generate them.
     if xvals is None:
         xvals = ax.get_xlim()
         xvals_rng = xvals[1] - xvals[0]
@@ -168,15 +171,15 @@
         else:
             xvals = np.linspace(xmin, xmax, len(all_lines) + 2)[1:-1]
 
         # Build matrix line -> xvalue
         ok_matrix = np.zeros((len(all_lines), len(all_lines)), dtype=bool)
 
         for i, line in enumerate(all_lines):
-            xdata = ensure_float(line.get_xdata())
+            xdata, _ = normalize_xydata(line)
             minx, maxx = min(xdata), max(xdata)
             for j, xv in enumerate(xvals):
                 ok_matrix[i, j] = minx < xv < maxx
 
         # If some xvals do not fall in their corresponding line,
         # find a better matching using maximum bipartite matching.
         if not np.all(np.diag(ok_matrix)):
@@ -187,46 +190,47 @@
 
             # Now reorder the xvalues
             old_xvals = xvals.copy()
             xvals[order] = old_xvals
     else:
         xvals = list(always_iterable(xvals))  # force the creation of a copy
 
-    labLines, labels = [], []
+    lab_lines, labels = [], []
     # Take only the lines which have labels other than the default ones
     for i, (line, xv) in enumerate(zip(all_lines, xvals)):
-        label = allLabels[all_lines.index(line)]
-        labLines.append(line)
+        label = all_labels[all_lines.index(line)]
+        lab_lines.append(line)
         labels.append(label)
 
         # Move xlabel if it is outside valid range
-        xdata = ensure_float(line.get_xdata())
+        xdata, _ = normalize_xydata(line)
         if not (min(xdata) <= xv <= max(xdata)):
             warnings.warn(
                 (
                     "The value at position %s in `xvals` is outside the range of its "
                     "associated line (xmin=%s, xmax=%s, xval=%s). Clipping it "
                     "into the allowed range."
                 )
                 % (i, min(xdata), max(xdata), xv),
                 UserWarning,
+                stacklevel=1,
             )
             new_xv = min(xdata) + (max(xdata) - min(xdata)) * 0.9
             xvals[i] = new_xv
 
     # Convert float values back to datetime in case of datetime axis
     if isinstance(ax.xaxis.converter, DateConverter):
         xvals = [num2date(x).replace(tzinfo=ax.xaxis.get_units()) for x in xvals]
 
     txts = []
     try:
         yoffsets = [float(yoffsets)] * len(all_lines)
     except TypeError:
         pass
-    for line, x, yoffset, label in zip(labLines, xvals, yoffsets, labels):
+    for line, x, yoffset, label in zip(lab_lines, xvals, yoffsets, labels):
         txts.append(
             labelLine(
                 line,
                 x,
                 label=label,
                 align=align,
                 drop_label=drop_label,
```

### Comparing `matplotlib_label_lines-0.5.1/labellines/line_label.py` & `matplotlib_label_lines-0.5.2/labellines/line_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 from typing import TYPE_CHECKING
 
 import matplotlib.patheffects as patheffects
 import numpy as np
 from matplotlib.text import Text
 
+from .utils import normalize_xydata
+
 if TYPE_CHECKING:
     from datetime import datetime
-    from typing import Any
+    from typing import Any, Literal, Optional, Union
 
     from matplotlib.axes import Axes
     from matplotlib.lines import Line2D
 
-    Position = float | datetime | np.datetime64
+    Position = Union[float, datetime, np.datetime64]
     ColorLike = Any  # mpl has no type annotations so this is just a crutch
-    # Once support for python <3.8 is dropped this should be Literal["auto"]
-    AutoLiteral = str
+    AutoLiteral = Literal["auto"]
 
 
 class LineLabel(Text):
     """This artist adds a label onto a preexisting Line2D object"""
 
     _line: Line2D
     """Annotated line"""
@@ -49,19 +50,19 @@
     _anchor_b: np.ndarray
     """Anchor B for rotation calculation, point of _line neighbouring this label"""
 
     def __init__(
         self,
         line: Line2D,
         x: Position,
-        label: str | None = None,
+        label: Optional[str] = None,
         align: bool = True,
         yoffset: float = 0,
         yoffset_logspace: bool = False,
-        outline_color: AutoLiteral | ColorLike | None = "auto",
+        outline_color: Optional[Union[AutoLiteral, ColorLike]] = "auto",
         outline_width: float = 8,
         **kwargs,
     ) -> None:
         """
 
         Parameters
         ----------
@@ -112,15 +113,14 @@
             rotation=self._rotation,
             rotation_mode="anchor",
             **kwargs,
         )
 
         # Apply outline effect
         if outline_color is not None:
-
             if outline_color == "auto":
                 outline_color = line.axes.get_facecolor()
 
             self.set_path_effects(
                 [
                     patheffects.Stroke(
                         linewidth=outline_width, foreground=outline_color
@@ -137,16 +137,15 @@
     def _update_anchors(self):
         """
         This helper method computes the position of the textbox and determines
         the anchor points needed to adjust the rotation
         """
         # Use the mpl-internal float representation (deals with datetime etc)
         x = self._line.convert_xunits(self._target_x)
-        xdata = self._line.get_xdata(orig=False)
-        ydata = self._line.get_ydata(orig=False)
+        xdata, ydata = normalize_xydata(self._line)
 
         mask = np.isfinite(ydata)
         if mask.sum() == 0:
             raise ValueError(f"The line {self._line} only contains nan!")
 
         # Find the first line segment surrounding x
         for i, (xa, xb) in enumerate(zip(xdata[:-1], xdata[1:])):
```

### Comparing `matplotlib_label_lines-0.5.1/labellines/test.py` & `matplotlib_label_lines-0.5.2/labellines/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,142 +6,146 @@
 from matplotlib.dates import UTC, DateFormatter, DayLocator
 from matplotlib.testing import setup
 
 from .core import labelLine, labelLines
 
 
 @pytest.fixture()
-def setupMpl():
+def setup_mpl():
     setup()
     plt.clf()
 
 
 @pytest.mark.mpl_image_compare
-def test_linspace(setupMpl):
+def test_linspace(setup_mpl):
     x = np.linspace(0, 1)
     K = [1, 2, 4]
 
     for k in K:
         plt.plot(x, np.sin(k * x), label=rf"$f(x)=\sin({k} x)$")
 
     labelLines(plt.gca().get_lines(), zorder=2.5)
     plt.xlabel("$x$")
     plt.ylabel("$f(x)$")
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_ylogspace(setupMpl):
+def test_ylogspace(setup_mpl):
     x = np.linspace(0, 1)
     K = [1, 2, 4]
 
     for k in K:
         plt.plot(x, np.exp(k * x), label=r"$f(x)=\exp(%s x)$" % k)
 
     plt.yscale("log")
     labelLines(plt.gca().get_lines(), zorder=2.5)
     plt.xlabel("$x$")
     plt.ylabel("$f(x)$")
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_xlogspace(setupMpl):
+def test_xlogspace(setup_mpl):
     x = np.linspace(0, 1)
     K = [1, 2, 4]
 
     for k in K:
         plt.plot(10**x, k * x, label=r"$f(x)=%s x$" % k)
 
     plt.xscale("log")
     labelLines(plt.gca().get_lines(), zorder=2.5)
     plt.xlabel("$x$")
     plt.ylabel("$f(x)$")
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_xylogspace(setupMpl):
-    x = np.geomspace(1e-1, 1e1)
+def test_xylogspace(setup_mpl):
+    x = np.geomspace(0.1, 1e1)
     K = np.arange(-5, 5, 2)
 
     for k in K:
-        plt.plot(x, x**k, label=rf"$f(x)=x^{{{k}}}$")
+        plt.plot(x, np.power(x, k), label=rf"$f(x)=x^{{{k}}}$")
 
     plt.xscale("log")
     plt.yscale("log")
     labelLines(plt.gca().get_lines(), zorder=2.5)
     plt.xlabel("$x$")
     plt.ylabel("$f(x)$")
+    plt.ylim(1e-6, 1e6)
+    # We need to fix the xlims to prevent funky xlims
+    # see PR #115
+    plt.xlim(0.1 / 1.2, 1e1 * 1.2)
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_align(setupMpl):
+def test_align(setup_mpl):
     x = np.linspace(0, 2 * np.pi)
     y = np.sin(x)
 
     lines = plt.plot(x, y, label=r"$\sin(x)$")
 
     labelLines(lines, align=False)
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_rotation_correction(setupMpl):
+def test_rotation_correction(setup_mpl):
     # Fix axes limits and plot line
     fig, ax = plt.subplots()
     ax.set_xlim(0, 1)
     ax.set_ylim(0, 1)
     lines = plt.plot((0, 1), (0, 2), label="rescaled")
 
     # Now label the line and THEN rescale the axes, to force label rotation
     labelLine(lines[0], 0.5)
     ax.set_ylim(0, 2)
 
     return fig
 
 
 @pytest.mark.mpl_image_compare
-def test_vertical(setupMpl):
+def test_vertical(setup_mpl):
     x = 0.5
 
     line = plt.axvline(x, label="axvline")
 
     labelLine(line, x)
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_labels_range(setupMpl):
+def test_labels_range(setup_mpl):
     x = np.linspace(0, 1)
 
     plt.plot(x, np.sin(x), label=r"$\sin x$")
     plt.plot(x, np.cos(x), label=r"$\cos x$")
 
     labelLines(plt.gca().get_lines(), xvals=(0, 0.5))
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_dateaxis_naive(setupMpl):
+def test_dateaxis_naive(setup_mpl):
     dates = [datetime(2018, 11, 1), datetime(2018, 11, 2), datetime(2018, 11, 3)]
 
     plt.plot(dates, [0, 5, 3], label="apples")
     plt.plot(dates, [3, 6, 2], label="banana")
     ax = plt.gca()
     ax.xaxis.set_major_locator(DayLocator())
     ax.xaxis.set_major_formatter(DateFormatter("%Y-%m-%d"))
 
     labelLines(ax.get_lines())
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_dateaxis_advanced(setupMpl):
+def test_dateaxis_advanced(setup_mpl):
     dates = [
         datetime(2018, 11, 1, tzinfo=UTC),
         datetime(2018, 11, 2, tzinfo=UTC),
         datetime(2018, 11, 5, tzinfo=UTC),
         datetime(2018, 11, 3, tzinfo=UTC),
     ]
 
@@ -152,79 +156,63 @@
     ax.xaxis.set_major_formatter(DateFormatter("%Y-%m-%d"))
 
     labelLines(ax.get_lines())
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_polar(setupMpl):
+def test_polar(setup_mpl):
     t = np.linspace(0, 2 * np.pi, num=128)
     plt.plot(np.cos(t), np.sin(t), label="$1/1$")
     plt.plot(np.cos(t), np.sin(2 * t), label="$1/2$")
     plt.plot(np.cos(3 * t), np.sin(t), label="$3/1$")
     ax = plt.gca()
 
     labelLines(ax.get_lines())
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_non_uniform_and_negative_spacing(setupMpl):
+def test_non_uniform_and_negative_spacing(setup_mpl):
     x = [1, -2, -3, 2, -4, -3]
     plt.plot(x, [1, 2, 3, 4, 2, 1], ".-", label="apples")
     plt.plot(x, [6, 5, 4, 2, 5, 5], "o-", label="banana")
     ax = plt.gca()
 
     labelLines(ax.get_lines())
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_errorbar(setupMpl):
+def test_errorbar(setup_mpl):
     x = np.linspace(0, 1, 20)
 
     y = x**0.5
     dy = x
     plt.errorbar(x, y, yerr=dy, label=r"$\sqrt{x}\pm x$")[0]
 
     y = x**3
     dy = x
     plt.errorbar(x, y, yerr=dy, label=r"$x^3\pm x$")[0]
 
     labelLines()
     return plt.gcf()
 
 
-def test_nan_warning():
-    x = np.array([0, 1, 2, 3])
-    y = np.array([np.nan, np.nan, 0, 1])
-
-    line = plt.plot(x, y, label="test")[0]
-
-    warn_msg = (
-        ".* could not be annotated due to `nans` values. "
-        "Consider using another location via the `x` argument."
-    )
-    with pytest.warns(UserWarning, match=warn_msg):
-        labelLine(line, 0.5)
-
-    labelLine(line, 2.5)
-
-
 def test_nan_failure():
     x = np.array([0, 1])
     y = np.array([np.nan, np.nan])
 
     line = plt.plot(x, y, label="test")[0]
     with pytest.raises(Exception):
         labelLine(line, 0.5)
 
 
 @pytest.mark.mpl_image_compare
-def test_label_range(setupMpl):
+def test_label_range(setup_mpl):
     x = np.linspace(0, 1)
     line = plt.plot(x, x**2, label="lorem ipsum")[0]
 
     # This should fail
     with pytest.raises(Exception):
         labelLine(line, -1)
     with pytest.raises(Exception):
@@ -233,27 +221,27 @@
     # This should work
     labelLine(line, 0.5)
 
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_negative_spacing(setupMpl):
+def test_negative_spacing(setup_mpl):
     x = np.linspace(1, -1)
     y = x**2
 
     line = plt.plot(x, y)[0]
 
     # Should not throw an error
     labelLine(line, 0.2, label="Test")
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_label_datetime_plot(setupMpl):
+def test_label_datetime_plot(setup_mpl):
     plt.clf()
     # data from the chinook database of iTunes music sales
     x = np.array(
         [
             "2009-01-31T00:00:00.000000000",
             "2009-02-28T00:00:00.000000000",
             "2009-03-31T00:00:00.000000000",
@@ -273,30 +261,30 @@
     # should not throw an error
     xlabel = datetime(2009, 3, 15)
     labelLine(line, xlabel, "USA")
     plt.tight_layout()
     return plt.gcf()
 
 
-def test_yoffset(setupMpl):
+def test_yoffset(setup_mpl):
     x = np.linspace(0, 1)
 
     for yoffset in ([-0.5, 0.5], 1, 1.2):  # try lists  # try int  # try float
         plt.clf()
         ax = plt.gca()
         ax.plot(x, np.sin(x) * 10, label=r"$\sin x$")
         ax.plot(x, np.cos(x) * 10, label=r"$\cos x$")
         lines = ax.get_lines()
         labelLines(
             lines, xvals=(0.2, 0.7), align=False, yoffsets=yoffset, bbox={"alpha": 0}
         )
 
 
 @pytest.mark.mpl_image_compare
-def test_outline(setupMpl):
+def test_outline(setup_mpl):
     x = np.linspace(-2, 2)
 
     plt.ylim(-1, 5)
     plt.xlim(-2, 2)
 
     for dy, xlabel, w in zip(
         np.linspace(-1, 1, 5),
@@ -307,15 +295,15 @@
         (line,) = plt.plot(x, y, label=f"width={w}")
         labelLine(line, xlabel, outline_width=w, outline_color="gray")
 
     return plt.gcf()
 
 
 @pytest.mark.mpl_image_compare
-def test_auto_layout(setupMpl):
+def test_auto_layout(setup_mpl):
     X = [[1, 2], [0, 1]]
     Y = [[0, 1], [0, 1]]
 
     lines = []
     for i, (x, y) in enumerate(zip(X, Y)):
         lines.extend(plt.plot(x, y, label=f"i={i}"))
 
@@ -344,15 +332,15 @@
             "associated line"
         ),
     ):
         labelLines(lines, xvals=[2])
 
 
 @pytest.mark.mpl_image_compare
-def test_errorbar_with_list(setupMpl):
+def test_errorbar_with_list(setup_mpl):
     np.random.seed(1234)
     fig, ax = plt.subplots()
     samples = ["a", "b"]
     pos = [-1, 1]
 
     x = list(np.arange(-4, 4.1, 0.1))
     ys = [list(np.random.rand(len(x))), list(np.random.rand(len(x)))]
@@ -361,14 +349,23 @@
     for sample, y in zip(samples, ys):
         lines.append(ax.errorbar(x, y, yerr=0.1, label=sample)[0])
 
     labelLines(lines, align=False, xvals=pos)
     return fig
 
 
+@pytest.mark.mpl_image_compare
+def test_labeling_axhline(setup_mpl):
+    fig, ax = plt.subplots()
+    ax.plot([10, 12, 13], [1, 2, 3], label="plot")
+    ax.axhline(y=2, label="axhline")
+    labelLines()
+    return fig
+
+
 @pytest.fixture
 def create_plot():
     fig, ax = plt.subplots()
     X = [0, 1]
     Y = [0, 1]
 
     lines = (
```

### Comparing `matplotlib_label_lines-0.5.1/labellines/utils.py` & `matplotlib_label_lines-0.5.2/labellines/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 from datetime import datetime
 
 import numpy as np
 from matplotlib.dates import date2num
+from matplotlib.lines import Line2D
 
 
-def ensure_float(value):
-    """Make sure datetime values are properly converted to floats."""
+def normalize_xydata(line: Line2D) -> tuple[np.ndarray, np.ndarray]:
+    """Make sure datetime values are properly converted to floats and convert
+    into data coordinates."""
+    # Convert the data into the data coordinates
+    line_t = line.get_transform().transform
+    axes_t = line.axes.transData.inverted().transform
+    x, y = axes_t(line_t(line.get_xydata())).T
+
+    x, y = _convert_to_float(x), _convert_to_float(y)
+    return x, y
+
+
+def _convert_to_float(value) -> float:
     try:
         # the last 3 boolean checks are for arrays with datetime64 and with
         # a timezone, see these SO posts:
         # https://stackoverflow.com/q/60714568/4549682
         # https://stackoverflow.com/q/23063362/4549682
         is_date_array = np.issubdtype(value.dtype, np.datetime64) or str(
             value.dtype
@@ -28,56 +40,51 @@
     except AttributeError:  # possibly int or other float/int dtype
         return value
 
 
 # From https://www.geeksforgeeks.org/maximum-bipartite-matching/
 class GFG:
     def __init__(self, graph):
-
         # residual graph
         self.graph = graph
         self.ppl = len(graph)
         self.jobs = len(graph[0])
 
     # A DFS based recursive function that returns true if a matching for vertex
     # u is possible
-    def bpm(self, u, matchR, seen):
-
+    def bpm(self, u, match_r, seen):
         # Try every job one by one
         for v in range(self.jobs):
-
             # If applicant u is interested
             # in job v and v is not seen
             if self.graph[u][v] and not seen[v]:
-
                 # Mark v as visited
                 seen[v] = True
 
                 # If job 'v' is not assigned to an applicant OR previously
                 # assigned applicant for job v (which is matchR[v]) has an
                 # alternate job available. Since v is marked as visited in the
                 # above line, matchR[v] in the following recursive call will not
                 # get job 'v' again
 
-                if matchR[v] == -1 or self.bpm(matchR[v], matchR, seen):
-                    matchR[v] = u
+                if match_r[v] == -1 or self.bpm(match_r[v], match_r, seen):
+                    match_r[v] = u
                     return True
         return False
 
     # Returns maximum number of matching
     def maxBPM(self):
         # An array to keep track of the applicants assigned to jobs. The value
         # of matchR[i] is the applicant number assigned to job i, the value -1
         # indicates nobody is assigned.
         matchR = [-1] * self.jobs
 
         # Count of jobs assigned to applicants
         result = 0
         for i in range(self.ppl):
-
             # Mark all jobs as not seen for next applicant.
             seen = [False] * self.jobs
 
             # Find if the applicant 'u' can get a job
             if self.bpm(i, matchR, seen):
                 result += 1
         return result, matchR
```

### Comparing `matplotlib_label_lines-0.5.1/matplotlib_label_lines.egg-info/PKG-INFO` & `matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 Metadata-Version: 2.1
 Name: matplotlib-label-lines
-Version: 0.5.1
+Version: 0.5.2
 Summary: Label lines in matplotlib.
 Home-page: https://github.com/cphyc/matplotlib-label-lines
 Author: Corentin Cadiou
 Author-email: contact@cphyc.me
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: AIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # matplotlib-label-lines
 [![Build status](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml/badge.svg)](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.1)](https://pypi.org/project/matplotlib-label-lines/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.2)](https://pypi.org/project/matplotlib-label-lines/)
 [![PyPI](https://img.shields.io/pypi/v/matplotlib-label-lines)](https://pypi.org/project/matplotlib-label-lines)
 [![codecov](https://codecov.io/gh/cphyc/matplotlib-label-lines/branch/master/graph/badge.svg)](https://codecov.io/gh/cphyc/matplotlib-label-lines)
 
 Easily label line(s) using matplotlib.
 
 The code is heavily based on http://stackoverflow.com/questions/16992038/inline-labels-in-matplotlib (original code from NauticalMile).
 
@@ -107,8 +102,9 @@
 
 labelLines(ax.get_lines(), xvals=(0.1, 1), zorder=2.5)
 
 fig.show()
 ```
 ![Example](https://raw.githubusercontent.com/cphyc/matplotlib-label-lines/master/example.png)
 
-
+# Citing
+If you're using this package for research purposes, consider citing the [Zenodo entry (https://zenodo.org/record/7428071)](https://zenodo.org/record/7428071).
```

