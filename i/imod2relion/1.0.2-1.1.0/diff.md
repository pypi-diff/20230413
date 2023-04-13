# Comparing `tmp/imod2relion-1.0.2.tar.gz` & `tmp/imod2relion-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imod2relion-1.0.2.tar", last modified: Tue Apr 11 04:01:16 2023, max compression
+gzip compressed data, was "imod2relion-1.1.0.tar", last modified: Thu Apr 13 13:22:03 2023, max compression
```

## Comparing `imod2relion-1.0.2.tar` & `imod2relion-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 04:01:16.370798 imod2relion-1.0.2/
--rw-r--r--   0 hzvictor   (501) staff       (20)      584 2023-04-11 04:01:16.370679 imod2relion-1.0.2/PKG-INFO
--rw-r--r--   0 hzvictor   (501) staff       (20)      179 2023-04-11 03:42:54.000000 imod2relion-1.0.2/README.md
-drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 04:01:16.369729 imod2relion-1.0.2/imod2relion/
--rw-r--r--   0 hzvictor   (501) staff       (20)       81 2023-04-11 04:01:04.000000 imod2relion-1.0.2/imod2relion/__init__.py
--rw-r--r--   0 hzvictor   (501) staff       (20)     2790 2023-04-11 03:18:38.000000 imod2relion-1.0.2/imod2relion/_utils.py
--rw-r--r--   0 hzvictor   (501) staff       (20)     3201 2023-04-11 03:30:08.000000 imod2relion-1.0.2/imod2relion/main.py
--rw-r--r--   0 hzvictor   (501) staff       (20)     1630 2023-04-10 15:42:42.000000 imod2relion-1.0.2/imod2relion/test.py
-drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-11 04:01:16.370515 imod2relion-1.0.2/imod2relion.egg-info/
--rw-r--r--   0 hzvictor   (501) staff       (20)      584 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/PKG-INFO
--rw-r--r--   0 hzvictor   (501) staff       (20)      316 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/SOURCES.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)        1 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/dependency_links.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       54 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/entry_points.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       45 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/requires.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       12 2023-04-11 04:01:16.000000 imod2relion-1.0.2/imod2relion.egg-info/top_level.txt
--rw-r--r--   0 hzvictor   (501) staff       (20)       38 2023-04-11 04:01:16.370840 imod2relion-1.0.2/setup.cfg
--rw-r--r--   0 hzvictor   (501) staff       (20)      960 2023-04-11 04:00:34.000000 imod2relion-1.0.2/setup.py
+drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-13 13:22:03.317889 imod2relion-1.1.0/
+-rw-r--r--   0 hzvictor   (501) staff       (20)      584 2023-04-13 13:22:03.317736 imod2relion-1.1.0/PKG-INFO
+-rw-r--r--   0 hzvictor   (501) staff       (20)      179 2023-04-11 03:42:54.000000 imod2relion-1.1.0/README.md
+drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-13 13:22:03.316305 imod2relion-1.1.0/imod2relion/
+-rw-r--r--   0 hzvictor   (501) staff       (20)       81 2023-04-13 13:21:17.000000 imod2relion-1.1.0/imod2relion/__init__.py
+-rw-r--r--   0 hzvictor   (501) staff       (20)     2799 2023-04-13 13:20:50.000000 imod2relion-1.1.0/imod2relion/_utils.py
+-rw-r--r--   0 hzvictor   (501) staff       (20)     3201 2023-04-11 03:30:08.000000 imod2relion-1.1.0/imod2relion/main.py
+drwxr-xr-x   0 hzvictor   (501) staff       (20)        0 2023-04-13 13:22:03.317518 imod2relion-1.1.0/imod2relion.egg-info/
+-rw-r--r--   0 hzvictor   (501) staff       (20)      584 2023-04-13 13:22:03.000000 imod2relion-1.1.0/imod2relion.egg-info/PKG-INFO
+-rw-r--r--   0 hzvictor   (501) staff       (20)      296 2023-04-13 13:22:03.000000 imod2relion-1.1.0/imod2relion.egg-info/SOURCES.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)        1 2023-04-13 13:22:03.000000 imod2relion-1.1.0/imod2relion.egg-info/dependency_links.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       54 2023-04-13 13:22:03.000000 imod2relion-1.1.0/imod2relion.egg-info/entry_points.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       45 2023-04-13 13:22:03.000000 imod2relion-1.1.0/imod2relion.egg-info/requires.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       12 2023-04-13 13:22:03.000000 imod2relion-1.1.0/imod2relion.egg-info/top_level.txt
+-rw-r--r--   0 hzvictor   (501) staff       (20)       38 2023-04-13 13:22:03.317949 imod2relion-1.1.0/setup.cfg
+-rw-r--r--   0 hzvictor   (501) staff       (20)      960 2023-04-11 04:00:34.000000 imod2relion-1.1.0/setup.py
```

### Comparing `imod2relion-1.0.2/PKG-INFO` & `imod2relion-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imod2relion
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool reading IMOD points, obtaining particles' info and generating .star file for RELION
 Home-page: https://github.com/ZhenHuangLab/imod2relion
 Author: Zhen Huang
 Author-email: hzvictor@zju.edu.cn
 License: BSD 3-Clause License
 Keywords: cryo-em,cryo-et,imod,relion,starfile
 Requires-Python: >=3.9
```

### Comparing `imod2relion-1.0.2/imod2relion/_utils.py` & `imod2relion-1.1.0/imod2relion/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,22 +33,22 @@
     return cal_posi_df
 
 def eulerangle(x1,x2,y1,y2,z1,z2):
     x = x2 - x1
     y = y2 - y1
     z = z2 - z1
     if x == 0:
-        phi = np.pi / 2
+        psi = np.pi / 2
     else:
-        phi = np.arctan2(y, x)
+        psi = np.arctan2(-y, x) + np.pi
     if z == 0:
         theta = np.pi / 2
     else:
         theta = np.arctan2(np.sqrt(x ** 2 + y ** 2), z)
-    psi = 0
+    phi = 0
     phi = np.rad2deg(phi)
     theta = np.rad2deg(theta)
     psi = np.rad2deg(psi)
     return phi, theta, psi
 
 def cal_eulerange(df):
     cal_eulerange_df = pd.DataFrame(columns=['rlnAngleRot', 'rlnAngleTilt', 'rlnAnglePsi'])
```

### Comparing `imod2relion-1.0.2/imod2relion/main.py` & `imod2relion-1.1.0/imod2relion/main.py`

 * *Files identical despite different names*

### Comparing `imod2relion-1.0.2/imod2relion.egg-info/PKG-INFO` & `imod2relion-1.1.0/imod2relion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imod2relion
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool reading IMOD points, obtaining particles' info and generating .star file for RELION
 Home-page: https://github.com/ZhenHuangLab/imod2relion
 Author: Zhen Huang
 Author-email: hzvictor@zju.edu.cn
 License: BSD 3-Clause License
 Keywords: cryo-em,cryo-et,imod,relion,starfile
 Requires-Python: >=3.9
```

### Comparing `imod2relion-1.0.2/setup.py` & `imod2relion-1.1.0/setup.py`

 * *Files identical despite different names*

