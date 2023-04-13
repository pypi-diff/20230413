# Comparing `tmp/kiauto-2.2.3.tar.gz` & `tmp/kiauto-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiauto-2.2.3.tar", last modified: Thu Apr  6 19:05:49 2023, max compression
+gzip compressed data, was "kiauto-2.2.4.tar", last modified: Thu Apr 13 14:15:04 2023, max compression
```

## Comparing `kiauto-2.2.3.tar` & `kiauto-2.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:05:49.381743 kiauto-2.2.3/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-06 19:04:40.000000 kiauto-2.2.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       67 2023-04-06 19:04:40.000000 kiauto-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17079 2023-04-06 19:05:49.381743 kiauto-2.2.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    13874 2023-04-06 19:04:40.000000 kiauto-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:05:49.377743 kiauto-2.2.3/kiauto/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-06 19:04:40.000000 kiauto-2.2.3/kiauto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14772 2023-04-06 19:04:40.000000 kiauto-2.2.3/kiauto/file_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:05:49.381743 kiauto-2.2.3/kiauto/interposer/
--rwxrwxr-x   0 root         (0) root         (0)    27344 2023-04-06 19:04:40.000000 kiauto-2.2.3/kiauto/interposer/libinterposer.so
--rw-rw-r--   0 root         (0) root         (0)    27535 2023-04-06 19:04:40.000000 kiauto-2.2.3/kiauto/interposer.py
--rw-rw-r--   0 root         (0) root         (0)     3755 2023-04-06 19:04:40.000000 kiauto-2.2.3/kiauto/log.py
--rw-rw-r--   0 root         (0) root         (0)    13108 2023-04-06 19:04:40.000000 kiauto-2.2.3/kiauto/misc.py
--rw-rw-r--   0 root         (0) root         (0)    18923 2023-04-06 19:04:40.000000 kiauto-2.2.3/kiauto/ui_automation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:05:49.377743 kiauto-2.2.3/kiauto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17079 2023-04-06 19:05:49.000000 kiauto-2.2.3/kiauto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-06 19:05:49.000000 kiauto-2.2.3/kiauto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 19:05:49.000000 kiauto-2.2.3/kiauto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-06 19:05:49.000000 kiauto-2.2.3/kiauto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-06 19:05:49.000000 kiauto-2.2.3/kiauto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 19:05:49.381743 kiauto-2.2.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1410 2023-04-06 19:04:40.000000 kiauto-2.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 19:05:49.381743 kiauto-2.2.3/src/
--rwxrwxr-x   0 root         (0) root         (0)    40519 2023-04-06 19:04:40.000000 kiauto-2.2.3/src/eeschema_do
--rwxrwxr-x   0 root         (0) root         (0)     6979 2023-04-06 19:04:40.000000 kiauto-2.2.3/src/kicad2step_do
--rwxrwxr-x   0 root         (0) root         (0)    75176 2023-04-06 19:04:40.000000 kiauto-2.2.3/src/pcbnew_do
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-12 16:15:23.000000 kiauto-2.2.4/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-04-12 16:15:23.000000 kiauto-2.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-04-13 14:15:04.587207 kiauto-2.2.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    13874 2023-04-12 16:15:23.000000 kiauto-2.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/kiauto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14848 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/kiauto/interposer/
+-rwxrwxr-x   0 root         (0) root         (0)    27344 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/interposer/libinterposer.so
+-rw-rw-r--   0 root         (0) root         (0)    27969 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/interposer.py
+-rw-rw-r--   0 root         (0) root         (0)     3755 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/log.py
+-rw-rw-r--   0 root         (0) root         (0)    14310 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    18923 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/ui_automation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/kiauto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 14:15:04.587207 kiauto-2.2.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1410 2023-04-12 16:15:23.000000 kiauto-2.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/src/
+-rwxrwxr-x   0 root         (0) root         (0)    40781 2023-04-12 16:15:23.000000 kiauto-2.2.4/src/eeschema_do
+-rwxrwxr-x   0 root         (0) root         (0)     6979 2023-04-12 16:15:23.000000 kiauto-2.2.4/src/kicad2step_do
+-rwxrwxr-x   0 root         (0) root         (0)    75176 2023-04-12 16:15:23.000000 kiauto-2.2.4/src/pcbnew_do
```

### Comparing `kiauto-2.2.3/LICENSE` & `kiauto-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.3/PKG-INFO` & `kiauto-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.3
+Version: 2.2.4
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.3/README.md` & `kiauto-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.3/kiauto/file_util.py` & `kiauto-2.2.4/kiauto/file_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,18 +159,19 @@
     if os.path.isfile(fname):
         logger.debug('Removing '+fname)
         os.remove(fname)
 
 
 def check_lib_table(fuser, fsys):
     if not os.path.isfile(fuser):
