# Comparing `tmp/mdast_cli-2023.4.3.tar.gz` & `tmp/mdast_cli-2023.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli-2023.4.3.tar", last modified: Tue Apr 11 07:30:15 2023, max compression
+gzip compressed data, was "mdast_cli-2023.4.4.tar", last modified: Thu Apr 13 17:47:49 2023, max compression
```

## Comparing `mdast_cli-2023.4.3.tar` & `mdast_cli-2023.4.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.486710 mdast_cli-2023.4.3/mdast_cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3589 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/app_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appgallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
--rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
--rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/store.py
--rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/firebase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/google_play.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/config.py
--rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/device.properties
--rw-r--r--   0 runner    (1001) docker     (122)    15468 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay.py
--rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/distribution_systems/rustore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/mdast_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/helpers/const.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli/mdast_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.490711 mdast_cli-2023.4.3/mdast_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-11 07:30:15.000000 mdast_cli-2023.4.3/mdast_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/mdast_cli_core/token.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 07:30:15.494711 mdast_cli-2023.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-11 07:29:47.000000 mdast_cli-2023.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.081592 mdast_cli-2023.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-13 17:47:49.081592 mdast_cli-2023.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.073592 mdast_cli-2023.4.4/mdast_cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.077592 mdast_cli-2023.4.4/mdast_cli/distribution_systems/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/app_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appgallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.077592 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.077592 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/google_play.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.081592 mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/device.properties
+-rw-r--r--   0 runner    (1001) docker     (122)    15468 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/googleplay.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/nexus2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/distribution_systems/rustore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.081592 mdast_cli-2023.4.4/mdast_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/helpers/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli/mdast_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.073592 mdast_cli-2023.4.4/mdast_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-13 17:47:49.000000 mdast_cli-2023.4.4/mdast_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-13 17:47:49.000000 mdast_cli-2023.4.4/mdast_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 17:47:49.000000 mdast_cli-2023.4.4/mdast_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-13 17:47:49.000000 mdast_cli-2023.4.4/mdast_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-13 17:47:49.000000 mdast_cli-2023.4.4/mdast_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 17:47:49.000000 mdast_cli-2023.4.4/mdast_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:49.081592 mdast_cli-2023.4.4/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/mdast_cli_core/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 17:47:49.081592 mdast_cli-2023.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-13 17:47:24.000000 mdast_cli-2023.4.4/setup.py
```

### Comparing `mdast_cli-2023.4.3/PKG-INFO` & `mdast_cli-2023.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast_cli
-Version: 2023.4.3
+Version: 2023.4.4
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.4.3/README.md` & `mdast_cli-2023.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/app_center.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/app_center.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,16 @@
         download_url = version_info.get('download_url')
 
         response = requests.get(download_url, headers=self.auth_header, allow_redirects=True)
         if response.status_code != 200:
             raise RuntimeError(f'AppCenter - Failed to download application. '
                                f'Request return status code: {response.status_code}')
 
-        file_name = '{0}-{1}.apk'.format(app_identifier, version_info['version'])
+        file_name = f'{version_info["bundle_identifier"]}-{version_info["short_version"]}' \
+                    f'.{version_info["fileExtension"]}'
         path_to_save = os.path.join(download_path, file_name)
 
         if not os.path.exists(download_path):
             os.mkdir(download_path)
 
         with open(path_to_save, 'wb') as file:
             file.write(response.content)
