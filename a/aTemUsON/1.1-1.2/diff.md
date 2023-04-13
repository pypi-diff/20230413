# Comparing `tmp/aTemUsON-1.1.tar.gz` & `tmp/aTemUsON-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aTemUsON-1.1.tar", last modified: Wed Apr 12 22:02:58 2023, max compression
+gzip compressed data, was "aTemUsON-1.2.tar", last modified: Thu Apr 13 03:12:29 2023, max compression
```

## Comparing `aTemUsON-1.1.tar` & `aTemUsON-1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.230475 aTemUsON-1.1/
--rw-r--r--   0 tonytran   (501) staff       (20)      118 2023-04-12 22:02:58.230305 aTemUsON-1.1/PKG-INFO
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.227293 aTemUsON-1.1/aTemUsON.egg-info/
--rw-r--r--   0 tonytran   (501) staff       (20)      118 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/PKG-INFO
--rw-r--r--   0 tonytran   (501) staff       (20)      701 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/SOURCES.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/dependency_links.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/top_level.txt
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.227466 aTemUsON-1.1/myLib/
--rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 aTemUsON-1.1/myLib/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.227639 aTemUsON-1.1/myLib/datastructures/
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:07:04.000000 aTemUsON-1.1/myLib/datastructures/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.228886 aTemUsON-1.1/myLib/datastructures/linear/
--rw-r--r--   0 tonytran   (501) staff       (20)     6671 2023-04-12 19:22:28.000000 aTemUsON-1.1/myLib/datastructures/linear/CDLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8054 2023-04-12 20:25:53.000000 aTemUsON-1.1/myLib/datastructures/linear/CSLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9156 2023-04-12 20:26:54.000000 aTemUsON-1.1/myLib/datastructures/linear/DLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 aTemUsON-1.1/myLib/datastructures/linear/QueueLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9938 2023-04-12 20:23:14.000000 aTemUsON-1.1/myLib/datastructures/linear/SLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 aTemUsON-1.1/myLib/datastructures/linear/StackLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:14:29.000000 aTemUsON-1.1/myLib/datastructures/linear/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.229602 aTemUsON-1.1/myLib/datastructures/nodes/
--rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 aTemUsON-1.1/myLib/datastructures/nodes/DNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 aTemUsON-1.1/myLib/datastructures/nodes/SNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 aTemUsON-1.1/myLib/datastructures/nodes/TNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:15:22.000000 aTemUsON-1.1/myLib/datastructures/nodes/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.230094 aTemUsON-1.1/myLib/datastructures/trees/
--rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 aTemUsON-1.1/myLib/datastructures/trees/AVL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 aTemUsON-1.1/myLib/datastructures/trees/BST.py
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 02:46:47.000000 aTemUsON-1.1/myLib/datastructures/trees/__init__.py
--rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-12 22:02:58.230541 aTemUsON-1.1/setup.cfg
--rw-r--r--   0 tonytran   (501) staff       (20)      215 2023-04-12 22:02:17.000000 aTemUsON-1.1/setup.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 03:12:29.553959 aTemUsON-1.2/
+-rw-r--r--   0 tonytran   (501) staff       (20)      118 2023-04-13 03:12:29.553769 aTemUsON-1.2/PKG-INFO
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 03:12:29.550530 aTemUsON-1.2/aTemUsON.egg-info/
+-rw-r--r--   0 tonytran   (501) staff       (20)      118 2023-04-13 03:12:29.000000 aTemUsON-1.2/aTemUsON.egg-info/PKG-INFO
+-rw-r--r--   0 tonytran   (501) staff       (20)      701 2023-04-13 03:12:29.000000 aTemUsON-1.2/aTemUsON.egg-info/SOURCES.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 03:12:29.000000 aTemUsON-1.2/aTemUsON.egg-info/dependency_links.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 03:12:29.000000 aTemUsON-1.2/aTemUsON.egg-info/top_level.txt
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 03:12:29.550695 aTemUsON-1.2/myLib/
+-rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 aTemUsON-1.2/myLib/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 03:12:29.550858 aTemUsON-1.2/myLib/datastructures/
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:07:04.000000 aTemUsON-1.2/myLib/datastructures/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 03:12:29.552109 aTemUsON-1.2/myLib/datastructures/linear/
+-rw-r--r--   0 tonytran   (501) staff       (20)     6671 2023-04-12 19:22:28.000000 aTemUsON-1.2/myLib/datastructures/linear/CDLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8054 2023-04-12 20:25:53.000000 aTemUsON-1.2/myLib/datastructures/linear/CSLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9156 2023-04-12 20:26:54.000000 aTemUsON-1.2/myLib/datastructures/linear/DLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 aTemUsON-1.2/myLib/datastructures/linear/QueueLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9938 2023-04-12 20:23:14.000000 aTemUsON-1.2/myLib/datastructures/linear/SLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 aTemUsON-1.2/myLib/datastructures/linear/StackLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:14:29.000000 aTemUsON-1.2/myLib/datastructures/linear/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 03:12:29.552825 aTemUsON-1.2/myLib/datastructures/nodes/
+-rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 aTemUsON-1.2/myLib/datastructures/nodes/DNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 aTemUsON-1.2/myLib/datastructures/nodes/SNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 aTemUsON-1.2/myLib/datastructures/nodes/TNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:15:22.000000 aTemUsON-1.2/myLib/datastructures/nodes/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 03:12:29.553520 aTemUsON-1.2/myLib/datastructures/trees/
+-rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 aTemUsON-1.2/myLib/datastructures/trees/AVL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 aTemUsON-1.2/myLib/datastructures/trees/BST.py
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 02:46:47.000000 aTemUsON-1.2/myLib/datastructures/trees/__init__.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 03:12:29.554030 aTemUsON-1.2/setup.cfg
+-rw-r--r--   0 tonytran   (501) staff       (20)      215 2023-04-13 03:12:25.000000 aTemUsON-1.2/setup.py
```

### Comparing `aTemUsON-1.1/aTemUsON.egg-info/SOURCES.txt` & `aTemUsON-1.2/aTemUsON.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/linear/CDLL.py` & `aTemUsON-1.2/myLib/datastructures/linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/linear/CSLL.py` & `aTemUsON-1.2/myLib/datastructures/linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/linear/DLL.py` & `aTemUsON-1.2/myLib/datastructures/linear/DLL.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/linear/QueueLL.py` & `aTemUsON-1.2/myLib/datastructures/linear/QueueLL.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/linear/SLL.py` & `aTemUsON-1.2/myLib/datastructures/linear/SLL.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/linear/StackLL.py` & `aTemUsON-1.2/myLib/datastructures/linear/StackLL.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/nodes/DNode.py` & `aTemUsON-1.2/myLib/datastructures/nodes/DNode.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/nodes/TNode.py` & `aTemUsON-1.2/myLib/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/trees/AVL.py` & `aTemUsON-1.2/myLib/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.1/myLib/datastructures/trees/BST.py` & `aTemUsON-1.2/myLib/datastructures/trees/BST.py`

 * *Files identical despite different names*

