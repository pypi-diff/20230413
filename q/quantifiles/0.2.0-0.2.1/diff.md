# Comparing `tmp/quantifiles-0.2.0.tar.gz` & `tmp/quantifiles-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantifiles-0.2.0.tar", last modified: Wed Apr 12 18:53:48 2023, max compression
+gzip compressed data, was "quantifiles-0.2.1.tar", last modified: Thu Apr 13 20:17:17 2023, max compression
```

## Comparing `quantifiles-0.2.0.tar` & `quantifiles-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.976854 quantifiles-0.2.0/
--rw-rw-rw-   0        0        0     1351 2023-03-12 18:13:35.000000 quantifiles-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4459 2023-04-12 18:53:48.976854 quantifiles-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2531 2023-03-26 21:36:14.000000 quantifiles-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.778313 quantifiles-0.2.0/quantifiles/
--rw-rw-rw-   0        0        0     1499 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/data.py
--rw-rw-rw-   0        0        0    18739 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/main.py
--rw-rw-rw-   0        0        0      486 2023-03-24 06:46:53.000000 quantifiles-0.2.0/quantifiles/path.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.935103 quantifiles-0.2.0/quantifiles/plot/
--rw-rw-rw-   0        0        0        0 2023-03-14 21:03:29.000000 quantifiles-0.2.0/quantifiles/plot/__init__.py
--rw-rw-rw-   0        0        0     1749 2023-03-28 19:15:19.000000 quantifiles-0.2.0/quantifiles/plot/autoplot.py
--rw-rw-rw-   0        0        0     3489 2023-03-28 19:15:19.000000 quantifiles-0.2.0/quantifiles/plot/baseplot.py
--rw-rw-rw-   0        0        0     5408 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/plot/colorplot.py
--rw-rw-rw-   0        0        0     2676 2023-03-24 06:46:53.000000 quantifiles-0.2.0/quantifiles/plot/header.py
--rw-rw-rw-   0        0        0     4695 2023-03-28 19:15:19.000000 quantifiles-0.2.0/quantifiles/plot/lineplot.py
--rw-rw-rw-   0        0        0     2118 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/plot/utils.py
--rw-rw-rw-   0        0        0    15748 2023-04-12 18:52:19.000000 quantifiles-0.2.0/quantifiles/plot/window.py
--rw-rw-rw-   0        0        0     2187 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/units.py
--rw-rw-rw-   0        0        0    10207 2023-03-26 21:36:14.000000 quantifiles-0.2.0/quantifiles/watcher.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.856501 quantifiles-0.2.0/quantifiles.egg-info/
--rw-rw-rw-   0        0        0     4459 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-12 18:53:48.000000 quantifiles-0.2.0/quantifiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 18:53:48.976854 quantifiles-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-04-12 18:52:19.000000 quantifiles-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:53:48.966338 quantifiles-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-19 19:21:13.000000 quantifiles-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1095 2023-03-26 21:36:14.000000 quantifiles-0.2.0/tests/test_data.py
--rw-rw-rw-   0        0        0      539 2023-03-19 19:21:13.000000 quantifiles-0.2.0/tests/test_units.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:17:17.629355 quantifiles-0.2.1/
+-rw-rw-rw-   0        0        0     1351 2023-03-12 18:13:35.000000 quantifiles-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4459 2023-04-13 20:17:17.629355 quantifiles-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2531 2023-03-26 21:36:14.000000 quantifiles-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:17:17.519525 quantifiles-0.2.1/quantifiles/
+-rw-rw-rw-   0        0        0     1499 2023-04-13 20:06:51.000000 quantifiles-0.2.1/quantifiles/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-03-26 21:36:14.000000 quantifiles-0.2.1/quantifiles/data.py
+-rw-rw-rw-   0        0        0    18739 2023-04-12 18:52:19.000000 quantifiles-0.2.1/quantifiles/main.py
+-rw-rw-rw-   0        0        0      486 2023-03-24 06:46:53.000000 quantifiles-0.2.1/quantifiles/path.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:17:17.613724 quantifiles-0.2.1/quantifiles/plot/
+-rw-rw-rw-   0        0        0        0 2023-03-14 21:03:29.000000 quantifiles-0.2.1/quantifiles/plot/__init__.py
+-rw-rw-rw-   0        0        0     1749 2023-03-28 19:15:19.000000 quantifiles-0.2.1/quantifiles/plot/autoplot.py
+-rw-rw-rw-   0        0        0     3489 2023-03-28 19:15:19.000000 quantifiles-0.2.1/quantifiles/plot/baseplot.py
+-rw-rw-rw-   0        0        0     5697 2023-04-13 20:14:25.000000 quantifiles-0.2.1/quantifiles/plot/colorplot.py
+-rw-rw-rw-   0        0        0     2676 2023-03-24 06:46:53.000000 quantifiles-0.2.1/quantifiles/plot/header.py
+-rw-rw-rw-   0        0        0     4695 2023-03-28 19:15:19.000000 quantifiles-0.2.1/quantifiles/plot/lineplot.py
+-rw-rw-rw-   0        0        0     5637 2023-04-13 19:29:01.000000 quantifiles-0.2.1/quantifiles/plot/snapshot.py
+-rw-rw-rw-   0        0        0     2118 2023-03-26 21:36:14.000000 quantifiles-0.2.1/quantifiles/plot/utils.py
+-rw-rw-rw-   0        0        0    13532 2023-04-13 19:05:22.000000 quantifiles-0.2.1/quantifiles/plot/window.py
+-rw-rw-rw-   0        0        0     2187 2023-03-26 21:36:14.000000 quantifiles-0.2.1/quantifiles/units.py
+-rw-rw-rw-   0        0        0    10207 2023-03-26 21:36:14.000000 quantifiles-0.2.1/quantifiles/watcher.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:17:17.582466 quantifiles-0.2.1/quantifiles.egg-info/
+-rw-rw-rw-   0        0        0     4459 2023-04-13 20:17:17.000000 quantifiles-0.2.1/quantifiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2023-04-13 20:17:17.000000 quantifiles-0.2.1/quantifiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:17:17.000000 quantifiles-0.2.1/quantifiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-13 20:17:17.000000 quantifiles-0.2.1/quantifiles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2023-04-13 20:17:17.000000 quantifiles-0.2.1/quantifiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 20:17:17.000000 quantifiles-0.2.1/quantifiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 20:17:17.629355 quantifiles-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-04-13 20:06:36.000000 quantifiles-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:17:17.613724 quantifiles-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-19 19:21:13.000000 quantifiles-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1095 2023-03-26 21:36:14.000000 quantifiles-0.2.1/tests/test_data.py
+-rw-rw-rw-   0        0        0      539 2023-03-19 19:21:13.000000 quantifiles-0.2.1/tests/test_units.py
```

### Comparing `quantifiles-0.2.0/LICENSE` & `quantifiles-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/PKG-INFO` & `quantifiles-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantifiles
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple databrowser for quantify datasets.
 Home-page: https://gitlab.com/dcrielaard/quantifiles
 Author: Damien Crielaard
 Author-email: damiencrielaard@gmail.com
 License: BSD 2-Clause License
         
         Copyright (c) 2023, Damien Crielaard
