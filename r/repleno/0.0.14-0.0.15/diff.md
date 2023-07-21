# Comparing `tmp/repleno-0.0.14.tar.gz` & `tmp/repleno-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repleno-0.0.14.tar", last modified: Thu Jul 20 16:46:48 2023, max compression
+gzip compressed data, was "repleno-0.0.15.tar", last modified: Fri Jul 21 12:19:20 2023, max compression
```

## Comparing `repleno-0.0.14.tar` & `repleno-0.0.15.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-20 16:46:48.092092 repleno-0.0.14/PKG-INFO
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2017 2023-06-26 17:07:24.000000 repleno-0.0.14/README.md
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     1009 2023-07-20 16:44:34.000000 repleno-0.0.14/pyproject.toml
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       38 2023-07-20 16:46:48.092092 repleno-0.0.14/setup.cfg
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/src/
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/src/repleno/
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)    34310 2023-07-20 15:36:30.000000 repleno-0.0.14/src/repleno/SKU.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)      519 2023-06-25 14:02:32.000000 repleno-0.0.14/src/repleno/__init__.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)       96 2023-06-25 14:02:32.000000 repleno-0.0.14/src/repleno/__main__.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)    27547 2023-07-20 16:43:32.000000 repleno-0.0.14/src/repleno/factory.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2310 2023-06-26 18:04:48.000000 repleno-0.0.14/src/repleno/order.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     9575 2023-07-06 16:17:59.000000 repleno-0.0.14/src/repleno/utils.py
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-20 16:46:48.092092 repleno-0.0.14/src/repleno.egg-info/
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/PKG-INFO
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)      330 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/SOURCES.txt
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        1 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/dependency_links.txt
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       28 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/requires.txt
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        8 2023-07-20 16:46:48.000000 repleno-0.0.14/src/repleno.egg-info/top_level.txt
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-21 12:19:20.915044 repleno-0.0.15/PKG-INFO
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2017 2023-06-26 17:07:24.000000 repleno-0.0.15/README.md
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     1009 2023-07-21 12:19:07.000000 repleno-0.0.15/pyproject.toml
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       38 2023-07-21 12:19:20.915044 repleno-0.0.15/setup.cfg
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/src/
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/src/repleno/
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)    35720 2023-07-21 12:11:55.000000 repleno-0.0.15/src/repleno/SKU.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)      519 2023-06-25 14:02:32.000000 repleno-0.0.15/src/repleno/__init__.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)       96 2023-06-25 14:02:32.000000 repleno-0.0.15/src/repleno/__main__.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)    27582 2023-07-21 12:11:40.000000 repleno-0.0.15/src/repleno/factory.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2310 2023-06-26 18:04:48.000000 repleno-0.0.15/src/repleno/order.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     9575 2023-07-06 16:17:59.000000 repleno-0.0.15/src/repleno/utils.py
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/src/repleno.egg-info/
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/PKG-INFO
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)      330 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/SOURCES.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        1 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/dependency_links.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       28 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/requires.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        8 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/top_level.txt
```

### Comparing `repleno-0.0.14/PKG-INFO` & `repleno-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repleno
-Version: 0.0.14
+Version: 0.0.15
 Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
 Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
 Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Manufacturing
```

### Comparing `repleno-0.0.14/README.md` & `repleno-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `repleno-0.0.14/pyproject.toml` & `repleno-0.0.15/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = 'repleno'
-version = '0.0.14'
+version = '0.0.15'
 authors = [
     {'name' = 'Afonso Schulz Albrecht', email = 'a.schulzalbrecht@gmail.com'},
 ]
 description = 'Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)'
 keywords = ['supply chain', 'bill of materials', 'material requirements planning', 'BOM', 'MRP']
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `repleno-0.0.14/src/repleno/SKU.py` & `repleno-0.0.15/src/repleno/SKU.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     def __init__(self, max_stack_size=None):
         self.records = {}
         self._skus = set()
         self._highest_level = None
         self._max_stack_size = max_stack_size
         self._stack_size = 0
+        self._collateral_side = None
 
     def store(self, sku, parent_skus, child_skus, direction, level=0):
         if not isinstance(sku, SKU):
             raise TypeError(f"sku must be an instance of Links, not of {type(sku)}")
 
         if isinstance(parent_skus, SKU):
             parent_skus = [parent_skus]
