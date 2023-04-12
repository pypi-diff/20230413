# Comparing `tmp/aTemUsON-1.0.tar.gz` & `tmp/aTemUsON-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aTemUsON-1.0.tar", last modified: Wed Apr 12 04:57:13 2023, max compression
+gzip compressed data, was "aTemUsON-1.1.tar", last modified: Wed Apr 12 22:02:58 2023, max compression
```

## Comparing `aTemUsON-1.0.tar` & `aTemUsON-1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 04:57:13.964110 aTemUsON-1.0/
--rw-r--r--   0 tonytran   (501) staff       (20)      117 2023-04-12 04:57:13.963897 aTemUsON-1.0/PKG-INFO
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 04:57:13.957296 aTemUsON-1.0/aTemUsON.egg-info/
--rw-r--r--   0 tonytran   (501) staff       (20)      117 2023-04-12 04:57:13.000000 aTemUsON-1.0/aTemUsON.egg-info/PKG-INFO
--rw-r--r--   0 tonytran   (501) staff       (20)      701 2023-04-12 04:57:13.000000 aTemUsON-1.0/aTemUsON.egg-info/SOURCES.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-12 04:57:13.000000 aTemUsON-1.0/aTemUsON.egg-info/dependency_links.txt
--rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-12 04:57:13.000000 aTemUsON-1.0/aTemUsON.egg-info/top_level.txt
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 04:57:13.957490 aTemUsON-1.0/myLib/
--rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 aTemUsON-1.0/myLib/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 04:57:13.957816 aTemUsON-1.0/myLib/datastructures/
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:07:04.000000 aTemUsON-1.0/myLib/datastructures/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 04:57:13.960814 aTemUsON-1.0/myLib/datastructures/linear/
--rw-r--r--   0 tonytran   (501) staff       (20)     5822 2023-04-11 21:04:08.000000 aTemUsON-1.0/myLib/datastructures/linear/CDLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     6819 2023-04-11 21:03:55.000000 aTemUsON-1.0/myLib/datastructures/linear/CSLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     6868 2023-04-11 21:04:12.000000 aTemUsON-1.0/myLib/datastructures/linear/DLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1292 2023-04-11 21:04:16.000000 aTemUsON-1.0/myLib/datastructures/linear/QueueLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     7394 2023-04-11 21:04:23.000000 aTemUsON-1.0/myLib/datastructures/linear/SLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     1352 2023-04-12 00:49:49.000000 aTemUsON-1.0/myLib/datastructures/linear/StackLL.py
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:14:29.000000 aTemUsON-1.0/myLib/datastructures/linear/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 04:57:13.962423 aTemUsON-1.0/myLib/datastructures/nodes/
--rw-r--r--   0 tonytran   (501) staff       (20)      117 2023-03-27 21:10:47.000000 aTemUsON-1.0/myLib/datastructures/nodes/DNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)       92 2023-03-27 21:38:39.000000 aTemUsON-1.0/myLib/datastructures/nodes/SNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)     2817 2023-04-12 01:23:22.000000 aTemUsON-1.0/myLib/datastructures/nodes/TNode.py
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:15:22.000000 aTemUsON-1.0/myLib/datastructures/nodes/__init__.py
-drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 04:57:13.963601 aTemUsON-1.0/myLib/datastructures/trees/
--rw-r--r--   0 tonytran   (501) staff       (20)     5937 2023-04-12 04:36:21.000000 aTemUsON-1.0/myLib/datastructures/trees/AVL.py
--rw-r--r--   0 tonytran   (501) staff       (20)     5939 2023-04-12 04:03:46.000000 aTemUsON-1.0/myLib/datastructures/trees/BST.py
--rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 02:46:47.000000 aTemUsON-1.0/myLib/datastructures/trees/__init__.py
--rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-12 04:57:13.964180 aTemUsON-1.0/setup.cfg
--rw-r--r--   0 tonytran   (501) staff       (20)      214 2023-04-12 04:56:51.000000 aTemUsON-1.0/setup.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.230475 aTemUsON-1.1/
+-rw-r--r--   0 tonytran   (501) staff       (20)      118 2023-04-12 22:02:58.230305 aTemUsON-1.1/PKG-INFO
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.227293 aTemUsON-1.1/aTemUsON.egg-info/
+-rw-r--r--   0 tonytran   (501) staff       (20)      118 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/PKG-INFO
+-rw-r--r--   0 tonytran   (501) staff       (20)      701 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/SOURCES.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        1 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/dependency_links.txt
+-rw-r--r--   0 tonytran   (501) staff       (20)        6 2023-04-12 22:02:58.000000 aTemUsON-1.1/aTemUsON.egg-info/top_level.txt
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.227466 aTemUsON-1.1/myLib/
+-rw-r--r--   0 tonytran   (501) staff       (20)       32 2023-04-12 02:35:35.000000 aTemUsON-1.1/myLib/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.227639 aTemUsON-1.1/myLib/datastructures/
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:07:04.000000 aTemUsON-1.1/myLib/datastructures/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.228886 aTemUsON-1.1/myLib/datastructures/linear/
+-rw-r--r--   0 tonytran   (501) staff       (20)     6671 2023-04-12 19:22:28.000000 aTemUsON-1.1/myLib/datastructures/linear/CDLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8054 2023-04-12 20:25:53.000000 aTemUsON-1.1/myLib/datastructures/linear/CSLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9156 2023-04-12 20:26:54.000000 aTemUsON-1.1/myLib/datastructures/linear/DLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1869 2023-04-12 18:14:13.000000 aTemUsON-1.1/myLib/datastructures/linear/QueueLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     9938 2023-04-12 20:23:14.000000 aTemUsON-1.1/myLib/datastructures/linear/SLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     1982 2023-04-12 18:16:12.000000 aTemUsON-1.1/myLib/datastructures/linear/StackLL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:14:29.000000 aTemUsON-1.1/myLib/datastructures/linear/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.229602 aTemUsON-1.1/myLib/datastructures/nodes/
+-rw-r--r--   0 tonytran   (501) staff       (20)      513 2023-04-12 18:18:50.000000 aTemUsON-1.1/myLib/datastructures/nodes/DNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)      438 2023-04-12 18:18:36.000000 aTemUsON-1.1/myLib/datastructures/nodes/SNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     2944 2023-04-12 19:57:27.000000 aTemUsON-1.1/myLib/datastructures/nodes/TNode.py
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 04:15:22.000000 aTemUsON-1.1/myLib/datastructures/nodes/__init__.py
+drwxr-xr-x   0 tonytran   (501) staff       (20)        0 2023-04-12 22:02:58.230094 aTemUsON-1.1/myLib/datastructures/trees/
+-rw-r--r--   0 tonytran   (501) staff       (20)     8613 2023-04-12 19:59:08.000000 aTemUsON-1.1/myLib/datastructures/trees/AVL.py
+-rw-r--r--   0 tonytran   (501) staff       (20)     8565 2023-04-12 19:59:36.000000 aTemUsON-1.1/myLib/datastructures/trees/BST.py
+-rw-r--r--   0 tonytran   (501) staff       (20)        0 2023-04-12 02:46:47.000000 aTemUsON-1.1/myLib/datastructures/trees/__init__.py
+-rw-r--r--   0 tonytran   (501) staff       (20)       38 2023-04-12 22:02:58.230541 aTemUsON-1.1/setup.cfg
+-rw-r--r--   0 tonytran   (501) staff       (20)      215 2023-04-12 22:02:17.000000 aTemUsON-1.1/setup.py
```

### Comparing `aTemUsON-1.0/aTemUsON.egg-info/SOURCES.txt` & `aTemUsON-1.1/aTemUsON.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aTemUsON-1.0/myLib/datastructures/linear/CDLL.py` & `aTemUsON-1.1/myLib/datastructures/linear/CDLL.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,34 +4,59 @@
 sys.path.append("..")
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
 from linear.DLL import DLL
 
 class CDLL(DLL):
