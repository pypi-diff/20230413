# Comparing `tmp/FlipperNested-1.8.5.tar.gz` & `tmp/FlipperNested-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.8.5.tar", last modified: Wed Apr 12 17:24:05 2023, max compression
+gzip compressed data, was "FlipperNested-1.9.0.tar", last modified: Thu Apr 13 18:37:40 2023, max compression
```

## Comparing `FlipperNested-1.8.5.tar` & `FlipperNested-1.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:05.871158 FlipperNested-1.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:05.867157 FlipperNested-1.8.5/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:05.871158 FlipperNested-1.8.5/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:05.871158 FlipperNested-1.8.5/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 17:24:05.000000 FlipperNested-1.8.5/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-12 17:24:05.000000 FlipperNested-1.8.5/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:24:05.000000 FlipperNested-1.8.5/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 17:24:05.000000 FlipperNested-1.8.5/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 17:24:05.000000 FlipperNested-1.8.5/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 17:24:05.000000 FlipperNested-1.8.5/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:05.871158 FlipperNested-1.8.5/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 17:24:05.871158 FlipperNested-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:24:05.871158 FlipperNested-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:05.871158 FlipperNested-1.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 17:23:57.000000 FlipperNested-1.8.5/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.083426 FlipperNested-1.9.0/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.083426 FlipperNested-1.9.0/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.083426 FlipperNested-1.9.0/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/tests/test_parse.py
```

### Comparing `FlipperNested-1.8.5/FlipperNested/bridge.py` & `FlipperNested-1.9.0/FlipperNested/bridge.py`

 * *Files 8% similar despite different names*

```diff
@@ -168,9 +168,23 @@
                 break
 
         self._rpc_read_answer()
 
     def file_delete(self, path=None):
         cmd_data = storage_pb2.DeleteRequest()
         cmd_data.path = path
+        cmd_data.recursive = True
 
         self._rpc_send_and_read_answer(cmd_data, "storage_delete_request")
+
+    def mkdir(self, path="/ext"):
+        cmd_data = storage_pb2.MkdirRequest()
+        cmd_data.path = path
+
+        rep_data = self._rpc_send_and_read_answer(cmd_data, "storage_mkdir_request")
+
+    def file_rename(self, old, new):
+        cmd_data = storage_pb2.RenameRequest()
+        cmd_data.old_path = old
+        cmd_data.new_path = new
+
+        self._rpc_send_and_read_answer(cmd_data, "storage_rename_request")
```

### Comparing `FlipperNested-1.8.5/FlipperNested/cli.py` & `FlipperNested-1.9.0/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/FlipperNested/main.py` & `FlipperNested-1.9.0/FlipperNested/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 def wrapper(queue, *args):
     queue.put(FlipperNested.calculate_keys(*args))
 
 
 class FlipperNested:
     VERSION = 2
     DEPTH_VALUES = {1: 25, 2: 50, 3: 100}
-    FLIPPER_PATH = "/ext/nfc/nested/"
+    FLIPPER_PATH = "/ext/nfc/.nested/"
+    LEGACY_PATH = "/ext/nfc/nested/"
 
     def __init__(self):
         self.connection = None
         self.filename = None
         self.nonces = None
         self.found_keys = None
         self.bruteforce_distance = [0, 0]
@@ -43,29 +44,29 @@
         lines = contents.splitlines()[1:]
         version_string = lines.pop(0)
         if "Version" not in version_string:
             print("No version info in", self.filename)
             return False
         file_version = int(version_string.split(": ")[1])
         if file_version != self.VERSION:
-            print("Invalid version for", self.filename)
-            print("You should update " + "app" if file_version < self.VERSION else "recovery script")
+            print("[!!!] Invalid version for", self.filename)
+            print("[!] You should update " + "app" if file_version < self.VERSION else "recovery script")
             return False
         if "Nested: Delay" in contents:
-            print("[Warning] Nested attack with delay was used, will try more PRNG values (will take more time)")
+            print("[!] Nested attack with delay was used, will try more PRNG values (will take more time)")
             result = re.search(r"Nested: Delay [0-9]*, distance ([0-9]*)", contents.strip())
-            print("[Info] Please select depth of check")
+            print("[?] Please select depth of check")
             print("[1] Fast: +-25 values")
             print("[2] Normal: +-50 values")
             print("[3] Full: +-100 values [Recommended, ~2Gb RAM usage]")
             print("[-] Custom [..any other value..]")
             depth = int(input("[1-3/custom] > "))
             distance = int(result.groups()[0])
             if depth < 1:
