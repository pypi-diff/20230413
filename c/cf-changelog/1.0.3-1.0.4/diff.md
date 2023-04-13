# Comparing `tmp/cf_changelog-1.0.3.tar.gz` & `tmp/cf_changelog-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-y4h97m2j\cf_changelog-1.0.3.tar", last modified: Thu Apr 13 15:41:18 2023, max compression
+gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-34n6inkb\cf_changelog-1.0.4.tar", last modified: Thu Apr 13 15:47:45 2023, max compression
```

## Comparing `cf_changelog-1.0.3.tar` & `cf_changelog-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/
--rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1503 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1169 2023-04-11 21:35:22.000000 cf_changelog-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog/
--rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.3/cf_changelog/__init__.py
--rw-rw-rw-   0        0        0     6820 2023-04-13 15:39:04.000000 cf_changelog-1.0.3/cf_changelog/cf_changelog.py
-drwxrwxrwx   0        0        0        0 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog.egg-info/
--rw-rw-rw-   0        0        0     1503 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/cf_changelog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 15:41:18.000000 cf_changelog-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-04-13 15:40:24.000000 cf_changelog-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/
+-rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1503 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-04-11 21:35:22.000000 cf_changelog-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog/
+-rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.4/cf_changelog/__init__.py
+-rw-rw-rw-   0        0        0     6944 2023-04-13 15:45:53.000000 cf_changelog-1.0.4/cf_changelog/cf_changelog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog.egg-info/
+-rw-rw-rw-   0        0        0     1503 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/cf_changelog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:47:45.000000 cf_changelog-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-04-13 15:46:06.000000 cf_changelog-1.0.4/setup.py
```

### Comparing `cf_changelog-1.0.3/LICENSE` & `cf_changelog-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_changelog-1.0.3/PKG-INFO` & `cf_changelog-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_changelog
-Version: 1.0.3
+Version: 1.0.4
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cf_changelog-1.0.3/README.md` & `cf_changelog-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cf_changelog-1.0.3/cf_changelog/cf_changelog.py` & `cf_changelog-1.0.4/cf_changelog/cf_changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Leave this file unchanged to abort adding entry.
 '''
     tf = tempfile.NamedTemporaryFile(mode='w+', suffix=".yaml", encoding='utf-8', delete=False)
     tf_name = tf.name
     tf.write(initial_message)
     tf.flush()
     tf.close()
-    print("Running editor", args.editor)
+    print("Running editor:", args.editor)
     call([args.editor, tf_name])
     
     with open(tf_name, mode='r', encoding='utf-8') as f:
         edited_message = f.read()
     if edited_message == initial_message:
         print("Aborted")
         return False
@@ -77,19 +77,22 @@
             if key not in new_entries:
                 new_entries[key] = []
             new_entries[key] += values
 
     print("Got new entries", new_entries)
     new_changelog_content = "# " + args.version
     for key, values in new_entries.items():
-        new_changelog_content += "\n"
-        new_changelog_content += "## " + key + '\n'
+        header_printed = False
         for value  in values:
             if not value:
                 continue
+            if not header_printed:
+                new_changelog_content += "\n"
+                new_changelog_content += "## " + key + '\n'
+                header_printed = True
             new_changelog_content += "- " + value + '\n'
     new_changelog_content += "\n"
     changelog_content = ""
     if os.path.isfile(args.changelog_file):
         with open(args.changelog_file, mode='r', encoding='utf-8') as f:
             changelog_content = f.read()
     changelog_content = new_changelog_content + changelog_content
```

### Comparing `cf_changelog-1.0.3/cf_changelog.egg-info/PKG-INFO` & `cf_changelog-1.0.4/cf_changelog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-changelog
-Version: 1.0.3
+Version: 1.0.4
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cf_changelog-1.0.3/setup.py` & `cf_changelog-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='cf_changelog',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version='1.0.3',
+      version='1.0.4',
       description='Conflict-Free Changelog manager',
       author='Paweł Sałek',
       author_email='salekpawel@gmail.com',
       url='https://gitlab.com/salekpawel/cf_changelog',
       packages=['cf_changelog', ],
       license="MIT",
       install_requires=[
```