@@ -76,16 +77,16 @@
             if level < self.records[sku]["sku_level"]:
                 self.records[sku]["sku_level"] = level
 
         if direction == "parents":
             if level > self.records[sku]["sku_level"]:
                 self.records[sku]["sku_level"] = level
 
-    def get_output(self, skus_only=False, attributes=None, hash_keys=False):
-        if skus_only:
+    def get_output(self, items_only=False, attributes=None, hash_keys=False):
+        if items_only:
             skus = self.records.keys()
             return { sku.item if not sku.location else (sku.item, sku.location) for sku in skus}
 
         f_result = deque()
         sku_id_pairs = {}
 
         for sku, val in self.records.items():
@@ -109,14 +110,15 @@
             id_prefix = "id_"  # so ID always starts with letters
             record = {
                 "id": id_prefix + sku_id,
                 "location": sku.location,
                 "item": sku.item,
                 "parents": list(sorted([id_prefix + i for i in parent_ids])),
                 "level": ((-1) * (val["sku_level"] - self._highest_level)) + 1,
+                "normalised_level": val["sku_level"],
             }
 
             if attributes:
                 for attr in attributes:
                     try:
                         record[attr] = getattr(sku, attr)
                     except Exception as e:
@@ -878,85 +880,115 @@
 
         return output.get_output(attributes=attributes)
 
 
     def get_collaterals(
         self,
         include_obsoletes=False,
-        skus_only=False,
+        items_only=False,
         attributes=None,
         max_stack_size=None,
         phaseout_skus=None,
+        child_only=False,
     ):
         """
-        # TODO: complete docstring
-
-        It returns a list of dictionaries with the following keys:
-
-        It generates a list of all items that meet the following criteria:
-            1. Items that use item_code as input material for their produciton;
+        It generates a list of all items identified as collaterals. 
+        An item is considered collateral if it meets the following criteria:
+            1. Items that use item_code as input material for their production;
             2. Items that are used as input material for item_code's production;
-            3. Any indirect items that satisfy the point 1 or 2.
+            3. Any indirect items that satisfy points 1 or 2.
 
         Parameters
         ----------
         include_obsoletes : bool, optional
             Obsolete items are not considered when gathering the collaterals, by
             default False
             
-        skus_only : bool, optional
-            It return a set with the SKU's that are collaterals, by default False
-
+        items_only : bool, optional
+            Returns a list of items that are identified as collaterals, instead
+            of a list of SKUs. By default False.
+            
         attributes : list[str], optional
             Returns the list of dictionaries including the SKU attributes
             specified here. The attributes here must match the SKU attribute
             names, by default None
             
         max_stack_size : int, optional
-            It throws an BufferError if the amount of collaterals collected exceeds
-            the stack size, by default None
-            
+            If the amount of collaterals collected exceeds the `max_stack_size`,
+            a BufferError is thrown. This is useful when the BOM is too large
+            and the method takes too long to run. By default None
+
+        only_child : bool, optional
+            If set to `True`, it ignores all parent items and scan only for
+            child collaterals. By default False
+
+        phaseout_skus : list, optional
+
+
+
         Returns
         -------
         list
-            If skus_only = True, it returns a list with the skus. 
-            Otherwise, it returns a list of dictionaries with the following
-            keys:
-            - # TODO: complete list
-            - + attributes (if specified)
+            If no parameter is passed that changes the output, it returns a list
+            of dictionaries with the following keys:
+                - ID;
+                - location: location of target item;
+                - item: target item;
+                - parents: immediate parents;
+                - level: The target item is assigned a value of 0, while its
+                children are assigned negative numbers (-1, -2, -3..) based on
+                their depth in the BOM, and its parents are assigned positive
+                numbers (+1, +2, +3...) based on their height;
+                
+            Note that the list is self-contained in the sense that all parents
+            have their own IDs in the output.
+            
+            If items_only = True, it returns a list with the collateral items.
 
+            If child_only = True, it searches for collaterals looking only at
+            the child items.
+        
         """
 
         # Breadth-first traversal (BFS) is used because it's easier to think
         # about the logic by levels
 
+        if not phaseout_skus:
+            phaseout_skus = set()
+
         if not include_obsoletes and self.obsolete:
             return []
 
         output = _OutputFormatter(max_stack_size=max_stack_size) 
 