-                print("Invalid input, using Normal depth")
+                print("[!] Invalid input, using Normal depth")
                 depth = 2
             if depth < 4:
                 self.bruteforce_distance = [distance - self.DEPTH_VALUES[depth], distance + self.DEPTH_VALUES[depth]]
             else:
                 self.bruteforce_distance = [distance - depth, distance + depth]
             lines.pop()
         for line in lines:
@@ -73,45 +74,57 @@
             sec, key_type = values[-2:]
             if not sec in self.nonces[key_type].keys():
                 self.nonces[key_type][sec] = []
             self.nonces[key_type][sec].append(values)
         return len(self.nonces["A"]) + len(self.nonces["B"]) > 0
 
     def extract_nonces_from_flipper(self):
+        self.check_legacy_folder()
         for file in self.connection.get_files(self.FLIPPER_PATH[:-1]):
             if file["name"].endswith(".nonces"):
                 if self.uid:
                     if file["name"].split(".")[0] != self.uid.upper():
                         continue
                 self.filename = file["name"]
-                print("Checking", file["name"])
+                print("[?] Checking", file["name"])
                 contents = self.connection.file_read(self.FLIPPER_PATH + file["name"]).decode()
                 if not self.parse_file(contents):
-                    print("Failed to parse", file["name"])
+                    print("[!] Failed to parse", file["name"])
                     continue
                 if self.save:
                     open(file["name"], "w+").write(contents)
-                    print("Saved nonces to", file["name"])
+                    print("[?] Saved nonces to", file["name"])
                 if self.recover_keys():
                     break
                 self.save_keys_to_flipper()
 
     def extract_nonces_from_file(self, file):
         self.filename = file.name
         if not self.parse_file(file.read()):
-            print("Failed to parse", self.filename)
+            print("[!] Failed to parse", self.filename)
             return
         self.recover_keys()
         self.save_keys_to_file()
 
+    def check_legacy_folder(self):
+        files = self.connection.get_files(self.LEGACY_PATH[:-1])
+        if len(files):
+            print("[!!!] Found files in legacy folder", self.LEGACY_PATH)
+            self.connection.mkdir(self.FLIPPER_PATH[:-1])
+            for file in files:
+                self.connection.file_rename(self.LEGACY_PATH + file['name'], self.FLIPPER_PATH + file['name'])
+            print("[!] Moved {} files to new directory".format(len(files)))
+            print("[!] You MUST update app to version 1.1.0 or you won't be able to check keys")
+            self.connection.file_delete(self.LEGACY_PATH[:-1])
+
     def recover_keys(self):
         for key_type in self.nonces.keys():
             for sector in self.nonces[key_type].keys():
                 for info in self.nonces[key_type][sector]:
-                    print("Recovering key type", key_type + ", sector", sector)
+                    print("[?] Recovering key type", key_type + ", sector", sector)
                     m = Manager()
                     q = m.Queue()
 
                     value = info[:-2]
                     value.append(self.bruteforce_distance)
                     value.append(self.progress_bar)
                     value.insert(0, q)
@@ -125,66 +138,66 @@
                         print("Stopping...")
                         p.kill()
                         return True
 
                     try:
                         keys = q.get(timeout=1).split(";")
                     except _queue.Empty:
-                        print("Something went VERY wrong in key recovery.\nYou MUST report this to developer!")
+                        print("[!!!] Something went VERY wrong in key recovery.\nYou MUST report this to developer!")
                         return
                     keys.pop()
 
                     print(f"Found {str(len(keys))} key(s):", keys)
 
                     if keys:
                         self.found_keys[key_type][sector] = keys
                         break
                     elif info == self.nonces[key_type][sector][-1]:
-                        print("Failed to find keys for this sector, try running Nested attack again")
+                        print("[!] Failed to find keys for this sector, try running Nested attack again")
 
     def save_keys_to_string(self):
         output = ""
         for key_type in self.found_keys.keys():
             for sector in self.found_keys[key_type].keys():
                 for key in self.found_keys[key_type][sector]:
                     output += f"Key {key_type} sector {str(sector).zfill(2)}: " + " ".join(
                         [key.upper()[i:i + 2] for i in range(0, len(key), 2)]) + "\n"
 
         keys = output.count("Key")
         if keys:
-            print("Found potential {} keys, use \"Check found keys\" in app".format(keys))
+            print("[+] Found potential {} keys, use \"Check found keys\" in app".format(keys))
         return output.strip()
 
     def save_keys_to_file(self):
         output = self.save_keys_to_string()
         if not output:
