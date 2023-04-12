# Comparing `tmp/limacharlie-4.4.0.tar.gz` & `tmp/limacharlie-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limacharlie-4.4.0.tar", last modified: Wed Apr 12 22:28:57 2023, max compression
+gzip compressed data, was "limacharlie-4.4.1.tar", last modified: Wed Apr 12 23:51:02 2023, max compression
```

## Comparing `limacharlie-4.4.0.tar` & `limacharlie-4.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.647088 limacharlie-4.4.0/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.0/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 22:28:57.647088 limacharlie-4.4.0/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10708 2021-10-28 22:41:03.000000 limacharlie-4.4.0/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.644088 limacharlie-4.4.0/limacharlie/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Configs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/DRCli.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     4570 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Extensions.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.0/limacharlie/Firehose.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10126 2023-02-09 00:21:23.000000 limacharlie-4.4.0/limacharlie/Hive.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/Jobs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.0/limacharlie/Logs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    52397 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Manager.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/Payloads.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15626 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/Query.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    18358 2022-12-01 23:01:05.000000 limacharlie-4.4.0/limacharlie/Replay.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.0/limacharlie/Replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.0/limacharlie/Search.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.0/limacharlie/Sensor.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.0/limacharlie/SpotCheck.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.0/limacharlie/Spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.0/limacharlie/Sync.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.0/limacharlie/Webhook.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/__init__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    13476 2023-04-12 22:28:28.000000 limacharlie-4.4.0/limacharlie/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.0/limacharlie/utils.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.646088 limacharlie-4.4.0/limacharlie.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/SOURCES.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/dependency_links.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/entry_points.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/requires.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-12 22:28:57.000000 limacharlie-4.4.0/limacharlie.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.0/limacharlie.egg-info/zip-safe
--rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-12 22:28:57.647088 limacharlie-4.4.0/setup.cfg
--rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-12 22:28:28.000000 limacharlie-4.4.0/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 22:28:57.647088 limacharlie-4.4.0/tests/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_artifacts.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.0/tests/test_core.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_insight.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.0/tests/test_spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.0/tests/test_sync.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.299804 limacharlie-4.4.1/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.1/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 23:51:02.299804 limacharlie-4.4.1/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10708 2021-10-28 22:41:03.000000 limacharlie-4.4.1/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.296804 limacharlie-4.4.1/limacharlie/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/Configs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/DRCli.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     4570 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/Extensions.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.1/limacharlie/Firehose.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10126 2023-02-09 00:21:23.000000 limacharlie-4.4.1/limacharlie/Hive.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/Jobs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.1/limacharlie/Logs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    52397 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/Manager.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/Payloads.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.1/limacharlie/Query.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.1/limacharlie/Replay.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.1/limacharlie/Replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.1/limacharlie/Search.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.1/limacharlie/Sensor.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.1/limacharlie/SpotCheck.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.1/limacharlie/Spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.1/limacharlie/Sync.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.1/limacharlie/Webhook.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-12 23:50:48.000000 limacharlie-4.4.1/limacharlie/__init__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    13476 2023-04-12 22:28:28.000000 limacharlie-4.4.1/limacharlie/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.1/limacharlie/utils.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.298804 limacharlie-4.4.1/limacharlie.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-12 23:51:02.000000 limacharlie-4.4.1/limacharlie.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.1/limacharlie.egg-info/zip-safe
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-12 23:51:02.299804 limacharlie-4.4.1/setup.cfg
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-12 23:50:48.000000 limacharlie-4.4.1/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-12 23:51:02.299804 limacharlie-4.4.1/tests/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_artifacts.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.1/tests/test_core.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_insight.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.1/tests/test_spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.1/tests/test_sync.py
```

### Comparing `limacharlie-4.4.0/LICENSE` & `limacharlie-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/README.md` & `limacharlie-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Configs.py` & `limacharlie-4.4.1/limacharlie/Configs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/DRCli.py` & `limacharlie-4.4.1/limacharlie/DRCli.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Extensions.py` & `limacharlie-4.4.1/limacharlie/Extensions.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Firehose.py` & `limacharlie-4.4.1/limacharlie/Firehose.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Hive.py` & `limacharlie-4.4.1/limacharlie/Hive.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Jobs.py` & `limacharlie-4.4.1/limacharlie/Jobs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Logs.py` & `limacharlie-4.4.1/limacharlie/Logs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Manager.py` & `limacharlie-4.4.1/limacharlie/Manager.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Payloads.py` & `limacharlie-4.4.1/limacharlie/Payloads.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Query.py` & `limacharlie-4.4.1/limacharlie/Query.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 class LCQuery( cmd.Cmd ):
     def __init__( self, replay, format, outFile ):
         self.intro = 'This LimaCharlie feature is in Beta, LCQL is likely going to evolve!\nThe LimaCharlie Query allows you to query the dataset in a more free-form fashion based on the LC Query Language.'
         self._timeFrame = "-10m"
         self._sensors = "*"
         self._events = "*"
