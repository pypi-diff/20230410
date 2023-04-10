# Comparing `tmp/DataStructuresLiamTheodore-1.0.3.tar.gz` & `tmp/DataStructuresLiamTheodore-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataStructuresLiamTheodore-1.0.3.tar", last modified: Sun Apr  9 20:00:17 2023, max compression
+gzip compressed data, was "DataStructuresLiamTheodore-1.0.4.tar", last modified: Mon Apr 10 00:51:25 2023, max compression
```

## Comparing `DataStructuresLiamTheodore-1.0.3.tar` & `DataStructuresLiamTheodore-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.529102 DataStructuresLiamTheodore-1.0.3/
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.523437 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/
--rw-r--r--   0 liammah    (501) staff       (20)      219 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/PKG-INFO
--rw-r--r--   0 liammah    (501) staff       (20)      695 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/SOURCES.txt
--rw-r--r--   0 liammah    (501) staff       (20)        1 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/dependency_links.txt
--rw-r--r--   0 liammah    (501) staff       (20)       15 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/top_level.txt
--rw-r--r--   0 liammah    (501) staff       (20)      219 2023-04-09 20:00:17.528876 DataStructuresLiamTheodore-1.0.3/PKG-INFO
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.523695 DataStructuresLiamTheodore-1.0.3/datastructures/
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.526359 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/
--rw-r--r--   0 liammah    (501) staff       (20)     4017 2023-04-09 02:22:21.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyCLL.py
--rw-r--r--   0 liammah    (501) staff       (20)     8425 2023-04-09 01:57:51.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyLL.py
--rw-r--r--   0 liammah    (501) staff       (20)     2172 2023-04-09 03:32:44.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/LLQueue.py
--rw-r--r--   0 liammah    (501) staff       (20)     1904 2023-04-07 16:54:07.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/LLStack.py
--rw-r--r--   0 liammah    (501) staff       (20)     3977 2023-04-09 03:41:36.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/SinglyCLL.py
--rw-r--r--   0 liammah    (501) staff       (20)     7251 2023-04-07 23:11:54.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/SinglyLL.py
--rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:59:08.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/__init__.py
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.527712 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/
--rw-r--r--   0 liammah    (501) staff       (20)      117 2023-04-07 16:52:52.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/DoublyNode.py
--rw-r--r--   0 liammah    (501) staff       (20)      100 2023-04-07 16:52:52.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/SinglyNode.py
--rw-r--r--   0 liammah    (501) staff       (20)     1754 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/TNode.py
--rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:58:49.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/__init__.py
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.528574 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/
--rw-r--r--   0 liammah    (501) staff       (20)     8558 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/AVL.py
--rw-r--r--   0 liammah    (501) staff       (20)     4797 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/BST.py
--rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:59:44.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/__init__.py
--rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:39:37.000000 DataStructuresLiamTheodore-1.0.3/datastructures/__init__.py
--rw-r--r--   0 liammah    (501) staff       (20)       38 2023-04-09 20:00:17.529183 DataStructuresLiamTheodore-1.0.3/setup.cfg
--rw-r--r--   0 liammah    (501) staff       (20)      333 2023-04-09 20:00:07.000000 DataStructuresLiamTheodore-1.0.3/setup.py
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-10 00:51:25.520999 DataStructuresLiamTheodore-1.0.4/
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-10 00:51:25.512289 DataStructuresLiamTheodore-1.0.4/DataStructuresLiamTheodore.egg-info/
+-rw-r--r--   0 liammah    (501) staff       (20)      236 2023-04-10 00:51:24.000000 DataStructuresLiamTheodore-1.0.4/DataStructuresLiamTheodore.egg-info/PKG-INFO
+-rw-r--r--   0 liammah    (501) staff       (20)      638 2023-04-10 00:51:25.000000 DataStructuresLiamTheodore-1.0.4/DataStructuresLiamTheodore.egg-info/SOURCES.txt
+-rw-r--r--   0 liammah    (501) staff       (20)        1 2023-04-10 00:51:24.000000 DataStructuresLiamTheodore-1.0.4/DataStructuresLiamTheodore.egg-info/dependency_links.txt
+-rw-r--r--   0 liammah    (501) staff       (20)       15 2023-04-10 00:51:25.000000 DataStructuresLiamTheodore-1.0.4/DataStructuresLiamTheodore.egg-info/top_level.txt
+-rw-r--r--   0 liammah    (501) staff       (20)      236 2023-04-10 00:51:25.520671 DataStructuresLiamTheodore-1.0.4/PKG-INFO
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-10 00:51:25.509916 DataStructuresLiamTheodore-1.0.4/datastructures/
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-10 00:51:25.516550 DataStructuresLiamTheodore-1.0.4/datastructures/linear/
+-rw-r--r--   0 liammah    (501) staff       (20)     3425 2023-04-09 22:53:44.000000 DataStructuresLiamTheodore-1.0.4/datastructures/linear/CDLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     3294 2023-04-09 22:47:47.000000 DataStructuresLiamTheodore-1.0.4/datastructures/linear/CSLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     7751 2023-04-09 22:53:44.000000 DataStructuresLiamTheodore-1.0.4/datastructures/linear/DLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     1462 2023-04-09 22:47:47.000000 DataStructuresLiamTheodore-1.0.4/datastructures/linear/QueueLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     7207 2023-04-09 21:36:31.000000 DataStructuresLiamTheodore-1.0.4/datastructures/linear/SLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     1612 2023-04-09 22:47:47.000000 DataStructuresLiamTheodore-1.0.4/datastructures/linear/StackLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:59:08.000000 DataStructuresLiamTheodore-1.0.4/datastructures/linear/__init__.py
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-10 00:51:25.518653 DataStructuresLiamTheodore-1.0.4/datastructures/nodes/
+-rw-r--r--   0 liammah    (501) staff       (20)      118 2023-04-09 21:25:58.000000 DataStructuresLiamTheodore-1.0.4/datastructures/nodes/DNode.py
+-rw-r--r--   0 liammah    (501) staff       (20)      101 2023-04-09 21:26:16.000000 DataStructuresLiamTheodore-1.0.4/datastructures/nodes/SNode.py
+-rw-r--r--   0 liammah    (501) staff       (20)     1754 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.4/datastructures/nodes/TNode.py
+-rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:58:49.000000 DataStructuresLiamTheodore-1.0.4/datastructures/nodes/__init__.py
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-10 00:51:25.520248 DataStructuresLiamTheodore-1.0.4/datastructures/trees/
+-rw-r--r--   0 liammah    (501) staff       (20)     8570 2023-04-09 23:31:16.000000 DataStructuresLiamTheodore-1.0.4/datastructures/trees/AVL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     4820 2023-04-09 23:31:16.000000 DataStructuresLiamTheodore-1.0.4/datastructures/trees/BST.py
+-rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:59:44.000000 DataStructuresLiamTheodore-1.0.4/datastructures/trees/__init__.py
+-rw-r--r--   0 liammah    (501) staff       (20)       38 2023-04-10 00:51:25.521127 DataStructuresLiamTheodore-1.0.4/setup.cfg
+-rw-r--r--   0 liammah    (501) staff       (20)      369 2023-04-09 21:29:43.000000 DataStructuresLiamTheodore-1.0.4/setup.py
```

### Comparing `DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/SOURCES.txt` & `DataStructuresLiamTheodore-1.0.4/DataStructuresLiamTheodore.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 setup.py
 DataStructuresLiamTheodore.egg-info/PKG-INFO
 DataStructuresLiamTheodore.egg-info/SOURCES.txt
 DataStructuresLiamTheodore.egg-info/dependency_links.txt
 DataStructuresLiamTheodore.egg-info/top_level.txt