-        logger.debug('Missing default sym-lib-table')
+        logger.debug('Missing default '+os.path.basename(fuser))
         for f in fsys:
             if os.path.isfile(f):
                 shutil.copy2(f, fuser)
+                logger.debug('Copied {} to {}'.format(f, fuser))
                 return
         logger.warning('Missing default system symbol table '+fsys[0] +
                        ' creating an empty one')  # pragma: no cover
         with open(fuser, 'wt') as f:
             f.write('({} )\n'.format(os.path.basename(fuser).replace('-', '_')))
         atexit.register(remove_lib_table, fuser)
```

### Comparing `kiauto-2.2.3/kiauto/interposer/libinterposer.so` & `kiauto-2.2.4/kiauto/interposer/libinterposer.so`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.3/kiauto/interposer.py` & `kiauto-2.2.4/kiauto/interposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,40 +337,48 @@
         fn = cfg.output_file
     os.environ['KIAUTO_INTERPOSER_FILENAME'] = fn
     if os.path.isfile(BOGUS_FILENAME):
         cfg.logger.warning('Removing bogus file `{}`'.format(BOGUS_FILENAME))
         os.remove(BOGUS_FILENAME)
 
 
-def send_keys(cfg, msg, keys, closes=None, delay_io=False):
+def send_keys(cfg, msg, keys, closes=None, delay_io=False, no_destroy=False):
     cfg.logger.info(msg)
     wait_point(cfg)
     if isinstance(keys, str):
         keys = ['key', keys]
     if delay_io:
         collect_io_from_queue(cfg)
     xdotool(keys)
     if closes is not None:
-        if isinstance(closes, str):
-            closes = [closes]
-        for w in closes:
-            wait_queue(cfg, 'GTK:Window Destroy:'+w)
+        if no_destroy:
+            wait_close_dialog_i(cfg)
+        else:
+            if isinstance(closes, str):
+                closes = [closes]
+            for w in closes:
+                try:
+                    wait_queue(cfg, 'GTK:Window Destroy:'+w, dialog_interrupts=True)
+                except InterruptedError:
+                    # KiCad 7.99
+                    xdotool(keys)
         wait_kicad_ready_i(cfg)
 
 
-def wait_create_i(cfg, name, fn=None):
+def wait_create_i(cfg, name, fn=None, forced_ext=None):
     """ Wait for open+close of the file.
         Also look for them in the collected_io messages.
         And if we just get close forget about the open. """
     cfg.logger.info('Wait for '+name+' file creation')
     wait_point(cfg)
     if fn is None:
         fn = cfg.output_file
-    open_msg = 'IO:open:'+fn
-    close_msg = 'IO:close:'+fn
+    fn_kicad = fn+'.'+forced_ext if forced_ext and cfg.ki8 else fn
+    open_msg = 'IO:open:'+fn_kicad
+    close_msg = 'IO:close:'+fn_kicad
     if cfg.collecting_io:
         cfg.collecting_io = False
         got_open = open_msg in cfg.collected_io
         got_close = close_msg in cfg.collected_io
     else:
         got_open = False
         got_close = False
@@ -381,14 +389,16 @@
         msg = wait_queue(cfg, [open_msg, close_msg], starts=True)
         got_close = msg.startswith(close_msg)
     if got_close:
         cfg.logger.debug('Found IO '+close_msg)
     else:
         wait_queue(cfg, close_msg, starts=True)
     wait_kicad_ready_i(cfg)
+    if forced_ext and cfg.ki8 and os.path.isfile(fn_kicad):
+        os.rename(fn_kicad, fn)
 
 
 def collect_dialog_messages(cfg, title):
     cfg.logger.info(title+' dialog found ...')
     cfg.logger.debug('Gathering potential dialog content')
     msgs = set()
     for msg in range(12):
@@ -584,19 +594,19 @@
             cfg.logger.warning("Retrying KiCad exit")
         # Wait until KiCad is sleeping again
         wait_kicad_ready_i(cfg, kicad_can_exit=True)
         # Retry the exit
         xdotool(['key', 'ctrl+q'])
 
 
-# def wait_close_dialog_i(cfg):
-#     """ Wait for the end of the main loop for the dialog.
-#         Then the main loop for the parent exits and enters again. """
-#     wait_queue(cfg, 'GTK:Main:Out', times=2)
-#     wait_queue(cfg, 'GTK:Main:In')
+def wait_close_dialog_i(cfg):
+    """ Wait for the end of the main loop for the dialog.
+        Then the main loop for the parent exits and enters again. """
+    wait_queue(cfg, 'GTK:Main:Out')
+    wait_queue(cfg, 'GTK:Main:In')
 
 
 def wait_and_show_progress(cfg, msg, regex_str, trigger, msg_reg, skip_match=None, with_windows=False):
     """ msg: The message we are waiting
         regex_str: A regex to extract the progress message (text after PANGO:)
         trigger: A text that must be start at the beginning to test using the regex (PANGO:trigger)
         msg_reg: Message to print before the info (msg_reg: MATCH)
```

