# Comparing `tmp/operbot-167.tar.gz` & `tmp/operbot-168.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operbot-167.tar", last modified: Wed Apr  5 13:41:17 2023, max compression
+gzip compressed data, was "operbot-168.tar", last modified: Thu Apr 13 21:20:32 2023, max compression
```

## Comparing `operbot-167.tar` & `operbot-168.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 13:41:17.959577 operbot-167/
--rw-r--r--   0 bart      (1000) bart      (1001)     7482 2023-04-05 13:41:17.959577 operbot-167/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4945 2023-04-05 12:44:10.000000 operbot-167/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 13:41:17.955577 operbot-167/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2681 2023-04-05 13:31:02.000000 operbot-167/bin/operbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1773 2023-04-05 12:12:57.000000 operbot-167/bin/operbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      220 2023-04-05 10:45:33.000000 operbot-167/bin/operbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1538 2023-04-05 12:13:15.000000 operbot-167/bin/operbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 13:41:17.955577 operbot-167/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      297 2023-04-05 12:10:08.000000 operbot-167/files/operbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 13:41:17.955577 operbot-167/operbot/
--rw-r--r--   0 bart      (1000) bart      (1001)      550 2023-04-05 12:11:36.000000 operbot-167/operbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1259 2023-04-05 10:46:23.000000 operbot-167/operbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5733 2023-04-05 10:46:23.000000 operbot-167/operbot/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 13:41:17.959577 operbot-167/operbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18816 2023-04-05 12:26:13.000000 operbot-167/operbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      898 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7777 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      547 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1003 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1001 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      311 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1455 2023-04-05 10:46:31.000000 operbot-167/operbot/modules/utility.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5003 2023-04-05 10:46:23.000000 operbot-167/operbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3109 2023-04-05 10:53:58.000000 operbot-167/operbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1343 2023-04-05 10:46:23.000000 operbot-167/operbot/threads.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 13:41:17.955577 operbot-167/operbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     7482 2023-04-05 13:41:17.000000 operbot-167/operbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      702 2023-04-05 13:41:17.000000 operbot-167/operbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-05 13:41:17.000000 operbot-167/operbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-05 13:41:17.000000 operbot-167/operbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-05 13:41:17.959577 operbot-167/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-05 13:28:16.000000 operbot-167/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 13:41:17.959577 operbot-167/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-05 12:37:11.000000 operbot-167/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-05 11:38:04.000000 operbot-167/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-05 11:38:19.000000 operbot-167/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4600 2023-04-05 11:39:34.000000 operbot-167/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1077 2023-04-05 11:57:03.000000 operbot-167/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-13 21:20:32.826808 operbot-168/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-13 20:09:14.000000 operbot-168/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.822808 operbot-168/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2528 2023-04-13 20:30:08.000000 operbot-168/bin/operbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      950 2023-04-13 20:18:15.000000 operbot-168/bin/operbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-13 20:44:02.000000 operbot-168/bin/operbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-13 20:17:12.000000 operbot-168/bin/operbotd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.822808 operbot-168/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-13 20:41:39.000000 operbot-168/files/operbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/operbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)       91 2023-04-13 20:37:44.000000 operbot-168/operbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-13 20:14:50.000000 operbot-168/operbot/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5943 2023-04-13 20:14:50.000000 operbot-168/operbot/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/operbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 20:14:58.000000 operbot-168/operbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-13 20:14:58.000000 operbot-168/operbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-13 20:22:31.000000 operbot-168/operbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-13 20:22:44.000000 operbot-168/operbot/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1130 2023-04-13 20:23:05.000000 operbot-168/operbot/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    16376 2023-04-13 21:02:22.000000 operbot-168/operbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      894 2023-04-13 20:23:30.000000 operbot-168/operbot/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7720 2023-04-13 20:24:16.000000 operbot-168/operbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-13 20:24:29.000000 operbot-168/operbot/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      997 2023-04-13 20:24:42.000000 operbot-168/operbot/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2023-04-13 20:25:06.000000 operbot-168/operbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-13 20:25:19.000000 operbot-168/operbot/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2632 2023-04-13 20:25:32.000000 operbot-168/operbot/modules/usr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4838 2023-04-13 20:14:50.000000 operbot-168/operbot/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-13 20:14:50.000000 operbot-168/operbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-13 20:14:50.000000 operbot-168/operbot/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-13 20:14:50.000000 operbot-168/operbot/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-13 20:14:50.000000 operbot-168/operbot/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/operbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      782 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-13 21:20:32.000000 operbot-168/operbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-13 21:20:32.826808 operbot-168/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-13 20:43:46.000000 operbot-168/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 21:20:32.826808 operbot-168/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-13 20:09:14.000000 operbot-168/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-13 20:09:14.000000 operbot-168/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-13 20:09:14.000000 operbot-168/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-13 20:09:14.000000 operbot-168/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-13 20:09:14.000000 operbot-168/test/test_storage.py
```

### Comparing `operbot-167/PKG-INFO` & `operbot-168/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 167
+Version: 168
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -206,28 +206,28 @@
         attribute access and provides a save/load to/from json files on disk.
         Objects can be searched with database functions and uses read-only files
         to improve persistence and a type in filename for reconstruction. Methods are
         factored out into functions to have a clean namespace to read JSON data into.
         
         basic usage is this::
         