-datastructures/__init__.py
-datastructures/Linear/DoublyCLL.py
-datastructures/Linear/DoublyLL.py
-datastructures/Linear/LLQueue.py
-datastructures/Linear/LLStack.py
-datastructures/Linear/SinglyCLL.py
-datastructures/Linear/SinglyLL.py
-datastructures/Linear/__init__.py
-datastructures/Nodes/DoublyNode.py
-datastructures/Nodes/SinglyNode.py
-datastructures/Nodes/TNode.py
-datastructures/Nodes/__init__.py
-datastructures/Trees/AVL.py
-datastructures/Trees/BST.py
-datastructures/Trees/__init__.py
+datastructures/linear/CDLL.py
+datastructures/linear/CSLL.py
+datastructures/linear/DLL.py
+datastructures/linear/QueueLL.py
+datastructures/linear/SLL.py
+datastructures/linear/StackLL.py
+datastructures/linear/__init__.py
+datastructures/nodes/DNode.py
+datastructures/nodes/SNode.py
+datastructures/nodes/TNode.py
+datastructures/nodes/__init__.py
+datastructures/trees/AVL.py
+datastructures/trees/BST.py
+datastructures/trees/__init__.py
```

### Comparing `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyCLL.py` & `DataStructuresLiamTheodore-1.0.4/datastructures/linear/CDLL.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,137 +1,112 @@
 from pathlib import Path
 import sys
 parent_dir = Path(__file__).resolve().parent.parent
 sys.path.append(str(parent_dir))
-from Nodes.DoublyNode import Node
-from Linear.DoublyLL import doublyLL
+from nodes.DNode import DNode
+from linear.DLL import DLL
 
-class doublyCLL(doublyLL):
+class CDLL(DLL):
     # Note that you can overload by including the exact same def statement (exact same method name, with same arguments) and when it is called on an instance of the child class, the override method will be called
     def __init__(self, newNode = None):
         self.head = newNode
         self.tail = newNode
         if newNode == None:
             self.size = 0
         else:
             self.head.next = self.head
             self.head.prev = self.head
             self.size = 1
             
-    def insertHead(self, newNode):
-        super().insertHead(newNode)
+    def InsertHead(self, newNode):
+        super().InsertHead(newNode)
         self.tail.next = self.head
         self.head.prev = self.tail
         
 
-    def insertTail(self, newNode):
-        super().insertTail(newNode)
+    def InsertTail(self, newNode):
+        super().InsertTail(newNode)
         self.tail.next = self.head
         self.head.prev = self.tail
 
 
-    def insert(self, newNode, position):
-        super().insert(newNode, position)
+    def Insert(self, newNode, position):
+        super().Insert(newNode, position)
         if position == 1 or position == self.size:
             self.tail.next = self.head
             self.head.prev = self.tail
 
-    def sortedInsert(self, newNode): # INCOMPLETE IMPLEMENTATION
-        sortNeeded = self.isSorted()
+    def SortedInsert(self, newNode): # INCOMPLETE IMPLEMENTATION
+        sortNeeded = self.IsSorted()
         if sortNeeded == False:
-            self.sort()
+            self.Sort()
 
         if self.size == 0:
-            self.insertHead(newNode)
+            self.InsertHead(newNode)
         elif newNode.data < self.head.data:
-            self.insertHead(newNode)
+            self.InsertHead(newNode)
         elif newNode.data > self.tail.data:
-            self.insertTail(newNode)
+            self.InsertTail(newNode)
         else:
             current_node = self.head
             while current_node.next is not self.head and current_node.next.data < newNode.data:
                 current_node = current_node.next
             newNode.prev = current_node
             newNode.next = current_node.next
             current_node.next.prev = newNode
             current_node.next = newNode
             self.size += 1
 
 
-    def isSorted(self):
-        return super().isSorted()
+    def IsSorted(self):
+        return super().IsSorted()
 
