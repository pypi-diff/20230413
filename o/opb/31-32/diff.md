# Comparing `tmp/opb-31.tar.gz` & `tmp/opb-32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opb-31.tar", last modified: Tue Apr 11 13:55:29 2023, max compression
+gzip compressed data, was "opb-32.tar", last modified: Thu Apr 13 12:46:06 2023, max compression
```

## Comparing `opb-31.tar` & `opb-32.tar`

### file list

```diff
@@ -1,43 +1,57 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.549208 opb-31/
--rw-r--r--   0 bart      (1000) bart      (1001)     6732 2023-04-11 13:55:29.549208 opb-31/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4466 2023-04-11 13:49:58.000000 opb-31/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1968 2023-04-11 13:53:03.000000 opb-31/bin/opb
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1003 2023-04-11 13:04:48.000000 opb-31/bin/opbc
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1181 2023-04-11 13:05:14.000000 opb-31/bin/opbd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/opb/
--rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-11 11:17:26.000000 opb-31/opb/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6007 2023-04-11 13:17:07.000000 opb-31/opb/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/opb/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      248 2023-04-11 11:17:10.000000 opb-31/opb/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      498 2023-04-11 11:25:09.000000 opb-31/opb/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1136 2023-04-11 11:23:17.000000 opb-31/opb/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18718 2023-04-11 12:43:17.000000 opb-31/opb/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-11 11:23:41.000000 opb-31/opb/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2931 2023-04-11 11:23:30.000000 opb-31/opb/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1001)    17740 2023-04-11 11:24:16.000000 opb-31/opb/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2366 2023-04-11 11:04:11.000000 opb-31/opb/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7736 2023-04-11 11:25:34.000000 opb-31/opb/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      535 2023-04-11 11:19:26.000000 opb-31/opb/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1008 2023-04-11 11:19:48.000000 opb-31/opb/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1004 2023-04-11 11:20:05.000000 opb-31/opb/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2461 2023-04-11 13:16:47.000000 opb-31/opb/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1001)      315 2023-04-11 11:23:52.000000 opb-31/opb/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5693 2023-04-11 11:04:11.000000 opb-31/opb/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4895 2023-04-11 11:03:12.000000 opb-31/opb/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-11 11:18:06.000000 opb-31/opb/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1918 2023-04-11 13:21:17.000000 opb-31/opb/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-11 11:03:44.000000 opb-31/opb/threads.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/opb.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     6732 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      648 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       16 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/namespace_packages.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-11 13:55:29.549208 opb-31/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1116 2023-04-11 13:50:48.000000 opb-31/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.549208 opb-31/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-11 11:01:25.000000 opb-31/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-11 11:01:25.000000 opb-31/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-11 11:01:25.000000 opb-31/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-11 11:01:25.000000 opb-31/test/test_objects.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.374288 opb-32/
+-rw-r--r--   0 bart      (1000) bart      (1001)       52 2023-04-13 12:34:46.000000 opb-32/MANIFEST.in
+-rw-r--r--   0 bart      (1000) bart      (1001)     7042 2023-04-13 12:46:06.370288 opb-32/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4672 2023-04-13 12:45:02.000000 opb-32/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2395 2023-04-13 12:34:46.000000 opb-32/bin/opb
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      936 2023-04-13 12:39:42.000000 opb-32/bin/opbc
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      209 2023-04-13 12:34:46.000000 opb-32/bin/opbctl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1147 2023-04-13 12:34:46.000000 opb-32/bin/opbd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)      301 2023-04-13 12:34:46.000000 opb-32/files/opb.service
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/mod/
+-rw-r--r--   0 bart      (1000) bart      (1001)      184 2023-04-13 12:34:46.000000 opb-32/mod/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2931 2023-04-13 12:34:46.000000 opb-32/mod/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17762 2023-04-13 12:34:46.000000 opb-32/mod/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2353 2023-04-13 12:34:46.000000 opb-32/mod/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2339 2023-04-13 12:34:46.000000 opb-32/mod/shl.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2461 2023-04-13 12:34:46.000000 opb-32/mod/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5693 2023-04-13 12:34:46.000000 opb-32/mod/wsd.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 12:34:46.000000 opb-32/modules/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/opb/
+-rw-r--r--   0 bart      (1000) bart      (1001)       97 2023-04-13 12:34:46.000000 opb-32/opb/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-13 12:34:46.000000 opb-32/opb/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5943 2023-04-13 12:34:46.000000 opb-32/opb/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/opb/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-13 12:34:46.000000 opb-32/opb/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-13 12:34:46.000000 opb-32/opb/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      410 2023-04-13 12:34:46.000000 opb-32/opb/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      498 2023-04-13 12:34:46.000000 opb-32/opb/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1136 2023-04-13 12:34:46.000000 opb-32/opb/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    16371 2023-04-13 12:34:46.000000 opb-32/opb/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      900 2023-04-13 12:34:46.000000 opb-32/opb/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7736 2023-04-13 12:34:46.000000 opb-32/opb/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      344 2023-04-13 12:34:46.000000 opb-32/opb/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1003 2023-04-13 12:34:46.000000 opb-32/opb/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      996 2023-04-13 12:34:46.000000 opb-32/opb/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      315 2023-04-13 12:34:46.000000 opb-32/opb/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2638 2023-04-13 12:34:46.000000 opb-32/opb/modules/usr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4838 2023-04-13 12:34:46.000000 opb-32/opb/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-13 12:34:46.000000 opb-32/opb/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-13 12:34:46.000000 opb-32/opb/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-13 12:34:46.000000 opb-32/opb/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-13 12:34:46.000000 opb-32/opb/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/opb.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7042 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      770 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-13 12:46:06.000000 opb-32/opb.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-13 12:46:06.374288 opb-32/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1556 2023-04-13 12:34:46.000000 opb-32/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-13 12:46:06.370288 opb-32/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-13 12:34:46.000000 opb-32/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-13 12:34:46.000000 opb-32/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-13 12:34:46.000000 opb-32/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-13 12:34:46.000000 opb-32/test/test_objects.py
```

### Comparing `opb-31/PKG-INFO` & `opb-32/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 31
+Version: 32
 Summary: object programming bot
 Home-page: http://github.com/operbot/opb
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -165,14 +165,27 @@
          rem - remove a rss feed by matching is to its url
          rss - add a feed to fetch, fetcher runs every 5 minutes
          thr - show the running threads
          tdo - adds a todo item, no options returns list of todo's
          upt - show uptime
         
         
