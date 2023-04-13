# Comparing `tmp/reixs-0.5.3.tar.gz` & `tmp/reixs-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.5.3.tar", last modified: Thu Apr 13 17:51:43 2023, max compression
+gzip compressed data, was "reixs-0.5.5.tar", last modified: Thu Apr 13 20:37:48 2023, max compression
```

## Comparing `reixs-0.5.3.tar` & `reixs-0.5.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.327485 reixs-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-13 17:51:26.000000 reixs-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 17:51:43.327485 reixs-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-13 17:51:26.000000 reixs-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 17:51:26.000000 reixs-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-13 17:51:43.331485 reixs-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.323485 reixs-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.327485 reixs-0.5.3/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    53721 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.327485 reixs-0.5.3/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.048618 reixs-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-13 20:37:38.000000 reixs-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 20:37:48.048618 reixs-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-13 20:37:38.000000 reixs-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 20:37:38.000000 reixs-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-13 20:37:48.048618 reixs-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.044618 reixs-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.048618 reixs-0.5.5/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    57205 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-13 20:37:38.000000 reixs-0.5.5/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:37:48.048618 reixs-0.5.5/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 20:37:48.000000 reixs-0.5.5/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.5.3/LICENSE` & `reixs-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/PKG-INFO` & `reixs-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.3
+Version: 0.5.5
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.3/README.md` & `reixs-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/setup.cfg` & `reixs-0.5.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.5.3
+version = 0.5.5
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls =
```

### Comparing `reixs-0.5.3/src/reixs/LoadData.py` & `reixs-0.5.5/src/reixs/LoadData.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,33 +21,35 @@
 
 # Edge Dict
 from .edges import EdgeDict
 
 # Data Processing Functions
 from .util import COLORP, all_list_entries_equal
 from .xeol import *
-from .add_subtract import ScanAddition, ScanSubtraction
+from .add_subtract import ScanAddition, ScanSubtraction, ImageAddition
 from .sca import loadSCAscans
 from .mca import loadMCAscans
 from .mesh import loadMeshScans
 from .rsxs_mcp import loadRSXS1dROIscans, loadRSXS2dROIscans, loadRSXSImageStack
+from .beamline_info import loadSCAbeamline, get_single_beamline_value
 
 #########################################################################################
 #########################################################################################
 
 
 class Load1d:
     """Class to load generic 1d (x,y) data."""
+
     def __init__(self):
         self.data = list()
         self.type = list()
         self.x_stream = list()
         self.filename = list()
-        self.plot_lim_x = [":",":"]
-        self.plot_lim_y = [":",":"]
+        self.plot_lim_x = [":", ":"]
+        self.plot_lim_y = [":", ":"]
         self.legend_loc = 'outside'
         self.plot_vlines = list()
         self.plot_hlines = list()
         self.plot_labels = list()
 
     def load(self, basedir, file, x_stream, y_stream, *args, **kwargs):
         """
@@ -105,38 +107,40 @@
                 binsize : int
                     Bin data by reducing data points via averaging.
                     Int must be exponent of 2.
                     default : None
         """
 
         # Set the defaults if not specified in **kwargs.
-        kwargs.setdefault("norm",True)
-        kwargs.setdefault("is_XAS",False)
+        kwargs.setdefault("norm", True)
+        kwargs.setdefault("is_XAS", False)
         # Append all REIXS scan objects to scan list in current object.
-        self.data.append(loadSCAscans(basedir, file, x_stream, y_stream, *args, **kwargs))
+        self.data.append(loadSCAscans(
+            basedir, file, x_stream, y_stream, *args, **kwargs))
         self.type.append(y_stream)
         self.x_stream.append(x_stream)
         self.filename.append(file)
 
-    def add(self, basedir, file, x_stream, y_stream, *args, **kwargs):       
+    def add(self, basedir, file, x_stream, y_stream, *args, **kwargs):
         """
         Add specified scans for selected streams.
 
         Parameters
         ----------
         See loader function.
         Adds all scans specified in *args.
         """
 
         # Set the defaults if not specified in **kwargs.
-        kwargs.setdefault("norm",False)
-        kwargs.setdefault("avg",False)
-        kwargs.setdefault("is_XAS",False)
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("avg", False)
+        kwargs.setdefault("is_XAS", False)
         # Append all REIXS scan objects to scan list in current object.
-        self.data.append(ScanAddition(basedir, file, x_stream, y_stream, *args, **kwargs))
+        self.data.append(ScanAddition(
+            basedir, file, x_stream, y_stream, *args, **kwargs))
         self.x_stream.append(x_stream)
         self.type.append(y_stream)
         self.filename.append(file)
 
     def subtract(self, basedir, file, x_stream, y_stream, *args, **kwargs):
         """
         Subtract specified scans for selected streams.
@@ -144,94 +148,95 @@
         Parameters
         ----------
         See loader function.
         Subtracts all scans from the first element. May add scans in first element by specifying list of scans as first *arg.
 
         """
         # Set the defaults if not specified in **kwargs.
-        kwargs.setdefault("norm",False)
-        kwargs.setdefault("is_XAS",False)
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("is_XAS", False)
         # Append all REIXS scan objects to scan list in current object.
-        self.data.append(ScanSubtraction(basedir, file, x_stream, y_stream, *args, **kwargs))
+        self.data.append(ScanSubtraction(
+            basedir, file, x_stream, y_stream, *args, **kwargs))
         self.x_stream.append(x_stream)
         self.type.append(y_stream)
         self.filename.append(file)
 
-    def xlim(self,lower,upper):
+    def xlim(self, lower, upper):
         """
         Set x-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_x[0] = lower
         self.plot_lim_x[1] = upper
 
-    def ylim(self,lower,upper):
+    def ylim(self, lower, upper):
         """
         Set y-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_y[0] = lower
         self.plot_lim_y[1] = upper
 
-    def plot_legend(self,pos):
+    def plot_legend(self, pos):
         """
         Overwrite default legend position.
 
         Parameters
         ----------
         pos : string
             See bokeh manual for available options.
         """
         self.legend_loc = pos
 
-    def vline(self,pos,**kwargs):
+    def vline(self, pos, **kwargs):
         """
         Draw a vertical line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_vlines.append([pos,kwargs])
-    
-    def hline(self,pos,**kwargs):
+        self.plot_vlines.append([pos, kwargs])
+
+    def hline(self, pos, **kwargs):
         """
         Draw a horizontal line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_hlines.append([pos,kwargs])
+        self.plot_hlines.append([pos, kwargs])
 
-    def label(self,pos_x,pos_y,text,**kwargs):
+    def label(self, pos_x, pos_y, text, **kwargs):
         """
         Draw a text box in the plot.
 
         Parameters
         ----------
         pos_x : float
         pos_y : float
         text : string
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_labels.append([pos_x,pos_y,text,kwargs])
+        self.plot_labels.append([pos_x, pos_y, text, kwargs])
 
     def plot(self, linewidth=4, title=None, xlabel=None, ylabel=None, plot_height=450, plot_width=700):
         """
         Plot all data assosciated with class instance/object.
 
         Parameters
         ----------
@@ -256,15 +261,15 @@
         # Get the colours for the glyphs.
         numlines = len(plot_data['scan'])
         plot_data['color'] = COLORP[0:numlines]
 
         source = ColumnDataSource(plot_data)
 
         # Set up the bokeh plot