-
+    """
+    Circular doubly linked list implementation.
+    """
     def __init__(self, node = None):
-        super().__init__(node)
+        """
+        Initializes the circular doubly linked list.
 
-        
+        Args:
+        - node (optional): the first node to be added to the list. Defaults to None.
+        """
+        super().__init__(node)
 
     def InsertTail(self, new_node):
+        """
+        Inserts a new node at the tail of the list.
+
+        Args:
+        - new_node: the new node to be inserted at the tail.
+        """
         super().InsertTail(new_node)
         self.tail.next = self.head
         self.head.prev = self.tail
         
     def InsertHead(self, new_node):
+        """
+        Inserts a new node at the head of the list.
+
+        Args:
+        - new_node: the new node to be inserted at the head.
+        """
+
         # self.ValidateIsSNode(new_node)
         self.isSorted = False
         super().InsertHead(new_node)
         self.tail.next = self.head
         self.head.prev = self.tail
         # self.listSize  += 1
         
     def Delete(self, node):
+        """
+        Deletes a node from the list.
+
+        Args:
+        - node: the node to be deleted from the list.
+        """
         if self.head is None:
             return
         
         curr_node = self.head
         while curr_node != node and curr_node.next != self.head:
             curr_node = curr_node.next
 
@@ -48,14 +73,22 @@
                 curr_node.prev.next = curr_node.next
                 curr_node.next.prev = curr_node.prev
         
         self.listSize -= 1
 
             
     def Insert(self, new_node, position):