+        **24/7**
+        
+        ::
+        
+         sudo cp /usr/local/opb/opb.service
+                 /etc/systemd/system``
+         sudo systemctl enable opb --now
+        
+         default is #opb on localhost
+        
+        use ``opbctl <cmd>`` as you would have use ``opb <cmd>``.
+        
+        
         **PROGRAMMING**
         
         
         The ``opb`` package provides an Object class, that mimics a dict while using
         attribute access and provides a save/load to/from json files on disk.
         Objects can be searched with database functions and uses read-only files
         to improve persistence and a type in filename for reconstruction. Methods are
```

### Comparing `opb-31/README.rst` & `opb-32/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -157,14 +157,27 @@
  rem - remove a rss feed by matching is to its url
  rss - add a feed to fetch, fetcher runs every 5 minutes
  thr - show the running threads
  tdo - adds a todo item, no options returns list of todo's
  upt - show uptime
 
 
+**24/7**
+
+::
+
+ sudo cp /usr/local/opb/opb.service
+         /etc/systemd/system``
+ sudo systemctl enable opb --now
+
+ default is #opb on localhost
+
+use ``opbctl <cmd>`` as you would have use ``opb <cmd>``.
+
+
 **PROGRAMMING**
 
 
 The ``opb`` package provides an Object class, that mimics a dict while using
 attribute access and provides a save/load to/from json files on disk.
 Objects can be searched with database functions and uses read-only files
 to improve persistence and a type in filename for reconstruction. Methods are
```

### Comparing `opb-31/bin/opbc` & `opb-32/bin/opbc`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 import opb.modules
 
 
 from opb.handler import Client, Error
 from opb.handler import command, parse
 from opb.persist import Persist
-from opb.scanner import scandir, scanpkg, importer
+from opb.scanner import scanpkg, importer
 
 
-Persist.workdir = os.path.expanduser('~/.opb')
+Persist.workdir = "/var/lib/opb/"
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
@@ -44,14 +44,13 @@
     for exc in got:
         Error.errors.remove(exc)
 
 
 def main():
     cfg = parse(' '.join(sys.argv[1:]))
     scanpkg(opb.modules, importer, doall=True)
-    scandir("modules", importer, doall=True)
     cli = CLI()
     command(cli, cfg.otxt)
     waiter()
 
 
 main()
```

### Comparing `opb-31/opb/clocked.py` & `opb-32/opb/clocked.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb/handler.py` & `opb-32/opb/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,18 +149,18 @@
 
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
         splitted = self.otxt.split()
         args = []
         _nr = -1
         for word in splitted:
@@ -252,16 +252,14 @@
 
 
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
```

### Comparing `opb-31/opb/modules/fnd.py` & `opb-32/opb/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb/modules/irc.py` & `opb-32/opb/modules/irc.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,31 +13,28 @@
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from opb.clocked import elapsed
 from opb.handler import Client, Command, Error, Event
 from opb.objects import Default, Object, keys, prt, update
-from opb.persist import find, fntime, last, write
+from opb.persist import last, write
 from opb.threads import launch
 
 
+from opb.modules.usr import Users
+
+
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
 
 
 NAME = "opb"
@@ -48,19 +45,14 @@
 
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
@@ -531,71 +523,14 @@
             self.sock.shutdown(2)
         except(ssl.SSLError,  OSError):
             pass
         Client.stop(self)
         Output.stop(self)
 
 
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
-
-
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(prt(
                         config,
                         keys(config),
@@ -603,47 +538,14 @@
                        )
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

### Comparing `opb-31/opb/modules/log.py` & `opb-32/opb/modules/log.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,13 +34,13 @@
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

### Comparing `opb-31/opb/modules/mbx.py` & `opb-32/mod/mbx.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb/modules/mdl.py` & `opb-32/mod/mdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 "genocide model"
 
 
 import datetime
 import time
 
 
-from opb.clocked import Repeater, elapsed
+from opb.clocked import Repeater
 from opb.handler import Event, Listens
 from opb.objects import Object, keys
 from opb.threads import launch
-
+from opb.utility import elapsed
 
 def __dir__():
     return (
         'mdl',
         'now',
         'start'
     )
```

### Comparing `opb-31/opb/modules/req.py` & `opb-32/mod/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # This file is placed in the Public Domain.
 # pylint: disable=C0114,C0115,C0116
 
 
-"""reconsider
-
-
-| **Information and Evidence Unit**
+"""| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
 
 Hello Office of the Prosecutor,
```

### Comparing `opb-31/opb/modules/rss.py` & `opb-32/opb/modules/rss.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb/modules/tdo.py` & `opb-32/opb/modules/tdo.py`

 * *Files 24% similar despite different names*

```diff
@@ -37,13 +37,13 @@
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

### Comparing `opb-31/opb/modules/thr.py` & `opb-32/opb/modules/thr.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,8 +39,8 @@
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

### Comparing `opb-31/opb/modules/udp.py` & `opb-32/mod/udp.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb/modules/wsd.py` & `opb-32/mod/wsd.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb/objects.py` & `opb-32/opb/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 from json import JSONDecoder, JSONEncoder
 
 
 def __dir__():
     return (
             'Default',
             'Object',
+            'dumps',
             'items',
             'keys',
             'kind',
+            'loads',
             'prt',
             'search',
             'update',
             'values',
            )
 
 
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
@@ -213,11 +211,10 @@
         return JSONEncoder.encode(self, o)
 
     def iterencode(self, o, _one_shot=False) -> str:
         ""
         return JSONEncoder.iterencode(self, o, _one_shot)
 
 
-
 def dumps(*args, **kw) -> str:
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
```

### Comparing `opb-31/opb/persist.py` & `opb-32/opb/persist.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb/scanner.py` & `opb-32/opb/scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # pylint: disable=C0116,E0401,E0402
 
 
 "introspection"
 
 
 import importlib
+import importlib.util
 import inspect
 import os
 
 
 from .handler import Command, spl
```

### Comparing `opb-31/opb/threads.py` & `opb-32/opb/threads.py`

 * *Files identical despite different names*

### Comparing `opb-31/opb.egg-info/PKG-INFO` & `opb-32/opb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 31
+Version: 32
 Summary: object programming bot
 Home-page: http://github.com/operbot/opb
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -165,14 +165,27 @@
          rem - remove a rss feed by matching is to its url
          rss - add a feed to fetch, fetcher runs every 5 minutes
          thr - show the running threads
          tdo - adds a todo item, no options returns list of todo's
          upt - show uptime
         
         
+        **24/7**
+        
+        ::
+        
+         sudo cp /usr/local/opb/opb.service
+                 /etc/systemd/system``
+         sudo systemctl enable opb --now
+        
+         default is #opb on localhost
+        
+        use ``opbctl <cmd>`` as you would have use ``opb <cmd>``.
+        
+        
         **PROGRAMMING**
         
         
         The ``opb`` package provides an Object class, that mimics a dict while using
         attribute access and provides a save/load to/from json files on disk.
         Objects can be searched with database functions and uses read-only files
         to improve persistence and a type in filename for reconstruction. Methods are
```

### Comparing `opb-31/test/test_decoder.py` & `opb-32/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `opb-31/test/test_inherit.py` & `opb-32/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `opb-31/test/test_objects.py` & `opb-32/test/test_objects.py`

 * *Files identical despite different names*

