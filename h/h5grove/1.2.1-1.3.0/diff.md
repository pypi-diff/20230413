# Comparing `tmp/h5grove-1.2.1.tar.gz` & `tmp/h5grove-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/h5grove/h5grove/dist/tmpx1a61d93/h5grove-1.2.1.tar", last modified: Thu Oct 27 09:17:19 2022, max compression
+gzip compressed data, was "/home/runner/work/h5grove/h5grove/dist/.tmp-xi4nym22/h5grove-1.3.0.tar", last modified: Thu Apr 13 14:10:10 2023, max compression
```

## Comparing `h5grove-1.2.1.tar` & `h5grove-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 09:17:19.000000 h5grove-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-10-27 09:16:25.000000 h5grove-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-10-27 09:16:25.000000 h5grove-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-10-27 09:17:19.000000 h5grove-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-10-27 09:16:25.000000 h5grove-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 09:17:19.000000 h5grove-1.2.1/example/
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-10-27 09:16:25.000000 h5grove-1.2.1/example/fastapi_app.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1641 2022-10-27 09:16:25.000000 h5grove-1.2.1/example/flask_app.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1246 2022-10-27 09:16:25.000000 h5grove-1.2.1/example/tornado_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 09:17:19.000000 h5grove-1.2.1/h5grove/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9288 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     4475 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3701 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/flask_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/tornado_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7809 2022-10-27 09:16:25.000000 h5grove-1.2.1/h5grove/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 09:17:19.000000 h5grove-1.2.1/h5grove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-10-27 09:17:19.000000 h5grove-1.2.1/h5grove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-27 09:17:19.000000 h5grove-1.2.1/h5grove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 09:17:19.000000 h5grove-1.2.1/h5grove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-10-27 09:17:19.000000 h5grove-1.2.1/h5grove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-27 09:17:19.000000 h5grove-1.2.1/h5grove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-10-27 09:16:25.000000 h5grove-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-10-27 09:17:19.000000 h5grove-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-27 09:16:25.000000 h5grove-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:10:10.000000 h5grove-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-13 14:09:19.000000 h5grove-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-13 14:09:19.000000 h5grove-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-13 14:10:10.000000 h5grove-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-13 14:09:19.000000 h5grove-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:10:10.000000 h5grove-1.3.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-13 14:09:19.000000 h5grove-1.3.0/example/fastapi_app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1641 2023-04-13 14:09:19.000000 h5grove-1.3.0/example/flask_app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1246 2023-04-13 14:09:19.000000 h5grove-1.3.0/example/tornado_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:10:10.000000 h5grove-1.3.0/h5grove/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/flask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/tornado_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-04-13 14:09:19.000000 h5grove-1.3.0/h5grove/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:10:10.000000 h5grove-1.3.0/h5grove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-13 14:10:10.000000 h5grove-1.3.0/h5grove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-13 14:10:10.000000 h5grove-1.3.0/h5grove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:10:10.000000 h5grove-1.3.0/h5grove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-13 14:10:10.000000 h5grove-1.3.0/h5grove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 14:10:10.000000 h5grove-1.3.0/h5grove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 14:09:19.000000 h5grove-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-13 14:10:10.000000 h5grove-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 14:09:19.000000 h5grove-1.3.0/setup.py
```

### Comparing `h5grove-1.2.1/LICENSE` & `h5grove-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h5grove-1.2.1/PKG-INFO` & `h5grove-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5grove
-Version: 1.2.1
+Version: 1.3.0
 Summary: Core utilities to serve HDF5 file contents
 Home-page: https://github.com/silx-kit/h5grove
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silx-kit/h5grove/-/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `h5grove-1.2.1/README.md` & `h5grove-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `h5grove-1.2.1/example/fastapi_app.py` & `h5grove-1.3.0/example/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `h5grove-1.2.1/example/flask_app.py` & `h5grove-1.3.0/example/flask_app.py`

 * *Files identical despite different names*

