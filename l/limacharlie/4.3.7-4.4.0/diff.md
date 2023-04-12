# Comparing `tmp/limacharlie-4.3.7.tar.gz` & `tmp/limacharlie-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limacharlie-4.3.7.tar", last modified: Thu Mar  9 00:18:22 2023, max compression
+gzip compressed data, was "limacharlie-4.4.0.tar", last modified: Wed Apr 12 22:28:57 2023, max compression
```

## Comparing `limacharlie-4.3.7.tar` & `limacharlie-4.4.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-03-09 00:18:22.522486 limacharlie-4.3.7/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.3.7/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-03-09 00:18:22.522486 limacharlie-4.3.7/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10708 2021-10-28 22:41:03.000000 limacharlie-4.3.7/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-03-09 00:18:22.518486 limacharlie-4.3.7/limacharlie/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     9789 2021-05-01 20:23:26.000000 limacharlie-4.3.7/limacharlie/Comms.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    47560 2022-12-11 17:16:58.000000 limacharlie-4.3.7/limacharlie/Configs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.3.7/limacharlie/DRCli.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.3.7/limacharlie/Firehose.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10126 2023-01-15 18:36:46.000000 limacharlie-4.3.7/limacharlie/Hive.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.3.7/limacharlie/Jobs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.3.7/limacharlie/Logs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    51790 2023-03-09 00:11:28.000000 limacharlie-4.3.7/limacharlie/Manager.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    13328 2021-03-23 21:34:15.000000 limacharlie-4.3.7/limacharlie/Net.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.3.7/limacharlie/Payloads.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15596 2022-12-11 19:19:59.000000 limacharlie-4.3.7/limacharlie/Query.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    18358 2022-12-11 17:16:58.000000 limacharlie-4.3.7/limacharlie/Replay.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.3.7/limacharlie/Replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-02-23 20:28:52.000000 limacharlie-4.3.7/limacharlie/Search.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-02-23 20:28:52.000000 limacharlie-4.3.7/limacharlie/Sensor.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.3.7/limacharlie/SpotCheck.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.3.7/limacharlie/Spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.3.7/limacharlie/Sync.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.3.7/limacharlie/Webhook.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2317 2023-03-09 00:17:46.000000 limacharlie-4.3.7/limacharlie/__init__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    13582 2023-02-23 20:28:52.000000 limacharlie-4.3.7/limacharlie/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-11 17:16:58.000000 limacharlie-4.3.7/limacharlie/utils.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-03-09 00:18:22.519486 limacharlie-4.3.7/limacharlie.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-03-09 00:18:22.000000 limacharlie-4.3.7/limacharlie.egg-info/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)      893 2023-03-09 00:18:22.000000 limacharlie-4.3.7/limacharlie.egg-info/SOURCES.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-03-09 00:18:22.000000 limacharlie-4.3.7/limacharlie.egg-info/dependency_links.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-03-09 00:18:22.000000 limacharlie-4.3.7/limacharlie.egg-info/entry_points.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-03-09 00:18:22.000000 limacharlie-4.3.7/limacharlie.egg-info/requires.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-03-09 00:18:22.000000 limacharlie-4.3.7/limacharlie.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.3.7/limacharlie.egg-info/zip-safe
--rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-03-09 00:18:22.523486 limacharlie-4.3.7/setup.cfg
--rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-03-09 00:17:46.000000 limacharlie-4.3.7/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-03-09 00:18:22.522486 limacharlie-4.3.7/tests/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.3.7/tests/test_artifacts.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-11 19:19:59.000000 limacharlie-4.3.7/tests/test_core.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.3.7/tests/test_insight.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.3.7/tests/test_replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.3.7/tests/test_spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.3.7/tests/test_sync.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.647088 limacharlie-4.4.0/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.0/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 22:28:57.647088 limacharlie-4.4.0/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10708 2021-10-28 22:41:03.000000 limacharlie-4.4.0/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.644088 limacharlie-4.4.0/limacharlie/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Configs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/DRCli.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     4570 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Extensions.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.0/limacharlie/Firehose.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10126 2023-02-09 00:21:23.000000 limacharlie-4.4.0/limacharlie/Hive.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/Jobs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.0/limacharlie/Logs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    52397 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Manager.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/Payloads.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    15626 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Query.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    18358 2022-12-01 23:01:05.000000 limacharlie-4.4.0/limacharlie/Replay.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.0/limacharlie/Replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.0/limacharlie/Search.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.0/limacharlie/Sensor.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.0/limacharlie/SpotCheck.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.0/limacharlie/Spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.0/limacharlie/Sync.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/Webhook.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/__init__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    13476 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.0/limacharlie/utils.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.646088 limacharlie-4.4.0/limacharlie.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.0/limacharlie.egg-info/zip-safe
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-12 22:28:57.647088 limacharlie-4.4.0/setup.cfg
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-12 22:28:28.000000 limacharlie-4.4.0/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.647088 limacharlie-4.4.0/tests/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_artifacts.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.0/tests/test_core.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_insight.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.0/tests/test_sync.py
```

### Comparing `limacharlie-4.3.7/LICENSE` & `limacharlie-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/README.md` & `limacharlie-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Configs.py` & `limacharlie-4.4.0/limacharlie/Configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,33 @@
 
 class LcConfigException( Exception ):
     pass
 
 class Configs( object ):
     '''Configs object to fetch and apply configs to and from organizations.'''
 