-         >>> from operbot import Object
+         >>> from operbot.objects import Object
          >>> o = Object()
          >>> o.key = "value"
          >>> o.key
          'value'
         
         Objects try to mimic a dictionary while trying to be an object with normal
         attribute access as well. hidden methods are provided, the methods are
         factored out into functions like get, items, keys, register, set, update
         and values.
         
         load/save from/to disk::
         
-         >>> from operbot import Object, read, write
+         >>> from operbot.persist import Object, read, write
          >>> o = Object()
          >>> o.key = "value"
          >>> p = write(o)
          >>> obj = Object()
          >>> read(obj, p)
          >>> obj.key
          'value'
```

### Comparing `operbot-167/README.rst` & `operbot-168/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -198,28 +198,28 @@
 attribute access and provides a save/load to/from json files on disk.
 Objects can be searched with database functions and uses read-only files
 to improve persistence and a type in filename for reconstruction. Methods are
 factored out into functions to have a clean namespace to read JSON data into.
 
 basic usage is this::
 
- >>> from operbot import Object
+ >>> from operbot.objects import Object
  >>> o = Object()
  >>> o.key = "value"
  >>> o.key
  'value'
 
 Objects try to mimic a dictionary while trying to be an object with normal
 attribute access as well. hidden methods are provided, the methods are
 factored out into functions like get, items, keys, register, set, update
 and values.
 
 load/save from/to disk::
 
- >>> from operbot import Object, read, write
+ >>> from operbot.persist import Object, read, write
  >>> o = Object()
  >>> o.key = "value"
  >>> p = write(o)
  >>> obj = Object()
  >>> read(obj, p)
  >>> obj.key
  'value'