### Comparing `h5grove-1.2.1/example/tornado_app.py` & `h5grove-1.3.0/example/tornado_app.py`

 * *Files identical despite different names*

### Comparing `h5grove-1.2.1/h5grove/content.py` & `h5grove-1.3.0/h5grove/content.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,20 @@
     import hdf5plugin  # noqa: F401
 except ImportError:
     pass
 
 from .models import LinkResolution, Selection
 from .utils import (
     NotFoundError,
+    QueryArgumentError,
     attr_metadata,
     convert,
     get_array_stats,
+    open_file_with_error_fallback,
+    parse_link_resolution_arg,
     stringify_dtype,
     get_filters,
     get_entity_from_file,
     hdf_path_join,
     get_dataset_slice,
     sorted_dict,
 )
@@ -270,25 +273,67 @@
 
 
 @contextlib.contextmanager
 def get_content_from_file(
     filepath: Union[str, Path],
     path: Optional[str],
     create_error: Callable[[int, str], Exception],
-    resolve_links: LinkResolution = LinkResolution.ONLY_VALID,
+    resolve_links_arg: Optional[str] = LinkResolution.ONLY_VALID,
     h5py_options: Dict[str, Any] = {},
 ):
+    f = open_file_with_error_fallback(filepath, create_error, h5py_options)
+
     try:
-        f = h5py.File(filepath, "r", **h5py_options)
-    except OSError as e:
-        if isinstance(e, FileNotFoundError) or "No such file or directory" in str(e):
-            raise create_error(404, "File not found!")
-        if isinstance(e, PermissionError) or "Permission denied" in str(e):
-            raise create_error(403, "Cannot read file: Permission denied!")
-        raise e
+        resolve_links = parse_link_resolution_arg(
+            resolve_links_arg,
+            fallback=LinkResolution.ONLY_VALID,
+        )
+    except QueryArgumentError as e:
+        raise create_error(422, str(e))
 
     try:
         yield create_content(f, path, resolve_links)
     except NotFoundError as e:
         raise create_error(404, str(e))
+    except QueryArgumentError as e:
+        raise create_error(422, str(e))
+    finally:
+        f.close()
+
+
+@contextlib.contextmanager
+def get_list_of_paths(
+    filepath: Union[str, Path],
+    base_path: Optional[str],
+    create_error: Callable[[int, str], Exception],
+    resolve_links_arg: Optional[str] = LinkResolution.ONLY_VALID,
+    h5py_options: Dict[str, Any] = {},
+):
+    f = open_file_with_error_fallback(filepath, create_error, h5py_options)
+
+    try:
+        resolve_links = parse_link_resolution_arg(
+            resolve_links_arg,
+            fallback=LinkResolution.ONLY_VALID,
+        )
+    except QueryArgumentError as e:
+        raise create_error(422, str(e))
+
+    names = []
+
+    def get_path(name: str):
+        full_path = hdf_path_join(base_path, name)
+        content = create_content(f, full_path, resolve_links)
+        names.append(content.path)
+
+    try:
+        base_content = create_content(f, base_path, resolve_links)
+        assert isinstance(base_content, GroupContent)
+        names.append(base_content.path)
+        base_content._h5py_entity.visit(get_path)
+        yield names
+    except NotFoundError as e:
+        raise create_error(404, str(e))
+    except QueryArgumentError as e:
+        raise create_error(422, str(e))
     finally:
         f.close()
```

### Comparing `h5grove-1.2.1/h5grove/encoders.py` & `h5grove-1.3.0/h5grove/encoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 from typing import Any, Callable, Dict, Optional, Union
 import numpy as np
 import orjson
 import h5py
 import tifffile
 
-from .utils import is_numeric_data
+from .utils import QueryArgumentError, is_numeric_data
 
 
 def bin_encode(array: np.ndarray) -> bytes:
     """Convert array to bytes.
 
     :param array: Data to convert
     """
