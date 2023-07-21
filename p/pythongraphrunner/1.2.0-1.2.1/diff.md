# Comparing `tmp/pythongraphrunner-1.2.0.tar.gz` & `tmp/pythongraphrunner-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythongraphrunner-1.2.0.tar", max compression
+gzip compressed data, was "pythongraphrunner-1.2.1.tar", max compression
```

## Comparing `pythongraphrunner-1.2.0.tar` & `pythongraphrunner-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-07-19 22:02:57.294835 pythongraphrunner-1.2.0/LICENSE
--rw-r--r--   0        0        0      490 2023-07-20 18:44:24.985859 pythongraphrunner-1.2.0/README.md
--rw-r--r--   0        0        0      405 2023-07-21 20:22:03.044066 pythongraphrunner-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7877 2023-07-21 20:21:47.295405 pythongraphrunner-1.2.0/pythongraphrunner/TaskGraph.py
--rw-r--r--   0        0        0        0 2023-07-21 20:21:47.295405 pythongraphrunner-1.2.0/pythongraphrunner/__init__.py
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 pythongraphrunner-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-19 22:02:57.294835 pythongraphrunner-1.2.1/LICENSE
+-rw-r--r--   0        0        0      490 2023-07-20 18:44:24.985859 pythongraphrunner-1.2.1/README.md
+-rw-r--r--   0        0        0      405 2023-07-21 21:19:54.320641 pythongraphrunner-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8476 2023-07-21 20:22:03.044066 pythongraphrunner-1.2.1/pythongraphrunner/TaskGraph.py
+-rw-r--r--   0        0        0       24 2023-07-21 21:16:41.796275 pythongraphrunner-1.2.1/pythongraphrunner/__init__.py
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 pythongraphrunner-1.2.1/PKG-INFO
```

### Comparing `pythongraphrunner-1.2.0/LICENSE` & `pythongraphrunner-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythongraphrunner-1.2.0/pythongraphrunner/TaskGraph.py` & `pythongraphrunner-1.2.1/pythongraphrunner/TaskGraph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Defines the utilities needed for a task graph
-from typing import Generic, TypeVar, Set, Callable, Optional, Dict, List
+from typing import Generic, TypeVar, Set, Callable, Optional, Dict, List, Tuple
 import uuid
 
 import networkx as nx
 
 class ItemBase:
   """
   This is the base
@@ -65,175 +65,197 @@
     items may be transferred to if an error occurs. These
     are not added to the graph to prevent the planner
     from trying to use these, but are used internally
     to enforce a valid response if an error condition
     is met
   """
   def __init__(self, startStates : List[str], endStates : List[str], errorEndStates : List[str], runner : Callable[ [T], str], id : Optional[str] = None):
-    self.__startStates = startStates
-    self.__endStates = endStates
-    self.__errorEndStates = errorEndStates
-    self.__runner = runner
+    self._startStates = startStates
+    self._endStates = endStates
+    self._errorEndStates = errorEndStates
+    self._runner = runner
 
-    self.__id : str = id if id is not None else uuid.uuid4().hex
+    self._id : str = id if id is not None else uuid.uuid4().hex
 
     # A set for valid outputs
-    self.__validOutputs : Set[str] = set( self.__endStates + self.__errorEndStates )
+    self._validOutputs : Set[str] = set( self._endStates + self._errorEndStates )
   
   # Getters for states
   @property
   def startStates(self) -> List[str]:
-    return self.__startStates
+    return self._startStates
   
   @property
   def endStates(self) -> List[str]:
-    return self.__endStates
+    return self._endStates
 
   @property
   def errorEndStates(self) -> List[str]:
-    return self.__errorEndStates
+    return self._errorEndStates
 
   # Getters for the id and runner
   @property
   def runner(self) -> Callable[ [T], str]:
-    return self.__runner
+    return self._runner
 
   @property
   def id(self) -> str:
-    return self.__id
+    return self._id
 
   def __call__(self, o : T) -> str:
     """
     Calls the internal runner,
     and verifies we exit into a valid
     state.
     """
-    outState = self.__runner(o)
+    outState = self._runner(o)
 
-    if outState not in self.__validOutputs:
+    if outState not in self._validOutputs:
       raise ValueError(f"Invalid output state {outState}!")
     else:
       return outState
 
 class TaskGraph(Generic[T]):
   """
   Represents a task graph. In here
   is a networkx graph, where each state
   is a node, and each edge has a callable
   that transitions between states
   """
   def __init__(self):
     # Constructing our graph
-    self.__graph = nx.DiGraph()
+    self._graph = nx.DiGraph()
     
     # Contains a set of states we allow
-    self.__states : Set[str] = set()
+    self._states : Set[str] = set()
 
     # For right now, I'll expirement with the task
     # graph owning the items. Will see if this works
-    self.__items : Dict[str, T] = {}
+    self._items : Dict[str, T] = {}
 
     # Maintains a set of discrepant items
-    self.__discrepantItems : Set[str] = set()
+    self._discrepantItems : Set[str] = set()
     
   def addState(self, stateName : str):
     """
     Adds a state to the graph
     """
-    self.__states.add(stateName)
-    self.__graph.add_node(stateName)
+    self._states.add(stateName)
+    self._graph.add_node(stateName)
   
   def addStates(self, stateNames : List[str]):
     """
     Adds a list of states to the graph
     """
     for stateName in stateNames:
       self.addState(stateName)
     
   def addEdge(self, taskEdge : TaskEdge[T]):
     """
     Adds an edge to the graph
     """
     # Check if the states are valid
     for state in taskEdge.startStates + taskEdge.endStates + taskEdge.errorEndStates:
-      if state not in self.__states:
+      if state not in self._states:
         raise ValueError(f"State {state} is not in the graph!")
     
     # Add the edge, as a node
-    self.__graph.add_node(taskEdge.id, edgeObj = taskEdge)
+    self._graph.add_node(taskEdge.id, edgeObj = taskEdge)
 
     # Add all edges to the node that aren't error edges
     for startState in taskEdge.startStates:
-      self.__graph.add_edge(startState, taskEdge.id)
+      self._graph.add_edge(startState, taskEdge.id)
     
     # Add all end states to the node
     for endState in taskEdge.endStates:
-      self.__graph.add_edge(taskEdge.id, endState)
+      self._graph.add_edge(taskEdge.id, endState)
   
   def addEdges(self, taskEdges : List[TaskEdge[T]]):
     """
     Adds a list of edges to the graph
     """
     for taskEdge in taskEdges:
       self.addEdge(taskEdge)
   
   def addItem(self, item : T):
     """
     Adds an item to the graph
     """
     # Check if the item is already in the graph
-    if item.id in self.__items:
+    if item.id in self._items:
       raise ValueError(f"Item with id {item.id} is already in the graph!")
     
     # Add the item to the graph
-    self.__items[item.id] = item
+    self._items[item.id] = item
 
     # Check if the item is discrepant, and
     # add it to the set if needed
     if item.isDiscrepant:
-      self.__discrepantItems.add(item.id)
+      self._discrepantItems.add(item.id)
+    
+  def removeItem(self, itemID : str):
+    """
+    Removes an item from the graph
+    """
+    # Check if the item is in the graph
+    if itemID not in self._items:
+      raise ValueError(f"Item with id {itemID} is not in the graph!")
+    
+    # Remove the item from the graph
+    self._items.pop(itemID)
+
+    # Check if the item is discrepant, and
+    # remove it from the set if needed
+    if itemID in self._discrepantItems:
+      self._discrepantItems.remove(itemID)
   
   def getItemCurrState(self, itemID : str) -> str:
-    return self.__items[itemID].currState
+    return self._items[itemID].currState
 
   def getItemDesiredState(self, itemID : str) -> str:
-    return self.__items[itemID].desiredState
+    return self._items[itemID].desiredState
 
   def getItem(self, itemID : str) -> T:
-    return self.__items[itemID]
+    return self._items[itemID]
+  
+  def getItemIDs(self) -> List[str]:
+    return list(self._items.keys())
+  
+  def getItems(self) -> List[ Tuple[str, T] ]:
+    return list(self._items.items())
   
   def updateItemStates(self, itemID : str, currState : str, desiredState : str):
-    if itemID not in self.__items:
+    if itemID not in self._items:
       raise ValueError(f"Item with id {itemID} is not in the graph!")
   
     # Update the item's states
-    self.__items[itemID].currState = currState
-    self.__items[itemID].desiredState = desiredState
+    self._items[itemID].currState = currState
+    self._items[itemID].desiredState = desiredState
 
     # Check if the item is discrepant, and
     # add it to the set if needed
-    if self.__items[itemID].isDiscrepant and itemID not in self.__discrepantItems:
-      self.__discrepantItems.add(itemID)
-    elif not self.__items[itemID].isDiscrepant and itemID in self.__discrepantItems:
-      self.__discrepantItems.remove(itemID)
+    if self._items[itemID].isDiscrepant and itemID not in self._discrepantItems:
+      self._discrepantItems.add(itemID)
+    elif not self._items[itemID].isDiscrepant and itemID in self._discrepantItems:
+      self._discrepantItems.remove(itemID)
   
   def fixItems(self):
     """
     For all discrepant items, run the
     appropriate transition
     """
-    for itemID in self.__discrepantItems:
+    for itemID in self._discrepantItems:
       # Get the item
-      item = self.__items[itemID]
+      item = self._items[itemID]
       startState = item.currState
       endState = item.desiredState
       
       # Determine the shortest path between
       # the current state and desired
-      path : list = list(nx.shortest_path( self.__graph, startState, endState))
+      path : list = list(nx.shortest_path( self._graph, startState, endState))
 
       # The index we're currently at. If
       # the state we enter into, which
       # is the return value from the
       # edge's callable, is not what we
       # expect, a deviation has occurred.
       # In this case, re-compute path and re-run
@@ -243,23 +265,23 @@
       # state, which is the terminal state, is
       # where we are aiming to enter. It doens't make
       # sense to keep on running transitions
       # after we've hit the destination. In that case,
       # change the destination to where you actually
       # want to go
       while idx < len(path) - 1:
-        nextState = self.__graph.nodes[path[idx]]["edgeObj"] (item)
+        nextState = self._graph.nodes[path[idx]]["edgeObj"] (item)
 
         # Set the item's curr state
         item.currState = nextState
 
         if nextState == path[idx + 1]:
           # In this branch, the transition was
           # as planned
           idx += 2
         else:
           # Transition went differently, re-run djkstra's, and
           # set idx to 1
           idx -= idx + 1
 
           path.clear()
-          path = path + list(nx.shortest_path( self.__graph, startState, endState ))
+          path = path + list(nx.shortest_path( self._graph, startState, endState ))
```

### Comparing `pythongraphrunner-1.2.0/PKG-INFO` & `pythongraphrunner-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythongraphrunner
-Version: 1.2.0
+Version: 1.2.1
 Summary: A micro-library that makes it easy to write code that runs as part of a state machine.
 License: MIT
 Author: Adithya Yerramsetty
 Author-email: adithyay@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