-            print("No keys found!")
+            print("[-] No keys found!")
             return
         filename = self.filename + ".keys"
         open(filename, "w+").write(output)
-        print("Saved keys to", filename)
+        print("[?] Saved keys to", filename)
 
     def save_keys_to_flipper(self):
         output = self.save_keys_to_string()
         if not output:
-            print("No keys found!")
+            print("[-] No keys found!")
             return
         filename = self.filename.replace("nonces", "keys")
         if self.save:
             open(filename, "w+").write(output)
-            print("Saved keys to", filename)
+            print("[?] Saved keys to", filename)
         try:
             self.connection.file_write(self.FLIPPER_PATH + filename, output.encode())
             if not self.preserve:
                 self.connection.file_delete(self.FLIPPER_PATH + self.filename)
         except:
             if not self.save:
                 open(filename, "w+").write(output)
-                print("Lost connection to Flipper!")
-                print("Saved keys to", filename)
+                print("[!] Lost connection to Flipper!")
+                print("[?] Saved keys to", filename)
 
     @staticmethod
     def parse_line(line):
         result = re.search(
             r"Nested: Key ([A-B]) cuid (0x[0-9a-f]*) nt0 (0x[0-9a-f]*) ks0 (0x[0-9a-f]*) par0 ([0-9a-f]*) nt1 (0x[0-9a-f]*) ks1 (0x[0-9a-f]*) par1 ([0-9a-f]*) sec (\d{1,2})",
             line.strip())
         groups = result.groups()