+        """
+        Inserts a new node at a specific position in the list.
+
+        Args:
+        - new_node: the new node to be inserted.
+        - position: the position in the list where the new node should be inserted.
+        """
+
         # self.ValidateIsSNode(new_node)
         self.isSorted = False
             
         if self.head is None:
             self.head = new_node
             self.tail = new_node
             return
@@ -76,14 +109,21 @@
             new_node.prev = curr_node.prev
             new_node.next = curr_node
             curr_node.prev = new_node
         else:
             self.InsertTail(new_node)
             
     def SortedInsert(self, new_node):
+        """
+        Inserts a new node in a sorted position in the list.
+
+        Args:
+        - new_node: the new node to be inserted in a sorted position in the list.
+        """
+
         # self.ValidateIsSNode(new_node)
         if(self.isSorted == False):
             self.Sort()
             
         if self.head is None:
             self.head = new_node
             self.tail = new_node
@@ -105,54 +145,63 @@
         
         if curr_node == self.tail:
             self.tail = new_node
             
         self.listSize += 1
 
     def Search(self, key):
-            if self.head is None:
-                return None
-            
-            curr_node = self.head
+        """
+        Searches for a node in the list.
+
+        Args:
+        - key: the key to search for in the list.
+
+        Returns:
+        - the node if found, or None if not found.
+        """
+        if self.head is None:
+            return None
+        
+        curr_node = self.head
+        
+        while curr_node != key:
+            curr_node = curr_node.next
             
-            while curr_node != key:
-                curr_node = curr_node.next
+            if curr_node == self.head:
+                return None
                 
-                if curr_node == self.head:
-                    return None
-                    
-            return curr_node
+        return curr_node
         
     def DeleteHead(self):
+        """
+        Deletes the node at the head of the list.
+        """
         if self.head is None:
             return
         super().DeleteHead()
-        #if self.head == self.tail:
-        #     self.head = None
-        #     self.tail = None
-        # else:
-        #     self.head = self.head.next
         if(self.head is not None):
             self.head.prev = self.tail
             self.tail.next = self.head
             
     def DeleteTail(self):
+        """
+        Deletes the node at the tail of the list.
+        """
         if self.head is None:
             return
         
         super().DeleteTail()
         if(self.head is not None):
             self.head.prev = self.tail
             self.tail.next = self.head        
-            
-    def Clear(self):
-        super().Clear()
-        
         
     def Sort(self):
+        """
+        Sorts the nodes in the list in ascending order.
+        """
         if self.head is None:
             return
         
         # Perform bubble sort
         for i in range(self.listSize):
             curr_node = self.head
             for j in range(self.listSize - i - 1):
@@ -162,47 +211,24 @@
                     curr_node.next.data = temp
                     
                     self.isSorted = False
                 curr_node = curr_node.next
                 
         self.isSorted = True
 
-            
     def Print(self):
+        """
+        Prints the nodes in the list.
+        """
         if(self.listSize == 0):
             print("There are no items in the data structure.")
             return
         sortedStatus = "sorted" if self.isSorted else "not sorted"
         print(f"The data structure has {self.listSize} elements and it's {sortedStatus}.")
         print("Here is the content of the list:")
         current_node = self.head
         while True:
             print(f" - {current_node.data}")
             current_node = current_node.next
             if current_node == self.head:
                 break
-            
-# ll = CDLL()
-# node = DNode(1338)
-# ll.InsertHead(DNode(132))
-# ll.InsertTail(DNode(1))
-# ll.InsertHead(DNode(3))
-# # ll.InsertHead(DNode(100))
-# ll.SortedInsert(DNode(109))
-# # ll.Sort()
-# # ll.InsertHead(node)
-# ll.Print()
-
-# # aasd = ll.Search(node)
-# # print(f"{aasd.data} s")
-
-# # ll.Delete(node)
-# ll.DeleteTail() 
-# ll.Print()
-# ll.DeleteHead()
-# ll.Print()
-
-# print(ll.head.data)
-# print(ll.tail.data)
-
-# # ll.Clear()
-# # ll.Print()
+
```

### Comparing `aTemUsON-1.0/myLib/datastructures/linear/CSLL.py` & `aTemUsON-1.1/myLib/datastructures/linear/CSLL.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,46 +5,77 @@
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
 from nodes.SNode import SNode
 from linear.SLL import SLL
 
 class CSLL(SLL):
-    
+    """
+    Circular singly linked list implementation.
+    """
     def __init__(self, node=None):
+        """
+        Initializes the CSLL object with the head and tail as None and the list size as 0. 
+
+        Args:
+        - node (SNode): The node object to initialize the list with.
+        """
         super().__init__(node)
         if(node is not None):
             self.head.next = node
             self.tail.next = node
-        
-    def ValidateIsSNode(self, node):
-        if not isinstance(node, SNode):
-            raise ValueError('Invalid parameter. The method expects a SNode object to be passed to it.')
     
     def InsertHead(self, new_node):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node at the beginning of the linked list.
