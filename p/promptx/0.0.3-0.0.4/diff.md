# Comparing `tmp/promptx-0.0.3.tar.gz` & `tmp/promptx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptx-0.0.3.tar", last modified: Wed Apr 12 06:18:31 2023, max compression
+gzip compressed data, was "promptx-0.0.4.tar", last modified: Thu Apr 13 19:44:31 2023, max compression
```

## Comparing `promptx-0.0.3.tar` & `promptx-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-12 06:18:31.142002 promptx-0.0.3/
--rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.3/LICENSE.md
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-12 06:18:31.142002 promptx-0.0.3/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.3/README.md
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-12 06:18:31.142002 promptx-0.0.3/promptx/
--rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.3/promptx/__init__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     5991 2023-04-12 06:16:21.000000 promptx-0.0.3/promptx/promptx.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-12 06:18:31.142002 promptx-0.0.3/promptx.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/top_level.txt
--rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-12 06:17:59.000000 promptx-0.0.3/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-12 06:18:31.142002 promptx-0.0.3/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-13 19:44:31.172291 promptx-0.0.4/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.4/LICENSE.md
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-13 19:44:31.172291 promptx-0.0.4/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.4/README.md
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-13 19:44:31.172291 promptx-0.0.4/promptx/
+-rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.4/promptx/__init__.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     5572 2023-04-13 19:42:05.000000 promptx-0.0.4/promptx/promptx.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-13 19:44:31.172291 promptx-0.0.4/promptx.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/top_level.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-13 19:42:26.000000 promptx-0.0.4/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-13 19:44:31.172291 promptx-0.0.4/setup.cfg
```

### Comparing `promptx-0.0.3/LICENSE.md` & `promptx-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.3/PKG-INFO` & `promptx-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `promptx-0.0.3/README.md` & `promptx-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.3/promptx/promptx.py` & `promptx-0.0.4/promptx/promptx.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # PromptX.  If not, see <http://www.gnu.org/licenses/>.
 
 import shlex
 import subprocess
-from typing import Optional, List
+from typing import List
 
 __all__ = [
     "PromptXError",
     "PromptXCmdError",
     "PromptXSelectError",
     "PromptX",
 ]
@@ -90,18 +90,18 @@
         # Create a basic list of command args
         self.base_cmd = shlex.split(" ".join((prompt_cmd, default_args)))
         self.temp_args = []
 
     def ask(
         self,
         options: List,
-        prompt: Optional[str] = None,
-        additional_args: Optional[str] = None,
-        select: Optional[str] = "first",
-        deliminator: Optional[str] = "\n",
+        prompt: str | None = None,
+        additional_args: str | None = None,
+        select: str = "first",
+        deliminator: str = "\n",
     ):
         """
         Ask the user to make a selection from the given options
         """
         # If check that select is properly set
         if select not in ["first", "last", "all"]:
             raise PromptXSelectError(select)
@@ -116,15 +116,15 @@
         if self.prompt_cmd == "fzf" and prompt is not None:
             cmd.append(f"--prompt={prompt}")
         elif prompt is not None:
             cmd.extend(["-p", prompt])
 
         # Start prompt_cmd with given args
         try:
-            prompt = subprocess.Popen(
+            proc = subprocess.Popen(
                 cmd,
                 universal_newlines=True,
                 stdin=subprocess.PIPE,
                 stdout=subprocess.PIPE,
                 stderr=stderr_file,
             )
         # Failed to execute constructed command
@@ -132,42 +132,32 @@
             raise PromptXError(cmd=cmd, err=err)
 
         # Reset temp_args
         self.temp_args = []
         # Create one long string similar to choice=$(printf '%s\n' "$@" | dmenu) in bash
         opts_str = deliminator.join(map(str, options))
         # Open stdin and populate choices
-        with prompt.stdin:
-            prompt.stdin.write(opts_str)
-
-        # Wait for selection
-        if prompt.wait() == 0:
-            # Process user selection
-            selection = prompt.stdout.read().rstrip().splitlines()
-            # Return the requested selection
-            if select == "first" and len(selection) > 0:
-                return selection[0]
-            elif select == "last" and len(selection) > 0:
-                return selection[-1]
-            elif len(selection) > 0:
-                return selection
-            else:
+        outs, errs = proc.communicate(input=opts_str)
+        if proc.wait() != 0:
+            # If no err return None as user hit escape
+            if errs == "":
                 return None
+            # Otherwise some error occured
+            raise PromptXError(cmd, errs)
 
-        # fzf has no error to read, return None
-        if stderr_file == None:
-            return None
-        # dmenu does print to stderr so we read it and return None
-        # unless an actual error was encountered
-        stderr = prompt.stderr.read()
-        # If no err return None as user hit escape
-        if stderr == "":
+        selection = outs.rstrip().splitlines()
+        # Return the requested selection
+        if select == "first" and len(selection) > 0:
+            return selection[0]
+        elif select == "last" and len(selection) > 0:
+            return selection[-1]
+        elif len(selection) > 0:
+            return selection
+        else:
             return None
-        # Otherwise some error occured
-        raise PromptXError(cmd, stderr)
 
     def add_args(
         self,
         additional_args: List,
         default_args: bool = False,
     ):
         """
```

### Comparing `promptx-0.0.3/promptx.egg-info/PKG-INFO` & `promptx-0.0.4/promptx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