```

### Comparing `operbot-167/bin/operbot` & `operbot-168/bin/operbot`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
+# pylint: disable=C0115,C0116,C0413,W0212,E0611,E0401,I1101
 
 
 'operator bot'
 
 
 import os
-import readline
 import sys
 import termios
 import time
 import traceback
 
 
 sys.path.insert(0, os.getcwd())
 
 
-from operbot.handler import Client, Command, Event, Handler, Listens
-from operbot.handler import command, parse, scan
-from operbot.objects import update
-from operbot.persist import Persist
-from operbot.threads import launch
+import operbot.modules
 
 
-from operbot.modules import cmd, flt, irc, log, rss, tdo, thr
+from operbot.handler import Client, Error, command, parse
+from operbot.persist import Persist
+from operbot.scanner import importer, scandir, scanpkg, starter
+from operbot.threads import launch
 
 
-Persist.workdir = os.path.expanduser('~/.operbot')
+MOD = "cmd,err,irc,rss,sts,thr"
+NAME = "operbot"
 
 
-scan(cmd)
-scan(flt)
-scan(irc)
-scan(log)
-scan(rss)
-scan(tdo)
-scan(thr)
+Persist.workdir = os.path.expanduser("~/.%s" % NAME)
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
@@ -48,14 +42,15 @@
         sys.stdout.flush()
 
 
 class Console(CLI):
 
     def handle(self, evt):
         CLI.handle(self, evt)
+        evt.wait()
 
     def poll(self):
         return self.event(input("> "))
 
 
 def daemon():
     pid = os.fork()
@@ -69,25 +64,19 @@
     ses = open('/dev/null', 'a+')
     os.dup2(sos.fileno(), sys.stdout.fileno())
     os.dup2(ses.fileno(), sys.stderr.fileno())
 
 
 def waiter():
     got = []
-    for ex in Handler.errors:
+    for ex in Error.errors:
         traceback.print_exception(type(ex), ex, ex.__traceback__)
         got.append(ex)
     for exc in got:
-        Handler.errors.remove(exc)
-    got = []
-    for ex in Command.errors:
-        traceback.print_exception(type(ex), ex, ex.__traceback__)
-        got.append(ex)
-    for exc in got:
-        Command.errors.remove(exc)
+        Error.errors.remove(exc)
 
 
 def wrap(func):
     fds = sys.stdin.fileno()
     gotterm = True
     try:
         old = termios.tcgetattr(fds)
@@ -97,37 +86,37 @@
         func()
     except (EOFError, KeyboardInterrupt):
         print('')
     finally:
         if gotterm:
             termios.tcsetattr(fds, termios.TCSADRAIN, old)
         waiter()
-      
+
 
 def main():
     dowait = False
     cfg = parse(' '.join(sys.argv[1:]))
+    if os.path.exists("modules"):
+        scandir("modules", importer, cfg.mod or MOD)
+    scanpkg(operbot.modules, importer, cfg.mod or MOD)
     if cfg.txt:
         cli = CLI()
         command(cli, cfg.otxt)
     elif 'd' in cfg.opts:
         daemon()
         dowait = True
     elif 'c' in cfg.opts:
         date = time.ctime(time.time()).replace('  ', ' ')
-        print(f'OPERBOT started {date}')
+        print(f'{NAME.upper()} started {date}')
         csl = Console()
         launch(csl.loop)
         dowait = True
     if dowait:
-        if os.path.exists("modules"):
-            from modules.scanner import importer, scandir
-            scandir("modules", importer, doall=True)
-        irc.start()
-        rss.start()
+        scanpkg(operbot.modules, starter, cfg.mod or MOD)
+        scandir("modules", starter, cfg.mod or MOD)
         while 1:
             time.sleep(1.0)
             waiter()
 
 
 wrap(main)
 waiter()
```

### Comparing `operbot-167/operbot/handler.py` & `operbot-168/operbot/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,167 +1,173 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,W0212,R0201,R0902,W0613,W0703,E0402,W0201
+# pylint: disable=C0115,C0116,W0212,R0201,R0902,W0613,W0703,E0402,W0201,R0903
 
 
 'handler'
 
 
 import inspect
 import queue
+import ssl
 import threading
 
 
 from .objects import Default, Object
 from .threads import launch
 
 
 def __dir__():
     return (
             'Client',
             'Command',
+            'Error',
             'Event',
             'Handler',
             'Listens',
             'command',
             'parse',
             'scan'
            )
 
 
 __all__ = __dir__()
 
 
-class Handler(Object):
+class Error(Object):
 
     errors = []
 
+    @staticmethod
+    def handle(ex):
+        exc = ex.with_traceback(ex.__traceback__)
+        Error.errors.append(exc)
+
+
+class Handler(Object):
+
     def __init__(self):
         Object.__init__(self)
         self.cbs = Object()
         self.queue = queue.Queue()
         self.stopped = threading.Event()
         self.register('command', self.handle)
 
     def dispatch(self, func, evt):
         try:
             func(evt)
         except Exception as ex:
             exc = ex.with_traceback(ex.__traceback__)
-            Handler.errors.append(exc)
+            Error.errors.append(exc)
             evt.ready()
 
     def event(self, txt):
         msg = Event()