```

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appgallery.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appgallery.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/appstore_client/store.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/appstore_client/store.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/firebase.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/firebase.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,77 +5,63 @@
 import google.auth.transport.requests
 import requests
 from google.oauth2 import service_account
 
 logger = logging.getLogger(__name__)
 
 
-def get_app_info(project_number, app_id, account_json_path):
-    try:
-        credentials = service_account.Credentials.from_service_account_file(account_json_path, scopes=[
+def get_token(account_info):
+    if isinstance(account_info, dict):
+        credentials = service_account.Credentials.from_service_account_info(account_info, scopes=[
+            'https://www.googleapis.com/auth/cloud-platform'])
+    else:
+        credentials = service_account.Credentials.from_service_account_file(account_info, scopes=[
             'https://www.googleapis.com/auth/cloud-platform'])
-        credentials.refresh(google.auth.transport.requests.Request())
-        google_id_token = credentials.token
-        headers = {'Authorization': f'Bearer {google_id_token}'}
+
+    credentials.refresh(google.auth.transport.requests.Request())
+    google_id_token = credentials.token
+    if 'ya29' in google_id_token:
+        return google_id_token
+
+    raise RuntimeError(f'Incorrect token {google_id_token}')
+
+
+def get_app_info(project_number, app_id, account_info):
+    try:
+        token = get_token(account_info)
+        headers = {'Authorization': f'Bearer {token}'}
         last_release_info_resp = requests.get(
             f'https://firebaseappdistribution.googleapis.com/v1/projects/{project_number}/apps/'
             f'{app_id}/releases?pageSize=1',
             headers=headers)
         release = last_release_info_resp.json()['releases'][0]
-    except Exception:
-        raise RuntimeError('Firebase - Failed to get application info.')
+    except Exception as e:
+        raise RuntimeError(f'Firebase - Failed to get application info: {e}')
+
+    logger.info(f"Firebase - found release {release['name']} with version - {release['displayVersion']}")
     return {
         'integration_type': 'firebase',
         'app_name': release['name'],
-        'version': release['buildVersion'],
+        'version_code': release['buildVersion'],
+        'version_name': release['displayVersion'],
         'create_time': release['createTime'],
         'download_link': release['binaryDownloadUri']
     }
 
 
-def check_firebase_login(account_json_path):
-    credentials = service_account.Credentials.from_service_account_file(account_json_path, scopes=[
-        'https://www.googleapis.com/auth/cloud-platform'])
-    credentials.refresh(google.auth.transport.requests.Request())
-    google_id_token = credentials.token
-    if 'ya29' in google_id_token:
-        return True
-    else:
-        return False
-
-
-def firebase_download_app(download_path, project_number, app_id, account_json_path, file_name=None,
+def firebase_download_app(download_path, project_number, app_id, account_info, file_name=None,
                           file_extension='apk'):
     logger.info(f'Firebase - Try to download {file_extension} from latest release in project - '
                 f'{project_number} with app id {app_id}')
-    try:
-        credentials = service_account.Credentials.from_service_account_file(account_json_path, scopes=[
-            'https://www.googleapis.com/auth/cloud-platform'])
-    except Exception:
-        raise RuntimeError('Firebase - service account json file does not exist')
-    try:
-        credentials.refresh(google.auth.transport.requests.Request())
-        google_id_token = credentials.token
-    except Exception:
-        raise RuntimeError('Firebase - incorrect data or no permissions for your account')
-    headers = {'Authorization': f'Bearer {google_id_token}'}
-    last_release_info_resp = requests.get(
-        f'https://firebaseappdistribution.googleapis.com/v1/projects/{project_number}/apps/'
-        f'{app_id}/releases?pageSize=1',
-        headers=headers)
-    if last_release_info_resp.status_code != 200:
-        raise RuntimeError('Firebase - no release found or incorrect project_number/app_id')
-    release = last_release_info_resp.json()['releases'][0]
-    app_download_link = release['binaryDownloadUri']
-    logger.info(f"Firebase - found release {release['name']} with version - {release['displayVersion']}")
-
+    app_info = get_app_info(project_number, app_id, account_info)
+    app_download_link = app_info['download_link']
     app_file = requests.get(app_download_link, allow_redirects=True)
 
     if file_name is None:
-        file_name = release['displayVersion']
+        file_name = app_info['version_name']
 
     path_to_file = f'{download_path}/{file_name}.{file_extension}'
 
     if not os.path.exists(download_path):
         os.mkdir(download_path)
         logger.info(f'Firebase - Creating directory {download_path} for downloading app from Firebase')
```

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/google_play.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/google_play.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/config.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/config.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/device.properties` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/device.properties`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/googleplay.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/nexus.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/nexus2.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/nexus2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/distribution_systems/rustore.py` & `mdast_cli-2023.4.4/mdast_cli/distribution_systems/rustore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/helpers/const.py` & `mdast_cli-2023.4.4/mdast_cli/helpers/const.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli/mdast_scan.py` & `mdast_cli-2023.4.4/mdast_cli/mdast_scan.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli.egg-info/PKG-INFO` & `mdast_cli-2023.4.4/mdast_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast-cli
-Version: 2023.4.3
+Version: 2023.4.4
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.4.3/mdast_cli.egg-info/SOURCES.txt` & `mdast_cli-2023.4.4/mdast_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli.egg-info/requires.txt` & `mdast_cli-2023.4.4/mdast_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli_core/api.py` & `mdast_cli-2023.4.4/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli_core/base.py` & `mdast_cli-2023.4.4/mdast_cli_core/base.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/mdast_cli_core/token.py` & `mdast_cli-2023.4.4/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.4.3/setup.py` & `mdast_cli-2023.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli",
 
 
-    version='2023.04.03',
+    version='2023.04.04',
 
 
 
     author="Dynamic-Mobile-Security",
     description="Dynamic-Mobile-Security",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