-    def __init__( self, oid = None, env = None, manager = None, isDontUseInfraService = False ):
+    def __init__( self, oid = None, env = None, manager = None, isDontUseInfraService = False, isUseExtension = False ):
         '''Create a Configs object.
 
         Args:
             oid (str): organization ID to operate on.
             env (str): environment name to use.
             manager (limacharlie.Manager): Manager object to use instead.
             isDontUseInfraService (bool): if True, do not use the LimaCharlie infrastructure-service to apply configs.
+            isUseExtension (bool): if True, use the infrastructure extension in the cloud instead of the service.
         '''
 
         self._confVersion = 3
         if manager is None:
             self._man = Manager( oid = oid, environment = env )
         else:
             self._man = manager
 
         self._isDontUseInfraService = isDontUseInfraService
+        self._isUseExtension = isUseExtension
 
         self._configRoots = {
             'rules',
             'outputs',
             'resources',
             'integrity',
             'fps',
@@ -140,31 +142,49 @@
         else:
             asConf = toConfigFile
 
         # If we can use the service, shortcut all this logic
         # and use the authoritative service in the cloud.
         if not self._isDontUseInfraService:
             try:
-                data = self._man.serviceRequest( 'infrastructure-service', {
-                    'action' : 'fetch',
-                    'sync_dr' : isRules,
-                    'sync_outputs' : isOutputs,
-                    'sync_resources' : isResources,
-                    'sync_integrity' : isIntegrity,
-                    'sync_fp' : isFPs,
-                    'sync_exfil' : isExfil,
-                    'sync_artifacts' : isArtifact,
-                    'sync_org_values' : isOrgConfigs,
-                    'sync_hives' : isHives, # must be map of hive names you want to fetch {"cloud_sensor":true, "fp":true, "dr-service":true, "dr-general": true}
-                    'sync_installation_keys' : isInstallationKeys,
-                    'sync_yara' : isYara,
-                }, isImpersonate = True )
+                if self._isUseExtension:
+                    data = self._man.extensionRequest( 'ext-infrastructure', 'fetch', {
+                        'options' : {
+                            'sync_dr' : isRules,
+                            'sync_outputs' : isOutputs,
+                            'sync_resources' : isResources,
+                            'sync_integrity' : isIntegrity,
+                            'sync_fp' : isFPs,
+                            'sync_exfil' : isExfil,
+                            'sync_artifacts' : isArtifact,
+                            'sync_org_values' : isOrgConfigs,
+                            'sync_hives' : isHives, # must be map of hive names you want to fetch {"cloud_sensor":true, "fp":true, "dr-service":true, "dr-general": true}
+                            'sync_installation_keys' : isInstallationKeys,
+                            'sync_yara' : isYara,
+                        },
+                    }, isImpersonate = True )
+                    asConf = data[ 'data' ][ 'org' ]
+                else:
+                    data = self._man.serviceRequest( 'infrastructure-service', {
+                        'action' : 'fetch',
+                        'sync_dr' : isRules,
+                        'sync_outputs' : isOutputs,
+                        'sync_resources' : isResources,
+                        'sync_integrity' : isIntegrity,
+                        'sync_fp' : isFPs,
+                        'sync_exfil' : isExfil,
+                        'sync_artifacts' : isArtifact,
+                        'sync_org_values' : isOrgConfigs,
+                        'sync_hives' : isHives, # must be map of hive names you want to fetch {"cloud_sensor":true, "fp":true, "dr-service":true, "dr-general": true}
+                        'sync_installation_keys' : isInstallationKeys,
+                        'sync_yara' : isYara,
+                    }, isImpersonate = True )
 
-                for k, v in yaml.safe_load( data[ 'org' ] ).items():
-                    asConf[ k ] = v
+                    for k, v in yaml.safe_load( data[ 'org' ] ).items():
+                        asConf[ k ] = v
 
                 # Apply a few of the translation layers.
                 exfilRules = asConf.get( 'exfil', None )
                 if exfilRules is not None:
                     for ruleName, rule in exfilRules.get( 'watch', {} ).items():
                         if '' == rule[ 'operator' ]:
                             # This is a [secret] rule, let's not mirror it since
@@ -318,32 +338,55 @@
                             continue
                         exfilRules[ 'watch' ][ ruleName ] = self._wrapExfilContent( rule )
                     for ruleName, rule in exfilRules.get( 'list', {} ).items():
                         exfilRules[ 'list' ][ ruleName ] = self._wrapExfilContent( rule )
                     asConf[ 'exfil' ] = exfilRules
 
                 finalConfig = yaml.safe_dump( asConf, version = (1,1) )
-                data = self._man.serviceRequest( 'infrastructure-service', {
-                    'is_dry_run' : isDryRun,
-                    'action' : 'push',
-                    'is_force' : isForce,
-                    'ignore_inaccessible' : isIgnoreInaccessible,
-                    'config' : finalConfig,
-                    'sync_dr' : isRules,
-                    'sync_outputs' : isOutputs,
-                    'sync_resources' : isResources,
-                    'sync_integrity' : isIntegrity,
-                    'sync_fp' : isFPs,
-                    'sync_exfil' : isExfil,
-                    'sync_artifacts' : isArtifact,
-                    'sync_org_values' : isOrgConfigs,
-                    'sync_hives' : isHives,
-                    'sync_installation_keys' : isInstallationKeys,
-                    'sync_yara' : isYara,
-                }, isImpersonate = True )
+
+                if self._isUseExtension:
+                    data = self._man.extensionRequest( 'ext-infrastructure', 'push', {
+                        'config' : finalConfig,
+                        'options' : {
+                            'is_dry_run' : isDryRun,
+                            'is_force' : isForce,
+                            'ignore_inaccessible' : isIgnoreInaccessible,
+                            'sync_dr' : isRules,
+                            'sync_outputs' : isOutputs,
+                            'sync_resources' : isResources,
+                            'sync_integrity' : isIntegrity,
+                            'sync_fp' : isFPs,
+                            'sync_exfil' : isExfil,
+                            'sync_artifacts' : isArtifact,
+                            'sync_org_values' : isOrgConfigs,
+                            'sync_hives' : isHives,
+                            'sync_installation_keys' : isInstallationKeys,
+                            'sync_yara' : isYara,
+                        },
+                    }, isImpersonate = True )
+                    data = data[ 'data' ]
+                else:
+                    data = self._man.serviceRequest( 'infrastructure-service', {
+                        'is_dry_run' : isDryRun,
+                        'action' : 'push',
+                        'is_force' : isForce,
+                        'ignore_inaccessible' : isIgnoreInaccessible,
+                        'config' : finalConfig,
+                        'sync_dr' : isRules,
+                        'sync_outputs' : isOutputs,
+                        'sync_resources' : isResources,
+                        'sync_integrity' : isIntegrity,
+                        'sync_fp' : isFPs,
+                        'sync_exfil' : isExfil,
+                        'sync_artifacts' : isArtifact,
+                        'sync_org_values' : isOrgConfigs,
+                        'sync_hives' : isHives,
+                        'sync_installation_keys' : isInstallationKeys,
+                        'sync_yara' : isYara,
+                    }, isImpersonate = True )
 
                 for op in data.get( 'ops', [] ):
                     if op[ 'is_added' ]:
                         yield ( '+', op[ 'type' ], op[ 'name' ] )
                     if op[ 'is_removed' ]:
                         yield ( '-', op[ 'type' ], op[ 'name' ] )
                     if not op[ 'is_added' ] and not op[ 'is_removed' ]:
@@ -887,14 +930,20 @@
                          help = 'if specified, emit verbose information about the push' )
     parser.add_argument( '--use-local-logic',
                          required = False,
                          default = False,
                          action = 'store_true',
                          dest = 'isDontUseInfraService',
                          help = 'if specified, use the local SDK syncing logic instead of cloud service' )