```

### Comparing `quantifiles-0.2.0/README.md` & `quantifiles-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/__init__.py` & `quantifiles-0.2.1/quantifiles/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from quantifiles.main import main
 
 from pathlib import Path
 
 __all__ = ["quantifiles", "__version__"]
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 def quantifiles(
     data_dir: str | Path | None = None,
     liveplotting: bool = False,
     log_level: int | str = logging.WARNING,
 ) -> None:
```

### Comparing `quantifiles-0.2.0/quantifiles/data.py` & `quantifiles-0.2.1/quantifiles/data.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/main.py` & `quantifiles-0.2.1/quantifiles/main.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/plot/autoplot.py` & `quantifiles-0.2.1/quantifiles/plot/autoplot.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/plot/baseplot.py` & `quantifiles-0.2.1/quantifiles/plot/baseplot.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/plot/colorplot.py` & `quantifiles-0.2.1/quantifiles/plot/colorplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         self.y = y
         self.z = z
 
         self.img = pyqtgraph.ImageItem()
         self.img.setColorMap(pyqtgraph.colormap.get(colormap))
 
         self.colorbar = pyqtgraph.ColorBarItem(width=16, cmap=colormap)
+        self.colorbar.setLabels(
+            right=f"{dataset[z].long_name} ({dataset[z].attrs['units']})"
+        )
 
         self.plot.addItem(self.img)
 
         # Check that necessary attributes are present in the dataset
         assert "long_name" in dataset[x].attrs, f"{x} attribute 'long_name' not found"
         assert "units" in dataset[x].attrs, f"{x} attribute 'units' not found"
         assert "long_name" in dataset[y].attrs, f"{y} attribute 'long_name' not found"
@@ -131,14 +134,18 @@
                 np.min(y_data),
                 np.max(x_data) - np.min(x_data),
                 np.max(y_data) - np.min(y_data),
             )
         )
         self.colorbar.setImageItem(self.img, insert_in=self.plot.plotItem)
 
+        limits = (np.nanmin(z_data), np.nanmax(z_data))
+        if limits[0] is not np.nan and limits[1] is not np.nan:
+            self.colorbar.setLevels(limits)
+
     def get_mouse_position_text(self, x: float, y: float) -> str:
         """
         Get the text to display when the mouse is moved over the plot.
 
         Parameters
         ----------
         x: float
```

### Comparing `quantifiles-0.2.0/quantifiles/plot/header.py` & `quantifiles-0.2.1/quantifiles/plot/header.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/plot/lineplot.py` & `quantifiles-0.2.1/quantifiles/plot/lineplot.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/plot/utils.py` & `quantifiles-0.2.1/quantifiles/plot/utils.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/plot/window.py` & `quantifiles-0.2.1/quantifiles/plot/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import xarray as xr
 
 from PyQt5 import QtWidgets, QtCore
 from PyQt5.QtCore import QSignalMapper
 
 from quantifiles.data import get_snapshot_as_dict
 from quantifiles.plot.baseplot import BasePlot
+from quantifiles.plot.snapshot import SnapshotTab
 
 logger = logging.getLogger(__name__)
 
 
 class GettableSelector(QtWidgets.QWidget):
     """
     A widget for selecting variables in a given xarray dataset.