@@ -98,25 +98,27 @@
     :param encoding:
         - `json` (default)
         - `bin`: nD array/scalars in bytes
         - `csv`: nD arrays in downloadable csv files
         - `npy`: nD arrays in downloadable npy files
         - `tiff`: 2D arrays in downloadable TIFF files
     :returns: A Response object containing content and headers
-    :raises ValueError: If encoding is not among the ones above.
+    :raises QueryArgumentError: If encoding is not among the ones above.
     """
     if encoding in ("json", None):
         return Response(
             orjson_encode(content),
             headers={"Content-Type": "application/json"},
         )
 
     content_array = np.array(content, copy=False)
     if not is_numeric_data(content_array):
-        raise ValueError(f"Unsupported encoding {encoding} for non-numeric content")
+        raise QueryArgumentError(
+            f"Unsupported encoding {encoding} for non-numeric content"
+        )
 
     if encoding == "bin":
         return Response(
             bin_encode(content_array),
             headers={
                 "Content-Type": "application/octet-stream",
             },
@@ -145,8 +147,8 @@
             tiff_encode(content_array),
             headers={
                 "Content-Type": "image/tiff",
                 "Content-Disposition": 'attachment; filename="data.tiff"',
             },
         )
 
-    raise ValueError(f"Unsupported encoding {encoding}")
+    raise QueryArgumentError(f"Unsupported encoding {encoding}")
```

### Comparing `h5grove-1.2.1/h5grove/fastapi_utils.py` & `h5grove-1.3.0/h5grove/fastapi_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 from pydantic import BaseSettings
 from typing import List, Optional, Union, Callable
 
 from .content import (
     DatasetContent,
     ResolvedEntityContent,
     get_content_from_file,
+    get_list_of_paths,
 )
 from .encoders import encode
-from .models import LinkResolution
-from .utils import parse_link_resolution_arg
 
 __all__ = [
     "router",
     "settings",
     "get_attr",
     "get_data",
     "get_meta",
@@ -112,18 +111,15 @@
 @router.get("/meta/")
 async def get_meta(
     file: str = Depends(add_base_path),
     path: str = "/",
     resolve_links: str = "only_valid",
 ):
     """`/meta/` endpoint handler"""
-    resolve_links = parse_link_resolution_arg(
-        resolve_links,
-        fallback=LinkResolution.ONLY_VALID,
-    )
+
     with get_content_from_file(file, path, create_error, resolve_links) as content:
         h5grove_response = encode(content.metadata(), "json")
         return Response(
             content=h5grove_response.content, headers=h5grove_response.headers
         )
 
 
@@ -134,7 +130,20 @@
     """`/stats/` endpoint handler"""
     with get_content_from_file(file, path, create_error) as content:
         assert isinstance(content, DatasetContent)
         h5grove_response = encode(content.data_stats(selection), "json")
         return Response(
             content=h5grove_response.content, headers=h5grove_response.headers
         )
+
+
+@router.get("/paths/")
+async def get_paths(
+    file: str = Depends(add_base_path),
+    path: str = "/",
+    resolve_links: str = "only_valid",
+):
+    with get_list_of_paths(file, path, create_error, resolve_links) as paths:
+        h5grove_response = encode(paths, "json")
+        return Response(
+            content=h5grove_response.content, headers=h5grove_response.headers
+        )
```

### Comparing `h5grove-1.2.1/h5grove/flask_utils.py` & `h5grove-1.3.0/h5grove/flask_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Helpers for usage with `Flask <https://flask.palletsprojects.com/>`_"""
 from werkzeug.exceptions import HTTPException
 from flask import Blueprint, current_app, request, Response, Request
 import os
 from typing import Any, Callable, Mapping, Optional
 
 
-from .content import DatasetContent, ResolvedEntityContent, get_content_from_file
+from .content import (
+    DatasetContent,
+    ResolvedEntityContent,
+    get_content_from_file,
+    get_list_of_paths,
+)
 from .encoders import encode
