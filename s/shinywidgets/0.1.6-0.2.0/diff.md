# Comparing `tmp/shinywidgets-0.1.6.tar.gz` & `tmp/shinywidgets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinywidgets-0.1.6.tar", last modified: Fri Mar 24 17:40:20 2023, max compression
+gzip compressed data, was "shinywidgets-0.2.0.tar", last modified: Thu Apr 13 19:45:06 2023, max compression
```

## Comparing `shinywidgets-0.1.6.tar` & `shinywidgets-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:40:20.945547 shinywidgets-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-03-24 17:40:20.949547 shinywidgets-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-24 17:40:20.949547 shinywidgets-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:40:20.937547 shinywidgets-0.1.6/shinywidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/_shinywidgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:40:20.945547 shinywidgets-0.1.6/shinywidgets/static/
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff
--rw-r--r--   0 runner    (1001) docker     (123)  3866031 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/libembed-amd.js
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js
--rw-r--r--   0 runner    (1001) docker     (123)    18568 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/output.js
--rw-r--r--   0 runner    (1001) docker     (123)  1006878 2023-03-24 17:40:03.000000 shinywidgets-0.1.6/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:40:20.937547 shinywidgets-0.1.6/shinywidgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-03-24 17:40:20.000000 shinywidgets-0.1.6/shinywidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-24 17:40:20.000000 shinywidgets-0.1.6/shinywidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:40:20.000000 shinywidgets-0.1.6/shinywidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:40:20.000000 shinywidgets-0.1.6/shinywidgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-24 17:40:20.000000 shinywidgets-0.1.6/shinywidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-24 17:40:20.000000 shinywidgets-0.1.6/shinywidgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.750275 shinywidgets-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-13 19:45:06.750275 shinywidgets-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 19:45:06.750275 shinywidgets-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.742275 shinywidgets-0.2.0/shinywidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_as_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/_shinywidgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.746275 shinywidgets-0.2.0/shinywidgets/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  3866031 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/libembed-amd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/output.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1006878 2023-04-13 19:44:48.000000 shinywidgets-0.2.0/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:45:06.742275 shinywidgets-0.2.0/shinywidgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 19:45:06.000000 shinywidgets-0.2.0/shinywidgets.egg-info/top_level.txt
```

### Comparing `shinywidgets-0.1.6/LICENSE` & `shinywidgets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/setup.cfg` & `shinywidgets-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 test_suite = tests
 include_package_data = True
 setup_requires = 
 	setuptools
 install_requires = 
 	ipywidgets>=7.6.5
 	jupyter_core
-	shiny>=0.2.0.9007
+	shiny>=0.3.0
 	python-dateutil>=2.8.2
 	importlib-metadata>=4.8.3,<5; python_version < "3.8"
 tests_require = 
 	pytest>=3
 zip_safe = False
 
 [options.extras_require]
```

### Comparing `shinywidgets-0.1.6/shinywidgets/_comm.py` & `shinywidgets-0.2.0/shinywidgets/_comm.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/_dependencies.py` & `shinywidgets-0.2.0/shinywidgets/_dependencies.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from htmltools._core import HTMLDependencySource
 from ipywidgets._version import (
     __html_manager_version__,  # pyright: ignore[reportUnknownVariableType]
 )
 from ipywidgets.widgets.domwidget import DOMWidget
 from ipywidgets.widgets.widget import Widget
 from jupyter_core.paths import jupyter_path  # type: ignore
-from shiny import Session
+from shiny import Session, ui
 
 from . import __version__
 
 
 # TODO: scripts/static_download.R should produce/update these
 def libembed_dependency() -> List[HTMLDependency]:
     return [
@@ -57,15 +57,17 @@
     )
 
 
 # TODO: this function might have to be recursive since it's technically
 # possible for a Widget to have traits that are themselves Widgets
 # (which could have their own npm module), but in practice, I haven't seen any cases
 # where a 3rd party widget can contain a 3rd party widget.
-def require_dependency(w: Widget, session: Session) -> Optional[HTMLDependency]:
+def require_dependency(
+    w: Widget, session: Session, warn_if_missing: bool = True
+) -> Optional[HTMLDependency]:
     """
     Obtain an HTMLDependency for a 3rd party ipywidget that points
     require('widget-npm-package') requests in the browser to the correct local path.
     """
 
     # The relevant npm package should be specified as an attribute on the widget
     # instance. If the widget is installed as a jupyter extension, in most cases, that
@@ -82,19 +84,21 @@
     # extension path (defined by `_jupyter_nbextension_paths` in __init__.py), but we
     # also don't have a fool-proof way to discovering the relevant __init__.py file,
     # which is why we only use look for it if the npm package isn't installed
     module_dir = jupyter_extension_path(module_name)
     if module_dir is None:
         module_dir = jupyter_extension_path(jupyter_extension_destination(w))
         if module_dir is None:
-            warnings.warn(
-                f"Failed to discover JavaScript dependencies for {type(w)}."
-                + " Make sure it is installed as a jupyter notebook extension.",
-                stacklevel=2,
-            )
+            if warn_if_missing:
+                warnings.warn(
+                    f"Couldn't find local path to widget extension for {type(w)}."
+                    + " Since a CDN fallback is provided, the widget will still render if an internet connection is available."
+                    + " To avoid depending on a CDN, make sure the widget is installed as a jupyter extension.",
+                    stacklevel=2,
+                )
             return None
 
     version = parse_version_safely(getattr(w, "_model_module_version", "1.0"))
     source = HTMLDependencySource(subdir=module_dir)
 
     dep = HTMLDependency(module_name, version, source=source)
     # Get the location where the dependency files will be mounted by the shiny app
