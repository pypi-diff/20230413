# Comparing `tmp/HawaData-0.2.6.tar.gz` & `tmp/HawaData-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.2.6.tar", last modified: Fri Mar 31 06:49:46 2023, max compression
+gzip compressed data, was "HawaData-0.2.7.tar", last modified: Thu Apr 13 04:01:49 2023, max compression
```

## Comparing `HawaData-0.2.6.tar` & `HawaData-0.2.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.753992 HawaData-0.2.6/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.740695 HawaData-0.2.6/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     1843 2023-03-31 06:49:46.000000 HawaData-0.2.6/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-03-31 06:49:46.000000 HawaData-0.2.6/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-03-31 06:49:46.000000 HawaData-0.2.6/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-03-31 06:49:46.000000 HawaData-0.2.6/HawaData.egg-info/requires.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-03-31 06:49:46.000000 HawaData-0.2.6/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     1843 2023-03-31 06:49:46.753734 HawaData-0.2.6/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.2.6/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.741269 HawaData-0.2.6/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.2.6/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.743952 HawaData-0.2.6/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.2.6/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.2.6/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.2.6/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.2.6/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.745813 HawaData-0.2.6/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.2.6/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8024 2023-03-29 04:22:50.000000 HawaData-0.2.6/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     4582 2023-03-31 06:23:45.000000 HawaData-0.2.6/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2691 2022-12-01 05:37:32.000000 HawaData-0.2.6/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.2.6/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.747033 HawaData-0.2.6/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.2.6/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.2.6/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.2.6/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.748406 HawaData-0.2.6/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.2.6/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22691 2023-03-31 06:48:57.000000 HawaData-0.2.6/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.2.6/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-03-31 06:49:46.754069 HawaData-0.2.6/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.2.6/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.749985 HawaData-0.2.6/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.2.6/test/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.2.6/test/mock.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.750862 HawaData-0.2.6/test/test_common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.2.6/test/test_common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      770 2022-12-01 12:37:40.000000 HawaData-0.2.6/test/test_common/test_common_data.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.751739 HawaData-0.2.6/test/test_data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.2.6/test/test_data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1521 2022-12-08 10:50:50.000000 HawaData-0.2.6/test/test_data/test_school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-03-31 06:49:46.753112 HawaData-0.2.6/test/test_paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.2.6/test/test_paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.2.6/test/test_paper/test_health_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.2.6/test/test_paper/test_mht_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.2.6/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.043039 HawaData-0.2.7/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.029796 HawaData-0.2.7/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1866 2023-04-13 04:01:48.000000 HawaData-0.2.7/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-13 04:01:48.000000 HawaData-0.2.7/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-13 04:01:48.000000 HawaData-0.2.7/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-13 04:01:48.000000 HawaData-0.2.7/HawaData.egg-info/requires.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-13 04:01:48.000000 HawaData-0.2.7/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1866 2023-04-13 04:01:49.042741 HawaData-0.2.7/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.2.7/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.030250 HawaData-0.2.7/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.2.7/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.032448 HawaData-0.2.7/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.2.7/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.2.7/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.2.7/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.2.7/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.034563 HawaData-0.2.7/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.2.7/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8024 2023-03-31 09:16:09.000000 HawaData-0.2.7/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     4582 2023-03-31 06:23:45.000000 HawaData-0.2.7/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2691 2022-12-01 05:37:32.000000 HawaData-0.2.7/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.2.7/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.035833 HawaData-0.2.7/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.2.7/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.2.7/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.2.7/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.037582 HawaData-0.2.7/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.2.7/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    23138 2023-04-13 03:53:21.000000 HawaData-0.2.7/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.2.7/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-13 04:01:49.043116 HawaData-0.2.7/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.2.7/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.039164 HawaData-0.2.7/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.2.7/test/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.2.7/test/mock.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.039899 HawaData-0.2.7/test/test_common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.2.7/test/test_common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.2.7/test/test_common/test_common_data.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.040727 HawaData-0.2.7/test/test_data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.2.7/test/test_data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1582 2023-04-13 03:55:31.000000 HawaData-0.2.7/test/test_data/test_school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-13 04:01:49.042123 HawaData-0.2.7/test/test_paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.2.7/test/test_paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.2.7/test/test_paper/test_health_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.2.7/test/test_paper/test_mht_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.2.7/test/test_query.py
```

### Comparing `HawaData-0.2.6/HawaData.egg-info/PKG-INFO` & `HawaData-0.2.7/HawaData.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.2.6
+Version: 0.2.7
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -67,7 +67,8 @@
 - 0.2.0 Add district data
 - 0.2.1 Move gender count data to health.
 - 0.2.2 Move health school to health report
 - 0.2.3 Fix cache year data
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
+- 0.2.7 Fix miss grade
```

### Comparing `HawaData-0.2.6/HawaData.egg-info/SOURCES.txt` & `HawaData-0.2.7/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/PKG-INFO` & `HawaData-0.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.2.6
+Version: 0.2.7
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -67,7 +67,8 @@
 - 0.2.0 Add district data
 - 0.2.1 Move gender count data to health.
 - 0.2.2 Move health school to health report
 - 0.2.3 Fix cache year data
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
+- 0.2.7 Fix miss grade
```

### Comparing `HawaData-0.2.6/README.md` & `HawaData-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/hawa/base/db.py` & `HawaData-0.2.7/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/hawa/base/init.py` & `HawaData-0.2.7/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/hawa/common/data.py` & `HawaData-0.2.7/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/hawa/common/query.py` & `HawaData-0.2.7/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/hawa/common/utils.py` & `HawaData-0.2.7/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/hawa/config.py` & `HawaData-0.2.7/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/hawa/paper/health.py` & `HawaData-0.2.7/hawa/paper/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,23 @@
             return
         key = f'{project.REDIS_PREFIX}{self.last_year_num}:data'
         if not self.redis.conn.exists(key):
             raise ValueError(f'last year data not exists: {key}')
         self.last_year = json.loads(self.redis.conn.get(key))
         res = []
         for grade in self.grade.grades:
-            year_code_score = pd.DataFrame(self.last_year[str(grade)]['code']).T
+            try:
+                year_code_score = pd.DataFrame(self.last_year[str(grade)]['code']).T
+            except KeyError:
+                temp_key = f'{project.REDIS_PREFIX}{self.last_year_num - 1}:data'
+                temp_last_year = json.loads(self.redis.conn.get(temp_key))
+                try:
+                    year_code_score = pd.DataFrame(temp_last_year[str(grade - 1)]['code']).T
+                except KeyError:
+                    year_code_score = pd.DataFrame(temp_last_year[str(grade - 3)]['code']).T
             year_code_score['i'] = [int(grade) * 10 + i for i in range(1, 11)]
             year_code_score.set_index('i', inplace=True)
             res.append(year_code_score)
         self.last_year_code_scores = pd.concat(res)
 
     def _to_count_c_code_scores(self):
         records = []
```

### Comparing `HawaData-0.2.6/hawa/paper/mht.py` & `HawaData-0.2.7/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/setup.py` & `HawaData-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/test/mock.py` & `HawaData-0.2.7/test/mock.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/test/test_common/test_common_data.py` & `HawaData-0.2.7/test/test_common/test_common_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from test.mock import prepare_test
 
 prepare_test()
 
 
 def test_common_init():
     rows = [
-        {"meta_unit_type": "school", "meta_unit_id": 3707030003, "target_year": 2021},
+        {"meta_unit_type": "school", "meta_unit_id": 1101089005, "target_year": 2023},
         # {"meta_unit_type": "district", "meta_unit_id": 370703, "target_year": 2021},
         # {"meta_unit_type": "city", "meta_unit_id": 331100, "target_year": 2021},
         # {"meta_unit_type": "province", "meta_unit_id": 410000, "target_year": 2021},
     ]
     for row in rows:
         logger.info(row)
         # common data without default  test_types and code_word_list
```

### Comparing `HawaData-0.2.6/test/test_data/test_school.py` & `HawaData-0.2.7/test/test_data/test_school.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from test.mock import prepare_test, validate_data_for_web
 
 prepare_test()
 
 
 def test_health_report_run():
     rows = [
-        {"meta_unit_id": 3707030003, "target_year": 2021},
+        # {"meta_unit_id": 5134010001, "target_year": 2021},
+        {"meta_unit_id": 1101089005, "target_year": 2023},
     ]
     for row in rows:
         logger.info(row)
         SchoolHealthReportData(**row)
 
 
 def test_mht_web_run():
```

### Comparing `HawaData-0.2.6/test/test_paper/test_health_data.py` & `HawaData-0.2.7/test/test_paper/test_health_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.2.6/test/test_query.py` & `HawaData-0.2.7/test/test_query.py`

 * *Files identical despite different names*