+    parser.add_argument( '--use-infra-extension',
+                         required = False,
+                         default = False,
+                         action = 'store_true',
+                         dest = 'isUseExtension',
+                         help = 'if specified, use the infrastructure extension instead of the service' )
     args = parser.parse_args( sourceArgs )
 
     if args.isDryRun:
         print( '!!! DRY RUN !!!' )
 
     if args.action not in ( 'fetch', 'push' ):
         print( "Action %s is not supported." % args.action )
@@ -949,15 +998,15 @@
     if args.isHiveDRService:
         hives['dr-service'] = True
     if args.isHiveCloudSensor:
         hives['cloud_sensor'] = True
     if args.isHiveFP:
         hives['fp'] = True
 
-    s = Configs( oid = args.oid, env = args.environment, isDontUseInfraService = args.isDontUseInfraService )
+    s = Configs( oid = args.oid, env = args.environment, isDontUseInfraService = args.isDontUseInfraService, isUseExtension = args.isUseExtension )
 
     if 'fetch' == args.action:
         s.fetch( args.config, isRules = args.isRules, isFPs = args.isFPs, isOutputs = args.isOutputs, isIntegrity = args.isIntegrity, isArtifact = args.isArtifact, isExfil = args.isExfil, isResources = args.isResources, isOrgConfigs = args.isOrgConfigs, isInstallationKeys = args.isInstallationKeys, isHives = hives, isYara = args.isYara )
     elif 'push' == args.action:
         for modification, category, element in s.push( args.config, isForce = args.isForce, isIgnoreInaccessible = args.isIgnoreInaccessible, isDryRun = args.isDryRun, isRules = args.isRules, isFPs = args.isFPs, isOutputs = args.isOutputs, isIntegrity = args.isIntegrity, isArtifact = args.isArtifact, isExfil = args.isExfil, isResources = args.isResources, isOrgConfigs = args.isOrgConfigs, isInstallationKeys = args.isInstallationKeys, isHives = hives, isYara = args.isYara, isVerbose = args.isVerbose ):
             print( '%s %s %s' % ( modification, category, element ) )
