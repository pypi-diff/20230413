# Comparing `tmp/foliantcontrib.showcommits-1.0.3.tar.gz` & `tmp/foliantcontrib.showcommits-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliantcontrib.showcommits-1.0.3.tar", last modified: Mon Jun 27 11:27:10 2022, max compression
+gzip compressed data, was "foliantcontrib.showcommits-1.0.4.tar", last modified: Thu Apr 13 07:32:21 2023, max compression
```

## Comparing `foliantcontrib.showcommits-1.0.3.tar` & `foliantcontrib.showcommits-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:27:10.106178 foliantcontrib.showcommits-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-27 11:26:57.000000 foliantcontrib.showcommits-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-06-27 11:27:10.106178 foliantcontrib.showcommits-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-06-27 11:26:57.000000 foliantcontrib.showcommits-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:27:10.106178 foliantcontrib.showcommits-1.0.3/foliant/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:27:10.106178 foliantcontrib.showcommits-1.0.3/foliant/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (121)    12926 2022-06-27 11:26:57.000000 foliantcontrib.showcommits-1.0.3/foliant/preprocessors/showcommits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:27:10.106178 foliantcontrib.showcommits-1.0.3/foliantcontrib.showcommits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-06-27 11:27:09.000000 foliantcontrib.showcommits-1.0.3/foliantcontrib.showcommits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-06-27 11:27:10.000000 foliantcontrib.showcommits-1.0.3/foliantcontrib.showcommits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 11:27:09.000000 foliantcontrib.showcommits-1.0.3/foliantcontrib.showcommits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-27 11:27:09.000000 foliantcontrib.showcommits-1.0.3/foliantcontrib.showcommits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-27 11:27:09.000000 foliantcontrib.showcommits-1.0.3/foliantcontrib.showcommits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-27 11:27:10.106178 foliantcontrib.showcommits-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-06-27 11:26:57.000000 foliantcontrib.showcommits-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:32:21.758579 foliantcontrib.showcommits-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 07:32:12.000000 foliantcontrib.showcommits-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-13 07:32:21.758579 foliantcontrib.showcommits-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-04-13 07:32:12.000000 foliantcontrib.showcommits-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:32:21.754579 foliantcontrib.showcommits-1.0.4/foliant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:32:21.758579 foliantcontrib.showcommits-1.0.4/foliant/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-04-13 07:32:12.000000 foliantcontrib.showcommits-1.0.4/foliant/preprocessors/showcommits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:32:21.758579 foliantcontrib.showcommits-1.0.4/foliantcontrib.showcommits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-13 07:32:21.000000 foliantcontrib.showcommits-1.0.4/foliantcontrib.showcommits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-13 07:32:21.000000 foliantcontrib.showcommits-1.0.4/foliantcontrib.showcommits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:32:21.000000 foliantcontrib.showcommits-1.0.4/foliantcontrib.showcommits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 07:32:21.000000 foliantcontrib.showcommits-1.0.4/foliantcontrib.showcommits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:32:21.000000 foliantcontrib.showcommits-1.0.4/foliantcontrib.showcommits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:32:21.758579 foliantcontrib.showcommits-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 07:32:12.000000 foliantcontrib.showcommits-1.0.4/setup.py
```

### Comparing `foliantcontrib.showcommits-1.0.3/LICENSE` & `foliantcontrib.showcommits-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `foliantcontrib.showcommits-1.0.3/PKG-INFO` & `foliantcontrib.showcommits-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.showcommits
-Version: 1.0.3
+Version: 1.0.4
 Summary: ShowCommits preprocessor for Foliant.
 Home-page: https://github.com/foliant-docs/foliantcontrib.showcommits
 Author: Artemy Lomov
 Author-email: artemy@lomov.ru
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `foliantcontrib.showcommits-1.0.3/README.md` & `foliantcontrib.showcommits-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `foliantcontrib.showcommits-1.0.3/foliant/preprocessors/showcommits.py` & `foliantcontrib.showcommits-1.0.4/foliant/preprocessors/showcommits.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,15 +242,14 @@
             flags=re.MULTILINE
         )
 
         commit_diff = commit_summary.group('diff')
 
         if self.options['escape_html']:
             commit_message = self._escape_html(commit_message)
-            commit_diff = self._escape_html(commit_diff)
 
         commit_info = (
             commits_template
         ).replace(
             '{{hash}}', commit_summary.group('hash')
         ).replace(
             '{{url}}',
@@ -301,15 +300,15 @@
 
         return output_history
 
     def process_showcommits(
             self,
             markdown_content: str,
             markdown_file_path: Path,
-    ) -> str:
+        ) -> str:
         markdown_file_in_src_dir_path = (
                 self.config['src_dir'] / markdown_file_path.relative_to(self.working_dir.resolve())
         ).resolve()
 
         source_file_rel_path = markdown_file_in_src_dir_path.relative_to(self.project_path.resolve())
         source_file_abs_path = self.repo_path / source_file_rel_path
 
@@ -329,14 +328,17 @@
             self.logger.warning(warning_message)
 
             return markdown_content
 
         source_file_git_history = self.get_source_file_git_history(source_file_abs_path)
         output_history = self.get_output_history(source_file_git_history, source_file_rel_path)
 
+        if self.context['backend'] == 'hugo':
+            output_history = output_history.replace('```diff', '```diff {style=borland}')
+
         if self.options['position'] == 'after_content':
             markdown_content += '\n\n' + output_history
 
         elif self.options['position'] == 'defined_by_tag':
             markdown_content = self.pattern.sub(output_history, markdown_content)
 
         return markdown_content
```

### Comparing `foliantcontrib.showcommits-1.0.3/foliantcontrib.showcommits.egg-info/PKG-INFO` & `foliantcontrib.showcommits-1.0.4/foliantcontrib.showcommits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.showcommits
-Version: 1.0.3
+Version: 1.0.4
 Summary: ShowCommits preprocessor for Foliant.
 Home-page: https://github.com/foliant-docs/foliantcontrib.showcommits
 Author: Artemy Lomov
 Author-email: artemy@lomov.ru
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `foliantcontrib.showcommits-1.0.3/setup.py` & `foliantcontrib.showcommits-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 setup(
     name='foliantcontrib.showcommits',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    version='1.0.3',
+    version='1.0.4',
     author='Artemy Lomov',
     author_email='artemy@lomov.ru',
     url='https://github.com/foliant-docs/foliantcontrib.showcommits',
     packages=['foliant.preprocessors'],
     license='MIT',
     platforms='any',
     install_requires=[
```

