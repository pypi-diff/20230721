# Comparing `tmp/SBMLDiagrams-1.3.7.tar.gz` & `tmp/SBMLDiagrams-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SBMLDiagrams-1.3.7.tar", last modified: Wed Jun 28 18:17:49 2023, max compression
+gzip compressed data, was "dist\SBMLDiagrams-1.3.8.tar", last modified: Fri Jul 21 00:28:32 2023, max compression
```

## Comparing `SBMLDiagrams-1.3.7.tar` & `SBMLDiagrams-1.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 18:17:49.386367 SBMLDiagrams-1.3.7/
--rw-rw-rw-   0        0        0     2653 2023-06-28 18:17:49.386367 SBMLDiagrams-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-02-23 20:31:51.000000 SBMLDiagrams-1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 18:17:49.375650 SBMLDiagrams-1.3.7/SBMLDiagrams/
--rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/__init__.py
--rw-rw-rw-   0        0        0       71 2023-06-18 04:43:04.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/_version.py
--rw-rw-rw-   0        0        0   122135 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/drawNetwork.py
--rw-rw-rw-   0        0        0   123007 2023-05-16 21:57:52.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/editSBML.py
--rw-rw-rw-   0        0        0   104489 2023-06-28 17:25:09.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/exportSBML.py
--rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/point.py
--rw-rw-rw-   0        0        0   346538 2023-06-28 18:11:53.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/processSBML.py
--rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/styleSBML.py
--rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/visualizeInfo.py
--rw-rw-rw-   0        0        0   157788 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.7/SBMLDiagrams/visualizeSBML.py
-drwxrwxrwx   0        0        0        0 2023-06-28 18:17:49.384350 SBMLDiagrams-1.3.7/SBMLDiagrams.egg-info/
--rw-rw-rw-   0        0        0     2653 2023-06-28 18:17:49.000000 SBMLDiagrams-1.3.7/SBMLDiagrams.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-28 18:17:49.000000 SBMLDiagrams-1.3.7/SBMLDiagrams.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 18:17:49.000000 SBMLDiagrams-1.3.7/SBMLDiagrams.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-06-28 18:17:49.000000 SBMLDiagrams-1.3.7/SBMLDiagrams.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-28 18:17:49.000000 SBMLDiagrams-1.3.7/SBMLDiagrams.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-28 18:17:49.387378 SBMLDiagrams-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2034 2023-06-08 15:50:51.000000 SBMLDiagrams-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:28:32.197172 SBMLDiagrams-1.3.8/
+-rw-rw-rw-   0        0        0     2653 2023-07-21 00:28:32.198168 SBMLDiagrams-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-02-23 20:31:51.000000 SBMLDiagrams-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 00:28:32.182208 SBMLDiagrams-1.3.8/SBMLDiagrams/
+-rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-07-21 00:26:46.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/_version.py
+-rw-rw-rw-   0        0        0   122135 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/drawNetwork.py
+-rw-rw-rw-   0        0        0   123007 2023-05-16 21:57:52.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/editSBML.py
+-rw-rw-rw-   0        0        0   104713 2023-07-20 22:23:28.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/exportSBML.py
+-rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/point.py
+-rw-rw-rw-   0        0        0   348077 2023-07-21 00:25:58.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/processSBML.py
+-rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/styleSBML.py
+-rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeInfo.py
+-rw-rw-rw-   0        0        0   158660 2023-07-20 22:35:30.000000 SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeSBML.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:28:32.196147 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/
+-rw-rw-rw-   0        0        0     2653 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-21 00:28:31.000000 SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 00:28:32.198168 SBMLDiagrams-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     2034 2023-06-08 15:50:51.000000 SBMLDiagrams-1.3.8/setup.py
```

### Comparing `SBMLDiagrams-1.3.7/PKG-INFO` & `SBMLDiagrams-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.3.7
+Version: 1.3.8
 Summary: Visualize, edit and write SBML files.
 Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
 Author-email: jxu2019@uw.edu
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
```

### Comparing `SBMLDiagrams-1.3.7/README.md` & `SBMLDiagrams-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/__init__.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/drawNetwork.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/drawNetwork.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/editSBML.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/editSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/exportSBML.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/exportSBML.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,16 +303,22 @@
             document.setModel(model)
 
             # create the Compartment and species
             comp_id_list = []
             for i in range(numCompartments):
                 comp_id_list.append(df_CompartmentData.iloc[i]['id']) 
 