### Comparing `kiauto-2.2.3/kiauto/log.py` & `kiauto-2.2.4/kiauto/log.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.3/kiauto/misc.py` & `kiauto-2.2.4/kiauto/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 # Name for testing versions
 NIGHTLY = 'nightly'
 # Scale factor for the timeouts
 TIME_OUT_MULT = 1.0
 
 KICAD_VERSION_5_99 = 5099000
 KICAD_VERSION_6_99 = 6099000
+KICAD_VERSION_7_99 = 7099000
 KICAD_SHARE = '/usr/share/kicad/'
 KICAD_NIGHTLY_SHARE = '/usr/share/kicad-nightly/'
 
 
 @contextmanager
 def hide_stderr():
     """ Low level stderr supression, used to hide KiCad bugs. """
@@ -121,18 +122,14 @@
             self.pcbnew += '-'+NIGHTLY
             self.kicad2step += '-'+NIGHTLY
             self.kicad_cli += '-'+NIGHTLY
             self.kicad_conf_dir += os.path.join(NIGHTLY, ng_ver)
             # Path to the Python module
             path.insert(0, '/usr/lib/kicad-nightly/lib/python3/dist-packages')
             os.environ['KICAD_PATH'] = '/usr/share/kicad-nightly'
-            # KiCad 7.0.0 rc2 workaround
-            # KiCad bug: https://gitlab.com/kicad/code/kicad/-/issues/13815
-            v = ng_ver[0]
-            os.environ['KICAD'+v+'_FOOTPRINT_DIR'] = '/usr/share/kicad-nightly/footprints'
         # Detect KiCad version
         try:
             import pcbnew
         except ImportError:
             logger.error("Failed to import pcbnew Python module."
                          " Is KiCad installed?"
                          " Do you need to add it to PYTHONPATH?")
@@ -151,16 +148,17 @@
         self.kicad_version_major = int(m.group(1))
         self.kicad_version_minor = int(m.group(2))
         self.kicad_version_patch = int(m.group(3))
         self.kicad_version = self.kicad_version_major*1000000+self.kicad_version_minor*1000+self.kicad_version_patch
         logger.debug('Detected KiCad v{}.{}.{} ({} {})'.format(self.kicad_version_major, self.kicad_version_minor,
                      self.kicad_version_patch, kicad_version, self.kicad_version))
         self.ki5 = self.kicad_version < KICAD_VERSION_5_99