+        self._stream = 'event'
         self._limitEvent = 0
         self._limitEval = 0
         self._billed = 0
         self._pricingBlock = 200000
         self._histfile = os.path.expanduser( '~/.limacharlie_history' )
         self._histfile_size = 1000
         self._outFile = outFile
@@ -159,29 +160,31 @@
             self._logOutput( f"{len( self._lastData )} results from cache" )
             toRender = self._lastData
             isFromCache = True
         else:
             sys.stdout.write( colored("Query running ", 'cyan') )
             if isCursorBased:
                 q = self._replay._doQuery( thisQuery,
-                                        limitEvent = self._limitEvent if self._limitEvent else None,
-                                        limitEval = self._limitEval if self._limitEval else None,
-                                        isCursorBased = isCursorBased )
+                                           limitEvent = self._limitEvent if self._limitEvent else None,
+                                           limitEval = self._limitEval if self._limitEval else None,
+                                           isCursorBased = isCursorBased,
+                                           stream = self._stream )
                 with Spinner():
                     response = q.next()
                     error = response.get( 'error', None )
                     if error:
                         self._logOutput( f"ERROR: {error}" )
                         return
             else:
                 with Spinner():
                     response = self._replay._doQuery( thisQuery,
                                                       limitEvent = self._limitEvent if self._limitEvent else None,
                                                       limitEval = self._limitEval if self._limitEval else None,
-                                                      isCursorBased = isCursorBased )
+                                                      isCursorBased = isCursorBased,
+                                                      stream = self._stream )
                     error = response.get( 'error', None )
                     if error:
                         self._logOutput( f"ERROR: {error}" )
                         return
 
             print( "" )
             thisBilled = response.get( 'stats', {} ).get( 'n_billed', 0 )
@@ -282,15 +285,16 @@
         '''Execute a command as a dry-run and get back aproximate cost of the query.'''
         sys.stdout.write( colored("Query running ", 'cyan') )
         with Spinner():
             response = self._replay._doQuery( f"{self._timeFrame} | {self._sensors} | {self._events} | {inp}",
                                             limitEvent = self._limitEvent if self._limitEvent else None,
                                             limitEval = self._limitEval if self._limitEval else None,
                                             isDryRun = True,
-                                            isCursorBased = False )
+                                            isCursorBased = False,
+                                            stream = self._stream )
         thisBilled = response.get( 'stats', {} ).get( 'n_billed', 0 )
         print( "Note that aproximate costs for queries with a time frame within the last 6h may be under-reported.")
         self._logOutput( f"Aproximate cost: ${(thisBilled / self._pricingBlock) / 100}" )
         self._logOutput( json.dumps( response, indent = 2 ) )
 
     def complete_dryrun( self, text, line, begidx, endidx ):
         return self.complete_q( text, line, begidx, endidx )
@@ -340,14 +344,18 @@
         '''Set the event types to query, like "NEW_PROCESS DNS_REQUEST'''
         self._events = inp
 
         self._populateSchema()
 
         self._setPrompt()
 