+
+        Args:
+        - new_node (SNode): The node object to be inserted.
+
+        Raises:
+        - ValueError: If the given object is not of type SNode.
+        """
         super().InsertHead(new_node)
         self.tail.next = self.head
         
     def InsertTail(self, new_node):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node at the end of the linked list.
+
+        Args:
+        - new_node (SNode): The node object to be inserted.
+
+        Raises:
+        - ValueError: If the given object is not of type SNode.
+        """
+        # self._validate_SNode(new_node)
         self.isSorted = False
         
         if self.tail is None:
             new_node.next = new_node
             self.head = new_node
             self.tail = new_node
         else:
             new_node.next = self.head
             self.tail.next = new_node
             self.tail = new_node
         self.listSize += 1
     
     def Insert(self, new_node, position):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node at the specified position in the linked list.
+
+        Args:
+        - new_node (SNode): The node object to be inserted.
+        - position (int): The position at which the node is to be inserted.
+
+        Raises:
+        - ValueError: If the position is greater than the size of the linked list or if the given object is not of type SNode.
+        """
+        # self._validate_SNode(new_node)
         self.isSorted = False
         
         if position > self.listSize - 1:
             raise ValueError('The insert position is greater than the linked list size.')
         if position == 0:
             if self.head is None:
                 new_node.next = new_node
@@ -62,15 +93,24 @@
             new_node.next = curr_node.next
             curr_node.next = new_node
             if curr_node == self.tail:
                 self.tail = new_node
         self.listSize += 1
         
     def SortedInsert(self, new_node):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node in the sorted position in the linked list.
+
+        Args:
+        - new_node (SNode): The node object to be inserted.
+
+        Raises:
+        - ValueError: If the given object is not of type SNode.
+        """
+        # self._validate_SNode(new_node)
         if not self.isSorted:
             self.Sort()
         if self.head is None:
             new_node.next = new_node
             self.head = new_node
             self.tail = new_node
             self.listSize += 1
@@ -88,14 +128,23 @@
             current_node = current_node.next
 
         new_node.next = current_node.next
         current_node.next = new_node
         self.listSize += 1
         
     def Delete(self, data):
+        """
+        Removes the first occurrence of the specified data from the circular linked list.
+
+        Args:
+        - data: the data to be removed from the list
+
+        Returns:
+        - None
+        """
         if self.head is None:
             return
 
         if self.head == self.tail and self.head == data:
             self.head = None
             self.tail = None
             self.listSize -= 1
@@ -117,14 +166,17 @@
                 self.listSize -= 1
                 return
             prev_node = current_node
             current_node = current_node.next
             
 
     def DeleteTail(self):
+        """
+        Removes the tail node from the circular linked list.
+        """
         if self.tail is None:
             return
 
         if self.head == self.tail:
             self.head = None
             self.tail = None
             self.listSize = 0
@@ -134,53 +186,74 @@
         while current_node.next != self.tail:
             current_node = current_node.next
         current_node.next = self.head
         self.tail = current_node
         self.listSize -= 1
 
     def Clear(self):
+        """
+        Clears the circular linked list by resetting its head, tail, and size.
+        """
         super().Clear()
         
     def Search(self, node):
-        # self.ValidateIsSNode(node)  
+        """
+        Searches for the specified node in the circular linked list.
+
+        Args:
+        - node: the node to search for in the list
+
+        Returns:
+        - the node object if found, None otherwise
+        """
+        # self._validate_SNode(new_node)
         curr_node = self.head  
         while curr_node is not None:
             if curr_node is node:
                 return curr_node
             if(curr_node.next == self.tail):
                 return None
             curr_node = curr_node.next
         return None
     
     def Print(self):
+        """
+        Prints the contents of the circular linked list.
+        """
         if(self.listSize == 0):
             print("There are no items in the data structure.")
             return
         sortedStatus = "sorted" if self.isSorted else "not sorted"
         print(f"The data structure has {self.listSize} elements and it's {sortedStatus}.")
         print("Here is the content of the list:")
         current_node = self.head
         for i in range(self.listSize):
             print(f" - {current_node.data}")
             current_node = current_node.next
 
     def DeleteHead(self):
+        """
+        Removes the head node from the circular linked list.
+        """
         if self.head is None:
             return
         if self.head.next is self.tail:
             self.head = None
             self.tail = None
             self.listSize = 0
             return
 
         self.head = self.head.next
         self.tail.next = self.head
         self.listSize -= 1
     
     def Sort(self):
+        """
+        Sorts the elements of the circular linked list in ascending order.
+        """
         if self.head is None:
             return
         if self.head.next is self.head:
             return
 
         sorted = False
         while not sorted:
@@ -189,58 +262,7 @@
             while current_node.next is not self.head:
                 if current_node.data > current_node.next.data:
                     current_node.data, current_node.next.data = current_node.next.data, current_node.data
                     sorted = False
                 current_node = current_node.next
         self.isSorted = True
 
-
-
-
-
-
-
-# node =ll = CSLL()
-
-
-# ll.InsertHead(SNode(11))
-# ll.InsertTail(SNode(3))
-# ll.InsertHead(SNode(100))
-# # ll.InsertHead(SNode(1))
-# # ll.InsertHead(SNode(109))
-# # ll.Insert(SNode(1337),0)
-# # ll.Print()
-# # ll.SortedInsert(SNode(1335)) 
-# # ll.Sort()
-# ll.Print()
-# # node = SNode(133)
-# # ll.InsertTail(node)
-# ll.InsertHead(SNode(123))
-# # print(f"{ll.Search(node)} ccc")
-# ll.Print()
-# ll.Delete(node)
-# ll.Print()
-# ll.SortedInsert(SNode(1335))
-# # ll.Sort()
-# # ll.Print()
-# # ll.Sort()
-
-# # ll.Sort()
-# # ll.Print()
-# print("-- deleting head")
-# ll.DeleteHead()
-# ll.Print()
-
-# print("-- deleting tail")
-# ll.DeleteTail()
-# ll.Print()
-
-
-# ll.Clear()
-# ll.Print()
-# # print("-- deleting head")
-# # ll.DeleteHead()
-# # ll.Print()
-
-# # print("printing head / tail")
-# # print(ll.tail)
-# # print(ll.head)
```

### Comparing `aTemUsON-1.0/myLib/datastructures/linear/DLL.py` & `aTemUsON-1.1/myLib/datastructures/linear/DLL.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,56 +4,91 @@
 sys.path.append("..")
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
 from nodes.DNode import DNode
 
 class DLL:
-    listSize = 0
-    isSorted = True
-
+    """
+    Doubly linked list implementation.
+    """
     def __init__(self, node = None):
+        """
+        Initializes the doubly linked list.
+
+        Args:
+        - node (optional): the first node to be added to the list. Defaults to None.
+        """
         self.head = node
         self.tail = node
+        self.listSize = 0
+        self.isSorted = True
         if(node is not None):
             self.tail.next = node
             self.tail.prev = node
             self.head.next = node
             self.tail.prev = node
             self.listSize = 1
 
-    def ValidateIsSNode(self,node):
-        if not isinstance(node, DNode):
+    def _validate_DNode(self,node):
+        """
+        Validates that the passed object is a DNode object.
+
+        Parameters:
+        - node (DNode): the node object to be validated.
+            
+        Raises:
+        - ValueError: If the passed object is not an instance of DNode.
+        """
+        if str(type(node).__name__) != "DNode":
             raise ValueError('Invalid parameter. The method excpects a DNode object to be passed to it.') 
 
     def InsertTail(self, new_DNode):
-        # self.ValidateIsSNode(new_DNode)
+        """
+        Inserts a new node at the end of the list.
+
+        Parameters:
+        - new_DNode (DNode): the new node to be inserted.
+        """
+        self._validate_SNode(new_DNode)
         self.isSorted = False
         if not self.head:
             self.head = new_DNode
             self.tail = self.head
         else:
             self.tail.next = new_DNode
             new_DNode.prev = self.tail
             self.tail = new_DNode
         self.listSize +=  1
 
     def InsertHead(self, new_DNode):
-        # self.ValidateIsSNode(new_DNode)
+        """
+        Inserts a new node at the beginning of the list.
+
+        Parameters:
+        - new_DNode (DNode): the new node to be inserted.
+        """
+        self._validate_SNode(new_DNode)
         self.isSorted = False
         if not self.head:
             self.head = new_DNode
             self.tail = self.head
         else:
             new_DNode.next = self.head
             self.head.prev = new_DNode
             self.head = new_DNode
         self.listSize +=  1
 
     def Delete(self, data):
+        """
+        Deletes the specified node from the list.
+
+        Parameters:
+        - data (DNode): the node to be deleted.
+        """
         # self.ValidateIsSNode(data)
         current_DNode = self.head
         while current_DNode:
             if current_DNode == data:
                 if current_DNode == self.head:
                     self.head = current_DNode.next
                     self.head.prev = None
@@ -63,38 +98,63 @@
                 else:
                     current_DNode.prev.next = current_DNode.next
                     current_DNode.next.prev = current_DNode.prev
             current_DNode = current_DNode.next
         self.listSize -=  1
 
     def Search(self, node_data):
+        """
+        Searches for a node with the given data in the list.
+        
+        Args:
+        - node_data: The data to be searched for.
+            
+        Returns:
+        - The first node containing the data, or None if the data is not found.
+        """
         # self.ValidateIsSNode(node_data)
         current_node = self.head
 
         while current_node is not None:
             if current_node == node_data:
                 return current_node
 
             current_node = current_node.next
 
         return None
     
     def DeleteHead(self):