+            flag_comp_def = 0
+            for i in range(numNodes):
+                comp_idx = df_NodeData.iloc[i]['comp_idx']
+                if comp_idx == -1:
+                    flag_comp_def = 1
+
             if numCompartments != 0:
-                if "_compartment_default_" not in comp_id_list:
+                if "_compartment_default_" not in comp_id_list and flag_comp_def == 1:
                     compartment = model.createCompartment()
                     comp_id="_compartment_default_"
                     compartment.setId(comp_id)
                     compartment.setConstant(True)
                     compartment.setVolume(1.)
                 for i in range(numCompartments):   
                     compartment = model.createCompartment()
```

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/point.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/point.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/processSBML.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/processSBML.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,24 @@
                             text_dim_w = text_boundingbox.getWidth()
                             text_dim_h = text_boundingbox.getHeight()                       
                             comp_text_content_list.append(text_content)
                             comp_text_position_list.append([text_pos_x, text_pos_y])
                             comp_text_dimension_list.append([text_dim_w, text_dim_h])
 
                 #print(comp_text_content_list)
+                # if "_compartment_default_" in comp_id_list:
+                #     numCompGlyphs -= 1
+                #     idx = comp_id_list.index("_compartment_default_")
+                #     comp_id_list.remove("_compartment_default_")
+                #     del compGlyph_id_list[idx]
+                #     del comp_dimension_list[idx]
+                #     del comp_position_list[idx] 
+                #     del comp_text_content_list[idx]
+                #     del comp_text_position_list[idx]
+                #     del comp_text_dimension_list[idx]
 
                 reaction_id_list = []
                 reactionGlyph_id_list = []
                 reaction_rev_list = []
                 reaction_center_list = []
                 reaction_size_list = []
                 kinetics_list = []
@@ -1797,37 +1807,53 @@
         numBoundaryNodes  = model.getNumBoundarySpecies()
         BoundaryNodes_ids = model.getListOfBoundarySpecies()
         numNodes = numFloatingNodes + numBoundaryNodes
         numRxns   = model.getNumReactions()
         Rxns_ids  = model.getListOfReactionIds()
         numComps  = model.getNumCompartments()
         Comps_ids = model.getListOfCompartmentIds()
+        # if "_compartment_default_" in Comps_ids:
+        #     numComps -= 1
+        #     Comps_ids.remove("_compartment_default_")
         comp_idx_id_list = []
         #Is this the same as comp_node_list?
         numNodes = numFloatingNodes + numBoundaryNodes
         comp_node_list = [0]*numComps #Note: numComps is different from numCompGlyphs
         for i in range(numComps):
             comp_node_list[i] = []
 
         #if there is layout info:
         if len(spec_id_list) != 0 or len(textGlyph_id_list) != 0 or len(gen_id_list) != 0:
+            # comp_specs_in_list = []
+            # for i in range(numComps):
+            #     comp_node_list[i] = []
+            # for i in range(numComps):#only consider the compartment with species in
+            #     for j in range(numFloatingNodes):
+            #         comp_id = model.getCompartmentIdSpeciesIsIn(FloatingNodes_ids[j])
+            #         if comp_id not in comp_specs_in_list:
+            #             comp_specs_in_list.append(comp_id)
+            #     for j in range(numBoundaryNodes):
+            #         comp_id = model.getCompartmentIdSpeciesIsIn(BoundaryNodes_ids[j])
+            #         if comp_id not in comp_specs_in_list:
+            #             comp_specs_in_list.append(comp_id)
             for i in range(numComps):
                 temp_id = Comps_ids[i]
                 comp_idx_id_list.append([i,temp_id])
                 vol= model.getCompartmentVolume(i)
                 if math.isnan(vol):
                     vol = 1.
                 position = [10.,10.]
                 dimension = compartmentDefaultSize
                 comp_fill_color = [255, 255, 255, 255]
                 comp_border_color = [255, 255, 255, 255]
                 comp_border_width = 2.0
                 text_content = ''
                 text_position = [0.,0.]
                 text_dimension = [0.,0.]
+                #if len(comp_id_list) != 0 and temp_id != "_compartment_default_" and (temp_id in comp_specs_in_list):
                 if len(comp_id_list) != 0:
                 #if mplugin is not None:
                     if temp_id == "_compartment_default_":
                         position = [10., 10.]
                         dimension = compartmentDefaultSize
                         #comp_border_color = [255, 255, 255, 255]
                         #comp_fill_color = [255, 255, 255, 255]
```

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/styleSBML.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/styleSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/visualizeInfo.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeInfo.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams/visualizeSBML.py` & `SBMLDiagrams-1.3.8/SBMLDiagrams/visualizeSBML.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,14 +449,24 @@
                                 text_dim_w = text_boundingbox.getWidth()
                                 text_dim_h = text_boundingbox.getHeight()                       
                                 comp_text_content_list.append(text_content)
                                 comp_text_position_list.append([text_pos_x, text_pos_y])
                                 comp_text_dimension_list.append([text_dim_w, text_dim_h])
 
                     #print(comp_text_content_list)