-        self.ki6 = not self.ki5 and self.kicad_version < KICAD_VERSION_6_99
-        self.ki7 = not self.ki5 and not self.ki6
+        self.ki6 = self.kicad_version >= KICAD_VERSION_5_99
+        self.ki7 = self.kicad_version >= KICAD_VERSION_6_99
+        self.ki8 = self.kicad_version >= KICAD_VERSION_7_99
         if self.ki7:
             # Now part of the kicad-cli tool
             self.kicad2step = self.kicad_cli
             self.drc_dialog_name = 'Design Rules Checker'
         else:
             self.drc_dialog_name = 'DRC Control'
         # Config file names
@@ -182,14 +180,15 @@
         self.conf_kicad_bkp = None
         if not self.ki5:
             self.conf_kicad += '.json'
             self.conf_kicad_json = True
         else:
             self.conf_kicad_json = False
         # Read the environment redefinitions used by KiCad
+        self.env = {}
         if os.path.isfile(self.conf_kicad):
             self.load_kicad_environment(logger)
             if 'KICAD_CONFIG_HOME' in self.env and self.ki5:
                 # The user is redirecting the configuration
                 # KiCad 5 unintentionally allows it, is a bug, and won't be fixed:
                 # https://forum.kicad.info/t/kicad-config-home-inconsistencies-and-detail/26875
                 self.kicad_conf_path = self.env['KICAD_CONFIG_HOME']
@@ -221,32 +220,58 @@
             self.pro_ext = 'pro'
             self.prl_ext = None
             self.conf_colors = self.conf_colors_bkp = None
             self.conf_3dview = self.conf_3dview_bkp = None
         # - hotkeys
         self.conf_hotkeys = os.path.join(self.kicad_conf_path, 'user.hotkeys')
         self.conf_hotkeys_bkp = None
+        # share path
+        kpath = os.environ.get('KICAD_PATH')
+        if kpath is None and self.env:
+            kpath = self.env.get('KICAD_PATH')
+        if kpath is None:
+            if os.path.isdir(KICAD_SHARE):
+                kpath = KICAD_SHARE
+            elif os.path.isdir(KICAD_NIGHTLY_SHARE):
+                kpath = KICAD_NIGHTLY_SHARE
+        if kpath is None:
+            logger.warning('Missing KiCad share dir')
+        else:
+            logger.debug('KiCad share dir: '+kpath)
+            vname = 'KICAD'+str(self.kicad_version_major)+'_FOOTPRINT_DIR'
+            # KiCad 7.0.0 rc2 workaround (also 7.0.1 and 7.99 april 2023)
+            # KiCad bug: https://gitlab.com/kicad/code/kicad/-/issues/13815
+            if vname not in os.environ:
+                # Footprint dir not defined, and needed for DRC
+                if self.env and vname in self.env:
+                    os.environ[vname] = self.env[vname]
+                else:
+                    os.environ[vname] = os.path.join(kpath, 'footprints')
+                logger.debug('Defining {} = {}'.format(vname, os.environ[vname]))
         # - sym-lib-table
         self.user_sym_lib_table = os.path.join(self.kicad_conf_path, 'sym-lib-table')
         self.user_fp_lib_table = os.path.join(self.kicad_conf_path, 'fp-lib-table')
         self.sys_sym_lib_table = [KICAD_SHARE+'template/sym-lib-table']
         self.sys_fp_lib_table = [KICAD_SHARE+'template/fp-lib-table']
         if ng_ver:
             # 20200912: sym-lib-table is missing
             self.sys_sym_lib_table.insert(0, KICAD_NIGHTLY_SHARE+'template/sym-lib-table')
             self.sys_fp_lib_table.insert(0, KICAD_NIGHTLY_SHARE+'template/fp-lib-table')
+        if kpath is not None:
+            self.sys_sym_lib_table.insert(0, os.path.join(kpath, 'template/sym-lib-table'))
+            self.sys_fp_lib_table.insert(0, os.path.join(kpath, 'template/fp-lib-table'))
         # Some details about the UI
         if not self.ki5:
             # KiCad 5.99.0
             # self.ee_window_title = r'\[.*\] — Eeschema$'  # "PROJECT [HIERARCHY_PATH] - Eeschema"