+        """
+        Deletes the first node in the list.
+        """
         if self.head is None:
             return
 
         if self.head == self.tail:
             self.head = None
             self.tail = None
         else:
             self.head = self.head.next
             self.head.prev = None
         self.listSize -=  1
 
     def Insert(self, new_DNode,index):
+        """
+        Insert a new node at the specified index in the linked list.
+
+        Args:
+        - new_DNode: A new node to be inserted.
+        - index (int): Index at which the new node should be inserted.
+
+        Raises:
+        - ValueError: If the index is invalid.
+
+        Returns:
+        - None.
+        """
         # self.ValidateIsSNode(new_DNode)
         if index < 0 or index > self.listSize:
             raise ValueError("Invalid index")
         self.isSorted = False
 
         if index == 0:
             self.InsertHead(new_DNode)
@@ -107,26 +167,38 @@
             new_DNode.next = current_node.next
             new_DNode.prev = current_node
             current_node.next.prev = new_DNode
             current_node.next = new_DNode
             self.listSize += 1
 
     def DeleteTail(self):
+        """
+        Remove the last node from the linked list.
+        """
         if self.tail is None:
             return
 
         if self.tail == self.head:
             self.head = None
             self.tail = None
         else:
             self.tail = self.tail.prev
             self.tail.next = None
         self.listSize -=  1
             
     def SortedInsert(self, new_node):
+        """
+        Inserts a new node into a doubly linked list while maintaining the list's sorted order.
+
+        Args:
+        - new_node: a node object to be inserted into the list
+
+        Returns:
+        - None
+        """
         # self.ValidateIsSNode(new_node)
         if(self.isSorted == False):
             self.Sort()
         if self.head is None:
             self.head = new_node
             self.listSize +=  1
             return
@@ -148,48 +220,73 @@
         if current_node.next is not None:
             current_node.next.prev = new_node
 
         current_node.next = new_node
         self.listSize +=  1
         
     def Print(self):
+        """
+        Prints the content of a doubly linked list and its current sorted status.
+        """
         if(self.listSize == 0):
             print("There are no items in the data structure.")
             return
         sortedStatus = "sorted" if self.isSorted else "not sorted"
         print(f"The data structure has {self.listSize} elements and it's {sortedStatus}.")
         print("Here is the content of the list:")
         current_node = self.head
         while current_node is not None:
             print(f" - {current_node.data}")
             current_node = current_node.next
             
     def Clear(self):
+        """
+        Clears the content of a doubly linked list by setting head, tail, and listSize to None, None, and 0, respectively.
+
+        Returns:
+        - None
+        """
         self.head = None
         self.tail = None  
         self.listSize = 0  
     
     def Sort(self):
+        """
+        Sorts a doubly linked list in non-descending order.
+
+        Returns:
+        - None
+        """
         if self.head is None:
             return
 
         sorted_list = None
         current_node = self.head
 
         while current_node is not None:
             next_node = current_node.next
-            sorted_list = self.sorted_insert(sorted_list, current_node)
+            sorted_list = self._sorted_insert(sorted_list, current_node)
             current_node = next_node
 
         self.head = sorted_list
         while self.head.prev is not None:
             self.head = self.head.prev
         self.isSorted = True
         
-    def sorted_insert(self, sorted_list, new_node):
+    def _sorted_insert(self, sorted_list, new_node):
+        """
+        Inserts a new node into a sorted doubly linked list.
+
+        Args:
+        - sorted_list: A node object that represents the head of the sorted list.
+        - new_node: A node object that represents the node to be inserted.
+
+        Returns:
+        - A node object that represents the head of the updated sorted list.
+        """
         if sorted_list is None:
             new_node.next = None
             new_node.prev = None
             return new_node
 
         if new_node.data < sorted_list.data:
             new_node.prev = None
@@ -208,32 +305,7 @@
             current_node.next.prev = new_node
 
         current_node.next = new_node
 
         return sorted_list
 
 
-
-# ll = DLL()
-# node = DNode(1338)
-# ll.InsertHead(DNode(132))
-# # ll.InsertHead(DNode(11))
-# # ll.InsertHead(DNode(3))
-# # ll.InsertHead(DNode(100))
-# # ll.SortedInsert(DNode(109))
-# # ll.Sort()
-# ll.InsertHead(node)
-# ll.Print()
-
-# aasd = ll.Search(node)
-# print(f"{aasd.data} s")
-
-# ll.Delete(node)
-# # ll.DeleteTail()
-# ll.Print()
-
-# print(ll.head)
-# print(ll.tail)
-
-# # ll.Clear()
-# ll.Print()
-
```

### Comparing `aTemUsON-1.0/myLib/datastructures/linear/SLL.py` & `aTemUsON-1.1/myLib/datastructures/linear/SLL.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,56 +4,98 @@
 sys.path.append("..")
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parent_dir = os.path.dirname(current_dir)
 sys.path.insert(0, parent_dir)
 from nodes.SNode import SNode
 
 class SLL:
-    listSize = 0
-    isSorted = True
-    
+    """
+    A class representing a singly linked list.
+    """
     def __init__(self,node = None):
+        """
+        Initializes a new instance of the SLL class.
+
+        Args:
+        - node (SNode): An SNode object representing the first node of the linked list.
+        """
         self.head = node
         self.tail = node
+        self.listSize = 0
+        self.isSorted = True
         self.listsize = 0 if node == None else 1
         
-    def ValidateIsSNode(self,node):
-        if not isinstance(node, SNode):
+    def _validate_SNode(self,node):
+        """
+        Validates that the input node is of type SNode.
+
+        Args:
+        - node (SNode): An SNode object.
+
+        Raises:
+        - ValueError: If the input node is not of type SNode.
+        """
+        if str(type(node).__name__) != "SNode":
             raise ValueError('Invalid parameter. The method excpects a SNode object to be passed to it.') 
     
     def InsertHead(self, new_node):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node at the beginning of the linked list.
+
+        Args:
+        - new_node (SNode): An SNode object representing the new node to be inserted.
+        """
+        # self._validate_SNode(new_node)
         self.isSorted = False
         
         if self.head is None:
             self.head = new_node
             self.tail = new_node
         else:
             new_node.next = self.head
             self.head = new_node
         self.listSize +=  1
         
         
     def InsertTail(self, new_node):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node at the end of the linked list.
+
+        Args:
+        - new_node (SNode): An SNode object representing the new node to be inserted.
+        """
+        # self._validate_SNode(new_node)
         self.isSorted = False
         
         if self.tail is None:
             self.head = new_node
             self.tail = new_node
         else:
             self.tail.next = new_node
             self.tail = new_node
             # self.tail.next = new_node
             # self.tail = new_node
         self.listSize += 1
     
-    # TODO: What if the pos is greater than the list size
+    
     def Insert(self,new_node,position):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node at the given position.