+                    # if "_compartment_default_" in comp_id_list:
+                    #     numCompGlyphs -= 1
+                    #     idx = comp_id_list.index("_compartment_default_")
+                    #     comp_id_list.remove("_compartment_default_")
+                    #     del compGlyph_id_list[idx]
+                    #     del comp_dimension_list[idx]
+                    #     del comp_position_list[idx] 
+                    #     del comp_text_content_list[idx]
+                    #     del comp_text_position_list[idx]
+                    #     del comp_text_dimension_list[idx]
 
                     reaction_id_list = []
                     reactionGlyph_id_list = []
                     reaction_rev_list = []
                     reaction_center_list = []
                     reaction_size_list = []
                     kinetics_list = []
@@ -1259,14 +1269,17 @@
             FloatingNodes_ids = model.getListOfFloatingSpecies()
             numBoundaryNodes  = model.getNumBoundarySpecies()
             BoundaryNodes_ids = model.getListOfBoundarySpecies()
             numRxns   = model.getNumReactions()
             Rxns_ids  = model.getListOfReactionIds()
             numComps  = model.getNumCompartments()
             Comps_ids = model.getListOfCompartmentIds()
+            # if "_compartment_default_" in Comps_ids:
+            #     numComps -= 1
+            #     Comps_ids.remove("_compartment_default_")
             numNodes = numFloatingNodes + numBoundaryNodes
             comp_node_list = [0]*numComps #Note: numComps is different from numCompGlyphs
             comp_specs_in_list = []
             for i in range(numComps):
                 comp_node_list[i] = []
             for i in range(numComps):#only consider the compartment with species in
                 for j in range(numFloatingNodes):
@@ -1288,14 +1301,15 @@
                         position = [0.,0.]
                         comp_fill_color = [255, 255, 255, 255]
                         comp_border_color = [255, 255, 255, 255]
                         comp_border_width = 2.0
                         text_content = ''
                         text_position = [0.,0.]
                         text_dimension = [0.,0.]
+                        #if len(comp_id_list) != 0 and temp_id != "_compartment_default_" and (temp_id in comp_specs_in_list):
                         if len(comp_id_list) != 0:
                         #if mplugin is not None:
                             if temp_id == "_compartment_default_":
                                 dimension = imageSize
                                 color_style.setImageSize(dimension)
                                 position = [0, 0]
                             for j in range(len(comp_id_list)):
```

### Comparing `SBMLDiagrams-1.3.7/SBMLDiagrams.egg-info/PKG-INFO` & `SBMLDiagrams-1.3.8/SBMLDiagrams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.3.7
+Version: 1.3.8
 Summary: Visualize, edit and write SBML files.
 Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
 Author-email: jxu2019@uw.edu
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
```

### Comparing `SBMLDiagrams-1.3.7/setup.py` & `SBMLDiagrams-1.3.8/setup.py`

 * *Files identical despite different names*