@@ -108,14 +112,21 @@
         version,
         source=source,
         all_files=True,
         head=tags.script(f"window.require.config({json.dumps(config)})"),
     )
 
 
+def bokeh_dependency() -> HTMLDependency:
+    from bokeh.resources import Resources
+
+    resources = Resources(mode="inline").render()
+    return ui.head_content(ui.HTML(resources))
+
+
 def jupyter_extension_path(module_name: str) -> Optional[str]:
     paths: List[str] = jupyter_path()
     module_dir = None
     for x in paths:
         dir = os.path.join(x, "nbextensions", module_name)
         if not os.path.exists(dir):
             continue
```

### Comparing `shinywidgets-0.1.6/shinywidgets/_serialization.py` & `shinywidgets-0.2.0/shinywidgets/_serialization.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/_shinywidgets.py` & `shinywidgets-0.2.0/shinywidgets/_shinywidgets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 from __future__ import annotations
 
-# TODO: export _as_widget()?
-__all__ = ("output_widget", "register_widget", "render_widget", "reactive_read")
+__all__ = (
+    "output_widget",
+    "register_widget",
+    "render_widget",
+    "reactive_read",
+    "as_widget",
+)
 
 import copy
 import importlib
 import inspect
 import json
 import os
 import tempfile
 from typing import Any, Awaitable, Callable, Optional, Sequence, Union, cast, overload
 from uuid import uuid4
 from weakref import WeakSet
 
-from htmltools import Tag, TagList, css, tags
+from htmltools import Tag, TagList, css, head_content, tags
 from ipywidgets._version import (
     __protocol_version__,  # pyright: ignore[reportUnknownVariableType]
 )
 from ipywidgets.widgets.widget import (
     _remove_buffers,  # pyright: ignore[reportUnknownVariableType, reportGeneralTypeIssues]
 )
 from ipywidgets.widgets.widget import Widget
 from shiny import Session, reactive
 from shiny._utils import run_coro_sync, wrap_async
 from shiny.http_staticfiles import StaticFiles
 from shiny.module import resolve_id
 from shiny.render import RenderFunction, RenderFunctionAsync
 from shiny.session import get_current_session, require_active_session
 
+from ._as_widget import as_widget
 from ._comm import BufferType, ShinyComm, ShinyCommManager
 from ._dependencies import (
     libembed_dependency,
     output_binding_dependency,
     require_dependency,
-    widget_pkg,
+)
+
+# Make it easier to customize the CDN fallback (and make it CDN-only)
+# https://ipywidgets.readthedocs.io/en/7.6.3/embedding.html#python-interface
+# https://github.com/jupyter-widgets/ipywidgets/blob/6f6156c7/packages/html-manager/src/libembed-amd.ts#L6-L14
+SHINYWIDGETS_CDN = os.getenv("SHINYWIDGETS_CDN", "https://cdn.jsdelivr.net/npm/")
+SHINYWIDGETS_CDN_ONLY = os.getenv("SHINYWIDGETS_CDN_ONLY", "false").lower() == "true"
+# Should shinywidgets warn if unable to find a local path to a widget extension?
+SHINYWIDGETS_EXTENSION_WARNING = (
+    os.getenv("SHINYWIDGETS_EXTENSION_WARNING", "false").lower() == "true"
 )
 
 
 def output_widget(
     id: str, *, width: Optional[str] = None, height: Optional[str] = None
 ) -> Tag:
     id = resolve_id(id)
     return tags.div(
         *libembed_dependency(),
         output_binding_dependency(),
+        head_content(
+            tags.script(
+                data_jupyter_widgets_cdn=SHINYWIDGETS_CDN,
+                data_jupyter_widgets_cdn_only=SHINYWIDGETS_CDN_ONLY,
+            )
+        ),
         id=id,
         class_="shiny-ipywidget-output shiny-report-size shiny-report-theme",
         style=css(width=width, height=height),
     )
 
 
 # --------------------------------------------------------------------------------------------
@@ -79,15 +100,18 @@
 
     # Get the initial state of the widget
     state, buffer_paths, buffers = _remove_buffers(w.get_state())  # type: ignore
 
     # Make sure window.require() calls made by 3rd party widgets
     # (via handle_comm_open() -> new_model() -> loadClass() -> requireLoader())
     # actually point to directories served locally by shiny
-    widget_dep = require_dependency(w, session)
+    if SHINYWIDGETS_CDN_ONLY:
+        widget_dep = None
+    else:
+        widget_dep = require_dependency(w, session, SHINYWIDGETS_EXTENSION_WARNING)
 
     # By the time we get here, the user has already had an opportunity to specify a model_id,
     # so it isn't yet populated, generate a random one so we can assign the same id to the comm
     if getattr(w, "_model_id", None) is None:
         w._model_id = uuid4().hex
 
     # Initialize the comm...this will also send the initial state of the widget
@@ -104,19 +128,21 @@
 
     # Some widget's JS make external requests for static files (e.g.,
     # ipyleaflet markers) under this resource path. Note that this assumes that
     # we're setting the data-base-url attribute on the <body> (which we should
     # be doing on load in js/src/output.ts)
     # https://github.com/jupyter-widgets/widget-cookiecutter/blob/9694718/%7B%7Bcookiecutter.github_project_name%7D%7D/js/lib/extension.js#L8
     if widget_dep and widget_dep.source:
-        session.app._dependency_handler.mount(
-            f"/nbextensions/{widget_dep.name}",
-            StaticFiles(directory=widget_dep.source["subdir"]),
-            name=f"{widget_dep.name}-nbextension-static-resources",
-        )
+        src_dir = widget_dep.source.get("subdir", "")
+        if src_dir:
+            session.app._dependency_handler.mount(
+                f"/nbextensions/{widget_dep.name}",
+                StaticFiles(directory=src_dir),
+                name=f"{widget_dep.name}-nbextension-static-resources",
+            )
 
     # everything after this point should be done once per session
     if session in SESSIONS:
         return
     SESSIONS.add(session)  # type: ignore
 
     # Somewhere inside ipywidgets, it makes requests for static files
@@ -171,15 +197,15 @@
     def __call__(self) -> object:
         return run_coro_sync(self.run())
 
     async def run(self) -> object:
         x = await self._fn()
         if x is None:
             return None
-        widget = _as_widget(x)
+        widget = as_widget(x)
         return {"model_id": widget.model_id}  # type: ignore
 
 
 class IPyWidgetAsync(IPyWidget, RenderFunctionAsync[Widget, object]):
     def __init__(self, fn: IPyWidgetRenderFuncAsync) -> None:
         if not inspect.iscoroutinefunction(fn):
             raise TypeError("IPyWidgetAsync requires an async function")
@@ -219,56 +245,14 @@
 
     if fn is None:
         return wrapper
     else:
         return wrapper(fn)
 
 
-# altair/pydeck/bokeh objects aren't directly renderable as an ipywidget,
-# but we can coerce them into one
-def _as_widget(x: object) -> Widget:
-    pkg = widget_pkg(x)
-    if pkg == "altair" and not isinstance(x, Widget):
-        try:
-            import altair
-            from vega.widget import VegaWidget
-
-            x = cast(altair.Chart, x)
-            x = VegaWidget(x.to_dict())  # type: ignore
-        except ImportError:
-            raise ImportError(
-                "To render altair charts, the ipyvega package must be installed."
-            )
-        except Exception as e:
-            raise RuntimeError(f"Failed to coerce {x} into a VegaWidget: {e}")
-
-    elif pkg == "pydeck" and not isinstance(x, Widget):
-        try:
-            x = x.show()
-        except Exception as e:
-            raise RuntimeError(f"Failed to coerce {x} into a DeckGLWidget: {e}")
-
-    elif pkg == "bokeh" and not isinstance(x, Widget):
-        try:
-            from jupyter_bokeh import BokehModel
-
-            x = BokehModel(x)  # type: ignore
-        except ImportError:
-            raise ImportError(
-                "To render bokeh charts, the jupyter_bokeh package must be installed."
-            )
-        except Exception as e:
-            raise RuntimeError(f"Failed to coerce {x} into a BokehModel: {e}")
-
-    if isinstance(x, Widget):
-        return x
-    else:
-        raise TypeError(f"{x} is not a coerce-able to a ipywidget.Widget object")
-
-
 def reactive_read(widget: Widget, names: Union[str, Sequence[str]]) -> Any:
     reactive_depend(widget, names)
     if isinstance(names, str):
         return getattr(widget, names)
     else:
         return tuple(getattr(widget, name) for name in names)
 
@@ -297,15 +281,15 @@
 
 def register_widget(
     id: str, widget: Widget, session: Optional[Session] = None
 ) -> Widget:
     if session is None:
         session = require_active_session(session)
 
-    w = _as_widget(widget)
+    w = as_widget(widget)
 
     @session.output(id=id)
     @render_widget
     def _():
         return w
 
     return w
```

### Comparing `shinywidgets-0.1.6/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf` & `shinywidgets-0.2.0/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2` & `shinywidgets-0.2.0/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot` & `shinywidgets-0.2.0/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg` & `shinywidgets-0.2.0/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff` & `shinywidgets-0.2.0/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/static/libembed-amd.js` & `shinywidgets-0.2.0/shinywidgets/static/libembed-amd.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js` & `shinywidgets-0.2.0/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets/static/output.js` & `shinywidgets-0.2.0/shinywidgets/static/output.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -17,54 +17,54 @@
             "./node_modules/base64-arraybuffer/dist/base64-arraybuffer.es5.js":
                 /*!************************************************************************!*\
                   !*** ./node_modules/base64-arraybuffer/dist/base64-arraybuffer.es5.js ***!
                   \************************************************************************/
                 /***/
                 ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