-        msg.orig = repr(self)
         msg.type = 'command'
-        msg.txt = txt
+        msg.orig = repr(self)
+        msg.parse(txt)
         return msg
 
     def handle(self, evt):
         func = getattr(self.cbs, evt.type, None)
         if func:
             evt._thr = launch(self.dispatch, func, evt, name=evt.cmd)
         return evt
 
     def loop(self):
-        while not self.stopped.set():
-            self.handle(self.poll())
+        while not self.stopped.is_set():
+            try:
+                self.handle(self.poll())
+            except (ssl.SSLError, EOFError, KeyboardInterrupt) as ex:
+                Error.handle(ex)
+                self.restart()
+
+    def one(self, txt):
+        return self.handle(self.event(txt))
 
     def poll(self):
         return self.queue.get()
 
     def put(self, evt):
         self.queue.put_nowait(evt)
 
     def register(self, cmd, func):
         setattr(self.cbs, cmd, func)
 
+    def restart(self):
+        self.stop()
+        self.start()
+
+    def start(self):
+        launch(self.loop)
+
     def stop(self):
         self.stopped.set()
+        self.queue.put_nowait(None)
 
 
 class Command(Object):
 
     cmds = Object()
-    errors = []
 
     @staticmethod
     def add(cmd, func):
         setattr(Command.cmds, cmd, func)
 
     @staticmethod
     def handle(evt):
         evt.parse(evt.txt)
         func = getattr(Command.cmds, evt.cmd, None)
         if func:
             try:
                 func(evt)
                 evt.show()
             except Exception as ex:
-                exc = ex.with_traceback(ex.__traceback__)
-                Command.errors.append(exc)
+                Error.handle(ex)
         evt.ready()
         return evt
 
 
 class Client(Handler):
 
     def __init__(self):
         Handler.__init__(self)
         Listens.add(self)
         self.register('command', Command.handle)
 
     def announce(self, txt):
         self.raw(txt)
 
-    def event(self, txt):
-        msg = Event()
-        msg.type = 'command'
-        msg.orig = repr(self)
-        msg.parse(txt)
-        return msg
-
-    def one(self, txt):
-        return self.handle(self.event(txt))
-
     def raw(self, txt):
         pass
 
     def say(self, channel, txt):
         self.raw(txt)
 
-    def start(self):
-        launch(self.loop)
-
-    def stop(self):
-        self.stopped.set()
-        self.queue.put_nowait(None)
-
 
 class Event(Default):
 
     __slots__ = ('_ready', '_thr')
 
     def __init__(self, *args, **kwargs):
         Default.__init__(self, *args, **kwargs)
         self._ready = threading.Event()
         self._thr = None
         self.args = []
         self.gets = Default()
+        self.opts = ""
         self.orig = None
         self.result = []
         self.sets = Default()
-        self.skip = Default()
 
     def parse(self, txt):
         self.otxt = txt
-        spl = self.otxt.split()
+        splitted = self.otxt.split()
         args = []
         _nr = -1
-        for word in spl:
+        for word in splitted:
             if word.startswith('-'):
                 try:
                     self.index = int(word[1:])
                 except ValueError:
                     self.opts = self.opts + word[1:2]
                 continue
             try:
@@ -246,16 +252,22 @@
 
 
 def parse(txt):
     cfg = Event()
     cfg.parse(txt)
     if "v" in cfg.opts:
         cfg.verbose = True
-    if "mod" in cfg.sets:
-        cfg.mod = cfg.sets.mod
     return cfg
 
 
 def scan(mod):
     for _key, cmd in inspect.getmembers(mod, inspect.isfunction):
         if 'event' in cmd.__code__.co_varnames:
             Command.add(cmd.__name__, cmd)
+
+
+def spl(txt):
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
```

### Comparing `operbot-167/operbot/modules/irc.py` & `operbot-168/operbot/modules/irc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0902,R0903,W0613,E1101,R0912,R0904,R0915,E0402
-
+# pylint: disable=C0115,C0116,R0902,R0903,W0613,E1101,R0912,R0904,R0915
+# pylint: disable=E0402,E0401
 
 'internet relay chat'
 
 
 import base64
 import os
 import queue