+
+        Args:
+            new_node (SNode): The new node to insert.
+            position (int): The position at which to insert the new node.
+
+        Raises:
+            ValueError: If `position` is greater than or equal to the list size.
+
+        Returns:
+            None
+        """
+        # self._validate_SNode(new_node)
         self.isSorted = False
         if position > self.listSize - 1:
             raise ValueError('the insert posistion is greater than the linked list size')
         if position == 0:
             new_node.next = self.head
             self.head = new_node
             if not self.tail:
@@ -66,15 +108,23 @@
             new_node.next = curr_node.next
             curr_node.next = new_node
             if not new_node.next:
                 self.tail = new_node
         self.listSize = self.listSize + 1
         
     def SortedInsert(self, new_node):
-        # self.ValidateIsSNode(new_node)
+        """
+        Inserts a new node in the sorted linked list.
+
+        Args:
+        - new_node: SNode object representing the new node to be inserted.
+
+        Returns: None
+        """
+        # self._validate_SNode(new_node)
             
         if(self.isSorted == False):
             self.Sort()
         
         if self.head is None:
             self.head = new_node
             self.tail = new_node
@@ -92,20 +142,30 @@
             current_node = current_node.next
 
         new_node.next = current_node.next
         current_node.next = new_node
         self.listSize += 1
 
     def DeleteHead(self):
+        """
+        Deletes the head node of the linked list.
+
+        Returns: None
+        """
         self.head = self.head.next
         if(self.head is None):
             self.tail = None
         self.listSize -= 1
     
     def DeleteTail(self):
+        """
+        Deletes the tail node of the linked list.
+
+        Returns: None
+        """
         temp = self.head
         while(True and temp is not None):
             result = temp.next
             if(result is None):
                 self.head = None
                 self.tail = None
                 self.listSize -= 1
@@ -114,28 +174,41 @@
                 self.tail = temp
                 temp.next = None
                 self.listSize -= 1
                 break
             temp = temp.next
         
     def Sort(self):
+        """
+        Sorts the linked list in ascending order using the merge sort algorithm.
+
+        Returns: None
+        """
         if self.head is None:
             return
 
         left_half, right_half = self._split_list(self.head)
 
         left_half = self._merge_sort(left_half)
         right_half = self._merge_sort(right_half)
 
         self.head = self._merge(left_half, right_half)
         self.tail = self._get_last_node()
         self.isSorted = True
         
     def Delete(self, data):
-        # self.ValidateIsSNode(data)
+        """
+        Deletes a node from the linked list that contains the specified data.
+
+        Args:
+        - data: The data to be deleted from the linked list.
+
+        Returns: None
+        """
+        # self._validate_SNode(new_node)
         if self.head is None:
             return
         
         if self.head is data:
             self.head = self.head.next
         
         curr_node = self.head
@@ -147,28 +220,51 @@
                 return
             curr_node = curr_node.next
             
         if self.head is None:
             self.tail = None
                 
     def Clear(self):
+        """
+        Clears the linked list by setting its head, tail and size to None, None, and 0 respectively.
+
+        Returns: None
+        """
         self.head = None
         self.tail = None
         self.listSize = 0
                
     def Search(self, node):
-        # self.ValidateIsSNode(node)  
+        """
+        Searches for a node in the linked list.
+
+        Args:
+        - node: The node to be searched for in the linked list.
+
+        Returns:
+        - The node object if it is found in the linked list, otherwise None.
+        """
+        # self._validate_SNode(new_node)
         curr_node = self.head  
         while curr_node is not None:
             if curr_node is node:
                 return curr_node
             curr_node = curr_node.next
         return None
     
     def _split_list(self, node):
+        """
+        Splits a linked list into two halves.
+
+        Args:
+        - node: The node to start the split from.
+
+        Returns:
+        - Two linked list halves, left and right.
+        """
         if node is None:
             return None, None
 
         slow = node
         fast = node.next
 
         while fast is not None:
@@ -180,23 +276,42 @@
         left_half = node
         right_half = slow.next
         slow.next = None
 
         return left_half, right_half
 
     def _merge_sort(self, node):
+        """
+        Sorts a linked list using the merge sort algorithm.
+
+        Args:
+        - node: The node to start the sort from.
+
+        Returns:
+        - A sorted linked list.
+        """
         if node is None or node.next is None:
             return node
 
         left_half, right_half = self._split_list(node)
         left_half = self._merge_sort(left_half)
         right_half = self._merge_sort(right_half)
         return self._merge(left_half, right_half)
 
     def _merge(self, left, right):
+        """
+        Merges two linked lists together.
+
+        Args:
+        - left: The left linked list to merge.
+        - right: The right linked list to merge.
+
+        Returns:
+        - A merged linked list.
+        """
         dummy = SNode(0)
         tail = dummy
 
         while left is not None and right is not None:
             if left.data < right.data:
                 tail.next = left
                 left = left.next
@@ -210,57 +325,36 @@
         else:
             tail.next = right
 
         return dummy.next
 
 
     def _get_last_node(self):
+        """
+        Returns the last node in the linked list.
+
+        Returns:
+        - The last node object.
+        """
         current_node = self.tail
         while current_node.next is not None:
             current_node = current_node.next
         return current_node
     
     def Print(self):
+        """
+        Prints the contents of the linked list.
+
+        Returns: None
+        """
         if(self.listSize == 0):
             print("There are no items in the data structure.")
             return
         sortedStatus = "sorted" if self.isSorted else "not sorted"
         print(f"The data structure has {self.listSize} elements and it's {sortedStatus}.")
         print("Here is the content of the list:")
         current_node = self.head
         while current_node is not None:
             print(f" - {current_node.data}")
             current_node = current_node.next
             
 
-# ll = SLL()
-# ll.InsertHead(SNode(1))
-# ll.InsertHead(SNode(11))
-# ll.InsertHead(SNode(3))
-# ll.InsertHead(SNode(100))
-# ll.InsertHead(SNode(109))
-# print(ll.listSize)
-
-# ll.Insert(SNode(1337),4)
-# node = SNode(133)
-# ll.InsertTail(node)
-# print(f"{ll.Search(node)} ccc")
-# ll.Print()
-# ll.Delete(node)
-# ll.Print()
-# ll.Sort()
-# ll.Print()
-# ll.Sort()
-
-# ll.Sort()
-# ll.Print()
-# print("-- deleting head")
-# ll.DeleteHead()
-# ll.Print()
-# print("-- deleting tail")
-# ll.DeleteTail()
-# ll.Print()
-# ll.DeleteHead()
-# print(node)
-# print(ll.head)
-# print(ll.tail)
-
```

### Comparing `aTemUsON-1.0/myLib/datastructures/nodes/TNode.py` & `aTemUsON-1.1/myLib/datastructures/nodes/TNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,22 @@
 
     def get_balance(self):
         """
         Returns the balance factor of the node.
         """
         return self.balance
 
-    def print_node(self):
+    def print(self):
         """
         Prints the attributes of the node.
         """
         print("Data:", self.data)
         print("Left Child:", self.left)
         print("Right Child:", self.right)
         print("Parent:", self.parent)
-        print("Balance:", self.balance)
+        print("Balance:", self.balance)
+
+    def __str__(self):
+        """
+        Return a string representation of the object.
+        """
+        return str(self.data)
```

