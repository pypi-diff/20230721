# Comparing `tmp/cjm-yolox-pytorch-0.0.98.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.98.tar", last modified: Sat Jul 15 00:11:48 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.99.tar", last modified: Sat Jul 15 00:24:50 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.98.tar` & `cjm-yolox-pytorch-0.0.99.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-15 00:11:48.642591 cjm-yolox-pytorch-0.0.98/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.98/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.98/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-15 00:11:48.642377 cjm-yolox-pytorch-0.0.98/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.98/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-15 00:11:48.639215 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-15 00:11:33.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12639 2023-07-15 00:11:33.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    17716 2023-07-15 00:11:33.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-15 00:11:33.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-15 00:11:33.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3149 2023-07-15 00:11:33.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-15 00:11:48.641836 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-15 00:11:48.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-15 00:11:48.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-15 00:11:48.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-15 00:11:48.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-15 00:11:48.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-15 00:11:48.000000 cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-15 00:11:01.000000 cjm-yolox-pytorch-0.0.98/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-15 00:11:48.642661 cjm-yolox-pytorch-0.0.98/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.98/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-15 00:24:50.577748 cjm-yolox-pytorch-0.0.99/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.99/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.99/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-15 00:24:50.577533 cjm-yolox-pytorch-0.0.99/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.99/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-15 00:24:50.574923 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-15 00:24:39.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12639 2023-07-15 00:24:39.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    17869 2023-07-15 00:24:39.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-15 00:24:39.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-15 00:24:39.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3149 2023-07-15 00:24:39.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-15 00:24:50.577149 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-15 00:24:50.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-15 00:24:50.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-15 00:24:50.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-15 00:24:50.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-15 00:24:50.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-15 00:24:50.000000 cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-15 00:23:55.000000 cjm-yolox-pytorch-0.0.99/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-15 00:24:50.577876 cjm-yolox-pytorch-0.0.99/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.99/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.98/LICENSE` & `cjm-yolox-pytorch-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.98/PKG-INFO` & `cjm-yolox-pytorch-0.0.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.98
+Version: 0.0.99
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.98/README.md` & `cjm-yolox-pytorch-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -214,21 +214,30 @@
             foreground_mask = class_preds.new_zeros(num_output_grid_boxes).bool()
             return (foreground_mask, class_targets, objectness_targets, bbox_targets,
                     l1_targets, 0)  # Return zero for num_positive_per_image
 
         # Calculate the offset for the prior boxes
         offset_output_grid_boxes = torch.cat([output_grid_boxes[:, :2] + output_grid_boxes[:, 2:] * 0.5, output_grid_boxes[:, 2:]], dim=-1)
 
-        # Assign ground truth objects to prior boxes and get assignment results
-        assignment_result = self.assigner.assign(
-            class_preds.sigmoid() * objectness_score.unsqueeze(1).sigmoid(),
-            offset_output_grid_boxes, decoded_bboxes, ground_truth_bboxes, ground_truth_labels)
+        
+        try:
+            
+            # Assign ground truth objects to prior boxes and get assignment results
+            assignment_result = self.assigner.assign(
+                class_preds.sigmoid() * objectness_score.unsqueeze(1).sigmoid(),
+                offset_output_grid_boxes, decoded_bboxes, ground_truth_bboxes, ground_truth_labels)
+        except Exception as e:
+            print("An error occurred with `self.assigner.assign()`\n: ", str(e))
 
-        # Use assignment results to sample prior boxes
-        sampling_result = self.sample(assignment_result, output_grid_boxes, ground_truth_bboxes)
+        
+        try:
+            # Use assignment results to sample prior boxes
+            sampling_result = self.sample(assignment_result, output_grid_boxes, ground_truth_bboxes)
+        except Exception as e:
+            print("An error occurred with `self.sample`\n: ", str(e))
         
         # Get the indices of positive (object-containing) samples
         positive_indices = sampling_result.positive_indices
         num_positive_per_image = positive_indices.size(0)
 
         # Get the maximum IoU values for the positive samples
         positive_ious = assignment_result.max_iou_values[positive_indices]
@@ -238,18 +247,14 @@
 
         # Initialize objectness targets as zeros and set the values at positive_indices to 1
         objectness_targets = torch.zeros_like(objectness_score).unsqueeze(-1)
         objectness_targets[positive_indices] = 1
 
         # Generate bounding box targets
         bbox_targets = sampling_result.positive_ground_truth_bboxes
-        
-        #---------------------------------------
-        print(bbox_targets.shape)
-        #---------------------------------------
 
         # Initialize L1 targets as zeros
         l1_targets = class_preds.new_zeros((num_positive_per_image, 4))
 
         # If use_l1 is True, calculate L1 targets
         if self.use_l1:
             l1_targets = self.get_l1_target(l1_targets, bbox_targets, output_grid_boxes[positive_indices])
```

### Comparing `cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.98/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.99/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.98
+Version: 0.0.99
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.98/settings.ini` & `cjm-yolox-pytorch-0.0.99/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.98
+version = 0.0.99
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.98/setup.py` & `cjm-yolox-pytorch-0.0.99/setup.py`

 * *Files identical despite different names*