-                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"decode\": () => (/* binding */ decode),\n/* harmony export */   \"encode\": () => (/* binding */ encode)\n/* harmony export */ });\n/*\n * base64-arraybuffer 1.0.2 <https://github.com/niklasvh/base64-arraybuffer>\n * Copyright (c) 2022 Niklas von Hertzen <https://hertzen.com>\n * Released under MIT License\n */\nvar chars = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/';\n// Use a lookup table to find the index.\nvar lookup = typeof Uint8Array === 'undefined' ? [] : new Uint8Array(256);\nfor (var i = 0; i < chars.length; i++) {\n    lookup[chars.charCodeAt(i)] = i;\n}\nvar encode = function (arraybuffer) {\n    var bytes = new Uint8Array(arraybuffer), i, len = bytes.length, base64 = '';\n    for (i = 0; i < len; i += 3) {\n        base64 += chars[bytes[i] >> 2];\n        base64 += chars[((bytes[i] & 3) << 4) | (bytes[i + 1] >> 4)];\n        base64 += chars[((bytes[i + 1] & 15) << 2) | (bytes[i + 2] >> 6)];\n        base64 += chars[bytes[i + 2] & 63];\n    }\n    if (len % 3 === 2) {\n        base64 = base64.substring(0, base64.length - 1) + '=';\n    }\n    else if (len % 3 === 1) {\n        base64 = base64.substring(0, base64.length - 2) + '==';\n    }\n    return base64;\n};\nvar decode = function (base64) {\n    var bufferLength = base64.length * 0.75, len = base64.length, i, p = 0, encoded1, encoded2, encoded3, encoded4;\n    if (base64[base64.length - 1] === '=') {\n        bufferLength--;\n        if (base64[base64.length - 2] === '=') {\n            bufferLength--;\n        }\n    }\n    var arraybuffer = new ArrayBuffer(bufferLength), bytes = new Uint8Array(arraybuffer);\n    for (i = 0; i < len; i += 4) {\n        encoded1 = lookup[base64.charCodeAt(i)];\n        encoded2 = lookup[base64.charCodeAt(i + 1)];\n        encoded3 = lookup[base64.charCodeAt(i + 2)];\n        encoded4 = lookup[base64.charCodeAt(i + 3)];\n        bytes[p++] = (encoded1 << 2) | (encoded2 >> 4);\n        bytes[p++] = ((encoded2 & 15) << 4) | (encoded3 >> 2);\n        bytes[p++] = ((encoded3 & 3) << 6) | (encoded4 & 63);\n    }\n    return arraybuffer;\n};\n\n\n//# sourceMappingURL=base64-arraybuffer.es5.js.map\n\n\n//# sourceURL=webpack://@jupyter-widgets/prism-embed-manager/./node_modules/base64-arraybuffer/dist/base64-arraybuffer.es5.js?");
+                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"decode\": () => (/* binding */ decode),\n/* harmony export */   \"encode\": () => (/* binding */ encode)\n/* harmony export */ });\n/*\n * base64-arraybuffer 1.0.2 <https://github.com/niklasvh/base64-arraybuffer>\n * Copyright (c) 2022 Niklas von Hertzen <https://hertzen.com>\n * Released under MIT License\n */\nvar chars = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/';\n// Use a lookup table to find the index.\nvar lookup = typeof Uint8Array === 'undefined' ? [] : new Uint8Array(256);\nfor (var i = 0; i < chars.length; i++) {\n    lookup[chars.charCodeAt(i)] = i;\n}\nvar encode = function (arraybuffer) {\n    var bytes = new Uint8Array(arraybuffer), i, len = bytes.length, base64 = '';\n    for (i = 0; i < len; i += 3) {\n        base64 += chars[bytes[i] >> 2];\n        base64 += chars[((bytes[i] & 3) << 4) | (bytes[i + 1] >> 4)];\n        base64 += chars[((bytes[i + 1] & 15) << 2) | (bytes[i + 2] >> 6)];\n        base64 += chars[bytes[i + 2] & 63];\n    }\n    if (len % 3 === 2) {\n        base64 = base64.substring(0, base64.length - 1) + '=';\n    }\n    else if (len % 3 === 1) {\n        base64 = base64.substring(0, base64.length - 2) + '==';\n    }\n    return base64;\n};\nvar decode = function (base64) {\n    var bufferLength = base64.length * 0.75, len = base64.length, i, p = 0, encoded1, encoded2, encoded3, encoded4;\n    if (base64[base64.length - 1] === '=') {\n        bufferLength--;\n        if (base64[base64.length - 2] === '=') {\n            bufferLength--;\n        }\n    }\n    var arraybuffer = new ArrayBuffer(bufferLength), bytes = new Uint8Array(arraybuffer);\n    for (i = 0; i < len; i += 4) {\n        encoded1 = lookup[base64.charCodeAt(i)];\n        encoded2 = lookup[base64.charCodeAt(i + 1)];\n        encoded3 = lookup[base64.charCodeAt(i + 2)];\n        encoded4 = lookup[base64.charCodeAt(i + 3)];\n        bytes[p++] = (encoded1 << 2) | (encoded2 >> 4);\n        bytes[p++] = ((encoded2 & 15) << 4) | (encoded3 >> 2);\n        bytes[p++] = ((encoded3 & 3) << 6) | (encoded4 & 63);\n    }\n    return arraybuffer;\n};\n\n\n//# sourceMappingURL=base64-arraybuffer.es5.js.map\n\n\n//# sourceURL=webpack://@jupyter-widgets/shiny-embed-manager/./node_modules/base64-arraybuffer/dist/base64-arraybuffer.es5.js?");
 
                     /***/
                 }),
 
             /***/
             "./src/comm.ts":
                 /*!*********************!*\
                   !*** ./src/comm.ts ***!
                   \*********************/
                 /***/
                 ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
