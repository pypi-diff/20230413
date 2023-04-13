# Comparing `tmp/me_setups-1.6.5.tar.gz` & `tmp/me_setups-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.6.5.tar", last modified: Tue Apr  4 19:47:08 2023, max compression
+gzip compressed data, was "me_setups-1.6.6.tar", last modified: Thu Apr 13 08:33:36 2023, max compression
```

## Comparing `me_setups-1.6.5.tar` & `me_setups-1.6.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-04 19:47:08.061246 me_setups-1.6.5/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-04 19:47:08.062245 me_setups-1.6.5/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.6.5/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1192 2023-04-04 19:47:08.063872 me_setups-1.6.5/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.6.5/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-04 19:47:08.015214 me_setups-1.6.5/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-04 19:47:08.029190 me_setups-1.6.5/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.6.5/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-04 19:47:08.049862 me_setups-1.6.5/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.6.5/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.6.5/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    10534 2023-04-04 16:39:15.000000 me_setups-1.6.5/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.6.5/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-04 19:47:08.061041 me_setups-1.6.5/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.6.5/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8546 2023-04-04 19:45:41.000000 me_setups-1.6.5/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11871 2023-04-04 16:39:15.000000 me_setups-1.6.5/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      178 2023-02-20 11:40:34.000000 me_setups-1.6.5/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4047 2023-02-27 18:33:55.000000 me_setups-1.6.5/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.6.5/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-04 19:47:08.041243 me_setups-1.6.5/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-04 19:47:07.000000 me_setups-1.6.5/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-04-04 19:47:07.000000 me_setups-1.6.5/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-04-04 19:47:07.000000 me_setups-1.6.5/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-04-04 19:47:07.000000 me_setups-1.6.5/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-04-04 19:47:07.000000 me_setups-1.6.5/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-13 08:33:36.648498 me_setups-1.6.6/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-13 08:33:36.649438 me_setups-1.6.6/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.6.6/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1192 2023-04-13 08:33:36.651401 me_setups-1.6.6/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.6.6/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-13 08:33:36.610492 me_setups-1.6.6/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-13 08:33:36.620147 me_setups-1.6.6/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.6.6/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-13 08:33:36.639353 me_setups-1.6.6/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.6.6/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.6.6/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    10534 2023-04-04 16:39:15.000000 me_setups-1.6.6/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.6.6/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-13 08:33:36.647476 me_setups-1.6.6/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.6.6/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8629 2023-04-13 08:32:16.000000 me_setups-1.6.6/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11846 2023-04-13 08:32:16.000000 me_setups-1.6.6/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      178 2023-02-20 11:40:34.000000 me_setups-1.6.6/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4047 2023-02-27 18:33:55.000000 me_setups-1.6.6/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.6.6/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-04-13 08:33:36.630371 me_setups-1.6.6/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-04-13 08:33:36.000000 me_setups-1.6.6/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-04-13 08:33:36.000000 me_setups-1.6.6/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-04-13 08:33:36.000000 me_setups-1.6.6/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-04-13 08:33:36.000000 me_setups-1.6.6/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-04-13 08:33:36.000000 me_setups-1.6.6/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.6.5/PKG-INFO` & `me_setups-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.6.5
+Version: 1.6.6
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.5/setup.cfg` & `me_setups-1.6.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.6.5
+version = 1.6.6
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.6.5/src/me_setups/boards/default_boards.py` & `me_setups-1.6.6/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.5/src/me_setups/boards/gas52.py` & `me_setups-1.6.6/src/me_setups/boards/gas52.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.5/src/me_setups/components/comp.py` & `me_setups-1.6.6/src/me_setups/components/comp.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,34 +82,36 @@
 
         Args:
             serial (Serial): serial port to read.
         """
         super().__init__(*args, **kwargs)
         self.daemon = True
         self.serial = serial
+        self.alive = threading.Event()
 
     def stop(self) -> None:
         """\
             Stop sniffing
         """
-        self.alive = False
+        self.alive.clear()
         self.join(5)
 
     def run(self) -> None:
-        self.alive = True
-        while self.alive and self.serial.is_open:
+        self.alive.set()
+        while self.alive.is_set() and self.serial.is_open:
             try:
                 self.serial.read(self.serial.in_waiting or 1)
             except SerialException:
                 break
             except OSError:
                 self.serial.close()
                 self.serial.open()
                 self.serial.read(self.serial.in_waiting or 1)
-        self.alive = False
+        if self.alive.is_set():
+            self.alive.clear()
 
     def __enter__(self) -> ReaderThread:
         self.start()
         return self
 
     def __exit__(
         self,
```

### Comparing `me_setups-1.6.5/src/me_setups/components/eqs.py` & `me_setups-1.6.6/src/me_setups/components/eqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     def get_all_frames(self) -> list[str]:
         """get all frames ran from the app_log
 
         Returns:
             list[str]: list contain all frames that ran
         """
         frames_string = "running frame:"
-        pat = re.compile(rf"{frames_string} (\d+)", re.IGNORECASE)
+        pat = re.compile(rf"{frames_string} (\d+)\n", re.IGNORECASE)
         stdout = self.ssh_cmd_stdout(
             f"grep -i {frames_string!r} /tmp/app_log.txt",
             skip_logging=True,
         )
         return pat.findall(stdout)
 
     def wait_for_frames(
@@ -246,17 +246,16 @@
         Returns:
             bool: if we got the given number of frames
         """
         _timeout = time.time() + timeout
         all_frames = []
         while time.time() < _timeout:
             all_frames = self.get_all_frames()
-            if all_frames:
-                self.logger.debug(f"last frame is: {all_frames[-1]}")
             if len(all_frames) > frames:
+                self.logger.debug(f"last frame is: {all_frames[-1]}")
                 return True
 
         self.logger.warning(f"did not run {frames} frames. frames got={all_frames}")
         return False
 
     def is_mest_alive(self) -> bool:
         """Return if MEST is alive"""
```

### Comparing `me_setups-1.6.5/src/me_setups/components/mcu.py` & `me_setups-1.6.6/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.6.5/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.6.6/src/me_setups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.6.5
+Version: 1.6.6
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.6.5/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.6.6/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