```

### Comparing `FlipperNested-1.8.5/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-1.9.0/FlipperNested/proto/flipper_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import FlipperNested.proto.storage_pb2 as storage__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rflipper.proto\x12\x02PB\x1a\rstorage.proto\"\x07\n\x05\x45mpty\"\r\n\x0bStopSession\"\xfb\x04\n\x04Main\x12\x12\n\ncommand_id\x18\x01 \x01(\r\x12)\n\x0e\x63ommand_status\x18\x02 \x01(\x0e\x32\x11.PB.CommandStatus\x12\x10\n\x08has_next\x18\x03 \x01(\x08\x12\x1a\n\x05\x65mpty\x18\x04 \x01(\x0b\x32\t.PB.EmptyH\x00\x12\'\n\x0cstop_session\x18\x13 \x01(\x0b\x32\x0f.PB.StopSessionH\x00\x12\x37\n\x14storage_info_request\x18\x1c \x01(\x0b\x32\x17.PB_Storage.InfoRequestH\x00\x12\x39\n\x15storage_info_response\x18\x1d \x01(\x0b\x32\x18.PB_Storage.InfoResponseH\x00\x12\x37\n\x14storage_list_request\x18\x07 \x01(\x0b\x32\x17.PB_Storage.ListRequestH\x00\x12\x39\n\x15storage_list_response\x18\x08 \x01(\x0b\x32\x18.PB_Storage.ListResponseH\x00\x12\x37\n\x14storage_read_request\x18\t \x01(\x0b\x32\x17.PB_Storage.ReadRequestH\x00\x12\x39\n\x15storage_read_response\x18\n \x01(\x0b\x32\x18.PB_Storage.ReadResponseH\x00\x12\x39\n\x15storage_write_request\x18\x0b \x01(\x0b\x32\x18.PB_Storage.WriteRequestH\x00\x12;\n\x16storage_delete_request\x18\x0c \x01(\x0b\x32\x19.PB_Storage.DeleteRequestH\x00\x42\t\n\x07\x63ontent\"\x8b\x01\n\x06Region\x12\x14\n\x0c\x63ountry_code\x18\x01 \x01(\x0c\x12\x1e\n\x05\x62\x61nds\x18\x02 \x03(\x0b\x32\x0f.PB.Region.Band\x1aK\n\x04\x42\x61nd\x12\r\n\x05start\x18\x01 \x01(\r\x12\x0b\n\x03\x65nd\x18\x02 \x01(\r\x12\x13\n\x0bpower_limit\x18\x03 \x01(\x05\x12\x12\n\nduty_cycle\x18\x04 \x01(\r*\xd6\x05\n\rCommandStatus\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x10\n\x0c\x45RROR_DECODE\x10\x02\x12\x19\n\x15\x45RROR_NOT_IMPLEMENTED\x10\x03\x12\x0e\n\nERROR_BUSY\x10\x04\x12(\n$ERROR_CONTINUOUS_COMMAND_INTERRUPTED\x10\x0e\x12\x1c\n\x18\x45RROR_INVALID_PARAMETERS\x10\x0f\x12\x1b\n\x17\x45RROR_STORAGE_NOT_READY\x10\x05\x12\x17\n\x13\x45RROR_STORAGE_EXIST\x10\x06\x12\x1b\n\x17\x45RROR_STORAGE_NOT_EXIST\x10\x07\x12#\n\x1f\x45RROR_STORAGE_INVALID_PARAMETER\x10\x08\x12\x18\n\x14\x45RROR_STORAGE_DENIED\x10\t\x12\x1e\n\x1a\x45RROR_STORAGE_INVALID_NAME\x10\n\x12\x1a\n\x16\x45RROR_STORAGE_INTERNAL\x10\x0b\x12!\n\x1d\x45RROR_STORAGE_NOT_IMPLEMENTED\x10\x0c\x12\x1e\n\x1a\x45RROR_STORAGE_ALREADY_OPEN\x10\r\x12\x1f\n\x1b\x45RROR_STORAGE_DIR_NOT_EMPTY\x10\x12\x12\x18\n\x14\x45RROR_APP_CANT_START\x10\x10\x12\x1b\n\x17\x45RROR_APP_SYSTEM_LOCKED\x10\x11\x12\x19\n\x15\x45RROR_APP_NOT_RUNNING\x10\x15\x12\x17\n\x13\x45RROR_APP_CMD_ERROR\x10\x16\x12)\n%ERROR_VIRTUAL_DISPLAY_ALREADY_STARTED\x10\x13\x12%\n!ERROR_VIRTUAL_DISPLAY_NOT_STARTED\x10\x14\x12\x1d\n\x19\x45RROR_GPIO_MODE_INCORRECT\x10:\x12\x1f\n\x1b\x45RROR_GPIO_UNKNOWN_PIN_MODE\x10;B\x1d\n\x1b\x63om.flipperdevices.protobufb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rflipper.proto\x12\x02PB\x1a\rstorage.proto\"\x07\n\x05\x45mpty\"\r\n\x0bStopSession\"\xe7\x06\n\x04Main\x12\x12\n\ncommand_id\x18\x01 \x01(\r\x12)\n\x0e\x63ommand_status\x18\x02 \x01(\x0e\x32\x11.PB.CommandStatus\x12\x10\n\x08has_next\x18\x03 \x01(\x08\x12\x1a\n\x05\x65mpty\x18\x04 \x01(\x0b\x32\t.PB.EmptyH\x00\x12\'\n\x0cstop_session\x18\x13 \x01(\x0b\x32\x0f.PB.StopSessionH\x00\x12\x37\n\x14storage_info_request\x18\x1c \x01(\x0b\x32\x17.PB_Storage.InfoRequestH\x00\x12\x39\n\x15storage_info_response\x18\x1d \x01(\x0b\x32\x18.PB_Storage.InfoResponseH\x00\x12\x37\n\x14storage_list_request\x18\x07 \x01(\x0b\x32\x17.PB_Storage.ListRequestH\x00\x12\x39\n\x15storage_list_response\x18\x08 \x01(\x0b\x32\x18.PB_Storage.ListResponseH\x00\x12\x37\n\x14storage_read_request\x18\t \x01(\x0b\x32\x17.PB_Storage.ReadRequestH\x00\x12\x39\n\x15storage_read_response\x18\n \x01(\x0b\x32\x18.PB_Storage.ReadResponseH\x00\x12\x39\n\x15storage_write_request\x18\x0b \x01(\x0b\x32\x18.PB_Storage.WriteRequestH\x00\x12;\n\x16storage_delete_request\x18\x0c \x01(\x0b\x32\x19.PB_Storage.DeleteRequestH\x00\x12\x39\n\x15storage_mkdir_request\x18\r \x01(\x0b\x32\x18.PB_Storage.MkdirRequestH\x00\x12\x37\n\x14storage_stat_request\x18\x18 \x01(\x0b\x32\x17.PB_Storage.StatRequestH\x00\x12\x39\n\x15storage_stat_response\x18\x19 \x01(\x0b\x32\x18.PB_Storage.StatResponseH\x00\x12;\n\x16storage_rename_request\x18\x1e \x01(\x0b\x32\x19.PB_Storage.RenameRequestH\x00\x42\t\n\x07\x63ontent\"\x8b\x01\n\x06Region\x12\x14\n\x0c\x63ountry_code\x18\x01 \x01(\x0c\x12\x1e\n\x05\x62\x61nds\x18\x02 \x03(\x0b\x32\x0f.PB.Region.Band\x1aK\n\x04\x42\x61nd\x12\r\n\x05start\x18\x01 \x01(\r\x12\x0b\n\x03\x65nd\x18\x02 \x01(\r\x12\x13\n\x0bpower_limit\x18\x03 \x01(\x05\x12\x12\n\nduty_cycle\x18\x04 \x01(\r*\xd6\x05\n\rCommandStatus\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x10\n\x0c\x45RROR_DECODE\x10\x02\x12\x19\n\x15\x45RROR_NOT_IMPLEMENTED\x10\x03\x12\x0e\n\nERROR_BUSY\x10\x04\x12(\n$ERROR_CONTINUOUS_COMMAND_INTERRUPTED\x10\x0e\x12\x1c\n\x18\x45RROR_INVALID_PARAMETERS\x10\x0f\x12\x1b\n\x17\x45RROR_STORAGE_NOT_READY\x10\x05\x12\x17\n\x13\x45RROR_STORAGE_EXIST\x10\x06\x12\x1b\n\x17\x45RROR_STORAGE_NOT_EXIST\x10\x07\x12#\n\x1f\x45RROR_STORAGE_INVALID_PARAMETER\x10\x08\x12\x18\n\x14\x45RROR_STORAGE_DENIED\x10\t\x12\x1e\n\x1a\x45RROR_STORAGE_INVALID_NAME\x10\n\x12\x1a\n\x16\x45RROR_STORAGE_INTERNAL\x10\x0b\x12!\n\x1d\x45RROR_STORAGE_NOT_IMPLEMENTED\x10\x0c\x12\x1e\n\x1a\x45RROR_STORAGE_ALREADY_OPEN\x10\r\x12\x1f\n\x1b\x45RROR_STORAGE_DIR_NOT_EMPTY\x10\x12\x12\x18\n\x14\x45RROR_APP_CANT_START\x10\x10\x12\x1b\n\x17\x45RROR_APP_SYSTEM_LOCKED\x10\x11\x12\x19\n\x15\x45RROR_APP_NOT_RUNNING\x10\x15\x12\x17\n\x13\x45RROR_APP_CMD_ERROR\x10\x16\x12)\n%ERROR_VIRTUAL_DISPLAY_ALREADY_STARTED\x10\x13\x12%\n!ERROR_VIRTUAL_DISPLAY_NOT_STARTED\x10\x14\x12\x1d\n\x19\x45RROR_GPIO_MODE_INCORRECT\x10:\x12\x1f\n\x1b\x45RROR_GPIO_UNKNOWN_PIN_MODE\x10;B\x1d\n\x1b\x63om.flipperdevices.protobufb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flipper_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.flipperdevices.protobuf'
-  _COMMANDSTATUS._serialized_start=841
-  _COMMANDSTATUS._serialized_end=1567
+  _COMMANDSTATUS._serialized_start=1077
+  _COMMANDSTATUS._serialized_end=1803
   _EMPTY._serialized_start=36
   _EMPTY._serialized_end=43
   _STOPSESSION._serialized_start=45
   _STOPSESSION._serialized_end=58
   _MAIN._serialized_start=61
