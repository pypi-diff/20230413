# Comparing `tmp/lupin-grognard-1.9.0.dev8.tar.gz` & `tmp/lupin-grognard-1.9.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-1.9.0.dev8.tar", last modified: Thu Mar  9 17:24:12 2023, max compression
+gzip compressed data, was "lupin-grognard-1.9.0.dev9.tar", last modified: Fri Mar 10 15:31:17 2023, max compression
```

## Comparing `lupin-grognard-1.9.0.dev8.tar` & `lupin-grognard-1.9.0.dev9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.492189 lupin-grognard-1.9.0.dev8/
--rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-1.9.0.dev8/LICENCE
--rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev8/MANIFEST.in
--rw-rw-rw-   0        0        0      513 2023-03-09 17:24:12.492189 lupin-grognard-1.9.0.dev8/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-1.9.0.dev8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.446913 lupin-grognard-1.9.0.dev8/lupin_grognard/
--rw-rw-rw-   0        0        0       28 2023-03-09 17:24:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/__init__.py
--rw-rw-rw-   0        0        0       79 2022-12-05 21:58:40.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.468349 lupin-grognard-1.9.0.dev8/lupin_grognard/core/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/__init__.py
--rw-rw-rw-   0        0        0    11229 2023-03-09 17:23:36.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/changelog.py
--rw-rw-rw-   0        0        0     1450 2023-02-16 15:33:02.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/check.py
--rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/cmd.py
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.472350 lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/
--rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/__init__.py
--rw-rw-rw-   0        0        0     2995 2023-03-09 14:36:52.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit.py
--rw-rw-rw-   0        0        0     1037 2023-02-07 15:57:39.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit_error.py
--rw-rw-rw-   0        0        0     1816 2023-02-17 13:17:51.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit_reporter.py
--rw-rw-rw-   0        0        0     4305 2023-02-16 10:46:43.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit_validator.py
--rw-rw-rw-   0        0        0     1206 2023-02-01 12:31:41.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/config.py
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.474867 lupin-grognard-1.9.0.dev8/lupin_grognard/core/format/
--rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/format/__init__.py
--rw-rw-rw-   0        0        0     2697 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/format/clang_format.py
--rw-rw-rw-   0        0        0     2598 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/format/cmake_format.py
--rw-rw-rw-   0        0        0     2900 2023-03-09 10:41:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/git.py
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.476870 lupin-grognard-1.9.0.dev8/lupin_grognard/core/tools/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/tools/__init__.py
--rw-rw-rw-   0        0        0     3459 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/core/tools/utils.py
--rw-rw-rw-   0        0        0     5104 2023-03-07 14:09:45.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/run.py
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.491188 lupin-grognard-1.9.0.dev8/lupin_grognard/templates/
--rw-rw-rw-   0        0        0      745 2023-03-08 14:46:13.000000 lupin-grognard-1.9.0.dev8/lupin_grognard/templates/changelog.j2
-drwxrwxrwx   0        0        0        0 2023-03-09 17:24:12.462837 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/
--rw-rw-rw-   0        0        0      513 2023-03-09 17:24:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-09 17:24:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 17:24:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-09 17:24:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      133 2023-03-09 17:24:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-09 17:24:12.000000 lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      938 2023-03-09 17:24:12.496433 lupin-grognard-1.9.0.dev8/setup.cfg
--rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.639008 lupin-grognard-1.9.0.dev9/
+-rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-1.9.0.dev9/LICENCE
+-rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev9/MANIFEST.in
+-rw-rw-rw-   0        0        0      513 2023-03-10 15:31:17.639008 lupin-grognard-1.9.0.dev9/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-1.9.0.dev9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.586808 lupin-grognard-1.9.0.dev9/lupin_grognard/
+-rw-rw-rw-   0        0        0       28 2023-03-10 15:31:17.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-12-05 21:58:40.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/__main__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.603872 lupin-grognard-1.9.0.dev9/lupin_grognard/core/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/__init__.py
+-rw-rw-rw-   0        0        0    10975 2023-03-10 15:14:22.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/changelog.py
+-rw-rw-rw-   0        0        0     1450 2023-02-16 15:33:02.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/check.py
+-rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/cmd.py
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.607873 lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/
+-rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/__init__.py
+-rw-rw-rw-   0        0        0     2995 2023-03-09 14:36:52.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit.py
+-rw-rw-rw-   0        0        0     1037 2023-02-07 15:57:39.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit_error.py
+-rw-rw-rw-   0        0        0     1816 2023-02-17 13:17:51.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit_reporter.py
+-rw-rw-rw-   0        0        0     4305 2023-02-16 10:46:43.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit_validator.py
+-rw-rw-rw-   0        0        0     1206 2023-02-01 12:31:41.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/config.py
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.609873 lupin-grognard-1.9.0.dev9/lupin_grognard/core/format/
+-rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/format/__init__.py
+-rw-rw-rw-   0        0        0     2697 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/format/clang_format.py
+-rw-rw-rw-   0        0        0     2598 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/format/cmake_format.py
+-rw-rw-rw-   0        0        0     3109 2023-03-10 15:05:05.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/git.py
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.610874 lupin-grognard-1.9.0.dev9/lupin_grognard/core/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     3459 2023-03-10 14:33:08.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/core/tools/utils.py
+-rw-rw-rw-   0        0        0     5104 2023-03-07 14:09:45.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/run.py
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.639008 lupin-grognard-1.9.0.dev9/lupin_grognard/templates/
+-rw-rw-rw-   0        0        0     1084 2023-03-10 09:09:00.000000 lupin-grognard-1.9.0.dev9/lupin_grognard/templates/changelog.j2
+drwxrwxrwx   0        0        0        0 2023-03-10 15:31:17.598842 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/
+-rw-rw-rw-   0        0        0      513 2023-03-10 15:31:17.000000 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 15:31:17.000000 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-10 15:31:17.000000 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-03-10 15:31:17.000000 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      133 2023-03-10 15:31:17.000000 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-03-10 15:31:17.000000 lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      938 2023-03-10 15:31:17.644037 lupin-grognard-1.9.0.dev9/setup.cfg
+-rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0.dev9/setup.py
```

### Comparing `lupin-grognard-1.9.0.dev8/LICENCE` & `lupin-grognard-1.9.0.dev9/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/PKG-INFO` & `lupin-grognard-1.9.0.dev9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 1.9.0.dev8
+Version: 1.9.0.dev9
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/changelog.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/changelog.py`

 * *Files 10% similar despite different names*

```diff
@@ -155,85 +155,82 @@
                 Union[List, List]: List of parents without index 0 and list of close issues"""
         parents_hash = commit.parents[1:]
         close_issues = commit.closes_issues if commit.closes_issues else []
         return parents_hash, close_issues
 
     def _is_commit_related_to_closed_issue(
         self, commit: Commit, commit_parents: List, close_issues: List
-    ) -> bool:
+    ) -> str:
         for index, hash in enumerate(commit_parents):
             if hash == commit.hash:
                 if close_issues:
                     return close_issues[index]
-        return ""
+        return None
 
-    def _append_title_with_matched_issue_for_feat_and_fix_type(
-        self, commits: List[str], commit: Commit, match_issue: str
+    def _append_title_with_matched_issue(
+        self, commits: List[str], commit: Commit, issue_number: str
     ) -> None:
-        """Append commit without type scope with matched issue for commit type feat and fix"""
-        url = self.git.get_remote_origin_url()
-        url_issue = (
-            f"[#{match_issue}]({url}/-/issues/{match_issue})" if match_issue else ""
-        )
-        commits.append(f"{commit.title_without_type_scope} {url_issue}")
-
-    def _append_title_with_matched_issue_for_other_type(
-        self, commits: List[str], commit: Commit, match_issue: str
-    ) -> None:
-        """Append commit with type and matched issue for other commit type"""
-        url = self.git.get_remote_origin_url()
-        url_issue = (
-            f"[#{match_issue}]({url}/-/issues/{match_issue})" if match_issue else ""
-        )
-        commits.append(f"{commit.title} {url_issue}")
+        """Append title without type and scope for feat and fix commit type,
+        append title for other commit type and append issue number and url if issue number is found"""
+        if commit.type == "feat" or commit.type == "fix":
+            commit_title = commit.title_without_type_scope
+        else:
+            commit_title = commit.title
+        if not issue_number:
+            commits.append([commit_title])
+        else:
+            url = f"{self.git.get_remote_origin_url()}/-/issues/{issue_number}"
+            commits.append([commit_title, issue_number, url])
 
     def _classify_commits_by_type_and_scope(
         self, commits: List[Commit]
     ) -> Dict[str, Union[Dict[str, List[str]], List[str]]]:
         """Classify commits by type and scope and exclude merge commits"""
         commits_feat_add, commits_feat_change, commits_feat_remove = [], [], []
         commits_fix, commits_other = [], []
-        commit_parents, close_issues, match_issue = "", "", ""
+        commit_parents, close_issues, issue_number = "", "", ""
 
         for commit in commits:
             if commit.title.startswith("Merge"):
                 (
                     commit_parents,
                     close_issues,
                 ) = self._get_parents_hash_and_close_issues_for_commit(commit=commit)
             if commit_parents:
-                match_issue = self._is_commit_related_to_closed_issue(
+                issue_number = self._is_commit_related_to_closed_issue(
                     commit=commit,
                     commit_parents=commit_parents,
                     close_issues=close_issues,
                 )
             match (commit.type, commit.scope):
                 case ("feat", "(add)"):
-                    self._append_title_with_matched_issue_for_feat_and_fix_type(
-                        commits=commits_feat_add, commit=commit, match_issue=match_issue
+                    self._append_title_with_matched_issue(
+                        commits=commits_feat_add,
+                        commit=commit,
+                        issue_number=issue_number,
                     )
                 case ("feat", "(change)"):
-                    self._append_title_with_matched_issue_for_feat_and_fix_type(
+                    self._append_title_with_matched_issue(
                         commits=commits_feat_change,
                         commit=commit,
-                        match_issue=match_issue,
+                        issue_number=issue_number,
                     )
                 case ("feat", "(remove)"):
-                    self._append_title_with_matched_issue_for_feat_and_fix_type(
+                    self._append_title_with_matched_issue(
                         commits=commits_feat_remove,
                         commit=commit,
-                        match_issue=match_issue,
+                        issue_number=issue_number,
                     )
                 case ("fix", None):
-                    self._append_title_with_matched_issue_for_feat_and_fix_type(
-                        commits=commits_fix, commit=commit, match_issue=match_issue
+                    self._append_title_with_matched_issue(
+                        commits=commits_fix, commit=commit, issue_number=issue_number
                     )
                 case (_, _) if commit.type is not None:
-                    self._append_title_with_matched_issue_for_other_type(
-                        commits=commits_other, commit=commit, match_issue=match_issue
+                    self._append_title_with_matched_issue(
+                        commits=commits_other, commit=commit, issue_number=issue_number
                     )
         return self._create_commit_dict(
             commits_feat_add=commits_feat_add,
             commits_feat_change=commits_feat_change,
             commits_feat_remove=commits_feat_remove,
             commits_fix=commits_fix,
             commits_other=commits_other,
```

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/check.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/check.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/cmd.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/cmd.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit_error.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit_error.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit_reporter.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit_reporter.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/commit/commit_validator.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/commit/commit_validator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/config.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/config.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/format/clang_format.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/format/clang_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/format/cmake_format.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/format/cmake_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/git.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/git.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import sys
 from typing import List
 
 from lupin_grognard.core.cmd import Command, run_command
 from lupin_grognard.core.config import COMMIT_DELIMITER
 
 
@@ -22,29 +23,30 @@
 
     def get_branch_name(self) -> str:
         return run_command(command="git branch --show-current").stdout
 
     def get_remote_origin_url(self) -> str:
         c = run_command(command="git config --get remote.origin.url")
         if c.return_code != 0:
-            print(f"Git error while getting project url: {c.stderr}")
-            sys.exit(1)
+            self._git_error(
+                msg=f"Git error while getting remote origin url: {c.stderr}"
+            )
         gitlab_url = c.stdout
         if gitlab_url.startswith("https://gitlab.com/"):
-            return gitlab_url
+            return gitlab_url[:-4] if gitlab_url.endswith(".git") else gitlab_url
         else:
             a = gitlab_url.find(":")
             if a != -1:
                 gitlab_url = gitlab_url.replace(":", "/")
             gitlab_location = gitlab_url.find("@gitlab.com")
             gitlab_url = gitlab_url[gitlab_location + 1 :]
             gitlab_url = "https://" + gitlab_url
             return gitlab_url[:-4] if gitlab_url.endswith(".git") else gitlab_url
 
-    def get_tags(self) -> List:
+    def get_tags(self) -> List[List]:
         """Returns a list of tags with the following format:
         [
             ["tag_name", "tag_hash", "tag_date"],
             ["tag_name", "tag_hash", "tag_date"],
             ...
         ]
         """
@@ -55,21 +57,25 @@
             f"%(objectname){inner_delimiter}"
             f"%(creatordate:format:{dateformat}){inner_delimiter}"
             f'%(object)"'
         )
         c = run_command(f"git tag --format={formatter} --sort=-creatordate")
 
         if c.return_code != 0:
-            print(f"Git error while getting tags: {c.stderr}")
-            sys.exit(1)
+            self._git_error(msg=f"Git error while getting tags: {c.stderr}")
         if not c.stdout:
             return []
 
         tags_list = [line for line in c.stdout.splitlines()]
         return [tag.split(inner_delimiter)[:-1] for tag in tags_list]
 
     def get_parents(self, commit_hash: str) -> List[str]:
         c = run_command(f"git show --format=%P -s {commit_hash}")
         if c.return_code != 0:
-            print(f"Git error while getting parents: {c.stderr}")
-            sys.exit(1)
+            self._git_error(
+                msg=f"Git error while getting parents of commit: {c.stderr}"
+            )
         return c.stdout.split(" ")
+
+    def _git_error(self, msg: str):
+        logging.error(msg)
+        sys.exit(1)
```

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/core/tools/utils.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard/run.py` & `lupin-grognard-1.9.0.dev9/lupin_grognard/run.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/PKG-INFO` & `lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 1.9.0.dev8
+Version: 1.9.0.dev9
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-1.9.0.dev8/lupin_grognard.egg-info/SOURCES.txt` & `lupin-grognard-1.9.0.dev9/lupin_grognard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0.dev8/setup.cfg` & `lupin-grognard-1.9.0.dev9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d67 726f 676e 6172   = lupin-grognar
 00000020: 640d 0a76 6572 7369 6f6e 203d 2031 2e39  d..version = 1.9
-00000030: 2e30 2e64 6576 380d 0a64 6573 6372 6970  .0.dev8..descrip
+00000030: 2e30 2e64 6576 390d 0a64 6573 6372 6970  .0.dev9..descrip
 00000040: 7469 6f6e 203d 204c 7570 696e 206c 696e  tion = Lupin lin
 00000050: 7465 7220 746f 6f6c 0d0a 6c6f 6e67 5f64  ter tool..long_d
 00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6b65  e: README.md..ke
 00000080: 7977 6f72 6473 203d 2063 6c69 2c20 6c69  ywords = cli, li
 00000090: 6e74 6572 0d0a 6c69 6365 6e73 6520 3d20  nter..license = 
 000000a0: 4d49 5420 4c69 6365 6e73 650d 0a63 6c61  MIT License..cla
```