-                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"ShinyComm\": () => (/* binding */ ShinyComm)\n/* harmony export */ });\n// This class is a striped down version of Comm from @jupyter-widgets/base\n// https://github.com/jupyter-widgets/ipywidgets/blob/88cec8/packages/base/src/services-shim.ts#L192-L335\n// Note that the Kernel.IComm implementation is located here\n// https://github.com/jupyterlab/jupyterlab/blob/master/packages/services/src/kernel/comm.ts\nclass ShinyComm {\n    constructor(model_id) {\n        this.comm_id = model_id;\n    }\n    // This might not be needed\n    get target_name() {\n        return \"jupyter.widgets\";\n    }\n    send(data, callbacks, metadata, buffers) {\n        const msg = {\n            content: { comm_id: this.comm_id, data: data },\n            metadata: metadata,\n            buffers: buffers || [],\n            // this doesn't seem relevant to the widget?\n            header: {}\n        };\n        const msg_txt = JSON.stringify(msg);\n        Shiny.setInputValue(\"shinywidgets_comm_send\", msg_txt, { priority: \"event\" });\n        // When client-side changes happen to the WidgetModel, this send method\n        // won't get called for _every_  change (just the first one). The\n        // expectation is that this method will eventually end up calling itself\n        // (via callbacks) when the server is ready (i.e., idle) to receive more\n        // updates. To make sense of this, see\n        // https://github.com/jupyter-widgets/ipywidgets/blob/88cec8b/packages/base/src/widget.ts#L550-L557\n        if (callbacks && callbacks.iopub && callbacks.iopub.status) {\n            setTimeout(() => {\n                // TODO: Call this when Shiny reports that it is idle?\n                const msg = { content: { execution_state: \"idle\" } };\n                callbacks.iopub.status(msg);\n            }, 0);\n        }\n        return this.comm_id;\n    }\n    open(data, callbacks, metadata, buffers) {\n        // I don't think we need to do anything here?\n        return this.comm_id;\n    }\n    close(data, callbacks, metadata, buffers) {\n        // I don't think we need to do anything here?\n        return this.comm_id;\n    }\n    on_msg(callback) {\n        this._msg_callback = callback.bind(this);\n    }\n    on_close(callback) {\n        this._close_callback = callback.bind(this);\n    }\n    handle_msg(msg) {\n        if (this._msg_callback)\n            this._msg_callback(msg);\n    }\n    handle_close(msg) {\n        if (this._close_callback)\n            this._close_callback(msg);\n    }\n}\n\n\n//# sourceURL=webpack://@jupyter-widgets/prism-embed-manager/./src/comm.ts?");
+                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"ShinyComm\": () => (/* binding */ ShinyComm)\n/* harmony export */ });\n/* harmony import */ var _utils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! ./utils */ \"./src/utils.ts\");\n\n// This class is a striped down version of Comm from @jupyter-widgets/base\n// https://github.com/jupyter-widgets/ipywidgets/blob/88cec8/packages/base/src/services-shim.ts#L192-L335\n// Note that the Kernel.IComm implementation is located here\n// https://github.com/jupyterlab/jupyterlab/blob/master/packages/services/src/kernel/comm.ts\nclass ShinyComm {\n    constructor(model_id) {\n        this.comm_id = model_id;\n        // TODO: make this configurable (see comments in send() below)?\n        this.throttler = new _utils__WEBPACK_IMPORTED_MODULE_0__.Throttler(100);\n    }\n    // This might not be needed\n    get target_name() {\n        return \"jupyter.widgets\";\n    }\n    send(data, callbacks, metadata, buffers) {\n        const msg = {\n            content: { comm_id: this.comm_id, data: data },\n            metadata: metadata,\n            buffers: buffers || [],\n            // this doesn't seem relevant to the widget?\n            header: {}\n        };\n        const msg_txt = JSON.stringify(msg);\n        // Since ipyleaflet can send mousemove events very quickly when hovering over the map,\n        // we throttle them to ensure that the server doesn't get overwhelmed. Said events\n        // generate a payload that looks like this:\n        // {\"method\": \"custom\", \"content\": {\"event\": \"interaction\", \"type\": \"mousemove\", \"coordinates\": [-17.76259815404015, 12.096729340756617]}}\n        //\n        // TODO: This is definitely not ideal. It would be better to have a way to specify/\n        // customize throttle rates instead of having such a targetted fix for ipyleaflet.\n        const is_mousemove = data.method === \"custom\" &&\n            data.content.event === \"interaction\" &&\n            data.content.type === \"mousemove\";\n        if (is_mousemove) {\n            this.throttler.throttle(() => {\n                Shiny.setInputValue(\"shinywidgets_comm_send\", msg_txt, { priority: \"event\" });\n            });\n        }\n        else {\n            this.throttler.flush();\n            Shiny.setInputValue(\"shinywidgets_comm_send\", msg_txt, { priority: \"event\" });\n        }\n        // When client-side changes happen to the WidgetModel, this send method\n        // won't get called for _every_  change (just the first one). The\n        // expectation is that this method will eventually end up calling itself\n        // (via callbacks) when the server is ready (i.e., idle) to receive more\n        // updates. To make sense of this, see\n        // https://github.com/jupyter-widgets/ipywidgets/blob/88cec8b/packages/base/src/widget.ts#L550-L557\n        if (callbacks && callbacks.iopub && callbacks.iopub.status) {\n            setTimeout(() => {\n                // TODO-future: it doesn't seem quite right to report that shiny is always idle.\n                // Maybe listen to the shiny-busy flag?\n                // const state = document.querySelector(\"html\").classList.contains(\"shiny-busy\") ? \"busy\" : \"idle\";\n                const msg = { content: { execution_state: \"idle\" } };\n                callbacks.iopub.status(msg);\n            }, 0);\n        }\n        return this.comm_id;\n    }\n    open(data, callbacks, metadata, buffers) {\n        // I don't think we need to do anything here?\n        return this.comm_id;\n    }\n    close(data, callbacks, metadata, buffers) {\n        // I don't think we need to do anything here?\n        return this.comm_id;\n    }\n    on_msg(callback) {\n        this._msg_callback = callback.bind(this);\n    }\n    on_close(callback) {\n        this._close_callback = callback.bind(this);\n    }\n    handle_msg(msg) {\n        if (this._msg_callback)\n            this._msg_callback(msg);\n    }\n    handle_close(msg) {\n        if (this._close_callback)\n            this._close_callback(msg);\n    }\n}\n\n\n//# sourceURL=webpack://@jupyter-widgets/shiny-embed-manager/./src/comm.ts?");
 
                     /***/
                 }),
 
             /***/
             "./src/output.ts":
                 /*!***********************!*\
                   !*** ./src/output.ts ***!
                   \***********************/
                 /***/
                 ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
