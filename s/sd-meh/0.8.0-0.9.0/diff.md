# Comparing `tmp/sd_meh-0.8.0.tar.gz` & `tmp/sd_meh-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.8.0.tar", max compression
+gzip compressed data, was "sd_meh-0.9.0.tar", max compression
```

## Comparing `sd_meh-0.8.0.tar` & `sd_meh-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-06-19 15:13:33.966544 sd_meh-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     1911 2023-06-19 15:13:33.966544 sd_meh-0.8.0/README.md
--rw-r--r--   0        0        0      390 2023-06-19 15:13:33.966544 sd_meh-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/__init__.py
--rw-r--r--   0        0        0    13427 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/merge.py
--rw-r--r--   0        0        0     6626 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1606 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/model.py
--rw-r--r--   0        0        0    10306 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/presets.py
--rw-r--r--   0        0        0    83496 2023-06-19 15:13:33.966544 sd_meh-0.8.0/sd_meh/rebasin.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 sd_meh-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-21 09:28:13.014860 sd_meh-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     1977 2023-07-21 09:28:13.014860 sd_meh-0.9.0/README.md
+-rw-r--r--   0        0        0      390 2023-07-21 09:28:13.014860 sd_meh-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/__init__.py
+-rw-r--r--   0        0        0    13752 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/merge.py
+-rw-r--r--   0        0        0     6626 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1606 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/model.py
+-rw-r--r--   0        0        0    10306 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/presets.py
+-rw-r--r--   0        0        0    83496 2023-07-21 09:28:13.014860 sd_meh-0.9.0/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 sd_meh-0.9.0/PKG-INFO
```

### Comparing `sd_meh-0.8.0/LICENSE.txt` & `sd_meh-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.8.0/README.md` & `sd_meh-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
 You can have a look at the provided `merge_models.py` cli for an example on how to use the function. Run `python3 merge_models.py --help` for a list of the available arguments.
 
 [Join](https://discord.gg/EZJuBfNVHh) our discord server for discussion and features/bugfix requests
 
 ## Changelog
 
+### 0.9.0
+- bugfixes
+- support for pix2pix and inpainting models
+
 ### 0.8.0
 - add `-bwpab, --block_weights_preset_alpha_b"` and `-pal, --presets_alpha_lambda` for presets interpolation (same for `beta`)
 - add `-ll, --logging_level`, default to `INFO`
 
 ### 0.7.0
 - add `-bwpa, --block_weights_preset_alpha` and `-bwpb, --block_weights_preset_beta` to use pre-defined merging weights. Have a look at the [wiki](https://github.com/s1dlx/meh/wiki/Presets) for all the presets
 - add `-wd, --work_device`
```

### Comparing `sd_meh-0.8.0/sd_meh/merge.py` & `sd_meh-0.9.0/sd_meh/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -405,37 +405,49 @@
 
         try:
             merge_method = getattr(merge_methods, merge_mode)
         except AttributeError as e:
             raise ValueError(f"{merge_mode} not implemented, aborting merge!") from e
 
         merge_args = get_merge_method_args(current_bases, thetas, key, work_device)
-        merged_key = merge_method(**merge_args).to(device)
+
+        # dealing wiht pix2pix and inpainting models
+        if (a_size := merge_args["a"].size()) != (b_size := merge_args["b"].size()):
+            print(key, a_size, b_size)
+            if a_size[1] > b_size[1]:
+                merged_key = merge_args["a"]
+            else:
+                merged_key = merge_args["b"]
+        else:
+            merged_key = merge_method(**merge_args).to(device)
 
         if weights_clip:
-            t0 = thetas["model_a"][key]
-            t1 = thetas["model_b"][key]
-            threshold = torch.maximum(torch.abs(t0), torch.abs(t1))
-            merged_key = torch.minimum(torch.maximum(merged_key, -threshold), threshold)
+            merged_key = clip_weights_key(thetas, merged_key, key)
 
         if precision == 16:
             merged_key = merged_key.half()
 
         return merged_key
 
 
 def clip_weights(thetas, merged):
-    for k, t0 in thetas["model_a"].items():
+    for k in thetas["model_a"].keys():
         if k in thetas["model_b"].keys():
-            t1 = thetas["model_b"][k]
-            th = torch.maximum(torch.abs(t0), torch.abs(t1))
-            merged.update({k: torch.minimum(torch.maximum(merged[k], -th), th)})
+            merged.update({k: clip_weights_key(thetas, merged[k], k)})
     return merged
 
 
+def clip_weights_key(thetas, merged_weights, key):
+    t0 = thetas["model_a"][key]
+    t1 = thetas["model_b"][key]
+    maximums = torch.maximum(t0, t1)
+    minimums = torch.minimum(t0, t1)
+    return torch.minimum(torch.maximum(merged_weights, minimums), maximums)
+
+
 @contextmanager
 def merge_key_context(*args, **kwargs):
     result = merge_key(*args, **kwargs)
     try:
         yield result
     finally:
         if result is not None:
```

### Comparing `sd_meh-0.8.0/sd_meh/merge_methods.py` & `sd_meh-0.9.0/sd_meh/merge_methods.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.8.0/sd_meh/model.py` & `sd_meh-0.9.0/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.8.0/sd_meh/presets.py` & `sd_meh-0.9.0/sd_meh/presets.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.8.0/sd_meh/rebasin.py` & `sd_meh-0.9.0/sd_meh/rebasin.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.8.0/PKG-INFO` & `sd_meh-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.8.0
+Version: 0.9.0
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -41,14 +41,18 @@
 
 You can have a look at the provided `merge_models.py` cli for an example on how to use the function. Run `python3 merge_models.py --help` for a list of the available arguments.
 
 [Join](https://discord.gg/EZJuBfNVHh) our discord server for discussion and features/bugfix requests
 
 ## Changelog
 
+### 0.9.0
+- bugfixes
+- support for pix2pix and inpainting models
+
 ### 0.8.0
 - add `-bwpab, --block_weights_preset_alpha_b"` and `-pal, --presets_alpha_lambda` for presets interpolation (same for `beta`)
 - add `-ll, --logging_level`, default to `INFO`
 
 ### 0.7.0
 - add `-bwpa, --block_weights_preset_alpha` and `-bwpb, --block_weights_preset_beta` to use pre-defined merging weights. Have a look at the [wiki](https://github.com/s1dlx/meh/wiki/Presets) for all the presets
 - add `-wd, --work_device`
```