-    def sort(self):
+    def Sort(self):
         i = self.head.next
         j = self.head
         for a in range(1, self.size): # a is some random variable to set the loop iterations
             key = i.data
             while j != self.tail and key < j.data:
                 j.next.data = j.data
                 j = j.prev
             j.next.data = key
             i = i.next
             j = i.prev
 
-    def search(self, newNode):
-        return(super().search(newNode))
+    def Search(self, newNode):
+        return(super().Search(newNode))
 
-    def deleteHead(self):
-        super().deleteHead()
+    def DeleteHead(self):
+        super().DeleteHead()
         self.tail.next = self.head
         self.head.prev = self.tail
 
-    def deleteTail(self):
-        super().deleteTail()
+    def DeleteTail(self):
+        super().DeleteTail()
         self.tail.next = self.head
         self.head.prev = self.tail
 
-    def delete(self, delNode):
+    def Delete(self, delNode):
         
-        super().delete(delNode)
+        super().Delete(delNode)
         
         self.tail.next = self.head
         self.head.prev = self.tail
 
-    def clear(self):
-        super().clear()
+    def Clear(self):
+        super().Clear()
 
-    def print(self):
+    def Print(self):
         print(f'The size of this doubly circular linked list is {self.size}.')
-        if self.isSorted():
+        if self.IsSorted():
             print("This doubly circular linked list is sorted.")
-        if not self.isSorted():
+        if not self.IsSorted():
             print("This doubly circular linked list is not sorted.")
         print("This doubly circular linked list contains:")
         current = self.head
         for i in range(self.size):
             print(current.data)
             current = current.next
 
 
 
 
-# def main():
-#     test1 = doublyCLL()
-#     test1.insertHead(Node(1))
-#     test1.insertHead(Node(2))
-#     test1.insertTail(Node(11))
-#     test1.insertTail(Node(7))
-#     test1.insertTail(Node(3))
-#     test1.insertTail(Node(60))
-#     test1.insertTail(Node(4))
-#     print(test1.search(Node(4)))
-#     test1.sort()
-#     test1.print()
-
-#     # test2 = doublyCLL()
-#     # test2.insertHead(Node(4))
-#     # test2.insertHead(Node(3))
-#     # test2.insertHead(Node(2))
-#     # test2.sort()
-#     # test2.print()
-
-# if __name__ == "__main__":
-#     main()
-
-    
-
```

### Comparing `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyLL.py` & `DataStructuresLiamTheodore-1.0.4/datastructures/linear/DLL.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import sys
 from pathlib import Path
 parent_dir = Path(__file__).resolve().parent.parent
 sys.path.append(str(parent_dir))
-from Nodes.DoublyNode import Node
+from nodes.DNode import DNode
 
 # This class does not extend the SLL class as it requires too much rewriting.
 
-class doublyLL:
+class DLL:
     def __init__(self, newNode = None):
         self.head = newNode
         self.tail = newNode
         if newNode == None:
             self.size = 0
         else:
             self.size = 1
 
     # InsertHead(node): Inserts node at the head of the list
-    def insertHead(self, newNode):
+    def InsertHead(self, newNode):
         if self.head is None:
             self.head = newNode
             self.tail = newNode
         else:
             self.head.prev = newNode
             newNode.next = self.head
             self.head = newNode
         self.size += 1
 
 
     # InsertTail(node): Inserts node at the tail of the list
-    def insertTail(self, newNode):
+    def InsertTail(self, newNode):
         if self.head is None:
             self.head = newNode
             self.tail = newNode
         else:
             self.tail.next = newNode
             self.tail.next.prev = self.tail
             self.tail = self.tail.next
         self.size += 1
 
     # Insert(node, position): Inserts node a the specified position
-    def insert(self, newNode, position): # DOUBLE CHECK: ASSUMING THAT THE POSITION STARTS FROM ZERO AND NOT ONE
+    def Insert(self, newNode, position): # DOUBLE CHECK: ASSUMING THAT THE POSITION STARTS FROM ZERO AND NOT ONE
         if position < 1 or position > (self.size + 1):
             print("Error. Out of range. Operation exited.")
         else:
             if self.head is None:
                 self.head = newNode
                 self.tail = newNode
             elif position == 1:
@@ -64,33 +64,33 @@
                 current_node.next.prev = newNode
                 current_node.next = newNode
                 newNode.prev = current_node
 
             self.size += 1
 
     # isSorted(self): Checks the current DLL to see if it is already sorted
-    def isSorted(self): # DOUBLE CHECK: HOW DO WE KNOW THAT IT IS SORTED IN THIS ORDER?
+    def IsSorted(self): # DOUBLE CHECK: HOW DO WE KNOW THAT IT IS SORTED IN THIS ORDER?
         if self.head is None or self.head.next is None:
             return True
         current = self.head
         for i in range(self.size-1):
             if current.next.data < current.data:
                 return False
             current = current.next
         return True
     
     #  SortedInsert(node): Inserts the node into its proper position in a sorted list
-    def sortedInsert(self, newNode):
-        if self.isSorted() == False:
-            self.sort()
+    def SortedInsert(self, newNode):
+        if self.IsSorted() == False:
+            self.Sort()
 
         if self.head is None:
-            self.insertHead(newNode)
+            self.InsertHead(newNode)
         elif newNode.data < self.head.data:
-            self.insertHead(newNode)
+            self.InsertHead(newNode)
         else:
             current_node = self.head
             while current_node.next is not None and current_node.next.data < newNode.data: # We should insert the newNode in the spot after the node this loop stops at
                 current_node = current_node.next
             
             # Insert the item at the found position
             newNode.prev = current_node
@@ -103,74 +103,74 @@
 
             current_node.next = newNode
 
             self.size += 1
             
         
     
-    def search(self, newNode):
+    def Search(self, newNode):
         if self.size == 0:
             return None
 
         current = self.head
         for i in range(self.size):
             if current.data == newNode.data:
                 return current
             else:
                 current = current.next
 
         return None
     