@@ -13,33 +13,28 @@
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from ..handler import Client, Command, Event
-from ..objects import Default, Object, keys, printable, update
-from ..persist import find, fntime, last, write
+from ..handler import Client, Command, Error, Event
+from ..objects import Default, Object, keys, prt, update
+from ..persist import last, write
 from ..threads import launch
 
 
-from .utility import elapsed
+from .usr import Users
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
-            'NoUser',
-            'Users',
-            'User',
-            'dlt',
             'cfg',
-            'met',
             'mre',
             'pwd',
             'start'
            )
 
 
 NAME = "operbot"
@@ -50,19 +45,14 @@
 
 def start():
     irc = IRC()
     irc.start()
     return irc
 
 
-class NoUser(Exception):
-
-    pass
-
-
 class Config(Default):
 
     channel = '#%s' % NAME
     control = '!'
     nick = NAME
     password = ''
     port = 6667
@@ -339,34 +329,27 @@
     def keep(self):
         while 1:
             self.connected.wait()
             self.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
-            time.sleep(10.0)
             if self.state.pongcheck:
                 self.state.pongcheck = False
                 self.keeprunning = False
-                self.stop()
-                launch(self.loop)
                 self.reconnect()
 
 
     def logon(self, server, nck):
-        assert server
-        assert nck
-        assert self.cfg.username
-        assert self.cfg.realname
         self.direct('NICK %s' % nck)
         self.direct(
-                 'USER %s %s %s :%s' % (self.cfg.username,
+                 'USER %s %s %s :%s' % (self.cfg.username or NAME,
                  server,
                  server,
-                 self.cfg.realname)
+                 self.cfg.realname or NAME)
                 )
 
     def kill(self, event):
         pass
 
     def log(self, event):
         pass
@@ -464,30 +447,35 @@
             msg = Event(event)
             msg.type = 'command'
             msg.parse(event.txt)
             self.handle(msg)
 
     def quit(self, event):
         if event.orig and event.orig in self.zelf:
-            self.reconnect()
+            self.stop()
 
     def raw(self, txt):
         txt = txt.rstrip()
         if not txt.endswith('\r\n'):
             txt += '\r\n'
         txt = txt[:512]
         txt += '\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
-            except (ssl.SSLError, ConnectionResetError, BrokenPipeError) as ex:
+            except (
+                    ssl.SSLError,
+                    ConnectionResetError,
+                    BrokenPipeError
+                   ) as ex:
                 time.sleep(5.0)
-                self.errors.append(ex)
+                Error.errors.append(ex)
                 self.stop()
+                return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
@@ -510,145 +498,54 @@
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
-        assert self.cfg.nick
-        assert self.cfg.server
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.connected.clear()
         self.joined.clear()
         launch(Client.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
-               self.cfg.server,
-               self.cfg.nick,
+               self.cfg.server or "localhost",
+               self.cfg.nick or NAME,
                int(self.cfg.port or '6667')
               )
         if not self.keeprunning:
             launch(self.keep)
 
     def stop(self):
         try:
             self.sock.shutdown(2)
         except(ssl.SSLError,  OSError):
             pass
         Client.stop(self)
