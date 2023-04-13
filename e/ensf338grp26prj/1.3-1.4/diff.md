# Comparing `tmp/ensf338grp26prj-1.3.tar.gz` & `tmp/ensf338grp26prj-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensf338grp26prj-1.3.tar", last modified: Thu Apr 13 19:30:06 2023, max compression
+gzip compressed data, was "ensf338grp26prj-1.4.tar", last modified: Thu Apr 13 19:43:26 2023, max compression
```

## Comparing `ensf338grp26prj-1.3.tar` & `ensf338grp26prj-1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:30:06.541511 ensf338grp26prj-1.3/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 19:30:06.541346 ensf338grp26prj-1.3/PKG-INFO
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:30:06.537940 ensf338grp26prj-1.3/ensf338grp26prj.egg-info/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 19:30:06.000000 ensf338grp26prj-1.3/ensf338grp26prj.egg-info/PKG-INFO
--rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 19:30:06.000000 ensf338grp26prj-1.3/ensf338grp26prj.egg-info/SOURCES.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 19:30:06.000000 ensf338grp26prj-1.3/ensf338grp26prj.egg-info/dependency_links.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 19:30:06.000000 ensf338grp26prj-1.3/ensf338grp26prj.egg-info/top_level.txt
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:30:06.538102 ensf338grp26prj-1.3/myLib/
--rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 ensf338grp26prj-1.3/myLib/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:30:06.538266 ensf338grp26prj-1.3/myLib/datastructures/
--rw-r--r--   0 tonytran   (501) staff       (20)      276 2023-04-13 19:29:34.000000 ensf338grp26prj-1.3/myLib/datastructures/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:30:06.539543 ensf338grp26prj-1.3/myLib/datastructures/linear/
--rw-r--r--   0 tonytran   (501) staff       (20)     6748 2023-04-13 17:35:15.000000 ensf338grp26prj-1.3/myLib/datastructures/linear/CDLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8090 2023-04-13 17:35:15.000000 ensf338grp26prj-1.3/myLib/datastructures/linear/CSLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9148 2023-04-13 17:35:15.000000 ensf338grp26prj-1.3/myLib/datastructures/linear/DLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.3/myLib/datastructures/linear/QueueLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9948 2023-04-13 17:35:15.000000 ensf338grp26prj-1.3/myLib/datastructures/linear/SLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 ensf338grp26prj-1.3/myLib/datastructures/linear/StackLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)      145 2023-04-13 19:26:47.000000 ensf338grp26prj-1.3/myLib/datastructures/linear/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:30:06.540367 ensf338grp26prj-1.3/myLib/datastructures/nodes/
--rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.3/myLib/datastructures/nodes/DNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.3/myLib/datastructures/nodes/SNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.3/myLib/datastructures/nodes/TNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)       74 2023-04-13 18:21:02.000000 ensf338grp26prj-1.3/myLib/datastructures/nodes/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:30:06.541044 ensf338grp26prj-1.3/myLib/datastructures/trees/
--rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.3/myLib/datastructures/trees/AVL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.3/myLib/datastructures/trees/BST.py
--rw-r--r--   0 tonytran   (501) staff       (20)       41 2023-04-13 19:27:33.000000 ensf338grp26prj-1.3/myLib/datastructures/trees/__init__.py
--rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 19:30:06.541577 ensf338grp26prj-1.3/setup.cfg
--rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 19:29:40.000000 ensf338grp26prj-1.3/setup.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:43:26.003801 ensf338grp26prj-1.4/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 19:43:26.003631 ensf338grp26prj-1.4/PKG-INFO
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:43:25.998847 ensf338grp26prj-1.4/ensf338grp26prj.egg-info/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 19:43:25.000000 ensf338grp26prj-1.4/ensf338grp26prj.egg-info/PKG-INFO
+-rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 19:43:25.000000 ensf338grp26prj-1.4/ensf338grp26prj.egg-info/SOURCES.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 19:43:25.000000 ensf338grp26prj-1.4/ensf338grp26prj.egg-info/dependency_links.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 19:43:25.000000 ensf338grp26prj-1.4/ensf338grp26prj.egg-info/top_level.txt
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:43:25.999011 ensf338grp26prj-1.4/myLib/
+-rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 ensf338grp26prj-1.4/myLib/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:43:25.999308 ensf338grp26prj-1.4/myLib/datastructures/
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 19:41:57.000000 ensf338grp26prj-1.4/myLib/datastructures/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:43:26.001692 ensf338grp26prj-1.4/myLib/datastructures/linear/
+-rw-r--r--   0 tonytran   (501) staff       (20)     6748 2023-04-13 17:35:15.000000 ensf338grp26prj-1.4/myLib/datastructures/linear/CDLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8090 2023-04-13 17:35:15.000000 ensf338grp26prj-1.4/myLib/datastructures/linear/CSLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9148 2023-04-13 17:35:15.000000 ensf338grp26prj-1.4/myLib/datastructures/linear/DLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.4/myLib/datastructures/linear/QueueLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9948 2023-04-13 17:35:15.000000 ensf338grp26prj-1.4/myLib/datastructures/linear/SLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 ensf338grp26prj-1.4/myLib/datastructures/linear/StackLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      166 2023-04-13 19:41:48.000000 ensf338grp26prj-1.4/myLib/datastructures/linear/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:43:26.002650 ensf338grp26prj-1.4/myLib/datastructures/nodes/
+-rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.4/myLib/datastructures/nodes/DNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.4/myLib/datastructures/nodes/SNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.4/myLib/datastructures/nodes/TNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       94 2023-04-13 19:42:18.000000 ensf338grp26prj-1.4/myLib/datastructures/nodes/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 19:43:26.003362 ensf338grp26prj-1.4/myLib/datastructures/trees/
+-rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.4/myLib/datastructures/trees/AVL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.4/myLib/datastructures/trees/BST.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       61 2023-04-13 19:42:06.000000 ensf338grp26prj-1.4/myLib/datastructures/trees/__init__.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 19:43:26.003862 ensf338grp26prj-1.4/setup.cfg
+-rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 19:42:23.000000 ensf338grp26prj-1.4/setup.py
```

### Comparing `ensf338grp26prj-1.3/ensf338grp26prj.egg-info/SOURCES.txt` & `ensf338grp26prj-1.4/ensf338grp26prj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/linear/CDLL.py` & `ensf338grp26prj-1.4/myLib/datastructures/linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/linear/CSLL.py` & `ensf338grp26prj-1.4/myLib/datastructures/linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/linear/DLL.py` & `ensf338grp26prj-1.4/myLib/datastructures/linear/DLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/linear/QueueLL.py` & `ensf338grp26prj-1.4/myLib/datastructures/linear/QueueLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/linear/SLL.py` & `ensf338grp26prj-1.4/myLib/datastructures/linear/SLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/linear/StackLL.py` & `ensf338grp26prj-1.4/myLib/datastructures/linear/StackLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/nodes/DNode.py` & `ensf338grp26prj-1.4/myLib/datastructures/nodes/DNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/nodes/TNode.py` & `ensf338grp26prj-1.4/myLib/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/trees/AVL.py` & `ensf338grp26prj-1.4/myLib/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.3/myLib/datastructures/trees/BST.py` & `ensf338grp26prj-1.4/myLib/datastructures/trees/BST.py`

 * *Files identical despite different names*

