# Comparing `tmp/os2ds-rules-0.0.1.tar.gz` & `tmp/os2ds-rules-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2ds-rules-0.0.1.tar", last modified: Thu Apr 13 09:50:42 2023, max compression
+gzip compressed data, was "os2ds-rules-0.0.2.tar", last modified: Thu Apr 13 11:13:23 2023, max compression
```

## Comparing `os2ds-rules-0.0.1.tar` & `os2ds-rules-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:50:42.280856 os2ds-rules-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-13 09:50:42.280856 os2ds-rules-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:50:42.280856 os2ds-rules-0.0.1/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/include/cpr-detector.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:50:42.280856 os2ds-rules-0.0.1/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/lib/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/lib/cpr-detector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/lib/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:50:42.284856 os2ds-rules-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:50:42.280856 os2ds-rules-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:50:42.280856 os2ds-rules-0.0.1/src/os2ds_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/src/os2ds_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/src/os2ds_rules/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/src/os2ds_rules/cpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-13 09:50:32.000000 os2ds-rules-0.0.1/src/os2ds_rules/name_rule.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:50:42.280856 os2ds-rules-0.0.1/src/os2ds_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-13 09:50:42.000000 os2ds-rules-0.0.1/src/os2ds_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 09:50:42.000000 os2ds-rules-0.0.1/src/os2ds_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:50:42.000000 os2ds-rules-0.0.1/src/os2ds_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 09:50:42.000000 os2ds-rules-0.0.1/src/os2ds_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/include/cpr-detector.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/lib/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/lib/cpr-detector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/lib/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/src/os2ds_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/cpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-13 11:13:15.000000 os2ds-rules-0.0.2/src/os2ds_rules/name_rule.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:13:23.030611 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 11:13:23.000000 os2ds-rules-0.0.2/src/os2ds_rules.egg-info/top_level.txt
```

### Comparing `os2ds-rules-0.0.1/LICENSE` & `os2ds-rules-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/PKG-INFO` & `os2ds-rules-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.1
+Version: 0.0.2
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `os2ds-rules-0.0.1/README.md` & `os2ds-rules-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/include/cpr-detector.hpp` & `os2ds-rules-0.0.2/include/cpr-detector.hpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/lib/address_rule.cpp` & `os2ds-rules-0.0.2/lib/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/lib/cpr-detector.cpp` & `os2ds-rules-0.0.2/lib/cpr-detector.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
         allow_separator = true;
 
       break;
     case CPRDetectorState::Second:
       if (allow_separator && is_space(*it)) {
         // Skip a space character.
         allow_separator = false;
+	++count;
         continue;
       }
 
       is_acceptable = make_predicate('0', '1');
       previous = cpr[2] =
           update(*it, CPRDetectorState::Third, state, is_acceptable);
 
@@ -206,14 +207,15 @@
         allow_separator = true;
 
       break;
     case CPRDetectorState::Fourth:
       if (allow_separator && is_space(*it)) {
         // Skip a space character.
         allow_separator = false;
+	++count;
         continue;
       }
 
       is_acceptable = is_digit;
 
       previous = cpr[4] =
           update(*it, CPRDetectorState::Fifth, state, is_acceptable);
@@ -234,14 +236,15 @@
         allow_separator = true;
 
       break;
     case CPRDetectorState::Sixth:
       if (allow_separator && is_separator(*it)) {
         // Skip one of the valid separator characters.
         allow_separator = false;
+	++count;
         continue;
       }
 
       is_acceptable = is_digit;
       previous = cpr[6] =
           update(*it, CPRDetectorState::Seventh, state, is_acceptable);
```

### Comparing `os2ds-rules-0.0.1/lib/name_rule.cpp` & `os2ds-rules-0.0.2/lib/name_rule.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
   if (in_word) {
     auto word_end = content.cend();
 
     if (contains(word_begin, word_end)) {
       MatchResult result(
           std::string(word_begin, word_end),
           static_cast<std::size_t>(std::distance(content.cbegin(), word_begin)),
-          static_cast<std::size_t>(std::distance(content.begin(), word_end)));
+          static_cast<std::size_t>(std::distance(content.begin(), word_end) - 1));
 
       results.push_back(result);
     }
   }
 
   return filter_matches(results);
 }
```

### Comparing `os2ds-rules-0.0.1/pyproject.toml` & `os2ds-rules-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os2ds-rules"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="HackTheOxidation", email="tomas.hagenau@protonmail.ch" },
 ]
 description = "Text processing tool for detecting Danish CPR-numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `os2ds-rules-0.0.1/setup.py` & `os2ds-rules-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/src/os2ds_rules/__init__.py` & `os2ds-rules-0.0.2/src/os2ds_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/src/os2ds_rules/address_rule.cpp` & `os2ds-rules-0.0.2/src/os2ds_rules/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/src/os2ds_rules/cpr.cpp` & `os2ds-rules-0.0.2/src/os2ds_rules/cpr.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/src/os2ds_rules/name_rule.cpp` & `os2ds-rules-0.0.2/src/os2ds_rules/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.1/src/os2ds_rules.egg-info/PKG-INFO` & `os2ds-rules-0.0.2/src/os2ds_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.1
+Version: 0.0.2
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