```

### Comparing `limacharlie-4.3.7/limacharlie/DRCli.py` & `limacharlie-4.4.0/limacharlie/DRCli.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Firehose.py` & `limacharlie-4.4.0/limacharlie/Firehose.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Hive.py` & `limacharlie-4.4.0/limacharlie/Hive.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Jobs.py` & `limacharlie-4.4.0/limacharlie/Jobs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Logs.py` & `limacharlie-4.4.0/limacharlie/Logs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Manager.py` & `limacharlie-4.4.0/limacharlie/Manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -842,14 +842,27 @@
         data = self._apiCall( 'service/%s/%s' % ( self._oid, serviceName ), POST, req )
         return data
 
     def replicantRequest( self, *args, **kwargs ):
         # Maintained for backwards compatibility post rename replicant => service.
         return self.serviceRequest( *args, **kwargs )
 
+    def extensionRequest( self, extensionName, action, data, isImpersonate = False ):
+        '''Issue a request to an Extension.
+
+        Args:
+            extensionName (str): the name of the Extension to task.
+            data (dict): JSON data to send to the Extension as a request.
+            isImpersonate (bool): if set to True, request the Service impersonate the caller.
+        Returns:
+            Dict with general success.
+        '''
+        from limacharlie.Extensions import Extension
+        return Extension( self ).request( extensionName, action, data, isImpersonated = isImpersonate )
+
     def getAvailableServices( self ):
         '''Get the list of Services currently available.
 
         Returns:
             List of Service names.
         '''
         data = self._apiCall( 'service/%s' % ( self._oid, ), GET )
