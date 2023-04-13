# Comparing `tmp/HawaData-0.2.8.tar.gz` & `tmp/HawaData-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.2.8.tar", last modified: Thu Apr 13 06:40:25 2023, max compression
+gzip compressed data, was "HawaData-0.2.9.tar", last modified: Thu Apr 13 07:04:42 2023, max compression
```

## Comparing `HawaData-0.2.8.tar` & `HawaData-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.221859 HawaData-0.2.8/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.211082 HawaData-0.2.8/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     1893 2023-04-13 06:40:25.000000 HawaData-0.2.8/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-13 06:40:25.000000 HawaData-0.2.8/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-13 06:40:25.000000 HawaData-0.2.8/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-13 06:40:25.000000 HawaData-0.2.8/HawaData.egg-info/requires.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-13 06:40:25.000000 HawaData-0.2.8/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     1893 2023-04-13 06:40:25.221635 HawaData-0.2.8/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.2.8/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.211540 HawaData-0.2.8/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.2.8/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.213508 HawaData-0.2.8/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.2.8/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.2.8/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.2.8/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.2.8/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.215231 HawaData-0.2.8/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.2.8/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8762 2023-04-13 06:33:34.000000 HawaData-0.2.8/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     4582 2023-03-31 06:23:45.000000 HawaData-0.2.8/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2691 2022-12-01 05:37:32.000000 HawaData-0.2.8/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.2.8/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.216408 HawaData-0.2.8/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.2.8/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.2.8/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.2.8/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.217672 HawaData-0.2.8/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.2.8/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22853 2023-04-13 06:36:14.000000 HawaData-0.2.8/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.2.8/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-13 06:40:25.221937 HawaData-0.2.8/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.2.8/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.218917 HawaData-0.2.8/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.2.8/test/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.2.8/test/mock.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.219567 HawaData-0.2.8/test/test_common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.2.8/test/test_common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.2.8/test/test_common/test_common_data.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.220188 HawaData-0.2.8/test/test_data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.2.8/test/test_data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1582 2023-04-13 03:55:31.000000 HawaData-0.2.8/test/test_data/test_school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 06:40:25.221320 HawaData-0.2.8/test/test_paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.2.8/test/test_paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.2.8/test/test_paper/test_health_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.2.8/test/test_paper/test_mht_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.2.8/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.486831 HawaData-0.2.9/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.473830 HawaData-0.2.9/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1922 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/requires.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-13 07:04:42.000000 HawaData-0.2.9/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1922 2023-04-13 07:04:42.486584 HawaData-0.2.9/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.2.9/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.474329 HawaData-0.2.9/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.2.9/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.476401 HawaData-0.2.9/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.2.9/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.2.9/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.2.9/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.2.9/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.478699 HawaData-0.2.9/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.2.9/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8762 2023-04-13 06:33:34.000000 HawaData-0.2.9/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     4582 2023-03-31 06:23:45.000000 HawaData-0.2.9/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2691 2022-12-01 05:37:32.000000 HawaData-0.2.9/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.2.9/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.479985 HawaData-0.2.9/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.2.9/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.2.9/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.2.9/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.480982 HawaData-0.2.9/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.2.9/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    22989 2023-04-13 07:01:46.000000 HawaData-0.2.9/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.2.9/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-13 07:04:42.486909 HawaData-0.2.9/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.2.9/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.482765 HawaData-0.2.9/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.2.9/test/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.2.9/test/mock.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.483602 HawaData-0.2.9/test/test_common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.2.9/test/test_common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.2.9/test/test_common/test_common_data.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.484603 HawaData-0.2.9/test/test_data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.2.9/test/test_data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1582 2023-04-13 03:55:31.000000 HawaData-0.2.9/test/test_data/test_school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 07:04:42.485967 HawaData-0.2.9/test/test_paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.2.9/test/test_paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.2.9/test/test_paper/test_health_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.2.9/test/test_paper/test_mht_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.2.9/test/test_query.py
```

### Comparing `HawaData-0.2.8/HawaData.egg-info/PKG-INFO` & `HawaData-0.2.9/HawaData.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -69,7 +69,8 @@
 - 0.2.2 Move health school to health report
 - 0.2.3 Fix cache year data
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
+- 0.2.9 Fix miss grade again
```

### Comparing `HawaData-0.2.8/HawaData.egg-info/SOURCES.txt` & `HawaData-0.2.9/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/PKG-INFO` & `HawaData-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -69,7 +69,8 @@
 - 0.2.2 Move health school to health report
 - 0.2.3 Fix cache year data
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
+- 0.2.9 Fix miss grade again
```

### Comparing `HawaData-0.2.8/README.md` & `HawaData-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/hawa/base/db.py` & `HawaData-0.2.9/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/hawa/base/init.py` & `HawaData-0.2.9/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/hawa/common/data.py` & `HawaData-0.2.9/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/hawa/common/query.py` & `HawaData-0.2.9/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/hawa/common/utils.py` & `HawaData-0.2.9/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/hawa/config.py` & `HawaData-0.2.9/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/hawa/paper/health.py` & `HawaData-0.2.9/hawa/paper/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,15 +443,16 @@
             return ''
 
     def compare_grade_gen_text(self):
         """生成整体分析标题及一句分析文本。"""
         data = {}
         for grade in self.grade.grades:
             sch = self.grade_score[grade].avg
-            year = self.last_year[str(grade)]['score']['total']
+            last_year_grade_data = self.get_last_year_miss(grade=grade)
+            year = last_year_grade_data['score']['total']
             data[grade] = sch - year
         total_dif = sum(data.values()) / len(data)
         diff = []
         if total_dif > 0:
             for k, v in data.items():
                 if v < 0:
                     diff.append(k)
@@ -474,15 +475,16 @@
         """描述全年级对比情况
         :param category: total/gender  total：总体比全国 / gender：男生比女生。
         """
         bigger, smaller = [], []
         for grade in self.grade.grades:
             if category == 'total':
                 first = self.grade_score[grade].avg
-                second = self.last_year[str(grade)]['score']['total']
+                last_year_grade_data = self.get_last_year_miss(grade=grade)
+                second = last_year_grade_data['score']['total']
             else:
                 first = self.summary_scores[grade]['M']
                 second = self.summary_scores[grade]['F']
             if first - second >= 5:
                 bigger.append(f"{project.grade_simple[grade]}年级")
             elif first - second <= -5:
                 smaller.append(f"{project.grade_simple[grade]}年级")
```

### Comparing `HawaData-0.2.8/hawa/paper/mht.py` & `HawaData-0.2.9/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/setup.py` & `HawaData-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/test/mock.py` & `HawaData-0.2.9/test/mock.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/test/test_common/test_common_data.py` & `HawaData-0.2.9/test/test_common/test_common_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/test/test_data/test_school.py` & `HawaData-0.2.9/test/test_data/test_school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/test/test_paper/test_health_data.py` & `HawaData-0.2.9/test/test_paper/test_health_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.8/test/test_query.py` & `HawaData-0.2.9/test/test_query.py`

 * *Files identical despite different names*