+    def do_set_stream( self, inp ):
+        '''Set the data stream to query, one of "event", "audit", "detect", defaults to "event"'''
+        self._stream = inp
+
     def complete_set_events( self, text, line, begidx, endidx ):
         return [ e for e in self._allEvents if e.startswith( text ) ]
 
     def _getAllEvents( self ):
         sys.stdout.write( colored("Fetching event list  ", 'cyan') )
         with Spinner():
             self._allEvents = [ e[4:] for e in self._replay._lc.getSchemas()[ 'event_types' ] if e.startswith( 'evt:' ) ]
```

### Comparing `limacharlie-4.4.0/limacharlie/Replay.py` & `limacharlie-4.4.1/limacharlie/Replay.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,50 +43,52 @@
             maxConcurrent (int): number of sensors windows to process in parallel.
             isInteractive (bool): if True, display progress updates to standard out.
         '''
 
         self._lc = manager
         self._replayURL = self._lc.getOrgURLs()[ 'replay' ]
 
-    def _doQuery( self, query, limitEvent = None, limitEval = None, isDryRun = False, isCursorBased = False ):
+    def _doQuery( self, query, limitEvent = None, limitEval = None, isDryRun = False, isCursorBased = False, stream = 'event' ):
         if not query:
             raise LcApiException( 'no query specified' )
 
         req = {
             'oid' : self._lc._oid,
             'query' : query,
             'limit_event' : 0 if limitEvent is None else limitEvent,
             'limit_eval' : 0 if limitEval is None else limitEval,
             'is_dry_run' : isDryRun,
             'event_source' : {
+                'stream' : stream,
                 'sensor_events' : {
                     'cursor' : '-' if isCursorBased else '',
                 },
             },
         }
 
         if not isCursorBased:
             return queryContext( self, req ).next()
 
         return queryContext( self, req )
 
-    def _scanHistoricalSensor( self, sid = None, startTime = None, endTime = None, events = None, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, isStateful = None, limitEvent = None, limitEval = None, isDryRun = False ):
+    def _scanHistoricalSensor( self, sid = None, startTime = None, endTime = None, events = None, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, isStateful = None, limitEvent = None, limitEval = None, isDryRun = False, stream = 'event' ):
         resp = None
 
         if ruleName is None and ruleContent is None:
             raise LcApiException( 'no rule specified' )
 
         req = {
             'oid' : self._lc._oid,
             'rule_source' : {
                 'rule_name' : '' if ruleName is None else ruleName,
                 'namespace' : '' if namespace is None else namespace,
                 'rule' : ruleContent,
             },
             'event_source' : {
+                'stream' : stream,
                 'sensor_events' : {
                     'sid' : '' if sid is None else sid,
                     'start_time' : 0 if startTime is None else startTime,
                     'end_time' : 0 if endTime is None else endTime,
                 },
                 'events' : events,
             },
@@ -104,76 +106,79 @@
                                   {},
                                   altRoot = 'https://%s/' % ( self._replayURL, ),
                                   rawBody = json.dumps( req ).encode(),
                                   contentType = 'application/json' )
 
         return resp
 
-    def scanHistoricalSensor( self, sid, startTime, endTime, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, limitEvent = None, limitEval = None, isStateful = None, isDryRun = False ):
+    def scanHistoricalSensor( self, sid, startTime, endTime, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, limitEvent = None, limitEval = None, isStateful = None, isDryRun = False, stream = 'event' ):
         '''Scan a specific sensor's data with a D&R rule.
 
         Args:
             sid (str): sensor ID to scan.
             startTime (int): seconds epoch to start scanning at.
             endTime (int): seconds epoch to stop scanning at.
             ruleName (str): the name of an existing D&R rule to use.
             namespace (str): the namespace the ruleName lives in.
             ruleContent (dict): D&R rule to use to scan, with a "detect" key and a "respond" key.
             isRunTrace (bool): if True, generate a trace of the evaluation.
             limitEvent (int): approximately limit the number of events evaluated.
             limitEval (int): approximately limit the number of rule evaluations.
             isIgnoreState (bool): if True, parallelize processing of single sensors to increase performance but limit effectiveness of stateful detection.
