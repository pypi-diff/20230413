# Comparing `tmp/ensf338grp26prj-1.7.tar.gz` & `tmp/ensf338grp26prj-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensf338grp26prj-1.7.tar", last modified: Thu Apr 13 20:04:58 2023, max compression
+gzip compressed data, was "ensf338grp26prj-1.8.tar", last modified: Thu Apr 13 21:17:30 2023, max compression
```

## Comparing `ensf338grp26prj-1.7.tar` & `ensf338grp26prj-1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:58.927722 ensf338grp26prj-1.7/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 20:04:58.927551 ensf338grp26prj-1.7/PKG-INFO
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:58.924142 ensf338grp26prj-1.7/ensf338grp26prj.egg-info/
--rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 20:04:58.000000 ensf338grp26prj-1.7/ensf338grp26prj.egg-info/PKG-INFO
--rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 20:04:58.000000 ensf338grp26prj-1.7/ensf338grp26prj.egg-info/SOURCES.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 20:04:58.000000 ensf338grp26prj-1.7/ensf338grp26prj.egg-info/dependency_links.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 20:04:58.000000 ensf338grp26prj-1.7/ensf338grp26prj.egg-info/top_level.txt
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:58.924322 ensf338grp26prj-1.7/myLib/
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:23.000000 ensf338grp26prj-1.7/myLib/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:58.924454 ensf338grp26prj-1.7/myLib/datastructures/
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 19:59:57.000000 ensf338grp26prj-1.7/myLib/datastructures/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:58.925723 ensf338grp26prj-1.7/myLib/datastructures/linear/
--rw-r--r--   0 tonytran   (501) staff       (20)     6748 2023-04-13 17:35:15.000000 ensf338grp26prj-1.7/myLib/datastructures/linear/CDLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8090 2023-04-13 17:35:15.000000 ensf338grp26prj-1.7/myLib/datastructures/linear/CSLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9148 2023-04-13 17:35:15.000000 ensf338grp26prj-1.7/myLib/datastructures/linear/DLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.7/myLib/datastructures/linear/QueueLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     9948 2023-04-13 17:35:15.000000 ensf338grp26prj-1.7/myLib/datastructures/linear/SLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 ensf338grp26prj-1.7/myLib/datastructures/linear/StackLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)      145 2023-04-13 19:45:04.000000 ensf338grp26prj-1.7/myLib/datastructures/linear/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:58.926540 ensf338grp26prj-1.7/myLib/datastructures/nodes/
--rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.7/myLib/datastructures/nodes/DNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.7/myLib/datastructures/nodes/SNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.7/myLib/datastructures/nodes/TNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)       74 2023-04-13 19:45:09.000000 ensf338grp26prj-1.7/myLib/datastructures/nodes/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:58.927268 ensf338grp26prj-1.7/myLib/datastructures/trees/
--rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.7/myLib/datastructures/trees/AVL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.7/myLib/datastructures/trees/BST.py
--rw-r--r--   0 tonytran   (501) staff       (20)       41 2023-04-13 19:59:24.000000 ensf338grp26prj-1.7/myLib/datastructures/trees/__init__.py
--rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 20:04:58.927782 ensf338grp26prj-1.7/setup.cfg
--rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 20:01:26.000000 ensf338grp26prj-1.7/setup.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.613416 ensf338grp26prj-1.8/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 21:17:30.613200 ensf338grp26prj-1.8/PKG-INFO
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.609265 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/
+-rw-r--r--   0 tonytran   (501) staff       (20)      125 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/PKG-INFO
+-rw-r--r--   0 tonytran   (501) staff       (20)      729 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/SOURCES.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/dependency_links.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-13 21:17:30.000000 ensf338grp26prj-1.8/ensf338grp26prj.egg-info/top_level.txt
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.609490 ensf338grp26prj-1.8/myLib/
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 20:04:23.000000 ensf338grp26prj-1.8/myLib/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.609649 ensf338grp26prj-1.8/myLib/datastructures/
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-13 19:59:57.000000 ensf338grp26prj-1.8/myLib/datastructures/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.610909 ensf338grp26prj-1.8/myLib/datastructures/linear/
+-rw-r--r--   0 tonytran   (501) staff       (20)     6679 2023-04-13 21:11:41.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/CDLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8319 2023-04-13 21:13:01.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/CSLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8984 2023-04-13 21:12:57.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/DLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/QueueLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8110 2023-04-13 21:12:49.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/SLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1952 2023-04-13 21:12:22.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/StackLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      145 2023-04-13 19:45:04.000000 ensf338grp26prj-1.8/myLib/datastructures/linear/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.611928 ensf338grp26prj-1.8/myLib/datastructures/nodes/
+-rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/DNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/SNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/TNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       74 2023-04-13 19:45:09.000000 ensf338grp26prj-1.8/myLib/datastructures/nodes/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-13 21:17:30.612685 ensf338grp26prj-1.8/myLib/datastructures/trees/
+-rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 ensf338grp26prj-1.8/myLib/datastructures/trees/AVL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 ensf338grp26prj-1.8/myLib/datastructures/trees/BST.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       62 2023-04-13 21:16:26.000000 ensf338grp26prj-1.8/myLib/datastructures/trees/__init__.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-13 21:17:30.613482 ensf338grp26prj-1.8/setup.cfg
+-rw-r--r--   0 tonytran   (501) staff       (20)      222 2023-04-13 21:16:32.000000 ensf338grp26prj-1.8/setup.py
```

### Comparing `ensf338grp26prj-1.7/ensf338grp26prj.egg-info/SOURCES.txt` & `ensf338grp26prj-1.8/ensf338grp26prj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/linear/CDLL.py` & `ensf338grp26prj-1.8/myLib/datastructures/linear/CDLL.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,35 +192,38 @@
             return
         
         super().DeleteTail()
         if(self.head is not None):
             self.head.prev = self.tail
             self.tail.next = self.head        
         