-    def deleteHead(self):
+    def DeleteHead(self):
         if self.head is None:
             print("Error. There are no items in the list.")
         else:
             self.head = self.head.next # Set the head to the next item in the list (or none)
 
             if self.head is not None:
                 self.head.prev = None # So it's not pointing to the old head
             else:
                 self.tail = None # So that tail is not corrupt
             
             self.size -= 1
     
-    def deleteTail(self):
+    def DeleteTail(self):
         if self.tail is None:
             print("Error. There are no items in the list.")
         else:
             self.tail = self.tail.prev
             if self.tail is not None:
                 self.tail.next = None
             else:
                 self.head = None
             self.size -= 1
     
-    def delete(self, delNode):
+    def Delete(self, delNode):
         # DOUBLE CHECK: JUST THE DATA HAS TO MATCH IN ORDER TO DELETE THIS
         # DOUBLE CHECK: IF THE DATA IS THE SAME FOR MANY NODES, DO WE DELETE ALL THE NODES OR JUST THE FIRST ONE?
         if delNode is None:
             return # If the deleted node is nothing
         if self.size == 0:
             return # If the list is empty
         
         else:
             current = self.head
             for i in range(0, self.size):
                 if current == self.head and current.data == delNode.data:
-                    self.deleteHead()
+                    self.DeleteHead()
                 elif current == self.tail and current.data == delNode.data:
-                    self.deleteTail()
+                    self.DeleteTail()
                 elif current.data == delNode.data:
                     current.prev.next = current.next
                     current.next.prev = current.prev
                     self.size -= 1
                 current = current.next
            
     
-    def sort(self):
+    def Sort(self):
         if self.head is None or self.head.next is None:
             return
 
         sorted_tail = self.head  # tail of the sorted portion of the list
         current = self.head.next  # node to be inserted into the sorted portion
 
         while current is not None:
@@ -199,51 +199,24 @@
                     if current.next is not None:
                         current.next.prev = current
             else:
                 sorted_tail = current
 
             current = current.next
     
-    def clear(self):
+    def Clear(self):
         self.head = None
         self.tail = None
         self.size = 0
 
-    def print(self):
+    def Print(self):
         print(f'The size of this doubly linked list is {self.size}.')
-        if self.isSorted():
+        if self.IsSorted():
             print("This doubly linked list is sorted.")
-        if not self.isSorted():
+        if not self.IsSorted():
             print("This doubly linked list is not sorted.")
         print("This doubly linked list contains:")
         current = self.head
         for i in range(self.size):
             print(current.data)
             current = current.next
 
-
-            
-        
-# Test Cases
-# def main():  # Delete later
-#     testDLL = doublyLL()
-#     testNode1 = Node(1)
-#     testNode2 = Node(2)
-#     testNode3 = Node(3)
-#     testNode4 = Node(4)
-#     testNode5 = Node(5)   
-#     testNode6 = Node(6)
-#     testNode6_2 = Node(6)
-#     testNode7 = Node(3)
-#     testDLL.insertTail(testNode1)
-#     testDLL.insertTail(testNode2)
-#     testDLL.insertTail(testNode3) 
-#     testDLL.insertTail(testNode4)
-#     testDLL.insertTail(testNode5,)
-#     testDLL.insertTail(testNode6)
-#     testDLL.insertTail(testNode6_2)
-#     testDLL.insertTail(testNode7)
-#     testDLL.Print()
-
-
-# if  __name__  == "__main__":
-#     main()
```

### Comparing `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/LLStack.py` & `DataStructuresLiamTheodore-1.0.4/datastructures/linear/StackLL.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,65 @@
 import sys
 from pathlib import Path
 parent_dir = Path(__file__).resolve().parent.parent
 sys.path.append(str(parent_dir))
-from Linear.SinglyLL import singlyLL
-from Nodes.SinglyNode import Node
-
-class LLStack(singlyLL):
+from linear.SLL import SLL
+from nodes.SNode import SNode
+class StackLL(SLL):
     def __init__(self, newNode = None):
         super().__init__(newNode)
     
-    def push(self, newNode): # Renamed push
-        super().insertHead(newNode)
+    def Push(self, newNode): # Renamed push
+        super().InsertHead(newNode)
 
-    def insertHead(self, newNode): # For overriding superclass method (now renamed to push)
+    def InsertHead(self, newNode): # For overriding superclass method (now renamed to push)
         return
 
-    def insertTail(self, newNode): # Do nothing
+    def InsertTail(self, newNode): # Do nothing
         return
 
-    def insert(self, newNode, position): # Do nothing
+    def Insert(self, newNode, position): # Do nothing
         return
 
-    def sortedInsert(self, newNode): # Do nothing
+    def SortedInsert(self, newNode): # Do nothing
         return
 
-    def isSorted(self):
-        return super().isSorted()
+    def IsSorted(self):
+        return super().IsSorted()
 
-    def sort(self):
+    def Sort(self):
         return
 
-    def search(self, newNode):
-        return (super().search(newNode))
+    def Search(self, newNode):
+        return (super().Search(newNode))
 
-    def pop(self): # Renamed pop
-        super().deleteHead()
+    def Pop(self): # Renamed pop
+        super().DeleteHead()
     
-    def deleteHead(self): # For overriding superclass method
+    def DeleteHead(self): # For overriding superclass method
         return
 
-    def deleteTail(self): # Do nothing
+    def DeleteTail(self): # Do nothing
         return
 
-    def delete(self, delNode): # Do nothing
+    def Delete(self, delNode): # Do nothing
         return
 
-    def clear(self):
-        super().clear()
+    def Clear(self):
+        super().Clear()
 
-    def print(self):
+    def Print(self):
         print(f'The size of this singly linked list stack is {self.size}.')
-        if self.isSorted():
+        if self.IsSorted():
             print("This singly linked list stack is sorted.")