-        p = figure(height=plot_height,width=plot_width,
+        p = figure(height=plot_height, width=plot_width,
                    tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
         p.multi_line(xs='x_stream', ys='y_stream', legend_group="legend",
                      line_width=linewidth, line_color='color', line_alpha=0.6,
                      hover_line_color='color', hover_line_alpha=1.0,
                      source=source)
 
         # Set up the information for hover box
@@ -289,27 +294,30 @@
             p.y_range.end = self.plot_lim_y[1]
 
         if self.plot_lim_x[0] != ':':
             p.x_range.start = self.plot_lim_x[0]
         if self.plot_lim_x[1] != ':':
             p.x_range.end = self.plot_lim_x[1]
 
-        if len(self.plot_hlines)>0:
+        if len(self.plot_hlines) > 0:
             for line_props in self.plot_hlines:
-                line = Span(location=line_props[0],dimension='width',**line_props[1])
+                line = Span(location=line_props[0],
+                            dimension='width', **line_props[1])
                 p.add_layout(line)
 
-        if len(self.plot_vlines)>0:
+        if len(self.plot_vlines) > 0:
             for line_props in self.plot_vlines:
-                line = Span(location=line_props[0],dimension='height',**line_props[1])
+                line = Span(
+                    location=line_props[0], dimension='height', **line_props[1])
                 p.add_layout(line)
 
-        if len(self.plot_labels)>0:
+        if len(self.plot_labels) > 0:
             for label_props in self.plot_labels:
-                label = Label(x=label_props[0],y=label_props[1],text=label_props[2],**label_props[3])
+                label = Label(
+                    x=label_props[0], y=label_props[1], text=label_props[2], **label_props[3])
                 p.add_layout(label)
 
         if title != None:
             p.title.text = str(title)
         if xlabel != None:
             p.xaxis.axis_label = str(xlabel)
         if ylabel != None:
@@ -393,135 +401,137 @@
 
     def exportWidgetStep(self, my):
         # Helper function for exporter widget.
         file = os.path.join(self.exportfile.selected_path,
                             self.exportfile.selected_filename)
         self.export(file)
 
-## The following classes all inherit from Load1d and provide quick-access to frequently used spectroscopy.
+# The following classes all inherit from Load1d and provide quick-access to frequently used spectroscopy.
+
+
 class XASLoader(Load1d):
     def load(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = 'Mono Energy'
-        kwargs.setdefault("norm",True)
+        kwargs.setdefault("norm", True)
         kwargs["is_XAS"] = True
-        super().load(basedir,file,x_stream,y_stream,*args,**kwargs)
+        super().load(basedir, file, x_stream, y_stream, *args, **kwargs)
 
     def plot(self, **kwargs):
-        kwargs.setdefault("title",'Absorption spectra normalized by mesh current')
-        kwargs.setdefault("xlabel","Incident Photon Energy (eV)")
+        kwargs.setdefault(
+            "title", 'Absorption spectra normalized by mesh current')
+        kwargs.setdefault("xlabel", "Incident Photon Energy (eV)")
         super().plot(**kwargs)
 
     def add(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "Mono Energy"
-        kwargs.setdefault("avg",True)
-        kwargs.setdefault("norm",True)
+        kwargs.setdefault("avg", True)
+        kwargs.setdefault("norm", True)
         kwargs["is_XAS"] = True
         super().add(basedir, file, x_stream, y_stream, *args, **kwargs)
 
     def subtract(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "Mono Energy"
-        kwargs.setdefault("norm",True)        
+        kwargs.setdefault("norm", True)
         kwargs["is_XAS"] = True
         super().subtract(basedir, file, x_stream, y_stream, *args, **kwargs)
 
 
 class XESLoader(Load1d):
     def load(self, basedir, file, y_stream, *args, **kwargs):
-        kwargs.setdefault("norm",False)
+        kwargs.setdefault("norm", False)
         x_stream = "MCP Energy"
         super().load(basedir, file, x_stream, y_stream, *
                      args, **kwargs)
 
     def plot(self, **kwargs):
-        kwargs.setdefault("title",'Summed MCP emission spectra')
-        kwargs.setdefault("xlabel","Uncalibrated MCP Energy (eV)")
-        kwargs.setdefault("ylabel","Counts (arb. units)")
+        kwargs.setdefault("title", 'Summed MCP emission spectra')
+        kwargs.setdefault("xlabel", "Uncalibrated MCP Energy (eV)")
+        kwargs.setdefault("ylabel", "Counts (arb. units)")
         super().plot(**kwargs)
 
     def add(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "MCP Energy"
-        kwargs.setdefault("avg",False)
-        kwargs.setdefault("norm",False)
+        kwargs.setdefault("avg", False)
+        kwargs.setdefault("norm", False)
         super().add(basedir, file, x_stream, y_stream, *args, **kwargs)
 
     def subtract(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "MCP Energy"
-        kwargs.setdefault("norm",False)
+        kwargs.setdefault("norm", False)
         super().subtract(basedir, file, x_stream, y_stream, *
                          args, **kwargs)
 
 
 class XRFLoader(Load1d):
     def load(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "SDD Energy"
-        kwargs.setdefault("norm",False)
+        kwargs.setdefault("norm", False)
         super().load(basedir, file, x_stream, y_stream, *
                      args, **kwargs)
 
     def plot(self, **kwargs):
-        kwargs.setdefault("title",'Summed SDD emission spectra')
-        kwargs.setdefault("xlabel","Uncalibrated SDD Energy (eV)")
-        kwargs.setdefault("ylabel","Counts (arb. units)")
+        kwargs.setdefault("title", 'Summed SDD emission spectra')
+        kwargs.setdefault("xlabel", "Uncalibrated SDD Energy (eV)")
+        kwargs.setdefault("ylabel", "Counts (arb. units)")
         super().plot(**kwargs)
 
     def add(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "SDD Energy"
-        kwargs.setdefault("norm",False)
-        kwargs.setdefault("avg",False)
-        super().add(basedir, file, x_stream, y_stream, *args,**kwargs)
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("avg", False)
+        super().add(basedir, file, x_stream, y_stream, *args, **kwargs)
 
     def subtract(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "SDD Energy"
-        kwargs.setdefault("norm",False)
+        kwargs.setdefault("norm", False)
         super().subtract(basedir, file, x_stream, y_stream, *
                          args, **kwargs)
 
 
 class XEOLLoader(Load1d):
     def load(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "XEOL Energy"
-        kwargs.setdefault("norm",False)
+        kwargs.setdefault("norm", False)
         super().load(basedir, file, x_stream, y_stream, *args, **kwargs)
 
     def plot(self, **kwargs):
-        kwargs.setdefault("title",'Summed XEOL spectra')
-        kwargs.setdefault("xlabel","Uncalibrated XEOL Wavelength (nm)")
-        kwargs.setdefault("ylabel","Counts (arb. units)")
+        kwargs.setdefault("title", 'Summed XEOL spectra')
+        kwargs.setdefault("xlabel", "Uncalibrated XEOL Wavelength (nm)")
+        kwargs.setdefault("ylabel", "Counts (arb. units)")
         super().plot(**kwargs)
 
     def add(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "XEOL Energy"
-        kwargs.setdefault("norm",False)
-        kwargs.setdefault("avg",False)
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("avg", False)
         super().add(basedir, file, x_stream, y_stream, *args, **kwargs)
 
     def subtract(self, basedir, file, y_stream, *args, **kwargs):
         x_stream = "XEOL Energy"
-        kwargs.setdefault("norm",False)
+        kwargs.setdefault("norm", False)
         super().subtract(basedir, file, x_stream, y_stream, *args, **kwargs)
 
 
 #########################################################################################
 
 class Load2d:
     """Class to load generic 2d (x,y, z) image data of a detector."""
 
     def __init__(self):
         self.data = list()
         self.x_stream = list()
         self.y_stream = list()
         self.detector = list()
         self.filename = list()
-        self.plot_lim_x = [":",":"]
-        self.plot_lim_y = [":",":"]
+        self.plot_lim_x = [":", ":"]
+        self.plot_lim_y = [":", ":"]
         self.plot_vlines = list()
         self.plot_hlines = list()
         self.plot_labels = list()
 
-
     def load(self, basedir, file, x_stream, y_stream, detector, *args, **kwargs):
         """
         Load one or multiple specific scan(s) for selected streams.
 
         Parameters
         ----------
         basedir : string
@@ -568,119 +578,153 @@
                     default: [None, None, None]
                 grid_y: list
                     Grid data evenly on specified grid [low,high,step size]
                     default: [None, None, None]
         """
 
         # Set the defaults if not specified in **kwargs.
-        kwargs.setdefault("norm",False)
-        kwargs.setdefault("xoffset",None)
-        kwargs.setdefault("xcoffset",None)
-        kwargs.setdefault("yoffset",None)
-        kwargs.setdefault("ycoffset",None)
-        kwargs.setdefault("background",None)
-        kwargs.setdefault("grid_x",[None, None, None])
-        kwargs.setdefault("grid_y",[None, None, None])
-        kwargs.setdefault("energyloss",False)
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("xoffset", None)
+        kwargs.setdefault("xcoffset", None)
+        kwargs.setdefault("yoffset", None)
+        kwargs.setdefault("ycoffset", None)
+        kwargs.setdefault("background", None)
+        kwargs.setdefault("grid_x", [None, None, None])
+        kwargs.setdefault("grid_y", [None, None, None])
+        kwargs.setdefault("energyloss", False)
 
         # Ensure that only one scan is loaded.
         if len(args) != 1:
             raise TypeError("You may only select one scan at a time")
         if self.data != []:
             raise TypeError("You can only append one scan per object")
-        self.data.append(loadMCAscans(basedir, file, x_stream, y_stream, detector, *args, **kwargs))
+        self.data.append(loadMCAscans(basedir, file, x_stream,
+                         y_stream, detector, *args, **kwargs))
         self.x_stream.append(x_stream)
         self.y_stream.append(y_stream)
         self.detector.append(detector)
         self.filename.append(file)
 
         if kwargs['energyloss'] == True:
             self.x_stream[-1] = "Energy loss (eV)"
             self.y_stream[-1] = "Mono Energy (eV)"
 
-    def xlim(self,lower,upper):
+    def add(self, basedir, file, x_stream, y_stream, detector, *args, **kwargs):
+        """
+        Add specified images for selected streams.
+
+        Parameters
+        ----------
+        See loader function.
+        Adds all scans specified in *args.
+        """
+
+        # Set the defaults if not specified in **kwargs.
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("xoffset", None)
+        kwargs.setdefault("xcoffset", None)
+        kwargs.setdefault("yoffset", None)
+        kwargs.setdefault("ycoffset", None)
+        kwargs.setdefault("background", None)
+        kwargs.setdefault("grid_x", [None, None, None])
+        kwargs.setdefault("grid_y", [None, None, None])
+        kwargs.setdefault("energyloss", False)
+
+        self.data.append(ImageAddition(basedir, file, x_stream,
+                         y_stream, detector, *args, **kwargs))
+        
+        self.x_stream.append(x_stream)
+        self.y_stream.append(y_stream)
+        self.detector.append(detector)
+        self.filename.append(file)
+
+        if kwargs['energyloss'] == True:
+            self.x_stream[-1] = "Energy loss (eV)"
+            self.y_stream[-1] = "Mono Energy (eV)"
+
+    def xlim(self, lower, upper):
         """
         Set x-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_x[0] = lower
         self.plot_lim_x[1] = upper
 
-    def ylim(self,lower,upper):
+    def ylim(self, lower, upper):
         """
         Set y-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_y[0] = lower
         self.plot_lim_y[1] = upper
 
-    def vline(self,pos,**kwargs):
+    def vline(self, pos, **kwargs):
         """
         Draw a vertical line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_vlines.append([pos,kwargs])
-    
-    def hline(self,pos,**kwargs):
+        self.plot_vlines.append([pos, kwargs])
+
+    def hline(self, pos, **kwargs):
         """
         Draw a horizontal line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_hlines.append([pos,kwargs])
+        self.plot_hlines.append([pos, kwargs])
 
-    def label(self,pos_x,pos_y,text,**kwargs):
+    def label(self, pos_x, pos_y, text, **kwargs):
         """
         Draw a text box in the plot.
 
         Parameters
         ----------
         pos_x : float
         pos_y : float
         text : string
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_labels.append([pos_x,pos_y,text,kwargs])
+        self.plot_labels.append([pos_x, pos_y, text, kwargs])
 
-    def plot(self,title=None, xlabel=None, ylabel=None, plot_height=600, plot_width=600):
+    def plot(self, title=None, xlabel=None, ylabel=None, plot_height=600, plot_width=600):
         """Plot all data assosciated with class instance/object."""
 
         # Iterate over the one (1) scan in object - this is for legacy reason and shall be removed in the future.
         for i, val in enumerate(self.data):
             for k, v in val.items():
 
                 # Create the figure
-                p = figure(height=plot_height,width=plot_width,tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
+                p = figure(height=plot_height, width=plot_width, tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
                            tools="pan,wheel_zoom,box_zoom,reset,hover,crosshair,save")
                 p.x_range.range_padding = p.y_range.range_padding = 0
 
                 # Gridded scales now calculated directly during the MCA load and only need to be referenced here
 
                 # must give a vector of image data for image parameter
                 color_mapper = LinearColorMapper(palette="Viridis256",
-                                                 low=v.detector.min(),
-                                                 high=v.detector.max())
+                                                 low=v.new_z.min(),
+                                                 high=v.new_z.max())
 
                 # Plot image and use limits as given by even grid.
                 p.image(image=[v.new_z], x=v.xmin, y=v.ymin, dw=v.xmax-v.xmin,
                         dh=v.ymax-v.ymin, color_mapper=color_mapper, level="image")
                 p.grid.grid_line_width = 0.5
 
                 # Defining properties of color mapper
@@ -697,27 +741,30 @@
                     p.y_range.end = self.plot_lim_y[1]
 
                 if self.plot_lim_x[0] != ':':
                     p.x_range.start = self.plot_lim_x[0]
                 if self.plot_lim_x[1] != ':':
                     p.x_range.end = self.plot_lim_x[1]
 
-                if len(self.plot_hlines)>0:
+                if len(self.plot_hlines) > 0:
                     for line_props in self.plot_hlines:
-                        line = Span(location=line_props[0],dimension='width',**line_props[1])
+                        line = Span(
+                            location=line_props[0], dimension='width', **line_props[1])
                         p.add_layout(line)
 
-                if len(self.plot_vlines)>0:
+                if len(self.plot_vlines) > 0:
                     for line_props in self.plot_vlines:
-                        line = Span(location=line_props[0],dimension='height',**line_props[1])
+                        line = Span(
+                            location=line_props[0], dimension='height', **line_props[1])
                         p.add_layout(line)
 
-                if len(self.plot_labels)>0:
+                if len(self.plot_labels) > 0:
                     for label_props in self.plot_labels:
-                        label = Label(x=label_props[0],y=label_props[1],text=label_props[2],**label_props[3])
+                        label = Label(
+                            x=label_props[0], y=label_props[1], text=label_props[2], **label_props[3])
                         p.add_layout(label)
 
             if title != None:
                 p.title.text = str(title)
             else:
                 p.title.text = f'{self.detector[i]} Image for Scan {k}'
             if xlabel != None:
@@ -756,15 +803,15 @@
                 # Gridded scales now calculated directly during the MCA load and only need to be referenced here
 
                 # Start writing string f
                 f.write("========================\n")
                 f.write(
                     f"F~{self.filename[i]}_S{v.scan}_{self.detector[i]}_{self.x_stream[i]}_{self.y_stream[i]}\n")
                 f.write("========================\n")
-                
+
                 # Start writing string g
                 g.write("========================\n")
                 g.write(
                     f"F~{self.filename[i]}_S{v.scan}_{self.detector[i]}_{self.x_stream[i]}_{self.y_stream[i]}\n")
                 g.write("========================\n")
 
                 # Append data to string now.
@@ -793,19 +840,19 @@
         f, g, = self.get_data()
 
         # Dump both strings in file.
         # Need to rewind memory location of String.IO to move to beginning.
         # Copy string content to file with shutil.
         with open(f"{filename}.txt_scale", "a") as scales:
             f.seek(0)
-            shutil.copyfileobj(f,scales)
+            shutil.copyfileobj(f, scales)
 
         with open(f"{filename}.txt_matrix", "a") as matrix:
             g.seek(0)
-            shutil.copyfileobj(g,matrix)
+            shutil.copyfileobj(g, matrix)
 
         print(f"Successfully wrote Image data to {filename}.txt")
 
     def exporter(self):
         """Interactive exporter widget."""
         current_dir = os.path.dirname(os.path.realpath("__file__"))
 
@@ -829,14 +876,15 @@
         file = os.path.join(self.exportfile.selected_path,
                             self.exportfile.selected_filename)
         self.export(file)
 
 
 class EEMsLoader(Load2d):
     """Specific 2d loader for excitation-emission-maps."""
+
     def load(self, basedir, file, detector, *args, **kwargs):
         x_stream = 'Mono Energy'
 
         if detector == "MCP":
             y_stream = "MCP Energy"
         elif detector == "SDD":
             y_stream = "SDD Energy"
@@ -859,35 +907,36 @@
         self.y_stream = list()
         self.z_stream = list()
         self.filename = list()
 
     def load(self, basedir, file, x_stream, y_stream, z_stream, *args, **kwargs):
 
         # Set the defaults if not specified in **kwargs.
-        kwargs.setdefault("norm",False)
-        kwargs.setdefault("xoffset",None)
-        kwargs.setdefault("xcoffset",None)
-        kwargs.setdefault("yoffset",None)
-        kwargs.setdefault("ycoffset",None)
-        kwargs.setdefault("background",None)
+        kwargs.setdefault("norm", False)
+        kwargs.setdefault("xoffset", None)
+        kwargs.setdefault("xcoffset", None)
+        kwargs.setdefault("yoffset", None)
+        kwargs.setdefault("ycoffset", None)
+        kwargs.setdefault("background", None)
         #kwargs.setdefault("grid_x",[None, None, None])
         #kwargs.setdefault("grid_y",[None, None, None])
 
-        self.data.append(loadMeshScans(basedir, file, x_stream, y_stream, z_stream, *args, **kwargs))
+        self.data.append(loadMeshScans(basedir, file, x_stream,
+                         y_stream, z_stream, *args, **kwargs))
         self.x_stream.append(x_stream)
         self.y_stream.append(y_stream)
         self.z_stream.append(z_stream)
         self.filename.append(file)
 
-    def plot(self,title=None, xlabel=None, ylabel=None, plot_height=600, plot_width=600):
+    def plot(self, title=None, xlabel=None, ylabel=None, plot_height=600, plot_width=600):
 
         for i, val in enumerate(self.data):
             for k, v in val.items():
 
-                p = figure(height=plot_height,width=plot_width,tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
+                p = figure(height=plot_height, width=plot_width, tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
                            tools="pan,wheel_zoom,box_zoom,reset,hover,crosshair,save")
                 p.x_range.range_padding = p.y_range.range_padding = 0
 
                 # Have the gridded data ready now from loader
 
                 # must give a vector of image data for image parameter
                 color_mapper = LinearColorMapper(palette="Viridis256",
@@ -913,15 +962,15 @@
                     p.title.text = f'{self.z_stream[i]} Histogram for Scan {k}'
                 if xlabel != None:
                     p.xaxis.axis_label = str(xlabel)
                 else:
                     p.xaxis.axis_label = str(self.x_stream[i])
                 if ylabel != None:
                     p.yaxis.axis_label = str(ylabel)
-                else:                
+                else:
                     p.yaxis.axis_label = f"{self.y_stream[i]}"
 
                 show(p)
 
     def get_data(self):
         f = io.StringIO()
         g = io.StringIO()
@@ -948,19 +997,19 @@
 
     def export(self, filename):
 
         f, g, = self.get_data()
 
         with open(f"{filename}.txt_scale", "a") as scales:
             f.seek(0)
-            shutil.copyfileobj(f,scales)
+            shutil.copyfileobj(f, scales)
 
         with open(f"{filename}.txt_matrix", "a") as matrix:
             g.seek(0)
-            shutil.copyfileobj(g,matrix)
+            shutil.copyfileobj(g, matrix)
 
         print(f"Successfully wrote Histogram data to {filename}.txt")
 
     def exporter(self):
         current_dir = os.path.dirname(os.path.realpath("__file__"))
 
         self.exportfile = FileChooser(current_dir)
@@ -991,99 +1040,99 @@
 
 
 class ImageROILoader():
     def __init__(self):
         self.data = list()
         self.filename = list()
         self.norm = list()
-        self.plot_lim_x = [":",":"]
-        self.plot_lim_y = [":",":"]
+        self.plot_lim_x = [":", ":"]
+        self.plot_lim_y = [":", ":"]
         self.legend_loc = 'outside'
         self.plot_vlines = list()
         self.plot_hlines = list()
         self.plot_labels = list()
 
     def load(self, basedir, file, images, axis, *args, x=[None, None], y=[None, None], norm=False, xoffset=None, xcoffset=None, yoffset=None, ycoffset=None, deriv=None):
         self.data.append(loadRSXS1dROIscans(basedir, file, images, axis, *args, x=x, y=y,
                          norm=norm, xoffset=xoffset, xcoffset=xcoffset, yoffset=yoffset, ycoffset=ycoffset, deriv=deriv))
         self.norm.append(norm)
         self.filename.append(file)
 
-    def xlim(self,lower,upper):
+    def xlim(self, lower, upper):
         """
         Set x-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_x[0] = lower
         self.plot_lim_x[1] = upper
 
-    def ylim(self,lower,upper):
+    def ylim(self, lower, upper):
         """
         Set y-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_y[0] = lower
         self.plot_lim_y[1] = upper
 
-    def plot_legend(self,pos):
+    def plot_legend(self, pos):
         """
         Overwrite default legend position.
 
         Parameters
         ----------
         pos : string
             See bokeh manual for available options.
         """
         self.legend_loc = pos
 
-    def vline(self,pos,**kwargs):
+    def vline(self, pos, **kwargs):
         """
         Draw a vertical line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_vlines.append([pos,kwargs])
-    
-    def hline(self,pos,**kwargs):
+        self.plot_vlines.append([pos, kwargs])
+
+    def hline(self, pos, **kwargs):
         """
         Draw a horizontal line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_hlines.append([pos,kwargs])
+        self.plot_hlines.append([pos, kwargs])
 
-    def label(self,pos_x,pos_y,text,**kwargs):
+    def label(self, pos_x, pos_y, text, **kwargs):
         """
         Draw a text box in the plot.
 
         Parameters
         ----------
         pos_x : float
         pos_y : float
         text : string
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_labels.append([pos_x,pos_y,text,kwargs])
+        self.plot_labels.append([pos_x, pos_y, text, kwargs])
 
     def plot(self, linewidth=4, title='Image ROI', xlabel=None, ylabel='Counts (arb. units)', plot_height=450, plot_width=700):
         plot_data = defaultdict(list)
         for i, val in enumerate(self.data):
             for k, v in val.items():
                 for image, imagevalue in v.caxis.items():
                     plot_data["x_stream"].append(imagevalue)
@@ -1096,15 +1145,15 @@
                     plot_data['legend'].append(f"S{v.scan}_I{image}")
 
         numlines = len(plot_data['scan'])
         plot_data['color'] = COLORP[0:numlines]
 
         source = ColumnDataSource(plot_data)
 
-        p = figure(height=plot_height,width=plot_width,
+        p = figure(height=plot_height, width=plot_width,
                    tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
         p.multi_line(xs='x_stream', ys='y_stream', legend_group="legend",
                      line_width=linewidth, line_color='color', line_alpha=0.6,
                      hover_line_color='color', hover_line_alpha=1.0,
                      source=source)
 
         p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
@@ -1127,27 +1176,30 @@
             p.y_range.end = self.plot_lim_y[1]
 
         if self.plot_lim_x[0] != ':':
             p.x_range.start = self.plot_lim_x[0]
         if self.plot_lim_x[1] != ':':
             p.x_range.end = self.plot_lim_x[1]
 
-        if len(self.plot_hlines)>0:
+        if len(self.plot_hlines) > 0:
             for line_props in self.plot_hlines:
-                line = Span(location=line_props[0],dimension='width',**line_props[1])
+                line = Span(location=line_props[0],
+                            dimension='width', **line_props[1])
                 p.add_layout(line)
 
-        if len(self.plot_vlines)>0:
+        if len(self.plot_vlines) > 0:
             for line_props in self.plot_vlines:
-                line = Span(location=line_props[0],dimension='height',**line_props[1])
+                line = Span(
+                    location=line_props[0], dimension='height', **line_props[1])
                 p.add_layout(line)
 
-        if len(self.plot_labels)>0:
+        if len(self.plot_labels) > 0:
             for label_props in self.plot_labels:
-                label = Label(x=label_props[0],y=label_props[1],text=label_props[2],**label_props[3])
+                label = Label(
+                    x=label_props[0], y=label_props[1], text=label_props[2], **label_props[3])
                 p.add_layout(label)
 
         p.toolbar.logo = None
 
         if all_list_entries_equal(plot_data['x_name']) == True:
             xlabel = plot_data['x_name'][0]
         else:
@@ -1224,93 +1276,93 @@
 
 
 class StackROILoader():
     def __init__(self):
         self.data = list()
         self.filename = list()
         self.norm = list()
-        self.plot_lim_x = [":",":"]
-        self.plot_lim_y = [":",":"]
+        self.plot_lim_x = [":", ":"]
+        self.plot_lim_y = [":", ":"]
         self.plot_vlines = list()
         self.plot_hlines = list()
         self.plot_labels = list()
 
     def load(self, basedir, file, axis, *args, x=[None, None], y=[None, None], norm=False, xoffset=None, xcoffset=None, yoffset=None, ycoffset=None):
         self.data.append(loadRSXS2dROIscans(basedir, file, axis, *args, x=x, y=y, norm=norm,
                          xoffset=xoffset, xcoffset=xcoffset, yoffset=yoffset, ycoffset=ycoffset))
         self.norm.append(norm)
         self.filename.append(file)
 
-    def xlim(self,lower,upper):
+    def xlim(self, lower, upper):
         """
         Set x-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_x[0] = lower
         self.plot_lim_x[1] = upper
 
-    def ylim(self,lower,upper):
+    def ylim(self, lower, upper):
         """
         Set y-axis plot window limits.
 
         Parameters
         ----------
         lower : float
         upper : float
         """
         self.plot_lim_y[0] = lower
         self.plot_lim_y[1] = upper
 
-    def vline(self,pos,**kwargs):
+    def vline(self, pos, **kwargs):
         """
         Draw a vertical line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_vlines.append([pos,kwargs])
-    
-    def hline(self,pos,**kwargs):
+        self.plot_vlines.append([pos, kwargs])
+
+    def hline(self, pos, **kwargs):
         """
         Draw a horizontal line in the plot.
 
         Parameters
         ----------
         pos : float
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_hlines.append([pos,kwargs])
+        self.plot_hlines.append([pos, kwargs])
 
-    def label(self,pos_x,pos_y,text,**kwargs):
+    def label(self, pos_x, pos_y, text, **kwargs):
         """
         Draw a text box in the plot.
 
         Parameters
         ----------
         pos_x : float
         pos_y : float
         text : string
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
-        self.plot_labels.append([pos_x,pos_y,text,kwargs])
-        
+        self.plot_labels.append([pos_x, pos_y, text, kwargs])
+
     def plot(self, title=None, xlabel=None, ylabel=None, plot_height=600, plot_width=600):
         for i, val in enumerate(self.data):
             for k, v in val.items():
 
-                p = figure(height=plot_height,width=plot_width,tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
+                p = figure(height=plot_height, width=plot_width, tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
                            tools="pan,wheel_zoom,box_zoom,reset,hover,crosshair,save")
                 p.x_range.range_padding = p.y_range.range_padding = 0
 
                 # must give a vector of image data for image parameter
                 color_mapper = LinearColorMapper(palette="Viridis256")
 
                 p.image(image=[v.imagemca], x=v.mcp_x.min(), y=v.mcp_y.min(), dw=v.mcp_x.max()-v.mcp_x.min(),
@@ -1331,27 +1383,30 @@
                     p.y_range.end = self.plot_lim_y[1]
 
                 if self.plot_lim_x[0] != ':':
                     p.x_range.start = self.plot_lim_x[0]
                 if self.plot_lim_x[1] != ':':
                     p.x_range.end = self.plot_lim_x[1]
 
-                if len(self.plot_hlines)>0:
+                if len(self.plot_hlines) > 0:
                     for line_props in self.plot_hlines:
-                        line = Span(location=line_props[0],dimension='width',**line_props[1])
+                        line = Span(
+                            location=line_props[0], dimension='width', **line_props[1])
                         p.add_layout(line)
 
-                if len(self.plot_vlines)>0:
+                if len(self.plot_vlines) > 0:
                     for line_props in self.plot_vlines:
-                        line = Span(location=line_props[0],dimension='height',**line_props[1])
+                        line = Span(
+                            location=line_props[0], dimension='height', **line_props[1])
                         p.add_layout(line)
 
-                if len(self.plot_labels)>0:
+                if len(self.plot_labels) > 0:
                     for label_props in self.plot_labels:
-                        label = Label(x=label_props[0],y=label_props[1],text=label_props[2],**label_props[3])
+                        label = Label(
+                            x=label_props[0], y=label_props[1], text=label_props[2], **label_props[3])
                         p.add_layout(label)
 
             if title != None:
                 p.title.text = str(title)
             else:
                 p.title.text = f'Image Stack ROI for Scan {k}'
             if xlabel != None:
@@ -1366,15 +1421,15 @@
             p.toolbar.logo = None
 
             show(p)
 
     def get_data(self):
         f = io.StringIO()
         g = io.StringIO()
-        
+
         for i, val in enumerate(self.data):
             for k, v in val.items():
                 f.write("========================\n")
                 f.write(
                     f"F~{self.filename[i]}_S{v.scan}_{v.caxis_labels[0]}_{v.caxis_labels[1]}\n")
                 f.write("========================\n")
 
@@ -1394,19 +1449,19 @@
 
     def export(self, filename):
 
         f, g, = self.get_data()
 
         with open(f"{filename}.txt_scale", "a") as scales:
             f.seek(0)
-            shutil.copyfileobj(f,scales)
+            shutil.copyfileobj(f, scales)
 
         with open(f"{filename}.txt_matrix", "a") as matrix:
             g.seek(0)
-            shutil.copyfileobj(g,matrix)
+            shutil.copyfileobj(g, matrix)
 
         print(f"Successfully wrote Image data to {filename}.txt")
 
     def exporter(self):
         current_dir = os.path.dirname(os.path.realpath("__file__"))
 
         self.exportfile = FileChooser(current_dir)
@@ -1451,15 +1506,15 @@
             r.data_source.data['dw'] = [v.x_max[f]-v.x_min[f]]
             r.data_source.data['dh'] = [v.y_max[f]-v.y_min[f]]
 
             push_notebook(handle=s)
 
         for i, val in enumerate(self.data):
             for k, v in val.items():
-                p = figure(height=plot_height,width=plot_width,tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
+                p = figure(height=plot_height, width=plot_width, tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")],
                            tools="pan,wheel_zoom,box_zoom,reset,hover,crosshair,save")
                 p.x_range.range_padding = p.y_range.range_padding = 0
 
                 # must give a vector of image data for image parameter
                 color_mapper = LinearColorMapper(palette="Viridis256")
 
                 simage = ColumnDataSource(data=dict(image=[v.imagemca[0]], x=[v.x_min[0]], y=[
@@ -1489,7 +1544,57 @@
                 if ylabel != None:
                     p.yaxis.axis_label = str(ylabel)
                 else:
                     p.yaxis.axis_label = v.mcpRSXS_axes[1]
 
                 s = show(p, notebook_handle=True)
                 display(widgets.interact(update, f=(0, len(v.imagemca)-1)))
+
+#########################################################################################
+
+
+class LoadBeamline(Load1d):
+    def load(self, basedir, file, key, **kwargs):
+        """
+        Load one or multiple specific scan(s) for selected streams.
+
+        Parameters
+        ----------
+        basedir : string
+            Specifiy the absolute or relative path to experimental data.
+        file : string
+            Specify the file name (either ASCII or HDF5).
+        key : string
+        **kwargs: multiple, optional
+            Options:
+                norm : boolean
+                    Norm the spectra to [0,1].
+                    default: True
+                xoffset : list of tuples
+                    Offset the x-axis by applying a polynomial fit.
+                    default: None
+                xcoffset : float
+                    Offset x-axis by constant value.
+                    default : None 
+                yoffset : list of tuples
+                    Offset the y-axis by applying a polynomial fit.
+                    default : None 
+                ycoffset : float
+                    Offset y-axis by constant value.
+                    default : None
+        """
+
+        # Append all REIXS scan objects to scan list in current object.
+        self.data.append(loadSCAbeamline(basedir, file, key, **kwargs))
+        self.type.append(key)
+        self.x_stream.append('Scan Number')
+        self.filename.append(file)
+
+    def add(*args):
+        raise UserWarning('Undefined')
+
+    def subtract(*args):
+        raise UserWarning('Undefined')
+
+
+def getBL(basedir, file, stream, *args):
+    get_single_beamline_value(basedir, file, stream, *args)
```

### Comparing `reixs-0.5.3/src/reixs/ReadData.py` & `reixs-0.5.5/src/reixs/ReadData.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,39 +42,41 @@
 
     # Return REIXS objects based on extension
     # Always default to HDF5
     if "." in header_file:
         return REIXS_HDF5(baseName, header_file, REIXSconfig, handle_exception)
     else:
         return REIXS_HDF5(baseName, str(header_file)+".h5", REIXSconfig, handle_exception)
-        
+
+
 class REIXS_HDF5(object):
     """REIXS data object  HDF5
 
         Parameters
         ----------
         baseName : string
             Give directory path of stored data file
         header_file : string
             Give name of header file with extension
         REIXSconfig : dict
             Spec paramter to python variable dict
     """
+
     def __init__(self, baseName, header_file, REIXSconfig, handle_exception):
         try:
             self.file = os.path.join(baseName, header_file)
         except:
             raise TypeError("You did not specify a directory path.")
         self.REIXSconfig = REIXSconfig
 
         self.handle_exception = handle_exception
 
     def Scan(self, scan):
         """Load one specific scan from specified data file
-        
+
         Parameters
         ----------
         scan : int
         """
         return self.myScan(self, scan)
 
     class myScan(object):
@@ -84,78 +86,90 @@
             try:
                 with h5py.File(self.file, 'r') as f:
 
                     try:
                         # Create dictionary for scan numbers
                         scanIndexDictHeader = dict()
                         for k in f.keys():
-                            if k.startswith("SCAN_"): # Groups must start with the SCAN prefix
+                            # Groups must start with the SCAN prefix
+                            if k.startswith("SCAN_"):
                                 scanIndexDictHeader[int(k.split("_")[1])] = k
                         my.scan = scanIndexDictHeader[scan]
 
                     except:
                         raise KeyError("Scan not defined.")
 
                     # Define selected special streams and detectors
                     try:
-                        my.mono_energy = np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_mono_energy"]}'])
+                        my.mono_energy = np.array(
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_mono_energy"]}'])
                     except:
                         raise UserWarning("Problem detecting energy.")
 
                     try:
-                        my.mesh_current = np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_mesh_current"]}'])
+                        my.mesh_current = np.array(
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_mesh_current"]}'])
                     except:
                         raise UserWarning("Problem detecting mesh current.")
 
                     try:
-                        my.sample_current = np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_sample_current"]}'])
+                        my.sample_current = np.array(
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_sample_current"]}'])
                     except:
                         raise UserWarning("Problem detecting sample current.")
 
                     try:
                         my.TEY = my.sample_current/my.mesh_current
                     except:
                         raise ValueError("Problem calculating TEY.")
 
                     try:
-                        my.sdd_data = np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_sdd_data"]}'])
+                        my.sdd_data = np.array(
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_sdd_data"]}'])
                         my.sdd_energy = np.array(
                             f[f'{my.scan}/{self.REIXSconfig["HDF5_sdd_energy"]}'])
                     except:
-                        warnings.warn("Could not load SDD data / SDD energy scale")
+                        warnings.warn(
+                            "Could not load SDD data / SDD energy scale")
 
                     try:
-                        my.xeol_data = np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_data"]}'],dtype=np.float)
-                        my.xeol_energy = np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_energy"]}'])
-                        my.xeol_background = np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_background"]}'],dtype=np.float)
+                        my.xeol_data = np.array(
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_data"]}'], dtype=np.float)
+                        my.xeol_energy = np.array(
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_energy"]}'])
+                        my.xeol_background = np.array(
+                            f[f'{my.scan}/{self.REIXSconfig["HDF5_xeol_background"]}'], dtype=np.float)
 
                     except:
-                        warnings.warn("Could not load XEOL data / XEOL emission scale")
+                        warnings.warn(
+                            "Could not load XEOL data / XEOL emission scale")
 
                     try:
                         my.mcp_data = np.transpose(
                             np.array(f[f'{my.scan}/{self.REIXSconfig["HDF5_mcp_data"]}']))
                         my.mcp_energy = np.array(
                             f[f'{my.scan}/{self.REIXSconfig["HDF5_mcp_energy"]}'])
                     except:
-                        warnings.warn("Could not load MCP data / MCP energy scale")
+                        warnings.warn(
+                            "Could not load MCP data / MCP energy scale")
 
                     # Populate a pandas dataframe with all SCA data
                     my.sca_data = pd.DataFrame()
                     try:
                         for entry in f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}']:
-                            if len(f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/{entry}'].shape) == 1 and len(f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/{entry}']) == len(f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/epoch']) :
+                            if len(f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/{entry}'].shape) == 1 and len(f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/{entry}']) == len(f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/epoch']):
                                 my.sca_data[str(entry)] = np.array(
-                                f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/{entry}'])
+                                    f[f'{my.scan}/{self.REIXSconfig["HDF5_sca_data"]}/{entry}'])
                     except:
-                        warnings.warn("Could not load SCAs from HDF5 container.")
+                        warnings.warn(
+                            "Could not load SCAs from HDF5 container.")
 
             except OSError as e:
                 obj = self.handle_exception(e)
-                
+
                 my.scan = scan
                 my.mono_energy = obj.Scan(scan).mono_energy
                 my.mesh_current = obj.Scan(scan).mesh_current
                 my.sample_current = obj.Scan(scan).sample_current
                 my.TEY = my.sample_current/my.mesh_current
                 try:
                     my.sdd_data = obj.Scan(scan).sdd_data
@@ -163,15 +177,16 @@
                 except:
                     warnings.warn("Could not load SDD data / SDD energy scale")
                 try:
                     my.xeol_data = obj.Scan(scan).xeol_data
                     my.xeol_energy = obj.Scan(scan).xeol_energy
                     my.xeol_background = obj.Scan(scan).xeol_background
                 except:
-                    warnings.warn("Could not load XEOL data / XEOL emission scale")
+                    warnings.warn(
+                        "Could not load XEOL data / XEOL emission scale")
                 try:
                     if obj.MCPRIXS == True:
                         my.mcp_data = obj.Scan(scan).mcp_data
                         my.mcp_energy = obj.Scan(scan).mcp_energy
                     elif obj.MCPRSXS == True:
                         my.mcpRSXS_scales = obj.Scan(scan).mcpRSXS_scales
                         my.mcpRSXS_scatters = obj.Scan(scan).mcpRSXS_scatters
@@ -188,21 +203,23 @@
             except:
                 raise ValueError("Scan Data not defined")
 
         def MCP_norm(my):
             """Normalize the counts of the MCP by incident flux at every given datapoint.
                This is only applied to EEMs."""
 
-            my.mcp_data_norm = np.transpose(rixs_readutil.detector_norm(my.mcp_data,my.mesh_current))
+            my.mcp_data_norm = np.transpose(
+                rixs_readutil.detector_norm(my.mcp_data, my.mesh_current))
 
             return my.mcp_data_norm
 
         def SDD_norm(my):
             """Normalize the counts of the SDD by incident flux at every given datapoint."""
-            my.sdd_data_norm = rixs_readutil.detector_norm(my.sdd_data,my.mesh_current[:,None])
+            my.sdd_data_norm = rixs_readutil.detector_norm(
+                my.sdd_data, my.mesh_current[:, None])
 
             return my.sdd_data_norm
 
         def XES(my):
             """Sum the MCP detector image over all recorded datapoints."""
 
             return rixs_readutil.XES(my.mcp_data)
@@ -259,15 +276,15 @@
             """Calculate TFY by summing over entire SDD image without ROI."""
             # Transform this to TFY spectrum (rows = incident energy points, columns = detector 'space')
 
             return rixs_readutil.TFY(my.sdd_data, my.mesh_current)
 
         def specPFY(my, mcp_lowE, mcp_highE):
             """Calculate spectrometer PFY based on ROI set.
-            
+
             Parameters
             ----------
             mcp_lowE : float
                 Lower energy cutoff for detector integration
             mcp_highE : float
                 Higher energy cutoff for detector integration
             """
@@ -304,14 +321,46 @@
         def RSXS_Images(my):
             """Stack the data with multiple images."""
             if not(hasattr(my, 'RSXSMCP_norm')):
                 my.RSXS_MCPnorm()
 
             return grid_stack(my.mcpRSXS_scales, my.RSXSMCP_norm)
 
+    def Info(self, keys):
+        """Load one specific scan from specified data file
+
+        Parameters
+        ----------
+        keys : list of key paths to the desired information
+        """
+        # Try opening hdf5 container
+        try:
+            with h5py.File(self.file, 'r') as f:
+                # Create dictionary for scan numbers
+                info_dict = dict()
+
+                if not isinstance(keys, list):
+                    keys = [keys]
+
+                for key in keys:
+                    info_dict[key] = dict()
+                    for k in f.keys():
+                        if k.startswith("SCAN_"):  # Groups must start with the SCAN prefix
+                            try:
+                                info_dict[key][int(
+                                    k.split("_")[1])] = f[f'{k}/{key}'][()].decode("utf-8")
+                            except AttributeError:
+                                info_dict[key][int(
+                                    k.split("_")[1])] = f[f'{k}/{key}'][()]
+
+        except:
+            raise KeyError("Error opening and processing file.")
+
+        return info_dict
+
 
 class REIXS_ASCII(object):
 
     """Returns all scans in a scan file."""
 
     def __init__(self, baseName, header_file, REIXSconfig):
         """
@@ -344,15 +393,15 @@
         except:
             raise TypeError("You did not specify a directory path.")
         self.REIXSconfig = REIXSconfig
 
         # Open the header file and read line by line
         with open(full_path_for_header_file) as f:
             for line in f:
-                if line.startswith('#S '): # Triggers a new scan
+                if line.startswith('#S '):  # Triggers a new scan
                     # Append new scan if list is currently populated in last element (scan)
                     if self.datasets[-1] != []:
                         # we are in a new block
                         self.datasets.append([])
 
                     # Ensures we can only load scans with the same scan number only once
                     if line.strip().split()[1] in self.scanNumbers:
@@ -367,31 +416,31 @@
 
                 # Header
                 elif line.startswith("#L"):
                     self.datasets[-1].append(line.strip("#L ").strip("\n"))
 
                 # Use this to generate mnemonic/long name dict
                 elif line.startswith('#J'):
-                    plist0 = line.strip().split(" ",1)
+                    plist0 = line.strip().split(" ", 1)
                     plist = plist0[1].split("  ")
                     self.full_names_counters += plist
 
                 elif line.startswith('#O'):
-                    plist0 = line.strip().split(" ",1)
+                    plist0 = line.strip().split(" ", 1)
                     plist = plist0[1].split("  ")
                     self.full_names_motors += plist
 
                 # Use this to generate mnemonic/long name dict
                 elif line.startswith('#j'):
-                    plist0 = line.strip().split(" ",1)
+                    plist0 = line.strip().split(" ", 1)
                     plist = plist0[1].split(" ")
                     self.mnemonics_counters += plist
 
                 elif line.startswith('#o'):
-                    plist0 = line.strip().split(" ",1)
+                    plist0 = line.strip().split(" ", 1)
                     plist = plist0[1].split(" ")
                     self.mnemonics_motors += plist
 
                 # Ignore empty spaces or commented lines
                 elif line.startswith('#') or line.startswith('\n'):
                     pass
 
@@ -403,15 +452,15 @@
         self.sdd_datasets = [[]]
         self.sdd_scanNumbers = []
         try:
             with open(f"{os.path.join(baseName,header_file)}"+"_sdd") as f_sdd:
                 next(f_sdd)
                 # Read file line by line
                 for line_sdd in f_sdd:
-                    if line_sdd.startswith('#S '): # Triggers new scan
+                    if line_sdd.startswith('#S '):  # Triggers new scan
                         if self.sdd_datasets[-1] != []:
                             # we are in a new block
                             self.sdd_datasets.append([])
                         self.sdd_scanNumbers.append(
                             line_sdd.strip().split()[1])
 
                     elif line_sdd.startswith('#') or line_sdd.startswith('\n'):
@@ -459,18 +508,19 @@
                 self.mcpRSXS_scale_headers = [[]]
                 self.mcpRSXS_scanNumbers = []
 
                 with open(f"{os.path.join(baseName,header_file)}"+"_mcp") as f_mcp:
                     next(f_mcp)
                     # Read file line by line
                     for line in f_mcp:
-                        if line.startswith('#S '): # Triggers new scan
+                        if line.startswith('#S '):  # Triggers new scan
                             if self.mcpRSXS_data[-1] != []:
                                 self.mcpRSXS_data.append([])
-                            if self.mcpRSXS_scale_headers[-1] != []: # Now need to also keep track of column headers
+                            # Now need to also keep track of column headers
+                            if self.mcpRSXS_scale_headers[-1] != []:
                                 self.mcpRSXS_scale_headers.append([])
 
                             self.mcpRSXS_scanNumbers.append(
                                 line.strip().split()[1])
 
                         # Append the header
                         elif line.startswith('#C ') or line.startswith('#@IMG'):
@@ -495,15 +545,15 @@
         self.xeol_datasets = [[]]
         self.xeol_scanNumbers = []
         try:
             with open(f"{os.path.join(baseName,header_file)}"+"_xeol") as f_xeol:
                 next(f_xeol)
                 # Load file line by line
                 for line_xeol in f_xeol:
-                    if line_xeol.startswith('#S '): # Triggers new scan
+                    if line_xeol.startswith('#S '):  # Triggers new scan
                         if self.xeol_datasets[-1] != []:
                             # we are in a new block
                             self.xeol_datasets.append([])
                         self.xeol_scanNumbers.append(
                             line_xeol.strip().split()[1])
 
                     # Ignore empty spaces
@@ -534,21 +584,25 @@
 
         if int(self.scanNumbers[-1]) != int(len(self.scanNumbers)):
             print("Scans not labelled consecutively!")
             print("Last Scan Number", self.scanNumbers[-1])
             print("Scans in File", len(self.scanNumbers))
 
         if len(self.mnemonics_motors) != len(self.full_names_motors):
-            raise UserWarning("Mismatch with nmemonic to full name dictionary (motors).")
+            raise UserWarning(
+                "Mismatch with nmemonic to full name dictionary (motors).")
 
         if len(self.mnemonics_counters) != len(self.full_names_counters):
-            raise UserWarning("Mismatch with nmemonic to full name dictionary (counters).")
+            raise UserWarning(
+                "Mismatch with nmemonic to full name dictionary (counters).")
 
-        self.mnemonic2name_motors = dict(zip(self.full_names_motors,self.mnemonics_motors))
-        self.mnemonic2name_counters = dict(zip(self.full_names_counters,self.mnemonics_counters))
+        self.mnemonic2name_motors = dict(
+            zip(self.full_names_motors, self.mnemonics_motors))
+        self.mnemonic2name_counters = dict(
+            zip(self.full_names_counters, self.mnemonics_counters))
 
         # Create dictionary for scan numbers
         # This is in case a detector was disabled for a specific scan,
         # so we know which list index to trigger
         self.scanIndexDictHeader = dict()
         for i, scanIndex in enumerate(self.scanNumbers):
             self.scanIndexDictHeader[int(scanIndex)] = i
@@ -653,47 +707,52 @@
             # Now append Epoch
             mnemonics_header.append("Epoch")
             # Do the counters last
             for entry in header_list[epoch_index+1:]:
                 mnemonics_header.append(self.mnemonic2name_counters[entry])
 
             if len(header_list) != len(mnemonics_header):
-                warnings.warn("Problem in converting long names to mnemonics in header file.")
+                warnings.warn(
+                    "Problem in converting long names to mnemonics in header file.")
 
             my.sca_data.columns = mnemonics_header
             # Ensures data type integrity
             my.sca_data = my.sca_data.apply(pd.to_numeric, errors='coerce')
 
             # Remove duplicate columns
-            my.sca_data = my.sca_data.loc[:,~my.sca_data.columns.duplicated()].copy()
+            my.sca_data = my.sca_data.loc[:, ~
+                                          my.sca_data.columns.duplicated()].copy()
 
             # Defines special streams
             # Added legacy support for previous spec variables
             try:
-                my.mono_energy = np.array(my.sca_data[self.REIXSconfig["ASCII_mono_energy"]])
+                my.mono_energy = np.array(
+                    my.sca_data[self.REIXSconfig["ASCII_mono_energy"]])
             except:
-                ## We leave this in for legacy support
+                # We leave this in for legacy support
                 try:
                     my.mono_energy = np.array(my.sca_data["beam"])
                 except:
                     raise TypeError("Problem determining energy.")
 
             try:
-                my.mesh_current = np.array(my.sca_data[self.REIXSconfig["ASCII_mesh_current"]])
+                my.mesh_current = np.array(
+                    my.sca_data[self.REIXSconfig["ASCII_mesh_current"]])
             except:
-                ## Leave this in for legacy support
+                # Leave this in for legacy support
                 try:
                     my.mesh_current = np.array(my.sca_data["i0"])
                 except:
                     raise TypeError("Problem determening mesh current")
 
             try:
-                my.sample_current = np.array(my.sca_data[self.REIXSconfig["ASCII_sample_current"]])
+                my.sample_current = np.array(
+                    my.sca_data[self.REIXSconfig["ASCII_sample_current"]])
             except:
-                ## Also leave this in for legacy support
+                # Also leave this in for legacy support
                 try:
                     my.sample_current = np.array(my.sca_data["tey"])
                 except:
                     raise TypeError("Problem determening sample current.")
 
             # Define total electron yield normalized by flux
             try:
@@ -721,15 +780,15 @@
                         self.mcp_datasets[my.scanmcpRIXS], max_rows=1024, dtype='float')
                     # Load the MCP MCA
                     my.mcp_data = np.loadtxt(
                         self.mcp_datasets[my.scanmcpRIXS], skiprows=1024, unpack=True)
                 except:
                     raise UserWarning("Could not RIXS MCP data from file.")
 
-            # Load the MCP data for RSXS endstation 
+            # Load the MCP data for RSXS endstation
             if my.MCPRSXS == True:
                 try:
                     # Keep track of scales in MCP file
                     my.mcpRSXS_scales = dict()
                     my.mcpRSXS_scatters = dict()
                     my.mcpRSXS_axes = self.mcpRSXS_scale_headers[my.scanmcpRSXS]
 
@@ -761,8 +820,8 @@
                     # Get the xeol background - this is not used (!)
                     my.xeol_background = np.loadtxt(
                         self.xeol_datasets[my.scanxeol], skiprows=2048, max_rows=2048)
                     # Load the actual xeol image
                     my.xeol_data = np.loadtxt(
                         self.xeol_datasets[my.scanxeol], skiprows=4096)
                 except:
-                    raise UserWarning("Could not load XEOL data from file.")
+                    raise UserWarning("Could not load XEOL data from file.")
```

### Comparing `reixs-0.5.3/src/reixs/add_subtract.py` & `reixs-0.5.5/src/reixs/add_subtract.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
-from scipy.interpolate import interp1d
+from scipy.interpolate import interp1d, interp2d
 from .sca import loadSCAscans
-from .simplemath import apply_offset, apply_savgol
+from .mca import loadMCAscans
+from .simplemath import apply_offset, apply_savgol, grid_data2d
 import warnings
 
 def ScanAddition(basedir, file, x_stream, y_stream, *args, avg=True, norm=False, is_XAS=False, background=None, xoffset=None, xcoffset=None, yoffset=None, ycoffset=None,energyloss=None,grid_x=[None,None,None],savgol=None,binsize=None,legend_item=None):
     """Internal function to handle scan addition.
 
         Parameters
         ----------
@@ -237,7 +238,76 @@
     if energyloss!=None:
         if energyloss == True:
             data[0].x_stream = MASTER_mono-data[0].x_stream
         else:
             data[0].x_stream = energyloss-data[0].x_stream
 
     return data
+
+def ImageAddition(basedir, file, x_stream, y_stream, detector, *args, norm=True, xoffset=None, xcoffset=None, yoffset=None, ycoffset=None,grid_x=[None, None, None],grid_y=[None, None,None], background=None, energyloss=False):
+    """Internal function to handle image addition.
+
+    Parameters
+    ----------
+    args : Same as for the Load2d class
+    kwargs: See Load2d class
+    """
+
+   # Define generic object in which all data will be stored
+    class added_object:
+        def __init__(self):
+            pass
+
+    # Ensure we only add a unique scan once
+    for i in args:
+        if args.count(i) > 1:
+            raise ValueError("Cannot add the same scan to itself")
+
+    # Get the appropriate data first - same loader as always
+    Scandata =  loadMCAscans(basedir, file, x_stream, y_stream, detector, *args, norm=False, xoffset=xoffset, xcoffset=xcoffset, yoffset=yoffset, ycoffset=ycoffset,grid_x=[None, None, None],grid_y=[None, None, None], background=background, energyloss=False)
+
+    # Iterate over all loaded scans
+    for i, (k, v) in enumerate(Scandata.items()):
+    # Set the first scan as master data
+        if i == 0:
+            MASTER_x_stream = v.new_x
+            MASTER_y_stream = v.new_y
+            MASTER_detector = v.new_z
+            MASTER_xmin = v.xmin
+            MASTER_xmax = v.xmax
+            MASTER_ymin = v.ymin
+            MASTER_ymax = v.ymax
+            name = str(k)+'+'
+        else:
+            # Ensure that we only add emission scans when the spectrometer energy scale is identical
+            if not np.array_equal(MASTER_y_stream, v.new_y):
+                    raise ValueError(
+                        "Cannot add spectra with different energy scales.")
+            
+            interp = interp2d(v.new_x,v.new_y,v.new_z)
+            new_z = interp(MASTER_x_stream,MASTER_y_stream)
+
+            MASTER_detector = np.add(MASTER_detector,new_z)
+            
+            name += "_" + str(k)
+
+    if energyloss == True:
+        MASTER_xmin, MASTER_xmax, MASTER_ymin, MASTER_ymax, MASTER_x_stream, MASTER_y_stream, MASTER_detector = grid_data2d(MASTER_x_stream, MASTER_y_stream, MASTER_detector, grid_x=grid_x,grid_y=grid_y,energyloss=energyloss)
+
+    # Place data in a dictionary with the same structure as a regular Load1d call, so that we can plot it
+    data = dict()
+    data[0] = added_object()
+    data[0].new_x = MASTER_x_stream
+    data[0].new_y = MASTER_y_stream
+    data[0].new_z = MASTER_detector
+    data[0].xmin = MASTER_xmin
+    data[0].xmax = MASTER_xmax
+    data[0].ymin = MASTER_ymin
+    data[0].ymax = MASTER_ymax
+
+    data[0].scan = name
+
+    # Normalize data to [0,1]
+    if norm == True:
+        data[0].MASTER_detector =  data[0].MASTER_detector / max(data[0].MASTER_detector)
+
+    return data
```

### Comparing `reixs-0.5.3/src/reixs/mca.py` & `reixs-0.5.5/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/mesh.py` & `reixs-0.5.5/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/parser.py` & `reixs-0.5.5/src/reixs/parser.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/rixs_readutil.py` & `reixs-0.5.5/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/rsxs_mcp.py` & `reixs-0.5.5/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/rsxs_readutil.py` & `reixs-0.5.5/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/sca.py` & `reixs-0.5.5/src/reixs/sca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/simplemath.py` & `reixs-0.5.5/src/reixs/simplemath.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/spec_config.py` & `reixs-0.5.5/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs/util.py` & `reixs-0.5.5/src/reixs/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,116 +2,140 @@
 from itertools import groupby
 import pandas as pd
 import numpy as np
 from scipy.interpolate import interp1d
 from collections.abc import MutableMapping
 
 #########################################################################################
+
+
 def all_list_entries_equal(iterable):
     """Checks if all entries in a list are equal"""
     g = groupby(iterable)
     return next(g, True) and not next(g, False)
 
 #########################################################################################
+
+
 def doesMatchPattern(string, patterns=[]):
     """Checks if a string matches specific patterns"""
     for p in patterns:
 
         # skip empty patterns
-        if not p: continue
+        if not p:
+            continue
 
         if re.search(p, string, re.I):
             return True
 
     return False
 
 #########################################################################################
+
+
 def get_roi(roi):
     """Gets the roi when ':' separated"""
     try:
         roi_low = float(roi.split(":")[0])
         roi_high = float(roi.split(":")[1])
     except:
         roi_low = float(roi)
         roi_high = float(roi)
 
-    return roi_low,roi_high
+    return roi_low, roi_high
 
 #########################################################################################
-def check_idx(idx_low,idx_high):
+
+
+def check_idx(idx_low, idx_high):
     """Check the index of an array. Add +1 to allow slicing."""
     if idx_low == idx_high:
         idx_high = idx_low+1
-    
-    return idx_low,idx_high
+
+    return idx_low, idx_high
 
 #########################################################################################
-def check_key_in_dict(key,dic):
+
+
+def check_key_in_dict(key, dic):
     """Checks if a specific key is ina dictionary"""
-    for k,v in dic.items():
+    for k, v in dic.items():
         if key == k:
             return True
 
 #########################################################################################
+
+
 def flatten(d):
     """Flattens a dictionary of dicts to one dictionary"""
     items = []
     for k, v in d.items():
         if isinstance(v, MutableMapping):
             items.extend(flatten(v).items())
         else:
             items.append((k, v))
     return dict(items)
 
-#########################################################################################            
+#########################################################################################
+
+
+def invert_dict(my_map):
+    return {v: k for k, v in my_map.items()}
+
+#########################################################################################
 # Palette for Bokeh Plots
 
+
 COLORP = ['#d60000', '#8c3bff', '#018700', '#00acc6', '#e6a500', '#ff7ed1', '#6b004f', '#573b00', '#005659', '#15e18c', '#0000dd', '#a17569', '#bcb6ff', '#bf03b8', '#645472', '#790000', '#0774d8', '#729a7c', '#ff7752', '#004b00', '#8e7b01', '#f2007b', '#8eba00', '#a57bb8', '#5901a3', '#e2afaf', '#a03a52', '#a1c8c8', '#9e4b00', '#546744', '#bac389', '#5e7b87',
- '#60383b', '#8287ff', '#380000', '#e252ff', '#2f5282', '#7ecaff', '#c4668e', '#008069', '#919eb6', '#cc7407', '#7e2a8e', '#00bda3', '#2db152', '#4d33ff', '#00e400', '#ff00cd', '#c85748', '#e49cff', '#1ca1ff', '#6e70aa', '#c89a69', '#77563b', '#03dae6', '#c1a3c3', '#ff6989', '#ba00fd', '#915280', '#9e0174', '#93a14f', '#364424', '#af6dff', '#596d00',
- '#ff3146', '#828056', '#006d2d', '#8956af', '#5949a3', '#773416', '#85c39a', '#5e1123', '#d48580', '#a32818', '#0087b1', '#ca0044', '#ffa056', '#eb4d00', '#6b9700', '#528549', '#755900', '#c8c33f', '#91d370', '#4b9793', '#4d230c', '#60345b', '#8300cf', '#8a0031', '#9e6e31', '#ac8399', '#c63189', '#015438', '#086b83', '#87a8eb', '#6466ef', '#c35dba',
- '#019e70', '#805059', '#826e8c', '#b3bfda', '#b89028', '#ff97b1', '#a793e1', '#698cbd', '#4b4f01', '#4801cc', '#60006e', '#446966', '#9c5642', '#7bacb5', '#cd83bc', '#0054c1', '#7b2f4f', '#fb7c00', '#34bf00', '#ff9c87', '#e1b669', '#526077', '#5b3a7c', '#eda5da', '#ef52a3', '#5d7e69', '#c3774f', '#d14867', '#6e00eb', '#1f3400', '#c14103', '#6dd4c1',
- '#46709e', '#a101c3', '#0a8289', '#afa501', '#a55b6b', '#fd77ff', '#8a85ae', '#c67ee8', '#9aaa85', '#876bd8', '#01baf6', '#af5dd1', '#59502a', '#b5005e', '#7cb569', '#4985ff', '#00c182', '#d195aa', '#a34ba8', '#e205e2', '#16a300', '#382d00', '#832f33', '#5d95aa', '#590f00', '#7b4600', '#6e6e31', '#335726', '#4d60b5', '#a19564', '#623f28', '#44d457',
- '#70aacf', '#2d6b4d', '#72af9e', '#fd1500', '#d8b391', '#79893b', '#7cc6d8', '#db9036', '#eb605d', '#eb5ed4', '#e47ba7', '#a56b97', '#009744', '#ba5e21', '#bcac52', '#87d82f', '#873472', '#aea8d1', '#e28c62', '#d1b1eb', '#36429e', '#3abdc1', '#669c4d', '#9e0399', '#4d4d79', '#7b4b85', '#c33431', '#8c6677', '#aa002d', '#7e0175', '#01824d', '#724967',
- '#727790', '#6e0099', '#a0ba52', '#e16e31', '#c46970', '#6d5b95', '#a33b74', '#316200', '#87004f', '#335769', '#ba8c7c', '#1859ff', '#909101', '#2b8ad4', '#1626ff', '#21d3ff', '#a390af', '#8a6d4f', '#5d213d', '#db03b3', '#6e56ca', '#642821', '#ac7700', '#a3bff6', '#b58346', '#9738db', '#b15093', '#7242a3', '#878ed1', '#8970b1', '#6baf36', '#5979c8',
- '#c69eff', '#56831a', '#00d6a7', '#824638', '#11421c', '#59aa75', '#905b01', '#f64470', '#ff9703', '#e14231', '#ba91cf', '#34574d', '#f7807c', '#903400', '#b3cd00', '#2d9ed3', '#798a9e', '#50807c', '#c136d6', '#eb0552', '#b8ac7e', '#487031', '#839564', '#d89c89', '#0064a3', '#4b9077', '#8e6097', '#ff5238', '#a7423b', '#006e70', '#97833d', '#dbafc8']
+          '#60383b', '#8287ff', '#380000', '#e252ff', '#2f5282', '#7ecaff', '#c4668e', '#008069', '#919eb6', '#cc7407', '#7e2a8e', '#00bda3', '#2db152', '#4d33ff', '#00e400', '#ff00cd', '#c85748', '#e49cff', '#1ca1ff', '#6e70aa', '#c89a69', '#77563b', '#03dae6', '#c1a3c3', '#ff6989', '#ba00fd', '#915280', '#9e0174', '#93a14f', '#364424', '#af6dff', '#596d00',
+          '#ff3146', '#828056', '#006d2d', '#8956af', '#5949a3', '#773416', '#85c39a', '#5e1123', '#d48580', '#a32818', '#0087b1', '#ca0044', '#ffa056', '#eb4d00', '#6b9700', '#528549', '#755900', '#c8c33f', '#91d370', '#4b9793', '#4d230c', '#60345b', '#8300cf', '#8a0031', '#9e6e31', '#ac8399', '#c63189', '#015438', '#086b83', '#87a8eb', '#6466ef', '#c35dba',
+          '#019e70', '#805059', '#826e8c', '#b3bfda', '#b89028', '#ff97b1', '#a793e1', '#698cbd', '#4b4f01', '#4801cc', '#60006e', '#446966', '#9c5642', '#7bacb5', '#cd83bc', '#0054c1', '#7b2f4f', '#fb7c00', '#34bf00', '#ff9c87', '#e1b669', '#526077', '#5b3a7c', '#eda5da', '#ef52a3', '#5d7e69', '#c3774f', '#d14867', '#6e00eb', '#1f3400', '#c14103', '#6dd4c1',
+          '#46709e', '#a101c3', '#0a8289', '#afa501', '#a55b6b', '#fd77ff', '#8a85ae', '#c67ee8', '#9aaa85', '#876bd8', '#01baf6', '#af5dd1', '#59502a', '#b5005e', '#7cb569', '#4985ff', '#00c182', '#d195aa', '#a34ba8', '#e205e2', '#16a300', '#382d00', '#832f33', '#5d95aa', '#590f00', '#7b4600', '#6e6e31', '#335726', '#4d60b5', '#a19564', '#623f28', '#44d457',
+          '#70aacf', '#2d6b4d', '#72af9e', '#fd1500', '#d8b391', '#79893b', '#7cc6d8', '#db9036', '#eb605d', '#eb5ed4', '#e47ba7', '#a56b97', '#009744', '#ba5e21', '#bcac52', '#87d82f', '#873472', '#aea8d1', '#e28c62', '#d1b1eb', '#36429e', '#3abdc1', '#669c4d', '#9e0399', '#4d4d79', '#7b4b85', '#c33431', '#8c6677', '#aa002d', '#7e0175', '#01824d', '#724967',
+          '#727790', '#6e0099', '#a0ba52', '#e16e31', '#c46970', '#6d5b95', '#a33b74', '#316200', '#87004f', '#335769', '#ba8c7c', '#1859ff', '#909101', '#2b8ad4', '#1626ff', '#21d3ff', '#a390af', '#8a6d4f', '#5d213d', '#db03b3', '#6e56ca', '#642821', '#ac7700', '#a3bff6', '#b58346', '#9738db', '#b15093', '#7242a3', '#878ed1', '#8970b1', '#6baf36', '#5979c8',
+          '#c69eff', '#56831a', '#00d6a7', '#824638', '#11421c', '#59aa75', '#905b01', '#f64470', '#ff9703', '#e14231', '#ba91cf', '#34574d', '#f7807c', '#903400', '#b3cd00', '#2d9ed3', '#798a9e', '#50807c', '#c136d6', '#eb0552', '#b8ac7e', '#487031', '#839564', '#d89c89', '#0064a3', '#4b9077', '#8e6097', '#ff5238', '#a7423b', '#006e70', '#97833d', '#dbafc8']
 #########################################################################################
 
+
 def to_quanty(file):
     """Manipulates data file such that it can be used as input for Quanty Fitting program.
-    
+
     Parameters
     ----------
     file : string
         Specify path to exported file.
-    
+
     """
     # Read the data file
 
-    df = pd.read_csv(file,header=1)
+    df = pd.read_csv(file, header=1)
     minimum = list()
     maximum = list()
     diff = list()
     interpObj = list()
     # Start interpolation process to common energy loss axis
-    for i,name in enumerate(df.columns):
+    for i, name in enumerate(df.columns):
         if name.endswith('MCP Energy'):
             minimum.append(df[name].min())
             maximum.append(df[name].max())
             diff.append(np.diff(df[name]).min())
             # Interpolate all data
-            interpObj.append(interp1d(np.array(df[name]),np.array(df.iloc[:,df.columns.get_loc(name)+1]),fill_value='extrapolate'))
+            interpObj.append(interp1d(np.array(df[name]), np.array(
+                df.iloc[:, df.columns.get_loc(name)+1]), fill_value='extrapolate'))
 
     # Calculate the number of points and generate linear space
-    numPoints = int(np.ceil((np.array(maximum).max() - np.array(minimum).min())/abs(np.array(diff).min())))
-    linspace = np.linspace(np.array(minimum).min(),np.array(maximum).max(),numPoints,endpoint=True)
+    numPoints = int(np.ceil((np.array(maximum).max() -
+                    np.array(minimum).min())/abs(np.array(diff).min())))
+    linspace = np.linspace(np.array(minimum).min(), np.array(
+        maximum).max(), numPoints, endpoint=True)
 
     # Create new pandas data frame
     dfint = pd.DataFrame(linspace)
 
     # Evaluate all interp objects on new lin space
     # and append to new data frame
-    for i,obj in enumerate(interpObj):
+    for i, obj in enumerate(interpObj):
         dfint[i+1] = obj(linspace)
 
     # Convert data frame to numpy and export
     npreturn = dfint.to_numpy()
-    np.savetxt(f"{file}_Quanty.txt",npreturn)
+    np.savetxt(f"{file}_Quanty.txt", npreturn)
```

### Comparing `reixs-0.5.3/src/reixs/xeol.py` & `reixs-0.5.5/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.3/src/reixs.egg-info/PKG-INFO` & `reixs-0.5.5/src/reixs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.3
+Version: 0.5.5
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.3/src/reixs.egg-info/SOURCES.txt` & `reixs-0.5.5/src/reixs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 src/reixs/LoadData.py
 src/reixs/ReadData.py
 src/reixs/__init__.py
 src/reixs/add_subtract.py
+src/reixs/beamline_info.py
 src/reixs/edges.py
 src/reixs/mca.py
 src/reixs/mesh.py
 src/reixs/parser.py
 src/reixs/rixs_readutil.py
 src/reixs/rsxs_mcp.py
 src/reixs/rsxs_readutil.py
```