-  _MAIN._serialized_end=696
-  _REGION._serialized_start=699
-  _REGION._serialized_end=838
-  _REGION_BAND._serialized_start=763
-  _REGION_BAND._serialized_end=838
+  _MAIN._serialized_end=932
+  _REGION._serialized_start=935
+  _REGION._serialized_end=1074
+  _REGION_BAND._serialized_start=999
+  _REGION_BAND._serialized_end=1074
 # @@protoc_insertion_point(module_scope)
```

### Comparing `FlipperNested-1.8.5/FlipperNested/proto/storage_pb2.py` & `FlipperNested-1.9.0/FlipperNested/proto/storage_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rstorage.proto\x12\nPB_Storage\"x\n\x04\x46ile\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.PB_Storage.File.FileType\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"\x1d\n\x08\x46ileType\x12\x08\n\x04\x46ILE\x10\x00\x12\x07\n\x03\x44IR\x10\x01\"\x1b\n\x0bInfoRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\"7\n\x0cInfoResponse\x12\x13\n\x0btotal_space\x18\x01 \x01(\x04\x12\x12\n\nfree_space\x18\x02 \x01(\x04\"\x1b\n\x0bListRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\".\n\x0cListResponse\x12\x1e\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x10.PB_Storage.File\"\x1b\n\x0bReadRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\".\n\x0cReadResponse\x12\x1e\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x10.PB_Storage.File\"<\n\x0cWriteRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x1e\n\x04\x66ile\x18\x02 \x01(\x0b\x32\x10.PB_Storage.File\"0\n\rDeleteRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\trecursive\x18\x02 \x01(\x08\x42%\n#com.flipperdevices.protobuf.storageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rstorage.proto\x12\nPB_Storage\"x\n\x04\x46ile\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.PB_Storage.File.FileType\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04size\x18\x03 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"\x1d\n\x08\x46ileType\x12\x08\n\x04\x46ILE\x10\x00\x12\x07\n\x03\x44IR\x10\x01\"\x1b\n\x0bInfoRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\"7\n\x0cInfoResponse\x12\x13\n\x0btotal_space\x18\x01 \x01(\x04\x12\x12\n\nfree_space\x18\x02 \x01(\x04\"\x1b\n\x0bListRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\".\n\x0cListResponse\x12\x1e\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x10.PB_Storage.File\"\x1b\n\x0bReadRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\".\n\x0cReadResponse\x12\x1e\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x10.PB_Storage.File\"\x1b\n\x0bStatRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\".\n\x0cStatResponse\x12\x1e\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x10.PB_Storage.File\"\x1c\n\x0cMkdirRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\"3\n\rRenameRequest\x12\x10\n\x08old_path\x18\x01 \x01(\t\x12\x10\n\x08new_path\x18\x02 \x01(\t\"<\n\x0cWriteRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x1e\n\x04\x66ile\x18\x02 \x01(\x0b\x32\x10.PB_Storage.File\"0\n\rDeleteRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\trecursive\x18\x02 \x01(\x08\x42%\n#com.flipperdevices.protobuf.storageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'storage_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n#com.flipperdevices.protobuf.storage'
@@ -33,12 +33,20 @@
   _LISTREQUEST._serialized_end=264
   _LISTRESPONSE._serialized_start=266
   _LISTRESPONSE._serialized_end=312
   _READREQUEST._serialized_start=314
   _READREQUEST._serialized_end=341
   _READRESPONSE._serialized_start=343
   _READRESPONSE._serialized_end=389