-        if not self.isSorted():
+        if not self.IsSorted():
             print("This singly linked list stack is not sorted.")
         print("This singly linked list stack contains:")
         current = self.head
         while current != None:
             print(current.data)
             current = current.next
 
-# def main():
-#     # test = LLStack(Node(2))
-#     # test.push(Node(1))
-#     # test.push(Node(3))
-#     # test.pop()
-#     # test.clear()
-#     # newObj = (test.search(Node(1)))
-#     # # print(newObj.data)
-#     # test.print()
 
-# if __name__ == "__main__":
-#     main()
```

### Comparing `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/SinglyLL.py` & `DataStructuresLiamTheodore-1.0.4/datastructures/linear/SLL.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,102 +1,102 @@
 import sys
 from pathlib import Path
 parent_dir = Path(__file__).resolve().parent.parent
 sys.path.append(str(parent_dir))
-from Nodes.SinglyNode import Node
+from nodes.SNode import SNode
 
-class singlyLL():
+class SLL():
 
     def __init__(self, newNode = None):
         if newNode is not None:
             self.head = newNode
             self.tail = newNode
             self.size = 1
         else:
             self.head = None
             self.tail = None
             self.size = 0
             
-    def insertHead(self, newNode):
+    def InsertHead(self, newNode):
         if self.head is None:
             self.head = newNode
             self.tail = newNode
             self.size += 1
         else:
             newNode.next = self.head
             self.head = newNode
             self.size += 1
     
-    def insertTail(self, newNode):
+    def InsertTail(self, newNode):
         if self.tail is None:
             self.head = newNode
             self.tail = newNode
             self.size += 1
         else:
             # newNode.tail = None
             self.tail.next = newNode
             self.tail = newNode
             self.size += 1
 
-    def insert(self, newNode, position):
+    def Insert(self, newNode, position):
         if position < 1 or position > (self.size + 1):
             raise ValueError("Invalid position")
         
         if position == 1:
-            self.insertHead(newNode)
+            self.InsertHead(newNode)
 
         elif position == self.size + 1:
-            self.insertTail(newNode)
+            self.InsertTail(newNode)
 
         else:
             current = self.head
             for i in range(1, position - 1):
                 current = current.next
             newNode.next = current.next
             current.next = newNode
             self.size += 1
 
-    def sortedInsert(self, newNode):
-        sortNeeded = self.isSorted()
+    def SortedInsert(self, newNode):
+        sortNeeded = self.IsSorted()
         if sortNeeded == False:
-            self.sort()
+            self.Sort()
 
         if self.size == 0:
-            self.insertHead(newNode)
+            self.InsertHead(newNode)
 
         else:
             if newNode.data < self.head.data:
-                self.insertHead(newNode)
+                self.InsertHead(newNode)
             elif newNode.data > self.tail.data:
-                self.insertTail(newNode)
+                self.InsertTail(newNode)
             else:
                 current = self.head.next
                 while current.next != self.tail and current.next.data < newNode.data:
                     current = current.next
                 newNode.next = current.next
                 current.next = newNode
                 self.size += 1
                     # if newNode.data > current.data :          
                     #     newNode.next = current.next
                     #     current.next = newNode
                     #     self.size += 1
                     #     break
                     # current = current.next
             
-    def isSorted(self):
+    def IsSorted(self):
         if self.head is None or self.head.next is None:
             return True
         current = self.head
         for i in range(self.size-1):
             if current.next.data < current.data:
                 return False
             current = current.next
         return True
 
-    def sort(self):
+    def Sort(self):
         if self.head == None or self.head.next == None:
             return
         sorted_tail = self.head
         current = self.head.next        
         for i in range(self.size-1):
             if current.data < sorted_tail.data:
                 sorted_tail.next = current.next # Cutting the current node out of the list 
@@ -117,54 +117,54 @@
             current = sorted_tail.next
 
         current = self.head
         for i in range(self.size-1): # better fix probably
             current = current.next
         self.tail = current
 
-    def search(self, newNode):
+    def Search(self, newNode):
         if self.size == 0:
             return None
 
         current = self.head
         for i in range(self.size):
             if current.data == newNode.data:
                 return current
             else:
                 current = current.next
 
         return None
 
-    def deleteHead(self):
+    def DeleteHead(self):
         if self.head is None:
             return
         elif self.head.next is None:
             self.head = None
             self.tail = None
             self.size -= 1
         else:
             self.head = self.head.next
             self.size -= 1
 
-    def deleteTail(self):
+    def DeleteTail(self):
         if self.tail is None:
             return
         current = self.head
 
         if current.next is None:
             self.tail = None
             self.head = None
             self.size -= 1
         while current.next != self.tail:
             current = current.next
         current.next = None
         self.tail = current
         self.size -= 1
 
-    def delete(self, delNode):
+    def Delete(self, delNode):
         if self.size == 0:
             return
         elif self.size == 1:
             if self.head.data == delNode.data:
                 self.head = None
                 self.tail = None
                 self.size -= 1
@@ -176,60 +176,60 @@
                     self.size -= 1
                 
                 if current.next == None:
                     return
                 
                 elif current.next == self.tail:
                     if current.next.data == delNode.data:
-                        self.deleteTail()
+                        self.DeleteTail()
                     return
                 
                 elif current.next.data == delNode.data:
                     current.next = (current.next).next
                     current = current.next
                     self.size -= 1
                 else:
                     current = current.next
     
-    def clear(self):
+    def Clear(self):
         self.head = None
         self.tail = None
         self.size = 0
 
-    def print(self):
+    def Print(self):
         print(f'The size of this singly linked list is {self.size}.')
-        if self.isSorted():
+        if self.IsSorted():
             print("This singly linked list is sorted.")