-        output = self._scan_this_and_parents(
-            collaterals=output,
-            include_obsoletes=include_obsoletes,
-            phaseout_set=phaseout_skus
-        )
+        if not child_only:
+            output = self._scan_parents(
+                collaterals=output,
+                include_obsoletes=include_obsoletes,
+                phaseout_set=phaseout_skus
+            )
+
         output = self._scan_children(
             collaterals=output,
             level=0,
             include_obsoletes=include_obsoletes,
             phaseout_set=phaseout_skus
         )
 
-        return output.get_output(skus_only, attributes, skus_only)
+        return output.get_output(items_only, attributes)
 
-    def _scan_this_and_parents(self, collaterals, include_obsoletes, phaseout_set):
+    def _scan_parents(self, collaterals, include_obsoletes, phaseout_set):
         p_collaterals = collaterals
 
-        child_skus = self.children if include_obsoletes else self.active_children  # just to record previous skus
-        queue = [(child_skus, self, 0)]  # (previous_sku, current_sku, level)
+        # Get following nodes
+        selected_parents = self.parents if include_obsoletes else self.active_parents
+        # Remove any SKU that is already in collaterals
+        selected_parents = selected_parents - collaterals._skus        
+        # enqueue (previous_sku, current_sku, level)
+        queue = [(self, sku, 1) for sku in selected_parents]  
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
                 # Filter out obsoletes if needed
                 selected_parents = sku.parents if include_obsoletes else sku.active_parents
 
@@ -965,41 +997,39 @@
                     sku=sku,
                     parent_skus=selected_parents,
                     child_skus=sku_ancestor,
                     level=level,
                     direction="parents",
                 )
 
-
                 # Scan the children and add the result to p_collaterals
-                if self != sku:
-                    p_collaterals = sku._scan_children(
-                        collaterals=p_collaterals, 
-                        level=level, 
-                        include_obsoletes=include_obsoletes,
-                        phaseout_set=phaseout_set
-                    )
+                p_collaterals = sku._scan_children(
+                    collaterals=p_collaterals, 
+                    level=level, 
+                    include_obsoletes=include_obsoletes,
+                    phaseout_set=phaseout_set
+                )
 
                 for parent_node in selected_parents:
                     queue.append((sku, parent_node, level + 1))
 
         return p_collaterals
 
     def _scan_children(self, collaterals, level, include_obsoletes, phaseout_set):
         """
         Check if child items should be part of collaterals when self is being
         obsoleted
         """
 
-        # Start from the children
+        # Get following nodes
         selected_children = self.children if include_obsoletes else self.active_children
         # Remove any SKU that is already in collaterals
         selected_children = selected_children - collaterals._skus        
-
-        queue = [(self, sku, level - 1) for sku in selected_children]
+        # enqueue (previous_sku, current_sku, level)
+        queue = [(self, sku, level - 1) for sku in selected_children]    
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
                 # Logic to see if child should be added
                 unique_parent = len(sku.parents) <= 1
                 endoflife_items = set(collaterals._skus).union(phaseout_set)
```

### Comparing `repleno-0.0.14/src/repleno/__init__.py` & `repleno-0.0.15/src/repleno/__init__.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.14/src/repleno/factory.py` & `repleno-0.0.15/src/repleno/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -701,20 +701,19 @@
             qty = d["qty"]
 
             output.append([item, date_from, date_to, qty])
 
         return output
 
 
-    def get_collaterals(self, target, skus_only=False, phaseouts=None):
-        
+    def get_collaterals(self, target, items_only=False, phaseouts=None, child_only=False): 
         sku = self.get_sku(target)
 
         phaseout_skus = set()
         for i in phaseouts:
             phaseout_skus.add(self.get_sku(i))
 
-        return sku.get_collaterals(skus_only=skus_only, phaseout_skus=phaseout_skus)
+        return sku.get_collaterals(items_only=items_only, phaseout_skus=phaseout_skus, child_only=child_only)
 
 
 def run():
     pass
```

### Comparing `repleno-0.0.14/src/repleno/order.py` & `repleno-0.0.15/src/repleno/order.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.14/src/repleno/utils.py` & `repleno-0.0.15/src/repleno/utils.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.14/src/repleno.egg-info/PKG-INFO` & `repleno-0.0.15/src/repleno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repleno
-Version: 0.0.14
+Version: 0.0.15
 Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
 Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
 Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Manufacturing
```