-from .models import LinkResolution
-from .utils import parse_bool_arg, parse_link_resolution_arg
+from .utils import parse_bool_arg
 
 
 __all__ = [
     "attr_route",
     "data_route",
     "meta_route",
+    "paths_route",
     "stats_route",
     "URL_RULES",
     "BLUEPRINT",
 ]
 
 
 def make_encoded_response(
@@ -73,23 +78,29 @@
         return make_encoded_response(data, format_arg)
 
 
 def meta_route():
     """`/meta/` endpoint handler"""
     filename = get_filename(request)
     path = request.args.get("path")
-    resolve_links = parse_link_resolution_arg(
-        request.args.get("resolve_links", None),
-        fallback=LinkResolution.ONLY_VALID,
-    )
+    resolve_links = request.args.get("resolve_links", None)
 
     with get_content_from_file(filename, path, create_error, resolve_links) as content:
         return make_encoded_response(content.metadata())
 
 
+def paths_route():
+    filename = get_filename(request)
+    path = request.args.get("path")
+    resolve_links = request.args.get("resolve_links", None)
+
+    with get_list_of_paths(filename, path, create_error, resolve_links) as paths:
+        return make_encoded_response(paths)
+
+
 def stats_route():
     """`/stats/` endpoint handler"""
     filename = get_filename(request)
     path = request.args.get("path")
     selection = request.args.get("selection")
 
     with get_content_from_file(filename, path, create_error) as content:
@@ -97,14 +108,15 @@
         return make_encoded_response(content.data_stats(selection))
 
 
 URL_RULES = {
     "/attr/": attr_route,
     "/data/": data_route,
     "/meta/": meta_route,
+    "/paths/": paths_route,
     "/stats/": stats_route,
 }
 """Mapping of Flask URL endpoints to handlers"""
 
 
 BLUEPRINT = Blueprint("h5grove", __name__)
 """Blueprint of h5grove endpoints.
```

### Comparing `h5grove-1.2.1/h5grove/models.py` & `h5grove-1.3.0/h5grove/models.py`

 * *Files identical despite different names*

### Comparing `h5grove-1.2.1/h5grove/tornado_utils.py` & `h5grove-1.3.0/h5grove/tornado_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from tornado.web import HTTPError, MissingArgumentError, RequestHandler
 
 from .content import (
     DatasetContent,
     EntityContent,
     ResolvedEntityContent,
     get_content_from_file,
+    get_list_of_paths,
 )
 from .encoders import Response, encode
-from .models import LinkResolution
-from .utils import parse_bool_arg, parse_link_resolution_arg
+from .utils import parse_bool_arg
 
 __all__ = [
     "BaseHandler",
     "AttributeHandler",
     "DataHandler",
     "MetadataHandler",
     "StatisticsHandler",
@@ -39,94 +39,117 @@
         file_path = self.get_query_argument("file")
         if file_path is None:
             raise MissingArgumentError("file")
 
         path = self.get_query_argument("path", None, strip=False)
 
         full_file_path = os.path.join(self.base_dir, file_path)
-        resolve_links = parse_link_resolution_arg(
-            self.get_query_argument("resolve_links", None),
-            fallback=LinkResolution.ONLY_VALID,
-        )
 
-        with get_content_from_file(
-            full_file_path, path, create_error, resolve_links
-        ) as content:
-            response = self.get_response(content)
+        response = self.get_response(
+            full_file_path, path, self.get_query_argument("resolve_links", None)
+        )
 
         for key, value in response.headers.items():
             self.set_header(key, value)
 
         self.write(response.content)
         self.finish()
 
-    def get_response(self, content: EntityContent) -> Response:
+    def get_response(
+        self, full_file_path: str, path: Optional[str], resolve_links: Optional[str]
+    ) -> Response:
         raise NotImplementedError
 
     def prepare(self):
         if self.allow_origin is not None:
             self.set_header("Access-Control-Allow-Origin", self.allow_origin)
 
     def write_error(self, status_code: int, **kwargs: Any) -> None:
         self.prepare()
         self.finish({"message": self._reason})
 
 
-class AttributeHandler(BaseHandler):
+class ContentHandler(BaseHandler):
+    def get_response(
+        self, full_file_path: str, path: Optional[str], resolve_links: Optional[str]
+    ) -> Response:
+        with get_content_from_file(
+            full_file_path, path, create_error, resolve_links
+        ) as content:
+            response = self.get_content_response(content)
+
+        return response
+
+    def get_content_response(self, content: EntityContent) -> Response:
+        raise NotImplementedError
+
+
+class AttributeHandler(ContentHandler):
     """/attr/ endpoint handler"""
 
-    def get_response(self, content: EntityContent) -> Response:
+    def get_content_response(self, content: EntityContent) -> Response:
         assert isinstance(content, ResolvedEntityContent)
 
         attr_keys = self.get_query_arguments("attr_keys", strip=False)
         # get_query_arguments returns an empty list if `attr_keys` is not present
         return encode(content.attributes(attr_keys if len(attr_keys) > 0 else None))
 
 
-class DataHandler(BaseHandler):
+class DataHandler(ContentHandler):
     """/data/ endpoint handler"""
 
-    def get_response(self, content: EntityContent) -> Response:
+    def get_content_response(self, content: EntityContent) -> Response:
         dtype = self.get_query_argument("dtype", None)
         format_arg = self.get_query_argument("format", None)
         selection = self.get_query_argument("selection", None)
         flatten = parse_bool_arg(
             self.get_query_argument("flatten", None), fallback=False
         )
 
         assert isinstance(content, DatasetContent)
         data = content.data(selection, flatten, dtype)
         return encode(data, format_arg)
 
 
-class MetadataHandler(BaseHandler):
+class MetadataHandler(ContentHandler):
     """/meta/ endpoint handler"""
 
-    def get_response(self, content: EntityContent) -> Response:
+    def get_content_response(self, content: EntityContent) -> Response:
         return encode(content.metadata())
 
 
-class StatisticsHandler(BaseHandler):
+class StatisticsHandler(ContentHandler):
     """/stats/ endpoint handler"""
 
-    def get_response(self, content: EntityContent) -> Response:
+    def get_content_response(self, content: EntityContent) -> Response:
         selection = self.get_query_argument("selection", None)
 
         assert isinstance(content, DatasetContent)
         return encode(content.data_stats(selection))
 
 
+class PathsHandler(BaseHandler):
+    def get_response(
+        self, full_file_path: str, path: Optional[str], resolve_links: Optional[str]
+    ) -> Response:
+        with get_list_of_paths(
+            full_file_path, path, create_error, resolve_links
+        ) as paths:
+            return encode(paths)
+
+
 # TODO: Setting the return type raises mypy errors
 def get_handlers(base_dir: Optional[str], allow_origin: Optional[str] = None):
     """Build h5grove handlers (`/attr`, `/data`, `/meta` and `/stats`).
 
     :param base_dir: Base directory from which the HDF5 files will be served
     :param allow_origin: Allowed origins for CORS
     :return type: List[Tuple[str, BaseHandler, dict]]
     """
     init_args = {"base_dir": base_dir, "allow_origin": allow_origin}
     return [
         (r"/attr/.*", AttributeHandler, init_args),
         (r"/data/.*", DataHandler, init_args),
         (r"/meta/.*", MetadataHandler, init_args),
+        (r"/paths/.*", PathsHandler, init_args),
         (r"/stats/.*", StatisticsHandler, init_args),
     ]
```

### Comparing `h5grove-1.2.1/h5grove/utils.py` & `h5grove-1.3.0/h5grove/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from pathlib import Path
 import h5py
 from h5py.version import version_tuple as h5py_version
 from os.path import basename
 import numpy as np
-from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
 from .models import H5pyEntity, LinkResolution, Selection, StrDtype
 
 
 class NotFoundError(Exception):
     pass
 
@@ -15,14 +16,18 @@
     pass
 
 
 class LinkError(NotFoundError):
     pass
 
 
+class QueryArgumentError(ValueError):
+    pass
+
+
 def _get_attr_id(entity_attrs: h5py.AttributeManager, attr_name: str):
     return entity_attrs.get_id(attr_name)
 
 
 def _legacy_get_attr_id(entity_attrs: h5py.AttributeManager, attr_name: str):
     return h5py.h5a.open(entity_attrs._id, entity_attrs._e(attr_name))
 
@@ -70,49 +75,52 @@
             raise LinkError(
                 f"Cannot resolve {link} at {path} of {basename(h5file.filename)}"
             )
 
     return h5file[path]
 
 
-def parse_slice(dataset: h5py.Dataset, slice_str: str) -> Tuple[Union[slice, int], ...]:
+def parse_slice(slice_str: str) -> Tuple[Union[slice, int], ...]:
+    """
+    Parses a string containing a slice under NumPy format.
+
+    Examples:
+        '5' => (5,)
+        '1, 2:5' => (1, slice(2,5))
+        '0:10:5, 2, 3:' => (slice(0, 10, 5), 2, slice(3, None, None))
+
+    :param slice_str: String containing the slice
+    """
     if "," not in slice_str:
-        return (parse_slice_member(slice_str, dataset.shape[0]),)
+        return (parse_slice_member(slice_str),)
 
     slice_members = slice_str.split(",")
 
-    if len(slice_members) > dataset.ndim:
-        raise TypeError(
-            f"{slice_str} is a {len(slice_members)}d slice while the dataset is {dataset.ndim}d"
-        )
-
-    return tuple(
-        parse_slice_member(s, dataset.shape[i]) for i, s in enumerate(slice_members)
-    )
+    return tuple(parse_slice_member(s) for s in slice_members)
 
 
-def parse_slice_member(slice_member: str, max_dim: int) -> Union[slice, int]:
+def parse_slice_member(slice_member: str) -> Union[slice, int]:
     if ":" not in slice_member:
         return int(slice_member)
 
     slice_params = slice_member.split(":")
     if len(slice_params) == 2:
         start, stop = slice_params
 
         return slice(
-            int(start) if start != "" else 0, int(stop) if stop != "" else max_dim
+            int(start) if start != "" else 0, int(stop) if stop != "" else None
         )
 
     if len(slice_params) == 3:
         start, stop, step = slice_params
 
         return slice(
-            int(start) if start != "" else 0,
-            int(stop) if stop != "" else max_dim,
-            int(step) if step != "" else 1,
+            int(start) if start != "" else None,
+            int(stop) if stop != "" else None,
+            int(step) if step != "" else None,
         )
 
     raise TypeError(f"{slice_member} is not a valid slice")
 
 
 def sorted_dict(*args: Tuple[str, Any]):
     return dict(sorted(args))
@@ -158,21 +166,26 @@
         - `safe`: Convert to a type supported by JS typedarray (https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/TypedArray)
     """
     if dtype in ("origin", None):
         return data
 
     if dtype == "safe":
         if not is_numeric_data(data):
-            raise ValueError(f"Unsupported dtype {dtype} for non-numeric content")
+            raise QueryArgumentError(
+                f"Unsupported dtype {dtype} for non-numeric content"
+            )
         return data.astype(_sanitize_dtype(data.dtype), order="C", copy=False)
 
-    raise ValueError(f"Unsupported dtype {dtype}")
+    raise QueryArgumentError(f"Unsupported dtype {dtype}")
+
 
+def is_numeric_data(data: Union[np.ndarray, np.number, np.bool_, bytes]) -> bool:
+    if not isinstance(data, (np.ndarray, np.number, np.bool_)):
+        return False
 
-def is_numeric_data(data: Union[np.ndarray, np.number, np.bool_]) -> bool:
     return np.issubdtype(data.dtype, np.number) or np.issubdtype(data.dtype, np.bool_)
 
 
 def get_array_stats(data: np.ndarray) -> Dict[str, Union[float, int, None]]:
     if data.size == 0:
         return {
             "strict_positive_min": None,
@@ -196,16 +209,16 @@
         "min": cast(np.min(data)),
         "max": cast(np.max(data)),
         "mean": cast(np.mean(data)),
         "std": cast(np.std(data)),
     }
 
 
-def hdf_path_join(prefix, suffix):
-    if prefix == "/":
+def hdf_path_join(prefix: Union[str, None], suffix: str):
+    if prefix is None or prefix == "/":
         return f"/{suffix}"
 
     return f'{prefix.rstrip("/")}/{suffix}'
 
 
 def parse_bool_arg(query_arg: Union[str, None], fallback: bool) -> bool:
     if query_arg is None:
@@ -228,25 +241,30 @@
 
     if query_arg in ("false", LinkResolution.NONE):
         return LinkResolution.NONE
 
     if query_arg == LinkResolution.ONLY_VALID:
         return LinkResolution.ONLY_VALID
 
-    raise ValueError(
-        f"{raw_query_arg} is not a valid value for link resolution. Accepted values are: {LinkResolution.ALL}, f{LinkResolution.NONE} or {LinkResolution.ONLY_VALID}"
+    raise QueryArgumentError(
+        f"{raw_query_arg} is not a valid value for link resolution. Accepted values are: {LinkResolution.ALL}, {LinkResolution.NONE} or {LinkResolution.ONLY_VALID}"
     )
 
 
 def get_dataset_slice(dataset: h5py.Dataset, selection: Selection):
     if selection is None:
         return dataset[()]
 
     if isinstance(selection, str):
-        return dataset[parse_slice(dataset, selection)]
+        parsed_slice = parse_slice(selection)
+        if len(parsed_slice) > dataset.ndim:
+            raise ValueError(
+                f"{selection} has too many members to slice a {dataset.ndim}D dataset"
+            )
+        return dataset[parsed_slice]
 
     return dataset[selection]
 
 
 def get_filters(
     dataset: h5py.Dataset,
 ) -> Optional[List[Dict[str, Union[int, str]]]]:
@@ -271,7 +289,24 @@
 def stringify_dtype(dtype: np.dtype) -> StrDtype:
     if dtype.fields is None:
         return dtype.str
 
     return {
         k: stringify_dtype(dtype_tuple[0]) for k, dtype_tuple in dtype.fields.items()
     }
+
+
+def open_file_with_error_fallback(
+    filepath: Union[str, Path],
+    create_error: Callable[[int, str], Exception],
+    h5py_options: Dict[str, Any] = {},
+) -> h5py.File:
+    try:
+        f = h5py.File(filepath, "r", **h5py_options)
+    except OSError as e:
+        if isinstance(e, FileNotFoundError) or "No such file or directory" in str(e):
+            raise create_error(404, "File not found!")
+        if isinstance(e, PermissionError) or "Permission denied" in str(e):
+            raise create_error(403, "Cannot read file: Permission denied!")
+        raise e
+
+    return f
```

### Comparing `h5grove-1.2.1/h5grove.egg-info/PKG-INFO` & `h5grove-1.3.0/h5grove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5grove
-Version: 1.2.1
+Version: 1.3.0
 Summary: Core utilities to serve HDF5 file contents
 Home-page: https://github.com/silx-kit/h5grove
 Author: European Synchrotron Radiation Facility
 Author-email: h5web@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silx-kit/h5grove/-/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `h5grove-1.2.1/setup.cfg` & `h5grove-1.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 	check-manifest
 	flake8
 	h5grove[fastapi]
 	h5grove[flask]
 	invoke
 	mypy
 	myst-parser
+	httpx >= 0.23
 	pytest
 	pytest-benchmark
 	pytest-cov
 	pytest-tornado
 	sphinx
 	sphinx-argparse
 	h5grove[tornado]
```

