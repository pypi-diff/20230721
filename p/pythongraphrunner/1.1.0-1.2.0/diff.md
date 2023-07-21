# Comparing `tmp/pythongraphrunner-1.1.0.tar.gz` & `tmp/pythongraphrunner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythongraphrunner-1.1.0.tar", max compression
+gzip compressed data, was "pythongraphrunner-1.2.0.tar", max compression
```

## Comparing `pythongraphrunner-1.1.0.tar` & `pythongraphrunner-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-07-19 22:02:57.294835 pythongraphrunner-1.1.0/LICENSE
--rw-r--r--   0        0        0      490 2023-07-20 18:44:24.985859 pythongraphrunner-1.1.0/README.md
--rw-r--r--   0        0        0      405 2023-07-21 09:50:13.559249 pythongraphrunner-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     8527 2023-07-21 09:49:53.374396 pythongraphrunner-1.1.0/src/pythongraphrunner/TaskGraph.py
--rw-r--r--   0        0        0       24 2023-07-21 09:47:41.364121 pythongraphrunner-1.1.0/src/pythongraphrunner/__init__.py
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 pythongraphrunner-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-19 22:02:57.294835 pythongraphrunner-1.2.0/LICENSE
+-rw-r--r--   0        0        0      490 2023-07-20 18:44:24.985859 pythongraphrunner-1.2.0/README.md
+-rw-r--r--   0        0        0      405 2023-07-21 20:22:03.044066 pythongraphrunner-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7877 2023-07-21 20:21:47.295405 pythongraphrunner-1.2.0/pythongraphrunner/TaskGraph.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:21:47.295405 pythongraphrunner-1.2.0/pythongraphrunner/__init__.py
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 pythongraphrunner-1.2.0/PKG-INFO
```

### Comparing `pythongraphrunner-1.1.0/LICENSE` & `pythongraphrunner-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythongraphrunner-1.1.0/src/pythongraphrunner/TaskGraph.py` & `pythongraphrunner-1.2.0/pythongraphrunner/TaskGraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Defines the utilities needed for a task graph
-from typing import Generic, TypeVar, Set, Callable, Optional, Dict, List, Tuple
+from typing import Generic, TypeVar, Set, Callable, Optional, Dict, List
 import uuid
 
 import networkx as nx
 
 class ItemBase:
   """
   This is the base
@@ -187,46 +187,24 @@
     # Add the item to the graph
     self.__items[item.id] = item
 
     # Check if the item is discrepant, and
     # add it to the set if needed
     if item.isDiscrepant:
       self.__discrepantItems.add(item.id)
-    
-  def removeItem(self, itemID : str):
-    """
-    Removes an item from the graph
-    """
-    # Check if the item is in the graph
-    if itemID not in self.__items:
-      raise ValueError(f"Item with id {itemID} is not in the graph!")
-    
-    # Remove the item from the graph
-    self.__items.pop(itemID)
-
-    # Check if the item is discrepant, and
-    # remove it from the set if needed
-    if itemID in self.__discrepantItems:
-      self.__discrepantItems.remove(itemID)
   
   def getItemCurrState(self, itemID : str) -> str:
     return self.__items[itemID].currState
 
   def getItemDesiredState(self, itemID : str) -> str:
     return self.__items[itemID].desiredState
 
   def getItem(self, itemID : str) -> T:
     return self.__items[itemID]
   
-  def getItemIDs(self) -> List[str]:
-    return list(self.__items.keys())
-  
-  def getItems(self) -> List[ Tuple[str, T] ]:
-    return list(self.__items.items())
-  
   def updateItemStates(self, itemID : str, currState : str, desiredState : str):
     if itemID not in self.__items:
       raise ValueError(f"Item with id {itemID} is not in the graph!")
   
     # Update the item's states
     self.__items[itemID].currState = currState
     self.__items[itemID].desiredState = desiredState
```

### Comparing `pythongraphrunner-1.1.0/PKG-INFO` & `pythongraphrunner-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythongraphrunner
-Version: 1.1.0
+Version: 1.2.0
 Summary: A micro-library that makes it easy to write code that runs as part of a state machine.
 License: MIT
 Author: Adithya Yerramsetty
 Author-email: adithyay@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