-                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @jupyter-widgets/html-manager */ \"@jupyter-widgets/html-manager\");\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var _comm__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! ./comm */ \"./src/comm.ts\");\n/* harmony import */ var _utils__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./utils */ \"./src/utils.ts\");\n\n\n\n/******************************************************************************\n * Define a custom HTMLManager for use with Shiny\n ******************************************************************************/\nclass OutputManager extends _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.HTMLManager {\n    // In a soon-to-be-released version of @jupyter-widgets/html-manager,\n    // display_view()'s first \"dummy\" argument will be removed... this shim simply\n    // makes it so that our manager can work with either version\n    // https://github.com/jupyter-widgets/ipywidgets/commit/159bbe4#diff-45c126b24c3c43d2cee5313364805c025e911c4721d45ff8a68356a215bfb6c8R42-R43\n    async display_view(view, options) {\n        const n_args = super.display_view.length;\n        if (n_args === 3) {\n            return super.display_view({}, view, options);\n        }\n        else {\n            // @ts-ignore\n            return super.display_view(view, options);\n        }\n    }\n}\n// Define our own custom module loader for Shiny\nconst shinyRequireLoader = async function (moduleName, moduleVersion) {\n    // shiny provides require.js and also sets `define.amd=false` to prevent <script>s\n    // with UMD loaders from triggering anonymous define() errors. shinywidgets should\n    // generally be able to avoid anonymous define errors though since there should only\n    // be one 'main' anonymous define() for the widget's module (located in a JS file that\n    // we've already require.config({paths: {...}})ed; and in that case, requirejs adds a\n    // data-requiremodule attribute to the <script> tag that shiny's custom define will\n    // recognize and use as the name).)\n    const oldAmd = window.define.amd;\n    // The is the original value for define.amd that require.js sets\n    window.define.amd = { jQuery: true };\n    // Store jQuery global since loading we load a module, it may overwrite it\n    // (qgrid is one good example)\n    const old$ = window.$;\n    const oldJQ = window.jQuery;\n    if (moduleName === 'qgrid') {\n        // qgrid wants to use base/js/dialog (if it's available) for full-screen tables\n        // https://github.com/quantopian/qgrid/blob/877b420/js/src/qgrid.widget.js#L11-L16\n        // Maybe that's worth supporting someday, but for now, we define it to be nothing\n        // to avoid require('qgrid') from producing an error\n        window.define(\"base/js/dialog\", [], function () { return null; });\n    }\n    return (0,_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.requireLoader)(moduleName, moduleVersion).finally(() => {\n        window.define.amd = oldAmd;\n        window.$ = old$;\n        window.jQuery = oldJQ;\n    });\n};\nconst manager = new OutputManager({ loader: shinyRequireLoader });\n/******************************************************************************\n* Define the Shiny binding\n******************************************************************************/\n// Ideally we'd extend Shiny's HTMLOutputBinding, but the implementation isn't exported\nclass IPyWidgetOutput extends Shiny.OutputBinding {\n    find(scope) {\n        return $(scope).find(\".shiny-ipywidget-output\");\n    }\n    onValueError(el, err) {\n        Shiny.unbindAll(el);\n        this.renderError(el, err);\n    }\n    renderValue(el, data) {\n        // Allow for a None/null value to hide the widget (css inspired by htmlwidgets)\n        if (!data) {\n            el.style.visibility = \"hidden\";\n            return;\n        }\n        else {\n            el.style.visibility = \"inherit\";\n        }\n        // At this time point, we should've already handled an 'open' message, and so\n        // the model should be ready to use\n        const model = manager.get_model(data.model_id);\n        if (!model) {\n            throw new Error(`No model found for id ${data.model_id}`);\n        }\n        model.then((m) => {\n            const view = manager.create_view(m, {});\n            view.then(v => {\n                manager.display_view(v, { el: el }).then(() => {\n                    // TODO: It would be better to .close() the widget here, but\n                    // I'm not sure how to do that yet (at least client-side)\n                    while (el.childNodes.length > 1) {\n                        el.removeChild(el.childNodes[0]);\n                    }\n                });\n            });\n        });\n    }\n}\nShiny.outputBindings.register(new IPyWidgetOutput(), \"shiny.IPyWidgetOutput\");\n/******************************************************************************\n* Handle messages from the server-side Widget\n******************************************************************************/\n// Initialize the comm and model when a new widget is created\n// This is basically our version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1144-L1176\nShiny.addCustomMessageHandler(\"shinywidgets_comm_open\", (msg_txt) => {\n    setBaseURL();\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    Shiny.renderDependencies(msg.content.html_deps);\n    const comm = new _comm__WEBPACK_IMPORTED_MODULE_1__.ShinyComm(msg.content.comm_id);\n    manager.handle_comm_open(comm, msg);\n});\n// Handle any mutation of the model (e.g., add a marker to a map, without a full redraw)\n// Basically out version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1200-L1215\nShiny.addCustomMessageHandler(\"shinywidgets_comm_msg\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_msg(msg);\n    });\n});\n// TODO: test that this actually works\nShiny.addCustomMessageHandler(\"shinywidgets_comm_close\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_close(msg);\n    });\n});\n// Our version of https://github.com/jupyter-widgets/widget-cookiecutter/blob/9694718/%7B%7Bcookiecutter.github_project_name%7D%7D/js/lib/extension.js#L8\nfunction setBaseURL(x = '') {\n    const base_url = document.querySelector('body').getAttribute('data-base-url');\n    if (!base_url) {\n        document.querySelector('body').setAttribute('data-base-url', x);\n    }\n}\n\n\n//# sourceURL=webpack://@jupyter-widgets/prism-embed-manager/./src/output.ts?");
+                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @jupyter-widgets/html-manager */ \"@jupyter-widgets/html-manager\");\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var _comm__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! ./comm */ \"./src/comm.ts\");\n/* harmony import */ var _utils__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./utils */ \"./src/utils.ts\");\nvar _a;\n\n\n\n/******************************************************************************\n * Define a custom HTMLManager for use with Shiny\n ******************************************************************************/\nclass OutputManager extends _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.HTMLManager {\n    // In a soon-to-be-released version of @jupyter-widgets/html-manager,\n    // display_view()'s first \"dummy\" argument will be removed... this shim simply\n    // makes it so that our manager can work with either version\n    // https://github.com/jupyter-widgets/ipywidgets/commit/159bbe4#diff-45c126b24c3c43d2cee5313364805c025e911c4721d45ff8a68356a215bfb6c8R42-R43\n    async display_view(view, options) {\n        const n_args = super.display_view.length;\n        if (n_args === 3) {\n            return super.display_view({}, view, options);\n        }\n        else {\n            // @ts-ignore\n            return super.display_view(view, options);\n        }\n    }\n}\n// Define our own custom module loader for Shiny\nconst shinyRequireLoader = async function (moduleName, moduleVersion) {\n    // shiny provides require.js and also sets `define.amd=false` to prevent <script>s\n    // with UMD loaders from triggering anonymous define() errors. shinywidgets should\n    // generally be able to avoid anonymous define errors though since there should only\n    // be one 'main' anonymous define() for the widget's module (located in a JS file that\n    // we've already require.config({paths: {...}})ed; and in that case, requirejs adds a\n    // data-requiremodule attribute to the <script> tag that shiny's custom define will\n    // recognize and use as the name).)\n    const oldAmd = window.define.amd;\n    // The is the original value for define.amd that require.js sets\n    window.define.amd = { jQuery: true };\n    // Store jQuery global since loading we load a module, it may overwrite it\n    // (qgrid is one good example)\n    const old$ = window.$;\n    const oldJQ = window.jQuery;\n    if (moduleName === 'qgrid') {\n        // qgrid wants to use base/js/dialog (if it's available) for full-screen tables\n        // https://github.com/quantopian/qgrid/blob/877b420/js/src/qgrid.widget.js#L11-L16\n        // Maybe that's worth supporting someday, but for now, we define it to be nothing\n        // to avoid require('qgrid') from producing an error\n        window.define(\"base/js/dialog\", [], function () { return null; });\n    }\n    return (0,_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.requireLoader)(moduleName, moduleVersion).finally(() => {\n        window.define.amd = oldAmd;\n        window.$ = old$;\n        window.jQuery = oldJQ;\n    });\n};\nconst manager = new OutputManager({ loader: shinyRequireLoader });\n/******************************************************************************\n* Define the Shiny binding\n******************************************************************************/\n// Ideally we'd extend Shiny's HTMLOutputBinding, but the implementation isn't exported\nclass IPyWidgetOutput extends Shiny.OutputBinding {\n    find(scope) {\n        return $(scope).find(\".shiny-ipywidget-output\");\n    }\n    onValueError(el, err) {\n        Shiny.unbindAll(el);\n        this.renderError(el, err);\n    }\n    renderValue(el, data) {\n        // Allow for a None/null value to hide the widget (css inspired by htmlwidgets)\n        if (!data) {\n            el.style.visibility = \"hidden\";\n            return;\n        }\n        else {\n            el.style.visibility = \"inherit\";\n        }\n        // At this time point, we should've already handled an 'open' message, and so\n        // the model should be ready to use\n        const model = manager.get_model(data.model_id);\n        if (!model) {\n            throw new Error(`No model found for id ${data.model_id}`);\n        }\n        model.then((m) => {\n            const view = manager.create_view(m, {});\n            view.then(v => {\n                manager.display_view(v, { el: el }).then(() => {\n                    // TODO: It would be better to .close() the widget here, but\n                    // I'm not sure how to do that yet (at least client-side)\n                    while (el.childNodes.length > 1) {\n                        el.removeChild(el.childNodes[0]);\n                    }\n                });\n            });\n        });\n    }\n}\nShiny.outputBindings.register(new IPyWidgetOutput(), \"shiny.IPyWidgetOutput\");\n// Due to the way HTMLManager (and widget implementations) get loaded (via\n// require.js), the binding registration above can happen _after_ Shiny has\n// already bound the DOM, especially in the dynamic UI case (i.e., output_binding()'s\n// dependencies don't come in until after initial page load). And, in the dynamic UI\n// case, UI is rendered asychronously via Shiny.shinyapp.taskQueue, so if it exists,\n// we probably need to re-bind the DOM after the taskQueue is done.\nconst taskQueue = (_a = Shiny === null || Shiny === void 0 ? void 0 : Shiny.shinyapp) === null || _a === void 0 ? void 0 : _a.taskQueue;\nif (taskQueue) {\n    taskQueue.enqueue(() => Shiny.bindAll(document.body));\n}\n/******************************************************************************\n* Handle messages from the server-side Widget\n******************************************************************************/\n// Initialize the comm and model when a new widget is created\n// This is basically our version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1144-L1176\nShiny.addCustomMessageHandler(\"shinywidgets_comm_open\", (msg_txt) => {\n    setBaseURL();\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    Shiny.renderDependencies(msg.content.html_deps);\n    const comm = new _comm__WEBPACK_IMPORTED_MODULE_1__.ShinyComm(msg.content.comm_id);\n    manager.handle_comm_open(comm, msg);\n});\n// Handle any mutation of the model (e.g., add a marker to a map, without a full redraw)\n// Basically out version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1200-L1215\nShiny.addCustomMessageHandler(\"shinywidgets_comm_msg\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_msg(msg);\n    });\n});\n// TODO: test that this actually works\nShiny.addCustomMessageHandler(\"shinywidgets_comm_close\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_close(msg);\n    });\n});\n// Our version of https://github.com/jupyter-widgets/widget-cookiecutter/blob/9694718/%7B%7Bcookiecutter.github_project_name%7D%7D/js/lib/extension.js#L8\nfunction setBaseURL(x = '') {\n    const base_url = document.querySelector('body').getAttribute('data-base-url');\n    if (!base_url) {\n        document.querySelector('body').setAttribute('data-base-url', x);\n    }\n}\n\n\n//# sourceURL=webpack://@jupyter-widgets/shiny-embed-manager/./src/output.ts?");
 
                     /***/
                 }),
 
             /***/
             "./src/utils.ts":
                 /*!**********************!*\
                   !*** ./src/utils.ts ***!
                   \**********************/
                 /***/
                 ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
