# Comparing `tmp/fastapi_versionizer-0.1.3.tar.gz` & `tmp/fastapi_versionizer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastapi_versionizer-0.1.3.tar", last modified: Tue Mar 14 06:29:51 2023, max compression
+gzip compressed data, was "dist/fastapi_versionizer-0.1.4.tar", last modified: Thu Apr 13 04:12:44 2023, max compression
```

## Comparing `fastapi_versionizer-0.1.3.tar` & `fastapi_versionizer-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/
--rw-r--r--   0 alexschimpf   (501) staff       (20)     3447 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/PKG-INFO
-drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/fastapi_versionizer.egg-info/
--rw-r--r--   0 alexschimpf   (501) staff       (20)     3447 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/fastapi_versionizer.egg-info/PKG-INFO
--rw-r--r--   0 alexschimpf   (501) staff       (20)      336 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/fastapi_versionizer.egg-info/SOURCES.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)       26 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/fastapi_versionizer.egg-info/requires.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)       20 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/fastapi_versionizer.egg-info/top_level.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)        1 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/fastapi_versionizer.egg-info/dependency_links.txt
--rw-r--r--   0 alexschimpf   (501) staff       (20)     1076 2022-12-22 21:04:28.000000 fastapi_versionizer-0.1.3/LICENSE
--rw-r--r--   0 alexschimpf   (501) staff       (20)     2690 2023-03-14 06:24:16.000000 fastapi_versionizer-0.1.3/README.md
--rw-r--r--   0 alexschimpf   (501) staff       (20)     1060 2023-03-14 06:24:55.000000 fastapi_versionizer-0.1.3/setup.py
-drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/fastapi_versionizer/
--rw-r--r--   0 alexschimpf   (501) staff       (20)      101 2022-12-22 21:10:07.000000 fastapi_versionizer-0.1.3/fastapi_versionizer/__init__.py
--rw-r--r--   0 alexschimpf   (501) staff       (20)     8442 2023-03-14 06:24:16.000000 fastapi_versionizer-0.1.3/fastapi_versionizer/versionizer.py
--rw-r--r--   0 alexschimpf   (501) staff       (20)        0 2022-12-23 09:34:59.000000 fastapi_versionizer-0.1.3/fastapi_versionizer/py.typed
--rw-r--r--   0 alexschimpf   (501) staff       (20)       38 2023-03-14 06:29:51.000000 fastapi_versionizer-0.1.3/setup.cfg
+drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     3653 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/PKG-INFO
+drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     3653 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/PKG-INFO
+-rw-r--r--   0 alexschimpf   (501) staff       (20)      336 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/SOURCES.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)       26 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/requires.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)       20 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/top_level.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)        1 2023-04-13 04:12:43.000000 fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/dependency_links.txt
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     1076 2022-12-22 21:04:28.000000 fastapi_versionizer-0.1.4/LICENSE
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     2896 2023-04-13 04:11:12.000000 fastapi_versionizer-0.1.4/README.md
+-rw-r--r--   0 alexschimpf   (501) staff       (20)     1060 2023-04-13 04:11:39.000000 fastapi_versionizer-0.1.4/setup.py
+drwxr-xr-x   0 alexschimpf   (501) staff       (20)        0 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/
+-rw-r--r--   0 alexschimpf   (501) staff       (20)      101 2022-12-22 21:10:07.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/__init__.py
+-rw-r--r--   0 alexschimpf   (501) staff       (20)    10234 2023-04-13 04:11:12.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/versionizer.py
+-rw-r--r--   0 alexschimpf   (501) staff       (20)        0 2022-12-23 09:34:59.000000 fastapi_versionizer-0.1.4/fastapi_versionizer/py.typed
+-rw-r--r--   0 alexschimpf   (501) staff       (20)       38 2023-04-13 04:12:44.000000 fastapi_versionizer-0.1.4/setup.cfg
```

### Comparing `fastapi_versionizer-0.1.3/PKG-INFO` & `fastapi_versionizer-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_versionizer
-Version: 0.1.3
+Version: 0.1.4
 Summary: API versionizer for FastAPI web applications
 Home-page: https://github.com/alexschimpf/fastapi-versionizer
 Author: Alex Schimpf
 Author-email: aschimpf1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -30,14 +30,16 @@
 
 ## Examples
 You can find examples in the [examples](https://github.com/alexschimpf/fastapi-versionizer/tree/main/examples) directory.
 
 ## Details
 - Routes can be annotated using the `@api_version` decorator
   - This essentially says, "This route is available from version (major, minor) onward, until a new version of the route is defined."
+- Routes can be annotated using the `@api_version_remove` decorator
+  - This essentially says, "This route is removed from version (major, minor) onward, until a new version of the route is defined again."
 - Use the `versionize` function on your FastAPI app to perform the versionizing magic
   - Each version results in a new mounted FastAPI sub-application with a version prefix you define
   - Unlike `fastapi_versioning`, this does not return a new FastAPI app, but applies the versioning directly to the app you provide
   - You can generate a "latest" alias for the latest version using `enable_latest` and `latest_prefix`
   - You can customize your OpenAPI schemas at runtime using `get_openapi`
     - This will be used to override the `openapi` function of all versioned FastAPI sub-applications
   - You can generate each versioned Swagger page using `get_docs` and `docs_url`
```

### Comparing `fastapi_versionizer-0.1.3/fastapi_versionizer.egg-info/PKG-INFO` & `fastapi_versionizer-0.1.4/fastapi_versionizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-versionizer
-Version: 0.1.3
+Version: 0.1.4
 Summary: API versionizer for FastAPI web applications
 Home-page: https://github.com/alexschimpf/fastapi-versionizer
 Author: Alex Schimpf
 Author-email: aschimpf1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -30,14 +30,16 @@
 
 ## Examples
 You can find examples in the [examples](https://github.com/alexschimpf/fastapi-versionizer/tree/main/examples) directory.
 
 ## Details
 - Routes can be annotated using the `@api_version` decorator
   - This essentially says, "This route is available from version (major, minor) onward, until a new version of the route is defined."
+- Routes can be annotated using the `@api_version_remove` decorator
+  - This essentially says, "This route is removed from version (major, minor) onward, until a new version of the route is defined again."
 - Use the `versionize` function on your FastAPI app to perform the versionizing magic
   - Each version results in a new mounted FastAPI sub-application with a version prefix you define
   - Unlike `fastapi_versioning`, this does not return a new FastAPI app, but applies the versioning directly to the app you provide
   - You can generate a "latest" alias for the latest version using `enable_latest` and `latest_prefix`
   - You can customize your OpenAPI schemas at runtime using `get_openapi`
     - This will be used to override the `openapi` function of all versioned FastAPI sub-applications
   - You can generate each versioned Swagger page using `get_docs` and `docs_url`
```

### Comparing `fastapi_versionizer-0.1.3/LICENSE` & `fastapi_versionizer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_versionizer-0.1.3/README.md` & `fastapi_versionizer-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 ## Examples
 You can find examples in the [examples](https://github.com/alexschimpf/fastapi-versionizer/tree/main/examples) directory.
 
 ## Details
 - Routes can be annotated using the `@api_version` decorator
   - This essentially says, "This route is available from version (major, minor) onward, until a new version of the route is defined."
+- Routes can be annotated using the `@api_version_remove` decorator
+  - This essentially says, "This route is removed from version (major, minor) onward, until a new version of the route is defined again."
 - Use the `versionize` function on your FastAPI app to perform the versionizing magic
   - Each version results in a new mounted FastAPI sub-application with a version prefix you define
   - Unlike `fastapi_versioning`, this does not return a new FastAPI app, but applies the versioning directly to the app you provide
   - You can generate a "latest" alias for the latest version using `enable_latest` and `latest_prefix`
   - You can customize your OpenAPI schemas at runtime using `get_openapi`
     - This will be used to override the `openapi` function of all versioned FastAPI sub-applications
   - You can generate each versioned Swagger page using `get_docs` and `docs_url`
```

### Comparing `fastapi_versionizer-0.1.3/setup.py` & `fastapi_versionizer-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='fastapi_versionizer',
-    version='0.1.3',
+    version='0.1.4',
     author='Alex Schimpf',
     author_email='aschimpf1@gmail.com',
     description='API versionizer for FastAPI web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/alexschimpf/fastapi-versionizer',
     package_data={'fastapi_versionizer': ['py.typed']},
```

### Comparing `fastapi_versionizer-0.1.3/fastapi_versionizer/versionizer.py` & `fastapi_versionizer-0.1.4/fastapi_versionizer/versionizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from fastapi import FastAPI
 from fastapi.responses import HTMLResponse
 from fastapi.routing import APIRoute, Mount
 from starlette.routing import BaseRoute, Route, WebSocketRoute
 from pydantic import BaseModel
 
 CallableT = TypeVar('CallableT', bound=Callable[..., Any])
+FastAPIT = TypeVar('FastAPIT', bound=FastAPI)
 
 
 class VersionModel(BaseModel):
     version: str
 
 
 class VersionsModel(BaseModel):
@@ -30,14 +31,30 @@
     def decorator(func: CallableT) -> CallableT:
         func._api_version = (major, minor)  # type: ignore
         return func
 
     return decorator
 
 
+def api_version_remove(
+    major: int,
+    minor: int = 0
+) -> Callable[[CallableT], CallableT]:
+    """
+    Annotates a route as being removed from the given version onward (until a
+    new version of the route is assigned again)
+    """
+
+    def decorator(func: CallableT) -> CallableT:
+        func._api_version_remove = (major, minor)  # type: ignore
+        return func
+
+    return decorator
+
+
 def versionize(
     app: FastAPI,
     version_format: str = '{major}.{minor}',
     prefix_format: str = '/v{major}_{minor}',
     default_version: Tuple[int, int] = (1, 0),
     enable_latest: bool = False,
     latest_prefix: str = '/latest',
@@ -88,28 +105,33 @@
     :return list of versions (in tuple form)
     """
 
     if latest_prefix == '/':
         raise ValueError('latest_prefix cannot be "/"')
 
     version_route_mapping = _get_version_route_mapping(app=app, default_version=default_version)
+    version_remove_route_mapping = _get_version_remove_route_mapping(app=app)
 
     unique_routes: Dict[str, BaseRoute] = {}
-    versions = sorted(version_route_mapping.keys())
+    versions = sorted(set(version_route_mapping.keys()) | set(version_remove_route_mapping.keys()))
     for version in versions:
         major, minor = version
         prefix = prefix_format.format(major=major, minor=minor)
         semver = version_format.format(major=major, minor=minor)
 
         for route in version_route_mapping[version]:
-            if isinstance(route, APIRoute):
-                for method in route.methods:
-                    unique_routes[route.path + '|' + method] = route
-            elif isinstance(route, WebSocketRoute):
-                unique_routes[route.path] = route
+            for unique_key in _get_unique_route_keys(route):
+                unique_routes[unique_key] = route
+
+        for route in version_remove_route_mapping[version]:
+            for unique_key in _get_unique_route_keys(route):
+                if unique_key in unique_routes:
+                    del unique_routes[unique_key]
+                else:
+                    raise ValueError(f'Route {unique_key!r} can\'t be removed in version {version}')
 
         versioned_app = _build_versioned_app(
             app=app,
             version=version,
             semver=semver,
             unique_routes=dict(sorted(unique_routes.items())) if sorted_routes else unique_routes,
             get_openapi=get_openapi,
@@ -147,14 +169,24 @@
                 version=version_format.format(major=major, minor=minor)
             ) for (major, minor) in versions
         ])
 
     return versions
 
 
+def _get_unique_route_keys(route: BaseRoute) -> List[str]:
+    result = []
+    if isinstance(route, APIRoute):
+        for method in route.methods:
+            result.append(route.path + '|' + method)
+    elif isinstance(route, WebSocketRoute):
+        result.append(route.path)
+    return result
+
+
 def _get_version_route_mapping(
     app: FastAPI,
     default_version: Tuple[int, int]
 ) -> Dict[Tuple[int, int], List[BaseRoute]]:
     version_route_mapping: Dict[Tuple[int, int], List[BaseRoute]] = defaultdict(list)
     version_routes = [
         _version_to_route(route=route, default_version=default_version) for route in app.routes
@@ -171,27 +203,48 @@
     default_version: Tuple[int, int],
 ) -> Tuple[Tuple[int, int], BaseRoute]:
     api_route = cast(Route, route)
     version = getattr(api_route.endpoint, '_api_version', default_version)
     return version, api_route
 
 
-def _build_versioned_app(
+def _get_version_remove_route_mapping(
     app: FastAPI,
+) -> Dict[Tuple[int, int], List[BaseRoute]]:
+    version_remove_route_mapping: Dict[Tuple[int, int], List[BaseRoute]] = defaultdict(list)
+    version_remove_routes = [_version_remove_to_route(route=route) for route in app.routes]
+
+    for version, route in version_remove_routes:
+        if version is not None:
+            version_remove_route_mapping[version].append(route)
+
+    return version_remove_route_mapping
+
+
+def _version_remove_to_route(
+    route: BaseRoute,
+) -> Tuple[Union[Tuple[int, int], None], BaseRoute]:
+    api_route = cast(Route, route)
+    version = getattr(api_route.endpoint, '_api_version_remove', None)
+    return version, api_route
+
+
+def _build_versioned_app(
+    app: FastAPIT,
     version: Tuple[int, int],
     semver: str,
     unique_routes: Dict[str, BaseRoute],
     get_openapi: Union[Callable[[FastAPI, Tuple[int, int]], Dict[str, Any]], None] = None,
     get_docs: Union[Callable[[Tuple[int, int]], HTMLResponse], None] = None,
     get_redoc: Union[Callable[[Tuple[int, int]], HTMLResponse], None] = None,
     **kwargs: Any
-) -> FastAPI:
+) -> FastAPIT:
     docs_url = kwargs.pop('docs_url', None)
     redoc_url = kwargs.pop('redoc_url', None)
-    versioned_app = FastAPI(
+    versioned_app = app.__class__(
         title=app.title,
         description=app.description,
         version=semver,
         docs_url=docs_url if not get_docs else None,
         redoc_url=redoc_url if not get_redoc else None,
         **kwargs
     )
```