@@ -272,72 +273,14 @@
     def add_plot(self, plot: QtWidgets.QWidget):
         self.plot_layout.addWidget(plot)
         plot.setSizePolicy(
             QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred
         )
 
 
-class SnapshotTab(QtWidgets.QWidget):
-    def __init__(self, snapshot: dict[str, any]):
-        super().__init__()
-        self.snapshot = snapshot
-
-        layout = QtWidgets.QVBoxLayout(self)
-
-        self.snapshot_tree = QtWidgets.QTreeWidget()
-        self.snapshot_tree.setHeaderLabels(["Name", "Value"])
-        self.snapshot_tree.setColumnWidth(0, 256)
-        self.snapshot_tree.setSortingEnabled(True)
-        self.snapshot_tree.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
-        self.snapshot_tree.customContextMenuRequested.connect(
-            self.show_copy_context_menu
-        )
-
-        self.add_snapshot_to_tree(self.snapshot_tree, self.snapshot)
-
-        layout.addWidget(self.snapshot_tree)
-        self.setLayout(layout)
-
-    def add_snapshot_to_tree(
-        self,
-        tree: QtWidgets.QTreeWidget,
-        snapshot: dict[str, any],
-        parent_key: str = "",
-    ):
-        for key, value in snapshot.items():
-            if isinstance(value, dict):
-                item = QtWidgets.QTreeWidgetItem(tree)
-                item.setText(0, key)
-                self.add_snapshot_to_tree(item, value, key)
-            else:
-                item = QtWidgets.QTreeWidgetItem(tree)
-                item.setText(0, f"{parent_key}.{key}" if parent_key else key)
-                item.setText(1, str(value))
-
-    def show_copy_context_menu(self, pos: QtCore.QPoint):
-        menu = QtWidgets.QMenu()
-
-        copy_action = menu.addAction("Copy")
-        action = menu.exec_(self.snapshot_tree.mapToGlobal(pos))
-        if action == copy_action:
-            current_item = self.snapshot_tree.currentItem()
-            item_parent = current_item.parent()
-            if item_parent is not None:
-                dict_copy = {}
-                for i in range(item_parent.childCount()):
-                    child_item = item_parent.child(i)
-                    key = child_item.text(0).split(".", 1)[
-                        -1
-                    ]  # Strip parent key from child key
-                    value = child_item.text(1)
-                    dict_copy[key] = value
-                clipboard = QtWidgets.QApplication.clipboard()
-                clipboard.setText(str(dict_copy))
-
-
 class PlotWindowContent(QtWidgets.QWidget):
     def __init__(
         self,
         parent: QtWidgets.QWidget | None = None,
         dataset: xr.Dataset | None = None,
         snapshot: dict[str, any] | None = None,
     ):
```

### Comparing `quantifiles-0.2.0/quantifiles/units.py` & `quantifiles-0.2.1/quantifiles/units.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles/watcher.py` & `quantifiles-0.2.1/quantifiles/watcher.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/quantifiles.egg-info/PKG-INFO` & `quantifiles-0.2.1/quantifiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantifiles
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple databrowser for quantify datasets.
 Home-page: https://gitlab.com/dcrielaard/quantifiles
 Author: Damien Crielaard
 Author-email: damiencrielaard@gmail.com
 License: BSD 2-Clause License
         
         Copyright (c) 2023, Damien Crielaard
```

### Comparing `quantifiles-0.2.0/quantifiles.egg-info/SOURCES.txt` & `quantifiles-0.2.1/quantifiles.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 quantifiles.egg-info/top_level.txt
 quantifiles/plot/__init__.py
 quantifiles/plot/autoplot.py
 quantifiles/plot/baseplot.py
 quantifiles/plot/colorplot.py
 quantifiles/plot/header.py
 quantifiles/plot/lineplot.py
+quantifiles/plot/snapshot.py
 quantifiles/plot/utils.py
 quantifiles/plot/window.py
 tests/__init__.py
 tests/test_data.py
 tests/test_units.py
```

### Comparing `quantifiles-0.2.0/setup.py` & `quantifiles-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="quantifiles",
-    version="0.2.0",
+    version="0.2.1",
     description="Simple databrowser for quantify datasets.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Damien Crielaard",
     author_email="damiencrielaard@gmail.com",
     url="https://gitlab.com/dcrielaard/quantifiles",
     license=license,
```

### Comparing `quantifiles-0.2.0/tests/test_data.py` & `quantifiles-0.2.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `quantifiles-0.2.0/tests/test_units.py` & `quantifiles-0.2.1/tests/test_units.py`

 * *Files identical despite different names*