-            # KiCad 6.x
-            if self.ki6:
-                self.ee_window_title = r'\[.*\] — Schematic Editor$'  # "PROJECT [HIERARCHY_PATH] - Schematic Editor"
-            else:
+            if self.ki7:
                 self.ee_window_title = r'.* — Schematic Editor$'  # "SHEET [HIERARCHY_PATH]? - Schematic Editor"
+            else:
+                # KiCad 6.x
+                self.ee_window_title = r'\[.*\] — Schematic Editor$'  # "PROJECT [HIERARCHY_PATH] - Schematic Editor"
             self.pn_window_title = r'.* — PCB Editor$'  # "PROJECT - PCB Editor"
             self.pn_simple_window_title = 'PCB Editor'
             kind = 'PCB' if self.is_pcbnew else 'Schematic'
             self.window_title_end = ' — '+kind+' Editor'
         else:
             # KiCad 5.1.6
             self.ee_window_title = r'Eeschema.*\.sch'  # "Eeschema - file.sch"
@@ -314,8 +339,8 @@
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2018-2023, INTI/Productize SPRL'
 __credits__ = ['Salvador E. Tropea', 'Seppe Stas', 'Jesse Vincent', 'Scott Bezek']
 __license__ = 'Apache 2.0'
 __email__ = 'stropea@inti.gob.ar'
 __status__ = 'stable'
 __url__ = 'https://github.com/INTI-CMNB/KiAuto/'
-__version__ = '2.2.3'
+__version__ = '2.2.4'
```

### Comparing `kiauto-2.2.3/kiauto/ui_automation.py` & `kiauto-2.2.4/kiauto/ui_automation.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.3/kiauto.egg-info/PKG-INFO` & `kiauto-2.2.4/kiauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.3
+Version: 2.2.4
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.3/setup.py` & `kiauto-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.3/src/eeschema_do` & `kiauto-2.2.4/src/eeschema_do`

 * *Files 1% similar despite different names*

```diff
@@ -441,29 +441,32 @@
     # Close the ERC dialog
     logger.info('Exit ERC')
     wait_point(cfg)
     xdotool(['key', 'Escape'])
 
 
 def eeschema_run_erc_schematic_6_0_i(cfg):
+    # KiCad 7.99 particularities:
+    # 1. Forces ".rpt" in the name, no matter what name was selected in the dialog and no matter if it already has an extension
+    # 2. The ERC dialog isn't destroyed, most probably hidden
     # Open the ERC dialog
     dialog, _ = open_dialog_i(cfg, 'Electrical Rules Checker', 'ctrl+shift+i', no_main=True)
     # Run the ERC
     send_keys(cfg, 'Run ERC', 'Return')
     # Wait for completion. The Close button is refreshed at the end
     wait_queue(cfg, 'GTK:Button Label:C_lose')
     # Save the report
     file_dlg, _ = open_dialog_i(cfg, 'Save Report to File', 'alt+s')
     # Paste the output file
     paste_bogus_filename(cfg)
     send_keys(cfg, 'Create the report', 'Return', closes=file_dlg, delay_io=True)
     # Wait until created
-    wait_create_i(cfg, 'ERC')
+    wait_create_i(cfg, 'ERC', forced_ext='rpt')
     # Close the ERC dialog
-    send_keys(cfg, 'Exit ERC', 'Escape', closes=dialog)
+    send_keys(cfg, 'Exit ERC', 'Escape', closes=dialog, no_destroy=cfg.ki8)
 
 
 def eeschema_run_erc_schematic(cfg):
     if cfg.ki5:
         if cfg.use_interposer:
             eeschema_run_erc_schematic_5_1_i(cfg)
         else:
```

### Comparing `kiauto-2.2.3/src/kicad2step_do` & `kiauto-2.2.4/src/kicad2step_do`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.3/src/pcbnew_do` & `kiauto-2.2.4/src/pcbnew_do`

 * *Files identical despite different names*