-
-
-class Users(Object):
-
-    @staticmethod
-    def allowed(origin, perm):
-        perm = perm.upper()
-        user = Users.get_user(origin)
-        val = False
-        if user and perm in user.perms:
-            val = True
-        return val
-
-    @staticmethod
-    def delete(origin, perm):
-        res = False
-        for user in Users.get_users(origin):
-            try:
-                user.perms.remove(perm)
-                write(user)
-                res = True
-            except ValueError:
-                pass
-        return res
-
-    @staticmethod
-    def get_users(origin=''):
-        selector = {'user': origin}
-        return find('user', selector)
-
-    @staticmethod
-    def get_user(origin):
-        users = list(Users.get_users(origin))
-        res = None
-        if len(users) > 0:
-            res = users[-1]
-        return res
-
-    @staticmethod
-    def perm(origin, permission):
-        user = Users.get_user(origin)
-        if not user:
-            raise NoUser(origin)
-        if permission.upper() not in user.perms:
-            user.perms.append(permission.upper())
-            write(user)
-        return user
-
-
-class User(Object):
-
-    def __init__(self, val=None):
-        Object.__init__(self)
-        self.user = ''
-        self.perms = []
-        if val:
-            update(self, val)
+        Output.stop(self)
 
 
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
-        event.reply(printable(
-                          config,
-                          keys(config),
-                          skip='control,password,realname,sleep,username')
-                         )
+        event.reply(prt(
+                        config,
+                        keys(config),
+                        skip='control,password,realname,sleep,username')
+                       )
     else:
         update(config, event.sets)
         write(config)
         event.reply('ok')
 
 
-def dlt(event):
-    if not event.args:
-        event.reply('dlt <username>')
-        return
-    selector = {'user': event.args[0]}
-    for obj in find('user', selector):
-        obj.__deleted__ = True
-        write(obj)
-        event.reply('ok')
-        break
-
-
-def met(event):
-    if not event.args:
-        nmr = 0
-        for obj in find('user'):
-            event.reply('%s %s %s %s' % (
-                                         nmr,
-                                         obj.user,
-                                         obj.perms,
-                                         elapsed(time.time() - fntime(obj.__fnm__)))
-                                        )
-            nmr += 1
-        if not nmr:
-            event.reply('no users introduced yet')
-        return
-    user = User()
-    user.user = event.rest
-    user.perms = ['USER']
-    write(user)
-    event.reply('ok')
-
-
 def mre(event):
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = event.bot()
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
```

### Comparing `operbot-167/operbot/modules/log.py` & `operbot-168/operbot/modules/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 'log'
 
 
 import time
 
 
+from ..clocked import elapsed
 from ..persist import find, fntime, write
 from ..objects import Object
 
 
-from .utility import elapsed
-
-
 def __dir__():
     return (
             'Log',
             'log',
            )
 
 
@@ -36,13 +34,13 @@
             event.reply('%s %s %s' % (
                                       nmr,
                                       obj.txt,
                                       elapsed(time.time() - fntime(obj.__oid__)))
                                      )
             nmr += 1
         if not nmr:
-            event.reply('log <txt>')
+            event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
     write(obj)
     event.reply('ok')
```

### Comparing `operbot-167/operbot/modules/rss.py` & `operbot-168/operbot/modules/rss.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,33 +14,29 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from ..clocked import Repeater
-from ..handler import Listens
-from ..objects import Object, printable, update
+from ..clocked import Repeater, elapsed
+from ..handler import Listens, spl
+from ..objects import Object, prt, update
 from ..persist import find, fntime, last, write
 from ..threads import launch, threaded
 
 
-from .utility import elapsed, spl
-
-
 def __dir__():
     return (
         'Feed',
         'Fetcher',
         'Repeater',
         'Rss',
         'Seen',
         'Timer',
-        'debug',
         'dpl',
         'ftc',
         'nme',
         'rem',
         'rss',
         'start'
     )
@@ -217,15 +213,15 @@
             return i.groups()
     return []
 
 
 def geturl(url):
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
-    req.add_header('User-agent', useragent('OPB - object programming bot'))
+    req.add_header('User-agent', useragent('OPERBOT - operator bot'))
     response = urllib.request.urlopen(req)
     response.data = response.read()
     return response
 
 
 def striphtml(text):
     clean = re.compile('<.*?>')
@@ -293,15 +289,15 @@
 
 def rss(event):
     if not event.rest:
         nrs = 0
         for feed in find('rss'):
             event.reply('%s %s %s' % (
                                    nrs,
-                                   printable(feed),
+                                   prt(feed),
                                    elapsed(time.time()-fntime(feed.__oid__))
                                   )
                        )
             nrs += 1
         if not nrs:
             event.reply('no rss feed found.')
         return