-        if not self.isSorted():
+        if not self.IsSorted():
             print("This singly linked list is not sorted.")
         print("This singly linked list contains:")
         current = self.head
         while current != None:
             print(current.data)
             current = current.next
         
-# def main():  # Delete later
-#     testNode1 = Node(0)
-#     testNode2 = Node(1)
-#     testNode3 = Node(6)
-#     testNode4 = Node(10)
-#     testNode5 = Node(2)
-#     testNode6 = Node(6)
-
-#     testLL = singlyLL()
-#     testLL.insertTail(testNode1)
-#     testLL.insertTail(testNode2)
-#     testLL.insertTail(testNode3)
-#     testLL.insertTail(testNode4)
-#     testLL.insertTail(testNode6)
-#     testLL.insertTail(testNode5)
-#     testLL.delete(testNode6)
-#     testLL.print()
-# if  __name__  == "__main__":
-#     main()
+def main():  # Delete later
+    testNode1 = SNode(0)
+    testNode2 = SNode(1)
+    testNode3 = SNode(6)
+    testNode4 = SNode(10)
+    testNode5 = SNode(2)
+    testNode6 = SNode(6)
+
+    testLL = SLL()
+    testLL.InsertTail(testNode1)
+    testLL.InsertTail(testNode2)
+    testLL.InsertTail(testNode3)
+    testLL.InsertTail(testNode4)
+    testLL.InsertTail(testNode6)
+    testLL.InsertTail(testNode5)
+    testLL.Delete(testNode6)
+    testLL.Print()
+if  __name__  == "__main__":
+    main()
```

### Comparing `DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/TNode.py` & `DataStructuresLiamTheodore-1.0.4/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.3/datastructures/Trees/AVL.py` & `DataStructuresLiamTheodore-1.0.4/datastructures/trees/AVL.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,245 +1,249 @@
 import sys
 from pathlib import Path
 parent_dir = Path(__file__).resolve().parent.parent
 sys.path.append(str(parent_dir))
-from Trees.BST import BST
-from Nodes.TNode import TNode
+from trees.BST import BST
+from nodes.TNode import TNode
 
 class AVL(BST):
     def __init__(self, arg = None):
         if arg == None:
             super().__init__()
         else:
             super().__init__(arg) # sets newNode as root 
             if self.root.leftChild is not None or self.root.rightChild is not None:
-                node_list = self.inorder_traversal()
+                node_list = self._inorderTraversal()
                 root = node_list[0]
                 self.root = root
                 root.balance = 0
                 root.leftChild = None
                 root.rightChild = None
                 node_list.remove(root)
                 for node in node_list:
                         node.parent = None
                         node.leftChild = None
                         node.rightChild = None
                         node.balance = 0
-                        self.insert(node) 
+                        self.Insert(node) 
     
-    def inorder_traversal(self, node=None, node_list=None):
+    def _inorderTraversal(self, node=None, node_list=None):
         if node_list is None:
             node_list = []
-        if self.getRoot() is None:
+        if self.GetRoot() is None:
             return
         if node is None:
-            node = self.getRoot()
+            node = self.GetRoot()
         queue = [node]
         while queue:
             curr_node = queue.pop(0)
-            left_height = self.get_subtree_height(curr_node.leftChild)
-            right_height = self.get_subtree_height(curr_node.rightChild)
+            left_height = self._getSubtreeHeight(curr_node.leftChild)
+            right_height = self._getSubtreeHeight(curr_node.rightChild)
             curr_node.balance = right_height - left_height
             node_list.append(curr_node)
             if curr_node.leftChild:
                 queue.append(curr_node.leftChild)
             if curr_node.rightChild:
                 queue.append(curr_node.rightChild)
         return node_list
 
-    def get_subtree_height(self, node=None):
+    def _getSubtreeHeight(self, node=None):
         if node is None:
             return -1
-        left_height = self.get_subtree_height(node.leftChild)
-        right_height = self.get_subtree_height(node.rightChild)
+        left_height = self._getSubtreeHeight(node.leftChild)
+        right_height = self._getSubtreeHeight(node.rightChild)
         return 1 + max(left_height, right_height)
 
-    def balance_tree(self, insert):
-        current = self.getRoot()
+    def _balanceTree(self, Insert):
+        current = self.GetRoot()
         pivot = current
         while current is not None:
             if current.balance > 0 or current.balance < 0:
                 pivot = current
-            if insert.data > current.data: # go right
+            if Insert.data > current.data: # go right
                 current = current.rightChild
             else:
                 current = current.leftChild # go left
 
         if pivot.balance == 1 or pivot.balance == -1:
-            if insert.data > pivot.data:
+            if Insert.data > pivot.data:
                 son = pivot.rightChild
             else:
                 son = pivot.leftChild
             ancestor = pivot.parent
 
-            if pivot.balance == 1 and insert.data < pivot.data or pivot.balance == -1 and insert.data > pivot.data: # case 2:
-                self.inorder_traversal()
+            if pivot.balance == 1 and Insert.data < pivot.data or pivot.balance == -1 and Insert.data > pivot.data: # case 2:
+                self._inorderTraversal()
                 return
             
-            insert = self.search(insert.data)
+            Insert = self.Search(Insert.data)
 
-            if pivot.balance < 0 and insert.data <= son.data: # case 3a 
-                self.rightRotate(pivot,son, ancestor, insert)
+            if pivot.balance < 0 and Insert.data <= son.data: # case 3a 
+                self._rightRotate(pivot,son, ancestor, Insert)
             
-            elif pivot.balance > 0 and insert.data> son.data:  # case 3a
-                self.leftRotate(pivot, son, ancestor, insert)
+            elif pivot.balance > 0 and Insert.data> son.data:  # case 3a
+                self._leftRotate(pivot, son, ancestor, Insert)
             
             else:
-                if insert.data > son.data:
+                if Insert.data > son.data:
                     grandson = son.rightChild
                 else:   
                     grandson = son.leftChild