+
     def Sort(self):
         """
-        Sorts the nodes in the list in ascending order.
+        Sorts the CDLL using the insertion sort algorithm.
         """
         if self.head is None:
             return
-        
-        # Perform bubble sort
-        for i in range(self.listSize):
-            curr_node = self.head
-            for j in range(self.listSize - i - 1):
-                if curr_node.data > curr_node.next.data:
-                    temp = curr_node.data
-                    curr_node.data = curr_node.next.data
-                    curr_node.next.data = temp
-                    
-                    self.isSorted = False
-                curr_node = curr_node.next
-                
+            
+        curr_node = self.head.next
+        while curr_node != self.head:
+            key = curr_node.data
+            prev_node = curr_node.prev
+            while prev_node != self.head.prev and prev_node.data > key:
+                prev_node.next.data = prev_node.data
+                prev_node = prev_node.prev
+            prev_node.next.data = key
+            curr_node = curr_node.next
         self.isSorted = True
 
+    
+
+    
+
+
     def Print(self):
         """
         Prints the nodes in the list.
         """
         if(self.listSize == 0):
             print("There are no items in the data structure.")
             return
```

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/linear/CSLL.py` & `ensf338grp26prj-1.8/myLib/datastructures/linear/CSLL.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 import os
 import sys
 sys.path.append("..")
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
-from nodes.SNode import SNode
 from linear.SLL import SLL
 
 class CSLL(SLL):
     """
     Circular singly linked list implementation.
     """
     def __init__(self, node=None):
@@ -243,27 +242,35 @@
             self.listSize = 0
             return
 
         self.head = self.head.next
         self.tail.next = self.head
         self.listSize -= 1
     
+
+
+
     def Sort(self):
-        """
-        Sorts the elements of the circular linked list in ascending order.
-        """
-        if self.head is None:
-            return
-        if self.head.next is self.head:
+        if self.head is None or self.head == self.tail:
             return
 
-        sorted = False
-        while not sorted:
-            sorted = True
-            current_node = self.head
-            while current_node.next is not self.head:
-                if current_node.data > current_node.next.data:
-                    current_node.data, current_node.next.data = current_node.next.data, current_node.data
-                    sorted = False
-                current_node = current_node.next
-        self.isSorted = True
+        sorted_tail = self.head
+        unsorted_head = self.head.next
 
+        while unsorted_head != self.head:
+            curr_node = unsorted_head
+            unsorted_head = unsorted_head.next
+
+            if curr_node.data < self.head.data:
+                sorted_tail.next = curr_node.next
+                curr_node.next = self.head
+                self.head = curr_node
+            elif curr_node.data >= sorted_tail.data:
+                sorted_tail = curr_node
+            else:
+                prev_node = self.head
+                while prev_node.next != curr_node and prev_node.next.data <= curr_node.data:
+                    prev_node = prev_node.next
+                sorted_tail.next = curr_node.next
+                curr_node.next = prev_node.next
+                prev_node.next = curr_node
+        self.isSorted = True
```

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/linear/DLL.py` & `ensf338grp26prj-1.8/myLib/datastructures/linear/DLL.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 import os
 import sys
 sys.path.append("..")
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
-from nodes.DNode import DNode
 
 class DLL:
     """
     Doubly linked list implementation.
     """
     def __init__(self, node = None):
         """
@@ -247,65 +246,52 @@
         """
         self.head = None
         self.tail = None  
         self.listSize = 0  
     
     def Sort(self):
         """
-        Sorts a doubly linked list in non-descending order.
-
-        Returns:
-        - None
+        Sorts the nodes in the list in ascending order based on their data.
         """