-                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"jsonParse\": () => (/* binding */ jsonParse)\n/* harmony export */ });\n/* harmony import */ var base64_arraybuffer__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! base64-arraybuffer */ \"./node_modules/base64-arraybuffer/dist/base64-arraybuffer.es5.js\");\n\n// On the server, we're using jupyter_client.session.json_packer to serialize messages,\n// and it encodes binary data (i.e., buffers) as base64, so decode it before passing it\n// along to the comm logic\nfunction jsonParse(x) {\n    const msg = JSON.parse(x);\n    msg.buffers = msg.buffers.map((b) => (0,base64_arraybuffer__WEBPACK_IMPORTED_MODULE_0__.decode)(b));\n    return msg;\n}\n\n\n//# sourceURL=webpack://@jupyter-widgets/prism-embed-manager/./src/utils.ts?");
+                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"Throttler\": () => (/* binding */ Throttler),\n/* harmony export */   \"jsonParse\": () => (/* binding */ jsonParse)\n/* harmony export */ });\n/* harmony import */ var base64_arraybuffer__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! base64-arraybuffer */ \"./node_modules/base64-arraybuffer/dist/base64-arraybuffer.es5.js\");\n\n// On the server, we're using jupyter_client.session.json_packer to serialize messages,\n// and it encodes binary data (i.e., buffers) as base64, so decode it before passing it\n// along to the comm logic\nfunction jsonParse(x) {\n    const msg = JSON.parse(x);\n    msg.buffers = msg.buffers.map((b) => (0,base64_arraybuffer__WEBPACK_IMPORTED_MODULE_0__.decode)(b));\n    return msg;\n}\nclass Throttler {\n    constructor(wait = 100) {\n        if (wait < 0)\n            throw new Error(\"wait must be a positive number\");\n        this.wait = wait;\n        this._reset();\n    }\n    // Try to execute the function immediately, if it is not waiting\n    // If it is waiting, update the function to be called\n    throttle(fn) {\n        if (fn.length > 0)\n            throw new Error(\"fn must not take any arguments\");\n        if (this.isWaiting) {\n            // If the timeout is currently waiting, update the func to be called\n            this.fnToCall = fn;\n        }\n        else {\n            // If there is nothing waiting, call it immediately\n            // and start the throttling\n            fn();\n            this._setTimeout();\n        }\n    }\n    // Execute the function immediately and reset the timeout\n    // This is useful when the timeout is waiting and we want to\n    // execute the function immediately to not have events be out\n    // of order\n    flush() {\n        if (this.fnToCall)\n            this.fnToCall();\n        this._reset();\n    }\n    _setTimeout() {\n        this.timeoutId = setTimeout(() => {\n            if (this.fnToCall) {\n                this.fnToCall();\n                this.fnToCall = null;\n                // Restart the timeout as we just called the function\n                // This call is the key step of Throttler\n                this._setTimeout();\n            }\n            else {\n                this._reset();\n            }\n        }, this.wait);\n    }\n    _reset() {\n        this.fnToCall = null;\n        clearTimeout(this.timeoutId);\n        this.timeoutId = null;\n    }\n    get isWaiting() {\n        return this.timeoutId !== null;\n    }\n}\n\n\n\n//# sourceURL=webpack://@jupyter-widgets/shiny-embed-manager/./src/utils.ts?");
 
                     /***/
                 }),
 
             /***/
             "@jupyter-widgets/html-manager":
                 /*!************************************************!*\
```

### Comparing `shinywidgets-0.1.6/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js` & `shinywidgets-0.2.0/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.1.6/shinywidgets.egg-info/SOURCES.txt` & `shinywidgets-0.2.0/shinywidgets.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 shinywidgets/__init__.py
+shinywidgets/_as_widget.py
 shinywidgets/_comm.py
 shinywidgets/_dependencies.py
 shinywidgets/_serialization.py
 shinywidgets/_shinywidgets.py
 shinywidgets.egg-info/PKG-INFO
 shinywidgets.egg-info/SOURCES.txt
 shinywidgets.egg-info/dependency_links.txt
```