-                if pivot.balance < 0 and insert.data > son.data: # case 3b
-                    self.leftRightRotate(pivot, son, grandson, ancestor,insert)
+                if pivot.balance < 0 and Insert.data > son.data: # case 3b
+                    self._leftRightRotate(pivot, son, grandson, ancestor,Insert)
                 
-                elif pivot.balance > 0 and insert.data < son.data: # case 3b
-                    self.rightLeftRotate(pivot, son, grandson,ancestor, insert)
+                elif pivot.balance > 0 and Insert.data < son.data: # case 3b
+                    self._rightLeftRotate(pivot, son, grandson,ancestor, Insert)
         else: #case 1
-            self.inorder_traversal()
+            self._inorderTraversal()
 
 
-    def rightRotate(self, pivot, son, ancestor, insert):
+    def _rightRotate(self, pivot, son, ancestor, Insert):
         if ancestor is not None:
             if ancestor.data > son.data:
                 ancestor.leftChild = son
             else:
                 ancestor.rightChild = son
             son.parent = ancestor
         pivot.leftChild = son.rightChild
         if son.rightChild is not None:
             son.rightChild.parent = pivot
 
-        if pivot == self.getRoot():
+        if pivot == self.GetRoot():
             # pivot.leftChild = son.rightChild
             self.root = son
             son.parent = None
         son.rightChild = pivot
         pivot.parent = son
         
         #adjust balances
         pivot.balance = 0
-        insert.balance = 0
+        Insert.balance = 0
 
 
-    def leftRotate(self, pivot, son, ancestor, insert):
+    def _leftRotate(self, pivot, son, ancestor, Insert):
         if ancestor is not None:
             if ancestor.data < son.data:
                 ancestor.rightChild = son
             else:
                 ancestor.leftChild = son
             son.parent = ancestor
 
         pivot.rightChild = son.leftChild
         if son.leftChild is not None:
             son.leftChild.parent = pivot
 
-        if pivot == self.getRoot():
+        if pivot == self.GetRoot():
             # pivot.rightChild = son.leftChild
             self.root = son
             son.parent = None
         son.leftChild = pivot
         pivot.parent = son
         
         #adjust balances
         pivot.balance = 0
-        insert.balance = 0
+        Insert.balance = 0
 
-    def rightLeftRotate(self, pivot, son, grandson, ancestor, insert):
-        self.rightRotate(son, grandson, pivot, insert)
-        self.leftRotate(pivot, grandson, ancestor, insert)
-        if insert.balance > grandson.balance:
+    def _rightLeftRotate(self, pivot, son, grandson, ancestor, Insert):
+        self._rightRotate(son, grandson, pivot, Insert)
+        self._leftRotate(pivot, grandson, ancestor, Insert)
+        if Insert.balance > grandson.balance:
             pivot.balance = -1
         else:
             pivot.balance = 0
             son.balance = 1
         
-        temp = insert
-        while (temp != pivot.leftChild and temp != pivot.rightChild  and temp != son.leftChild and temp != son.rightChild) and grandson != insert:
-            right = self.get_subtree_height(temp.rightChild)
-            left = self.get_subtree_height(temp.leftChild)
+        temp = Insert
+        while (temp != pivot.leftChild and temp != pivot.rightChild  and temp != son.leftChild and temp != son.rightChild) and grandson != Insert:
+            right = self._getSubtreeHeight(temp.rightChild)
+            left = self._getSubtreeHeight(temp.leftChild)
             temp.balance = right - left
             temp = temp.parent
 
-    def leftRightRotate(self, pivot, son, grandson,ancestor, insert):
-        self.leftRotate(son,grandson,pivot, insert)
-        self.rightRotate(pivot, grandson, ancestor, insert)
-        if insert.balance < grandson.balance:
+    def _leftRightRotate(self, pivot, son, grandson,ancestor, Insert):
+        self._leftRotate(son,grandson,pivot, Insert)
+        self._rightRotate(pivot, grandson, ancestor, Insert)
+        if Insert.balance < grandson.balance:
             pivot.balance = 1
         else:
             pivot.balance = 0
             son.balance = -1
 
-        temp = insert
-        while (temp != pivot.leftChild and temp != pivot.rightChild  and temp != son.leftChild and temp != son.rightChild) and grandson != insert:
-            right = self.get_subtree_height(temp.rightChild)
-            left = self.get_subtree_height(temp.leftChild)
+        temp = Insert
+        while (temp != pivot.leftChild and temp != pivot.rightChild  and temp != son.leftChild and temp != son.rightChild) and grandson != Insert:
+            right = self._getSubtreeHeight(temp.rightChild)
+            left = self._getSubtreeHeight(temp.leftChild)
             temp.balance = right - left
             temp = temp.parent
 
-    def insert(self, arg):
+    def Insert(self, arg):
         if isinstance(arg, int):
             node = TNode(arg)
         else:
             node = arg
-        self.inorder_traversal()
-        super().insert(node)
-        self.balance_tree(node)
+        self._inorderTraversal()
+        super().Insert(node)
+        self._balanceTree(node)
         
-    def setRoot(self, newNode):
+    def SetRoot(self, newNode):
         if isinstance(newNode, int):
             newRoot = TNode(newNode)
         else:
             newRoot = newNode
-        node_list = self.inorder_traversal() # store prexisting tree
+        node_list = self._inorderTraversal() # store prexisting tree
         if newRoot.leftChild is not None or newRoot.rightChild is not None:
             self.root = newRoot
-            node_list1 = self.inorder_traversal()
+            node_list1 = self._inorderTraversal()
             root = node_list1[0]
             node_list1.remove(root)
             root.balance = 0
             root.leftChild = None
             root.rightChild = None
             for node in node_list1:
                     node.parent = None
                     node.leftChild = None
                     node.rightChild = None
                     node.balance = 0