+            stream (str): data stream to replay.
 
         Returns:
             a dict containing results of the query.
         '''
 
-        resp = self._scanHistoricalSensor( sid = sid, startTime = startTime, endTime = endTime, ruleName = ruleName, namespace = namespace, ruleContent = ruleContent, isRunTrace = isRunTrace, limitEvent = limitEvent, limitEval = limitEval, isStateful = isStateful, isDryRun = isDryRun )
+        resp = self._scanHistoricalSensor( sid = sid, startTime = startTime, endTime = endTime, ruleName = ruleName, namespace = namespace, ruleContent = ruleContent, isRunTrace = isRunTrace, limitEvent = limitEvent, limitEval = limitEval, isStateful = isStateful, isDryRun = isDryRun, stream = stream )
         
         return resp
 
-    def scanEntireOrg( self, startTime, endTime, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, limitEvent = None, limitEval = None, isStateful = None, isDryRun = False ):
+    def scanEntireOrg( self, startTime, endTime, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, limitEvent = None, limitEval = None, isStateful = None, isDryRun = False, stream = 'event' ):
         '''Scan an entire organization's data with a D&R rule.
 
         Args:
             startTime (int): seconds epoch to start scanning at.
             endTime (int): seconds epoch to stop scanning at.
             ruleName (str): the name of an existing D&R rule to use.
             namespace (str): the namespace the ruleName lives in.
             ruleContent (dict): D&R rule to use to scan, with a "detect" key and a "respond" key.
             isRunTrace (bool): if True, generate a trace of the evaluation.
             limitEvent (int): approximately limit the number of events evaluated.
             limitEval (int): approximately limit the number of rule evaluations.
             isIgnoreState (bool): if True, parallelize processing of single sensors to increase performance but limit effectiveness of stateful detection.
+            stream (str): data stream to replay.
 
         Returns:
             a dict containing results of the query.
         '''
         
-        resp = self._scanHistoricalSensor( startTime = startTime, endTime = endTime, ruleName = ruleName, namespace = namespace, ruleContent = ruleContent, isRunTrace = isRunTrace, limitEvent = limitEvent, limitEval = limitEval, isStateful = isStateful, isDryRun = isDryRun )
+        resp = self._scanHistoricalSensor( startTime = startTime, endTime = endTime, ruleName = ruleName, namespace = namespace, ruleContent = ruleContent, isRunTrace = isRunTrace, limitEvent = limitEvent, limitEval = limitEval, isStateful = isStateful, isDryRun = isDryRun, stream = stream )
 
         return resp
 
-    def scanEvents( self, events, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, limitEvent = None, limitEval = None, isDryRun = False ):
+    def scanEvents( self, events, ruleName = None, namespace = None, ruleContent = None, isRunTrace = False, limitEvent = None, limitEval = None, isDryRun = False, stream = 'event' ):
         '''Scan the specific events with a D&R rule.
 
         Args:
             events (list): list of events to scan.
             ruleName (str): the name of an existing D&R rule to use.
             namespace (str): the namespace the ruleName lives in.
             ruleContent (dict): D&R rule to use to scan, with a "detect" key and a "respond" key.
             isRunTrace (bool): if True, generate a trace of the evaluation.
             limitEvent (int): approximately limit the number of events evaluated.
             limitEval (int): approximately limit the number of rule evaluations.
+            stream (str): data stream to replay.
 
         Returns:
             a dict containing results of the query.
         '''
 
-        resp = self._scanHistoricalSensor( events = events, ruleName = ruleName, namespace = namespace, ruleContent = ruleContent, isRunTrace = isRunTrace, limitEvent = limitEvent, limitEval = limitEval, isDryRun = isDryRun )
+        resp = self._scanHistoricalSensor( events = events, ruleName = ruleName, namespace = namespace, ruleContent = ruleContent, isRunTrace = isRunTrace, limitEvent = limitEvent, limitEval = limitEval, isDryRun = isDryRun, stream = stream )
 
         return resp
 
     def validateRule( self, ruleContent ):
         '''Validate a D&R rule compiles properly.
 
         Args:
@@ -298,14 +303,21 @@
     parser.add_argument( '--dry-run',
                          action = 'store_true',
                          default = None,
                          required = False,
                          dest = 'isDryRun',
                          help = 'if set, the request will be simulated and the maximum number of evaluations expected will be returned.' )
 
+    parser.add_argument( '--stream',
+                         type = str,
+                         required = False,
+                         dest = 'stream',
+                         default = 'event',
+                         help = 'data stream to replay, like "event", "audit", "detect", defaults to "event".' )
+
     args = parser.parse_args( sourceArgs )
 
     replay = Replay( Manager() )
 
     ruleContent = None
     if args.ruleContent is not None:
         with open( args.ruleContent, 'rb' ) as f:
@@ -342,26 +354,28 @@
                                                         ruleName = args.ruleName,
                                                         namespace = args.namespace,
                                                         ruleContent = ruleContent,
                                                         isRunTrace = args.isRunTrace,
                                                         limitEvent = args.limitEvent,
                                                         limitEval = args.limitEval,
                                                         isStateful = args.isStateful,
-                                                        isDryRun = args.isDryRun )
+                                                        isDryRun = args.isDryRun,
+                                                        stream = args.stream )
             elif args.isEntireOrg:
                 response = replay.scanEntireOrg( start,
                                                  end,
                                                  ruleName = args.ruleName,
                                                  namespace = args.namespace,
                                                  ruleContent = ruleContent,
                                                  isRunTrace = args.isRunTrace,
                                                  limitEvent = args.limitEvent,
                                                  limitEval = args.limitEval,
                                                  isStateful = args.isStateful,
-                                                 isDryRun = args.isDryRun )
+                                                 isDryRun = args.isDryRun,
+                                                 stream = args.stream )
             else:
                 raise LcApiException( '--sid or --entire-org must be specified' )
         else:
             # We are using an events file.
             with open( args.events, 'rb' ) as f:
                 fileContent = f.read().decode()
             # We support two formats.
@@ -385,13 +399,14 @@
             response = replay.scanEvents( events,
                                           ruleName = args.ruleName,
                                           namespace = args.namespace,
                                           ruleContent = ruleContent,
                                           isRunTrace = args.isRunTrace,
                                           limitEvent = args.limitEvent,
                                           limitEval = args.limitEval,
-                                          isDryRun = args.isDryRun )
+                                          isDryRun = args.isDryRun,
+                                          stream = args.stream )
 
     print( json.dumps( response, indent = 2 ) )
 
 if '__main__' == __name__:
     main()
```

### Comparing `limacharlie-4.4.0/limacharlie/Replicants.py` & `limacharlie-4.4.1/limacharlie/Replicants.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Search.py` & `limacharlie-4.4.1/limacharlie/Search.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Sensor.py` & `limacharlie-4.4.1/limacharlie/Sensor.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/SpotCheck.py` & `limacharlie-4.4.1/limacharlie/SpotCheck.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Spout.py` & `limacharlie-4.4.1/limacharlie/Spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Sync.py` & `limacharlie-4.4.1/limacharlie/Sync.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/Webhook.py` & `limacharlie-4.4.1/limacharlie/Webhook.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/__init__.py` & `limacharlie-4.4.1/limacharlie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """limacharlie API for limacharlie.io"""
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 # Global API Credentials
 import os
```

### Comparing `limacharlie-4.4.0/limacharlie/__main__.py` & `limacharlie-4.4.1/limacharlie/__main__.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie/utils.py` & `limacharlie-4.4.1/limacharlie/utils.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/limacharlie.egg-info/SOURCES.txt` & `limacharlie-4.4.1/limacharlie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/setup.py` & `limacharlie-4.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 setup( name = 'limacharlie',
        version = __version__,
```

### Comparing `limacharlie-4.4.0/tests/test_artifacts.py` & `limacharlie-4.4.1/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/tests/test_core.py` & `limacharlie-4.4.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/tests/test_insight.py` & `limacharlie-4.4.1/tests/test_insight.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/tests/test_spout.py` & `limacharlie-4.4.1/tests/test_spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.0/tests/test_sync.py` & `limacharlie-4.4.1/tests/test_sync.py`

 * *Files identical despite different names*