```

### Comparing `operbot-167/operbot/modules/tdo.py` & `operbot-168/operbot/modules/tdo.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 'todo'
 
 
 import time
 
 
+from ..clocked import elapsed
 from ..objects import Object
 from ..persist import find, fntime, write
 
 
-from .utility import elapsed
-
-
 class Todo(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
@@ -39,13 +37,13 @@
         for obj in find('todo'):
             event.reply('%s %s %s' % (
                                       nr,
                                       obj.txt,
                                       elapsed(time.time()-fntime(obj.__oid__))))
             nr += 1
         if not nr:
-            event.reply("nothing todo")
+            event.reply("no todo")
         return
     o = Todo()
     o.txt = event.rest
     write(o)
     event.reply('ok')
```

### Comparing `operbot-167/operbot/modules/thr.py` & `operbot-168/operbot/modules/thr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0114,C0115,C0116,E1101,E0402
 
 
-"list running commands."
+"list running threads."
 
 
 import threading
 import time
 
 
+from ..clocked import elapsed
 from ..objects import Object, update
 
 
-from .utility import elapsed
-
 def __dir__():
     return (
             'thr',
            )
 
 
 __all__ = __dir__()
 
 
-
 starttime = time.time()
 
 
 def thr(event):
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
         if str(thread).startswith('<_'):
@@ -41,8 +39,8 @@
         result.append((uptime, thread.name))
     res = []
     for uptime, txt in sorted(result, key=lambda x: x[0]):
         res.append('%s/%s' % (txt, elapsed(uptime)))
     if res:
         event.reply(' '.join(res))
     else:
-        event.reply('no threads running')
+        event.reply('no threads')
```

### Comparing `operbot-167/operbot/objects.py` & `operbot-168/operbot/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 from json import JSONDecoder, JSONEncoder
 
 
 def __dir__():
     return (
             'Default',
             'Object',
+            'dumps',
             'items',
             'keys',
             'kind',
-            'printable',
+            'loads',
+            'prt',
             'search',
             'update',
             'values',
            )
 
 
 __all__ = __dir__()
@@ -85,15 +87,15 @@
 def kind(obj) -> str:
     kin = str(type(obj)).split()[-1][1:-2]
     if kin == "type":
         kin = obj.__name__
     return kin
 
 
-def printable(obj, args="", skip="", plain=False):
+def prt(obj, args="", skip="", plain=False):
     res = []
     keyz = []
     if "," in args:
         keyz = args.split(",")
     if not keyz:
         keyz = keys(obj)
     for key in sorted(keyz):
@@ -172,18 +174,14 @@
         return Object(val)
 
     def raw_decode(self, s, idx=0) -> (int, Object):
         ""
         return JSONDecoder.raw_decode(self, s, idx)
 
 
-def load(fpt, *args, **kw) -> Object:
-    return json.load(fpt, *args, cls=ObjectDecoder, **kw)
-
-
 def loads(string, *args, **kw) -> Object:
     return json.loads(string, *args, cls=ObjectDecoder, **kw)
 
 
 class ObjectEncoder(JSONEncoder):
 
     def __init__(self, *args, **kw):
@@ -213,15 +211,10 @@
         return JSONEncoder.encode(self, o)
 
     def iterencode(self, o, _one_shot=False) -> str:
         ""
         return JSONEncoder.iterencode(self, o, _one_shot)
 
 
-def dump(*args, **kw) -> None:
-    kw["cls"] = ObjectEncoder
-    return json.dump(*args, **kw)
-
-
 def dumps(*args, **kw) -> str:
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
```

### Comparing `operbot-167/operbot/persist.py` & `operbot-168/operbot/persist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Tihs file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,R0903,E0402
 
 
 "persistence"
 
 
+import json
 import os
 import pathlib
 import time
 import _thread
 
 
-from .objects import Object, dump, load, kind, search, update
+from .objects import Object, ObjectDecoder, ObjectEncoder
+from .objects import kind, search, update
 
 
 def __dir__():
     return (
             'Persist',
             'cdir',
             'last',
@@ -25,32 +27,34 @@
             'write'
            )
 
 
 __all__ = __dir__()
 
 
-NAME = "operbot"
-
-
 disklock = _thread.allocate_lock()
 
 
 class Persist(Object):
 
-    workdir = os.path.expanduser("~/.%s" % NAME)
+    workdir = os.path.expanduser("~/.opr")
 
 
 def cdir(pth) -> None:
     if not pth.endswith(os.sep):
         pth = os.path.dirname(pth)
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
 
+def dump(*args, **kw) -> None:
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
 def files() -> []:
     return os.listdir(os.path.join(Persist.workdir, "store"))
 
 
 def fns(match) -> []:
     assert Persist.workdir
     dname = ''
@@ -70,14 +74,18 @@
 
 def hook(otp) -> Object:
     obj = Object()
     read(obj, otp)
     return obj
 
 
+def load(fpt, *args, **kw) -> Object:
+    return json.load(fpt, *args, cls=ObjectDecoder, **kw)
+
+
 def path(pth) -> str:
     return os.path.join(Persist.workdir, 'store', pth)
 
 
 def read(obj, pth) -> None:
     pth = path(pth)
     with disklock:
@@ -105,15 +113,15 @@
 
 
 def find(match, selector=None) -> []:
     if selector is None:
         selector = {}
     for fnm in fns(match):
         obj = hook(fnm)
-        if '__deleted__' in obj and obj.__deleted__:
+        if '__deleted__' in obj:
             continue
         if selector and not search(obj, selector):
             continue
         yield obj
 
 
 def last(obj, selector=None) -> None:
```

### Comparing `operbot-167/operbot.egg-info/PKG-INFO` & `operbot-168/operbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 167
+Version: 168
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -206,28 +206,28 @@
         attribute access and provides a save/load to/from json files on disk.
         Objects can be searched with database functions and uses read-only files
         to improve persistence and a type in filename for reconstruction. Methods are
         factored out into functions to have a clean namespace to read JSON data into.
         
         basic usage is this::
         
-         >>> from operbot import Object
+         >>> from operbot.objects import Object
          >>> o = Object()
          >>> o.key = "value"
          >>> o.key
          'value'
         
         Objects try to mimic a dictionary while trying to be an object with normal
         attribute access as well. hidden methods are provided, the methods are
         factored out into functions like get, items, keys, register, set, update
         and values.
         
         load/save from/to disk::
         
-         >>> from operbot import Object, read, write
+         >>> from operbot.persist import Object, read, write
          >>> o = Object()
          >>> o.key = "value"
          >>> p = write(o)
          >>> obj = Object()
          >>> read(obj, p)
          >>> obj.key
          'value'
```

### Comparing `operbot-167/setup.py` & `operbot-168/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name="operbot",
-    version="167",
+    version="168",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/operbot",
     description="operator bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

### Comparing `operbot-167/test/test_decoder.py` & `operbot-168/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `operbot-167/test/test_inherit.py` & `operbot-168/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `operbot-167/test/test_objects.py` & `operbot-168/test/test_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 "object tests"
 
 
 import unittest
 
 
 from operbot.objects import Object, items, keys, update, values
-from operbot.objects import printable, kind
+from operbot.objects import prt, kind
 
 
 VALIDJSON = '{"test": "bla"}'
 
 
 attrs1 = (
          'Object',
@@ -154,15 +154,15 @@
 
     def test_str(self):
         obj = Object()
         self.assertEqual(str(obj), "{}")
 
     def test_printable(self):
         obj = Object()
-        self.assertEqual(printable(obj), "")
+        self.assertEqual(prt(obj), "")
 
     def test_getattr(self):
         obj = Object()
         obj.key = "value"
         self.assertEqual(getattr(obj, "key"), "value")
 
     def test_keys(self):
```

### Comparing `operbot-167/test/test_storage.py` & `operbot-168/test/test_storage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # This file is placed in the Public Domain.
+# pylint: disable=C0115,C0116
+
+
+"storage tests"
 
 
-import json
 import os
 import unittest
 
 
 from operbot.objects import Object
 from operbot.persist import Persist, path, write
```