```

### Comparing `limacharlie-4.3.7/limacharlie/Payloads.py` & `limacharlie-4.4.0/limacharlie/Payloads.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Query.py` & `limacharlie-4.4.0/limacharlie/Query.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                                 limitEvent = args.limitEvent,
                                 limitEval = args.limitEval,
                                 isDryRun = args.isDryRun,
                                 isCursorBased = False )
 
     error = response.get( 'error', None )
     if error:
-        print( f"ERROR: {error}" )
+        print( "ERROR: %s" % ( error, ) )
         return
     for result in response[ 'results' ]:
         if args.isPretty:
             print( json.dumps( result[ 'data' ], indent = 2 ) )
         else:
             print( json.dumps( result[ 'data' ] ) )
 
@@ -101,15 +101,15 @@
         self.intro = 'This LimaCharlie feature is in Beta, LCQL is likely going to evolve!\nThe LimaCharlie Query allows you to query the dataset in a more free-form fashion based on the LC Query Language.'
         self._timeFrame = "-10m"
         self._sensors = "*"
         self._events = "*"
         self._limitEvent = 0
         self._limitEval = 0
         self._billed = 0
-        self._pricingBlock = 25000
+        self._pricingBlock = 200000
         self._histfile = os.path.expanduser( '~/.limacharlie_history' )
         self._histfile_size = 1000
         self._outFile = outFile
         self._replay = replay
         self._format = format
         self._lastData = None
         self._lastQuery = None
@@ -144,16 +144,16 @@
             return
         with open( self._outFile, 'a' ) as f:
             f.write( output )
             f.write( "\n" )
 
     def do_q( self, inp, isCursorBased = True ):
         '''Query (paged).'''
-        thisQuery = f"{self._timeFrame} | {self._sensors} | {self._events} | {inp}"
-        cacheKey = f"{self._limitEval}{self._limitEvent}{thisQuery}"
+        thisQuery = "%s | %s | %s | %s" % ( self._timeFrame, self._sensors, self._events, inp )
+        cacheKey = "%s%s%s" % ( self._limitEval, self._limitEvent, thisQuery )
 
         q = None
         isFromCache = False
 
         # Check if the is the same last query we did, if so, re-use the result.
         if cacheKey == self._lastQuery:
             self._logOutput( f"{len( self._lastData )} results from cache" )
