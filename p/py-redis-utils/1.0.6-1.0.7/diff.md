# Comparing `tmp/py-redis-utils-1.0.6.tar.gz` & `tmp/py-redis-utils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-1.0.6.tar", last modified: Thu Apr 13 08:45:40 2023, max compression
+gzip compressed data, was "py-redis-utils-1.0.7.tar", last modified: Thu Apr 13 11:17:15 2023, max compression
```

## Comparing `py-redis-utils-1.0.6.tar` & `py-redis-utils-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 08:45:40.217774 py-redis-utils-1.0.6/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-04-13 08:45:40.217774 py-redis-utils-1.0.6/PKG-INFO
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.0.6/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 08:45:40.217774 py-redis-utils-1.0.6/py_redis_utils.egg-info/
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)      414 2023-04-13 08:45:40.000000 py-redis-utils-1.0.6/py_redis_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)      259 2023-04-13 08:45:40.000000 py-redis-utils-1.0.6/py_redis_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)        1 2023-04-13 08:45:40.000000 py-redis-utils-1.0.6/py_redis_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)       21 2023-04-13 08:45:40.000000 py-redis-utils-1.0.6/py_redis_utils.egg-info/requires.txt
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)       13 2023-04-13 08:45:40.000000 py-redis-utils-1.0.6/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 08:45:40.217774 py-redis-utils-1.0.6/pyredisutils/
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)       40 2023-04-11 16:05:30.000000 py-redis-utils-1.0.6/pyredisutils/__init__.py
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6128 2023-04-13 08:43:37.000000 py-redis-utils-1.0.6/pyredisutils/_auth_deco.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-04-13 08:45:40.217774 py-redis-utils-1.0.6/setup.cfg
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)      696 2023-04-13 08:45:05.000000 py-redis-utils-1.0.6/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/PKG-INFO
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     1361 2023-04-11 16:05:30.000000 py-redis-utils-1.0.7/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/py_redis_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      414 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      259 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       21 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       13 2023-04-13 11:17:15.000000 py-redis-utils-1.0.7/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/pyredisutils/
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)       40 2023-04-11 16:05:30.000000 py-redis-utils-1.0.7/pyredisutils/__init__.py
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6158 2023-04-13 11:13:28.000000 py-redis-utils-1.0.7/pyredisutils/_auth_deco.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-04-13 11:17:15.664458 py-redis-utils-1.0.7/setup.cfg
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)      696 2023-04-13 11:16:56.000000 py-redis-utils-1.0.7/setup.py
```

### Comparing `py-redis-utils-1.0.6/README.md` & `py-redis-utils-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.0.6/pyredisutils/_auth_deco.py` & `py-redis-utils-1.0.7/pyredisutils/_auth_deco.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def jwt_redis_auth(redis_instance: redis,
                    channel_name: str,
                    pub_message: dict,
                    response_template: dict):
     def funct_decorator(org_function):
         @wraps(org_function)
-        def authorize():
+        def authorize(*args, **kwargs):
             """
             Authorization method that runs before all request to check if upcoming request
             is authorized in the system.
             """
             publish_message = copy.deepcopy(pub_message)
             response_message = copy.deepcopy(response_template)
 
@@ -82,15 +82,15 @@
                     )
                     return _make_response("Gateway Timeout", 504)
                 pubsub.unsubscribe(channel_name + ".reply")
             except redis.exceptions.ConnectionError:
                 logging.error("Redis refused to connect.")
                 return _make_response("Bad Gateway", 502)
 
-            return org_function()
+            return org_function(*args, **kwargs)
 
         return authorize
 
     return funct_decorator
 
 
 def _transform_dict(data, new_token: str = "", new_id: str = "") -> dict:
```

### Comparing `py-redis-utils-1.0.6/setup.py` & `py-redis-utils-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
```