-                    self.insert(node) 
+                    self.Insert(node) 
 
         if node_list is not None: 
             self.root = newRoot
             for node in node_list:
                 node.parent = None
                 node.leftChild = None
                 node.rightChild = None
                 node.balance = 0
-                self.insert(node)    
+                self.Insert(node)    
         else:
             self.root = newRoot
 
-    def getRoot(self):
-        return super().getRoot()
+    def GetRoot(self):
+        return super().GetRoot()
             
-    def delete(self, data):
-        super().delete(data)
-        node_list = self.inorder_traversal()
+    def Delete(self, data):
+        super().Delete(data)
+        node_list = self._inorderTraversal()
         root = node_list[0]
         self.root = root
         root.balance = 0
         root.leftChild = None
         root.rightChild = None
         node_list.remove(root)
         for node in node_list:
                 node.parent = None
                 node.leftChild = None
                 node.rightChild = None
                 node.balance = 0
-                self.insert(node) 
+                self.Insert(node) 
     
-    def search(self, data):
-        return super().search(data)
+    def Search(self, data):
+        return super().Search(data)
     
     def printInOrder(self):
         super().printInOrder()
     
     def printBF(self):
-        super().printBF()
+        super().printBF()
+
+  
+
+
```

### Comparing `DataStructuresLiamTheodore-1.0.3/datastructures/Trees/BST.py` & `DataStructuresLiamTheodore-1.0.4/datastructures/trees/BST.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from pathlib import Path
 import sys
 parent_dir = Path(__file__).resolve().parent.parent
 sys.path.append(str(parent_dir))
-from Nodes.TNode import TNode
+from nodes.TNode import TNode
 
 class BST:
     def __init__(self, arg = None):
         if arg == None:
             self.root = None
         elif isinstance(arg, int):
             self.root = TNode(arg)
         else: # If the argument is a TNode
             self.root = arg
 
-    def setRoot(self, newRoot):
+    def SetRoot(self, newRoot):
         nodesList = []
         def traverse(node):
             if node is not None:
                 traverse(node.leftChild)
                 nodesList.append(node)
                 traverse(node.rightChild)
         traverse(self.root)
 
         if isinstance(newRoot, int):
             self.root = TNode(newRoot)
         elif isinstance(newRoot, TNode):
             self.root = newRoot
     
         for node in nodesList:
-            self.insert(node)
+            self.Insert(node)
 
-    def getRoot(self):
+    def GetRoot(self):
         return self.root
 
-    def insert(self, arg): 
+    def Insert(self, arg): 
         if isinstance(arg, int):
             node = TNode(arg)
         else: # If the argument is a TNode
             node = arg
         data = node.data
         
         current = self.root
@@ -54,18 +54,18 @@
             self.root = node
         elif data <= parent.data:
             parent.leftChild = TNode(data, parent)
         else:
             parent.rightChild = TNode(data, parent)
     
     # NOTE: NEED TO WRITE UNIT TESTS FOR THE BOUNDARY CASE WHERE THERE ARE MANY NODES WITH THE SAME VALUE
-    # Finds the node with val as data and delete it, if not found prints a statement that the value is not in the tree.
-    def delete(self, value):
+    # Finds the node with val as data and Delete it, if not found prints a statement that the value is not in the tree.
+    def Delete(self, value):
         # if self.root:
-        while self.search(value):
+        while self.Search(value):
             self.root = self._delete(value, self.root)
     
     def _delete(self, value, node): # HELPER METHOD
         if not node:
             return None
         
         if value < node.data:
@@ -85,70 +85,71 @@
     
     def _find_min_node(self, node): # HELPER METHOD
         while node.leftChild:
             node = node.leftChild
         return node
 
 
-    def search(self, val):
+    def Search(self, val):
         current = self.root
         while current is not None:
             if val == current.data:
                 return current
             elif val < current.data:
                 current = current.leftChild
             else:
                 current = current.rightChild
 
+     
     def printInOrder(self):
         def traverse(node):
             if node is not None:
                 traverse(node.leftChild)
-                print(node.data)
+                print(node.toString())
                 traverse(node.rightChild)
         traverse(self.root)
 
     def printBF(self):
         queue = []
         queue.append(self.root)
         current_level_count = 1  # number of nodes in the current level
         next_level_count = 0  # number of nodes in the next level
         while len(queue) > 0:
             current = queue.pop(0) # Remove from the front of the queue
-            print(current.data, end=' ')  # print without new line
+            print(current.toString(), end=' ')  # print without new line
             current_level_count -= 1
             if current.leftChild is not None:
                 queue.append(current.leftChild)
                 next_level_count += 1
             if current.rightChild is not None:
                 queue.append(current.rightChild)
                 next_level_count += 1
             if current_level_count == 0:
                 # All nodes in the current level have been printed
                 # Move to the next line and update counts
                 print()
                 current_level_count = next_level_count
                 next_level_count = 0
 
-    
+        
 
 def main():
     testNode1 = TNode(6)
     testNode2 = TNode(4)
     testNode3 = TNode(9)
     testNode4 = TNode(2)
     testNode5 = TNode(5)   
     testNode6 = TNode(7)
     testNode7 = TNode(3)
     testBST = BST(testNode1)
-    testBST.insert(testNode2)
-    testBST.insert(9)
-    testBST.insert(2)
-    testBST.insert(5)
-    testBST.insert(testNode6)
-    testBST.insert(testNode7)
-    testBST.insert(2)
-    testBST.insert(2)
+    testBST.Insert(testNode2)
+    testBST.Insert(9)
+    testBST.Insert(2)
+    testBST.Insert(5)
+    testBST.Insert(testNode6)
+    testBST.Insert(testNode7)
+    testBST.Insert(2)
+    testBST.Insert(2)
     testBST.printBF()
 
 if  __name__  == "__main__":
-    main()    
+    main()
```