```

### Comparing `limacharlie-4.3.7/limacharlie/Replay.py` & `limacharlie-4.4.0/limacharlie/Replay.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Replicants.py` & `limacharlie-4.4.0/limacharlie/Replicants.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Search.py` & `limacharlie-4.4.0/limacharlie/Search.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Sensor.py` & `limacharlie-4.4.0/limacharlie/Sensor.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/SpotCheck.py` & `limacharlie-4.4.0/limacharlie/SpotCheck.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Spout.py` & `limacharlie-4.4.0/limacharlie/Spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Sync.py` & `limacharlie-4.4.0/limacharlie/Sync.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/Webhook.py` & `limacharlie-4.4.0/limacharlie/Webhook.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie/__init__.py` & `limacharlie-4.4.0/limacharlie/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """limacharlie API for limacharlie.io"""
 
-__version__ = "4.3.7"
+__version__ = "4.4.0"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 # Global API Credentials
 import os
@@ -56,13 +56,12 @@
 from .Webhook import Webhook
 from .Sync import Sync
 from .Configs import Configs
 from .SpotCheck import SpotCheck
 from .Payloads import Payloads
 from .Logs import Logs
 from .Logs import Logs as Artifacts
-from .Comms import Comms
-from .Net import Net
 from .Hive import Hive
 from .Hive import HiveRecord
+from .Extensions import Extension
 from .utils import LcApiException
 from . import Replicants as services
```

### Comparing `limacharlie-4.3.7/limacharlie/__main__.py` & `limacharlie-4.4.0/limacharlie/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,23 +200,20 @@
                              dest = 'outputName',
                              help = 'send data to a named output instead.' )
         args = parser.parse_args( sys.argv[ 2: ] )
         _man = Manager()
         _sensor = _man.sensor( str( args.sid ) )
         for event in _sensor.getHistoricEvents( args.start, args.end, limit = args.limit, eventType = args.eventType, outputName = args.outputName ):
             print( json.dumps( event ) )
-    elif args.action.lower() == 'comms':
-        from .Comms import main as cmdMain
-        cmdMain( sys.argv[ 2 : ] )
-    elif args.action.lower() == 'net':
-        from .Net import main as cmdMain
-        cmdMain( sys.argv[ 2 : ] )
     elif args.action.lower() == 'hive':
         from .Hive import main as cmdMain
         cmdMain( sys.argv[ 2 : ] )
+    elif args.action.lower() == 'extension':
+        from .Extensions import main as cmdMain
+        cmdMain( sys.argv[ 2 : ] )
     elif args.action.lower() == 'create_org':
         from . import Manager
         import json
         parser = argparse.ArgumentParser( prog = 'limacharlie create_org' )
         parser.add_argument( 'name',
                              type = str,
                              help = 'name of the organization to create.' )
```

### Comparing `limacharlie-4.3.7/limacharlie/utils.py` & `limacharlie-4.4.0/limacharlie/utils.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/limacharlie.egg-info/SOURCES.txt` & `limacharlie-4.4.0/limacharlie.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-limacharlie/Comms.py
 limacharlie/Configs.py
 limacharlie/DRCli.py
+limacharlie/Extensions.py
 limacharlie/Firehose.py
 limacharlie/Hive.py
 limacharlie/Jobs.py
 limacharlie/Logs.py
 limacharlie/Manager.py
-limacharlie/Net.py
 limacharlie/Payloads.py
 limacharlie/Query.py
 limacharlie/Replay.py
 limacharlie/Replicants.py
 limacharlie/Search.py
 limacharlie/Sensor.py
 limacharlie/SpotCheck.py
```

### Comparing `limacharlie-4.3.7/setup.py` & `limacharlie-4.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "4.3.7"
+__version__ = "4.4.0"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 setup( name = 'limacharlie',
        version = __version__,
```

### Comparing `limacharlie-4.3.7/tests/test_artifacts.py` & `limacharlie-4.4.0/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/tests/test_core.py` & `limacharlie-4.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/tests/test_insight.py` & `limacharlie-4.4.0/tests/test_insight.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/tests/test_spout.py` & `limacharlie-4.4.0/tests/test_spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.3.7/tests/test_sync.py` & `limacharlie-4.4.0/tests/test_sync.py`

 * *Files identical despite different names*