-        if self.head is None:
+        if self.isSorted:
             return
 
-        sorted_list = None
-        current_node = self.head
+        if self.head is None or self.head.next is None:
+            self.isSorted = True
+            return
 
-        while current_node is not None:
-            next_node = current_node.next
-            sorted_list = self._sorted_insert(sorted_list, current_node)
-            current_node = next_node
-
-        self.head = sorted_list
-        while self.head.prev is not None:
-            self.head = self.head.prev
-        self.isSorted = True
-        
-    def _sorted_insert(self, sorted_list, new_node):
-        """
-        Inserts a new node into a sorted doubly linked list.
+        # start with the second node
+        current_node = self.head.next
 
-        Args:
-        - sorted_list: A node object that represents the head of the sorted list.
-        - new_node: A node object that represents the node to be inserted.
+        while current_node is not None:
+            # get the data of the current node
+            data = current_node.data
 
-        Returns:
-        - A node object that represents the head of the updated sorted list.
-        """
-        if sorted_list is None:
-            new_node.next = None
-            new_node.prev = None
-            return new_node
-
-        if new_node.data < sorted_list.data:
-            new_node.prev = None
-            new_node.next = sorted_list
-            sorted_list.prev = new_node
-            return new_node
+            # find the position to insert the current node
+            insert_node = current_node.prev
+            while insert_node is not None and insert_node.data > data:
+                insert_node = insert_node.prev
+
+            # remove the current node from its current position
+            current_node.prev.next = current_node.next
+            if current_node.next is not None:
+                current_node.next.prev = current_node.prev
+
+            # insert the current node at the correct position
+            if insert_node is None:
+                current_node.prev = None
+                current_node.next = self.head
+                self.head.prev = current_node
+                self.head = current_node
+            else:
+                current_node.prev = insert_node
+                current_node.next = insert_node.next
+                if insert_node.next is not None:
+                    insert_node.next.prev = current_node
+                insert_node.next = current_node
 
-        current_node = sorted_list
-        while current_node.next is not None and current_node.next.data < new_node.data:
+            # move to the next node
             current_node = current_node.next
 