-  _WRITEREQUEST._serialized_start=391
-  _WRITEREQUEST._serialized_end=451
-  _DELETEREQUEST._serialized_start=453
-  _DELETEREQUEST._serialized_end=501
+  _STATREQUEST._serialized_start=391
+  _STATREQUEST._serialized_end=418
+  _STATRESPONSE._serialized_start=420
+  _STATRESPONSE._serialized_end=466
+  _MKDIRREQUEST._serialized_start=468
+  _MKDIRREQUEST._serialized_end=496
+  _RENAMEREQUEST._serialized_start=498
+  _RENAMEREQUEST._serialized_end=549
+  _WRITEREQUEST._serialized_start=551
+  _WRITEREQUEST._serialized_end=611
+  _DELETEREQUEST._serialized_start=613
+  _DELETEREQUEST._serialized_end=661
 # @@protoc_insertion_point(module_scope)
```

### Comparing `FlipperNested-1.8.5/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-1.9.0/FlipperNested.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.5
+Version: 1.9.0
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.8.5/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-1.9.0/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/LICENSE.md` & `FlipperNested-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/bucketsort.c` & `FlipperNested-1.9.0/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/bucketsort.h` & `FlipperNested-1.9.0/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/crapto1.c` & `FlipperNested-1.9.0/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/crapto1.h` & `FlipperNested-1.9.0/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/crypto1.c` & `FlipperNested-1.9.0/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/library.c` & `FlipperNested-1.9.0/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/library.h` & `FlipperNested-1.9.0/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/parity.h` & `FlipperNested-1.9.0/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/progress.c` & `FlipperNested-1.9.0/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/NestedSolver/python.c` & `FlipperNested-1.9.0/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/PKG-INFO` & `FlipperNested-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.5
+Version: 1.9.0
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.8.5/README.md` & `FlipperNested-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.5/setup.py` & `FlipperNested-1.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                           libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="1.8.5",
+    version="1.9.0",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
```

### Comparing `FlipperNested-1.8.5/tests/test_calculate.py` & `FlipperNested-1.9.0/tests/test_calculate.py`

 * *Files identical despite different names*

