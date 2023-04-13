# Comparing `tmp/ensf338grp26prj-1.1.tar.gz` & `tmp/ensf338grp26prj-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensf338grp26prj-1.1.tar", last modified: Thu Apr 13 18:07:46 2023, max compression
+gzip compressed data, was "ensf338grp26prj-1.2.tar", last modified: Thu Apr 13 18:21:24 2023, max compression
```

## Comparing `ensf338grp26prj-1.1.tar` & `ensf338grp26prj-1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:07:46.218906 ensf338grp26prj-1.1/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 18:07:46.218717 ensf338grp26prj-1.1/PKG-INFO
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:07:46.215295 ensf338grp26prj-1.1/ensf338grp26prj.egg-info/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 18:07:46.000000 ensf338grp26prj-1.1/ensf338grp26prj.egg-info/PKG-INFO
--rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 18:07:46.000000 ensf338grp26prj-1.1/ensf338grp26prj.egg-info/SOURCES.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 18:07:46.000000 ensf338grp26prj-1.1/ensf338grp26prj.egg-info/dependency_links.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 18:07:46.000000 ensf338grp26prj-1.1/ensf338grp26prj.egg-info/top_level.txt
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:07:46.215458 ensf338grp26prj-1.1/myLib/
--rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 ensf338grp26prj-1.1/myLib/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:07:46.215615 ensf338grp26prj-1.1/myLib/datastructures/
--rw-r--r--   0 tonytran   (501) staff       (20)       51 2023-04-13 17:52:14.000000 ensf338grp26prj-1.1/myLib/datastructures/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:07:46.217107 ensf338grp26prj-1.1/myLib/datastructures/linear/
--rw-r--r--   0 tonytran   (501) staff       (20)     6748 2023-04-13 17:35:15.000000 ensf338grp26prj-1.1/myLib/datastructures/linear/CDLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8090 2023-04-13 17:35:15.000000 ensf338grp26prj-1.1/myLib/datastructures/linear/CSLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9148 2023-04-13 17:35:15.000000 ensf338grp26prj-1.1/myLib/datastructures/linear/DLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.1/myLib/datastructures/linear/QueueLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9948 2023-04-13 17:35:15.000000 ensf338grp26prj-1.1/myLib/datastructures/linear/SLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 ensf338grp26prj-1.1/myLib/datastructures/linear/StackLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)      139 2023-04-13 18:06:41.000000 ensf338grp26prj-1.1/myLib/datastructures/linear/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:07:46.217903 ensf338grp26prj-1.1/myLib/datastructures/nodes/
--rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.1/myLib/datastructures/nodes/DNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.1/myLib/datastructures/nodes/SNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.1/myLib/datastructures/nodes/TNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)       71 2023-04-13 18:05:34.000000 ensf338grp26prj-1.1/myLib/datastructures/nodes/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:07:46.218464 ensf338grp26prj-1.1/myLib/datastructures/trees/
--rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.1/myLib/datastructures/trees/AVL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.1/myLib/datastructures/trees/BST.py
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 02:46:47.000000 ensf338grp26prj-1.1/myLib/datastructures/trees/__init__.py
--rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 18:07:46.218964 ensf338grp26prj-1.1/setup.cfg
--rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 18:07:43.000000 ensf338grp26prj-1.1/setup.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:21:24.750731 ensf338grp26prj-1.2/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 18:21:24.750549 ensf338grp26prj-1.2/PKG-INFO
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:21:24.746891 ensf338grp26prj-1.2/ensf338grp26prj.egg-info/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 18:21:24.000000 ensf338grp26prj-1.2/ensf338grp26prj.egg-info/PKG-INFO
+-rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 18:21:24.000000 ensf338grp26prj-1.2/ensf338grp26prj.egg-info/SOURCES.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 18:21:24.000000 ensf338grp26prj-1.2/ensf338grp26prj.egg-info/dependency_links.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 18:21:24.000000 ensf338grp26prj-1.2/ensf338grp26prj.egg-info/top_level.txt
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:21:24.747063 ensf338grp26prj-1.2/myLib/
+-rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 ensf338grp26prj-1.2/myLib/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:21:24.747358 ensf338grp26prj-1.2/myLib/datastructures/
+-rw-r--r--   0 tonytran   (501) staff       (20)       53 2023-04-13 18:20:23.000000 ensf338grp26prj-1.2/myLib/datastructures/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:21:24.748764 ensf338grp26prj-1.2/myLib/datastructures/linear/
+-rw-r--r--   0 tonytran   (501) staff       (20)     6748 2023-04-13 17:35:15.000000 ensf338grp26prj-1.2/myLib/datastructures/linear/CDLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8090 2023-04-13 17:35:15.000000 ensf338grp26prj-1.2/myLib/datastructures/linear/CSLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9148 2023-04-13 17:35:15.000000 ensf338grp26prj-1.2/myLib/datastructures/linear/DLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.2/myLib/datastructures/linear/QueueLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9948 2023-04-13 17:35:15.000000 ensf338grp26prj-1.2/myLib/datastructures/linear/SLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 ensf338grp26prj-1.2/myLib/datastructures/linear/StackLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      145 2023-04-13 18:21:11.000000 ensf338grp26prj-1.2/myLib/datastructures/linear/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:21:24.749486 ensf338grp26prj-1.2/myLib/datastructures/nodes/
+-rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.2/myLib/datastructures/nodes/DNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.2/myLib/datastructures/nodes/SNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.2/myLib/datastructures/nodes/TNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       74 2023-04-13 18:21:02.000000 ensf338grp26prj-1.2/myLib/datastructures/nodes/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 18:21:24.750326 ensf338grp26prj-1.2/myLib/datastructures/trees/
+-rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.2/myLib/datastructures/trees/AVL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.2/myLib/datastructures/trees/BST.py
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 02:46:47.000000 ensf338grp26prj-1.2/myLib/datastructures/trees/__init__.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 18:21:24.750800 ensf338grp26prj-1.2/setup.cfg
+-rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 18:21:22.000000 ensf338grp26prj-1.2/setup.py
```

### Comparing `ensf338grp26prj-1.1/ensf338grp26prj.egg-info/SOURCES.txt` & `ensf338grp26prj-1.2/ensf338grp26prj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/linear/CDLL.py` & `ensf338grp26prj-1.2/myLib/datastructures/linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/linear/CSLL.py` & `ensf338grp26prj-1.2/myLib/datastructures/linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/linear/DLL.py` & `ensf338grp26prj-1.2/myLib/datastructures/linear/DLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/linear/QueueLL.py` & `ensf338grp26prj-1.2/myLib/datastructures/linear/QueueLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/linear/SLL.py` & `ensf338grp26prj-1.2/myLib/datastructures/linear/SLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/linear/StackLL.py` & `ensf338grp26prj-1.2/myLib/datastructures/linear/StackLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/nodes/DNode.py` & `ensf338grp26prj-1.2/myLib/datastructures/nodes/DNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/nodes/TNode.py` & `ensf338grp26prj-1.2/myLib/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/trees/AVL.py` & `ensf338grp26prj-1.2/myLib/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.1/myLib/datastructures/trees/BST.py` & `ensf338grp26prj-1.2/myLib/datastructures/trees/BST.py`

 * *Files identical despite different names*