-        new_node.prev = current_node
-        new_node.next = current_node.next
-
-        if current_node.next is not None:
-            current_node.next.prev = new_node
-
-        current_node.next = new_node
-
-        return sorted_list
+        self.isSorted = True
```

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/linear/QueueLL.py` & `ensf338grp26prj-1.8/myLib/datastructures/linear/QueueLL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/linear/SLL.py` & `ensf338grp26prj-1.8/myLib/datastructures/linear/SLL.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 import os
 import sys
 sys.path.append("..")
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
-from nodes.SNode import SNode
 
 class SLL:
     """
     A class representing a singly linked list.
     """
     def __init__(self,node = None):
         """
@@ -178,28 +177,37 @@
                 temp.next = None
                 self.listSize -= 1
                 break
             temp = temp.next
         
     def Sort(self):
         """
-        Sorts the linked list in ascending order using the merge sort algorithm.
+        Sorts the linked list in ascending order using the insertion sort algorithm.
 
         Returns: None
         """
-        if self.head is None:
+        if self.head is None or self.head.next is None:
             return
 
-        left_half, right_half = self._split_list(self.head)
-
-        left_half = self._merge_sort(left_half)
-        right_half = self._merge_sort(right_half)
+        new_head = None
+        current = self.head
+        while current is not None:
+            next_node = current.next
+            if new_head is None or current.data < new_head.data:
+                current.next = new_head
+                new_head = current
+            else:
+                temp = new_head
+                while temp.next is not None and current.data > temp.next.data:
+                    temp = temp.next
+                current.next = temp.next
+                temp.next = current
+            current = next_node
 
-        self.head = self._merge(left_half, right_half)
-        self.tail = self._get_last_node()
+        self.head = new_head
         self.isSorted = True
         
     def Delete(self, data):
         """
         Deletes a node from the linked list that contains the specified data.
 
         Args:
@@ -249,103 +257,15 @@
         self._validate_SNode(node)
         curr_node = self.head  
         while curr_node is not None:
             if curr_node is node:
                 return curr_node
             curr_node = curr_node.next
         return None
-    
-    def _split_list(self, node):
-        """
-        Splits a linked list into two halves.
-
-        Args:
-        - node: The node to start the split from.
-
-        Returns:
-        - Two linked list halves, left and right.
-        """
-        if node is None:
-            return None, None
-
-        slow = node
-        fast = node.next
-
-        while fast is not None:
-            fast = fast.next
-            if fast is not None:
-                slow = slow.next
-                fast = fast.next
-
-        left_half = node
-        right_half = slow.next
-        slow.next = None
-
-        return left_half, right_half
-
-    def _merge_sort(self, node):
-        """
-        Sorts a linked list using the merge sort algorithm.
-
-        Args:
-        - node: The node to start the sort from.
-
-        Returns:
-        - A sorted linked list.
-        """
-        if node is None or node.next is None:
-            return node
-
-        left_half, right_half = self._split_list(node)
-        left_half = self._merge_sort(left_half)
-        right_half = self._merge_sort(right_half)
-        return self._merge(left_half, right_half)
-
-    def _merge(self, left, right):
-        """
-        Merges two linked lists together.
-
-        Args:
-        - left: The left linked list to merge.
-        - right: The right linked list to merge.
-
-        Returns:
-        - A merged linked list.
-        """
-        dummy = SNode(0)
-        tail = dummy
-
-        while left is not None and right is not None:
-            if left.data < right.data:
-                tail.next = left
-                left = left.next
-            else:
-                tail.next = right
-                right = right.next
-            tail = tail.next
-
-        if left is not None:
-            tail.next = left
-        else:
-            tail.next = right
-
-        return dummy.next
-
 
-    def _get_last_node(self):
-        """
-        Returns the last node in the linked list.
-
-        Returns:
-        - The last node object.
-        """
-        current_node = self.tail
-        while current_node.next is not None:
-            current_node = current_node.next
-        return current_node
     
     def Print(self):
         """
         Prints the contents of the linked list.
 
         Returns: None
         """
```

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/linear/StackLL.py` & `ensf338grp26prj-1.8/myLib/datastructures/linear/StackLL.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import sys
 sys.path.append("..")
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
 from linear.SLL import SLL
-from nodes.SNode import SNode
 
 class StackLL(SLL):
     """
     A stack class
     """
     def __init__(self, node=None):
         """
```

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/nodes/DNode.py` & `ensf338grp26prj-1.8/myLib/datastructures/nodes/DNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/nodes/TNode.py` & `ensf338grp26prj-1.8/myLib/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/trees/AVL.py` & `ensf338grp26prj-1.8/myLib/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `ensf338grp26prj-1.7/myLib/datastructures/trees/BST.py` & `ensf338grp26prj-1.8/myLib/datastructures/trees/BST.py`

 * *Files identical despite different names*

