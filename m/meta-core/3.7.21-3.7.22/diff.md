# Comparing `tmp/meta-core-3.7.21.tar.gz` & `tmp/meta-core-3.7.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-core-3.7.21.tar", last modified: Fri Jul 21 05:38:27 2023, max compression
+gzip compressed data, was "dist/meta-core-3.7.22.tar", last modified: Fri Jul 21 06:48:54 2023, max compression
```

## Comparing `meta-core-3.7.21.tar` & `meta-core-3.7.22.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 05:38:27.000000 meta-core-3.7.21/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 05:38:27.000000 meta-core-3.7.21/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.21/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 05:38:27.000000 meta-core-3.7.21/meta_core.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 05:38:27.000000 meta-core-3.7.21/meta_core.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)     1026 2023-07-21 05:38:27.000000 meta-core-3.7.21/meta_core.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 05:38:27.000000 meta-core-3.7.21/meta_core.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-07-21 05:38:27.000000 meta-core-3.7.21/meta_core.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:27.000000 meta-core-3.7.21/meta_core.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 05:38:27.000000 meta-core-3.7.21/meta_core.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 05:38:27.000000 meta-core-3.7.21/metacore/
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.21/metacore/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 05:38:27.000000 meta-core-3.7.21/metacore/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.21/metacore/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4338 2023-07-21 04:58:45.000000 meta-core-3.7.21/metacore/app/ad_segment.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.21/metacore/app/segment.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 05:38:27.000000 meta-core-3.7.21/metacore/open_clip/
--rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/coca_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/constants.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/factory.py
--rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/generation_utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/hf_configs.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/hf_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/loss.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7216 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/modified_resnet.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/openai.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/pretrained.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/push_to_hf_hub.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/timm_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/tokenizer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/transform.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/transformer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.21/metacore/open_clip/version.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 05:38:27.000000 meta-core-3.7.21/metacore/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.21/metacore/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.21/metacore/utils/f3net.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.21/metacore/utils/model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.21/metacore/utils/prompt_ensemble.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-21 05:38:27.000000 meta-core-3.7.21/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      666 2023-07-21 05:35:18.000000 meta-core-3.7.21/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 06:48:54.000000 meta-core-3.7.22/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 06:48:54.000000 meta-core-3.7.22/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.22/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 06:48:54.000000 meta-core-3.7.22/meta_core.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 06:48:54.000000 meta-core-3.7.22/meta_core.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1026 2023-07-21 06:48:54.000000 meta-core-3.7.22/meta_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 06:48:54.000000 meta-core-3.7.22/meta_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-07-21 06:48:54.000000 meta-core-3.7.22/meta_core.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 06:48:54.000000 meta-core-3.7.22/meta_core.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 06:48:54.000000 meta-core-3.7.22/meta_core.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 06:48:54.000000 meta-core-3.7.22/metacore/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.22/metacore/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 06:48:54.000000 meta-core-3.7.22/metacore/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.22/metacore/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4371 2023-07-21 06:04:22.000000 meta-core-3.7.22/metacore/app/ad_segment.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.22/metacore/app/segment.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 06:48:54.000000 meta-core-3.7.22/metacore/open_clip/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/coca_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/constants.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/factory.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/generation_utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/hf_configs.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/hf_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/loss.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7216 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/modified_resnet.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/openai.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/pretrained.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/push_to_hf_hub.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/timm_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/tokenizer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/transform.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/transformer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.22/metacore/open_clip/version.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 06:48:54.000000 meta-core-3.7.22/metacore/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.22/metacore/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.22/metacore/utils/f3net.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.22/metacore/utils/model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.22/metacore/utils/prompt_ensemble.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-21 06:48:54.000000 meta-core-3.7.22/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      666 2023-07-21 06:46:49.000000 meta-core-3.7.22/setup.py
```

### Comparing `meta-core-3.7.21/meta_core.egg-info/SOURCES.txt` & `meta-core-3.7.22/meta_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/app/ad_segment.py` & `meta-core-3.7.22/metacore/app/ad_segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
                 anomaly_map = F.interpolate(anomaly_map.permute(0, 2, 1).view(B, 2, H, H),
                                             size=self.image_size, mode='bilinear', align_corners=True)
                 anomaly_map = torch.softmax(anomaly_map, dim=1)[:, 1, :, :]
                 anomaly_maps.append(anomaly_map.cpu().numpy())
             anomaly_map = np.sum(anomaly_maps, axis=0)
 
         mask = normalize(anomaly_map[0]) > thre
+        torch.cuda.empty_cache()
         return mask
 
     @staticmethod
     def get_rect(mask):
         mask = (mask * 255).astype(np.uint8)
         _, pred = cv2.threshold(mask, 128, 255, cv2.THRESH_BINARY)
         contours, _ = cv2.findContours(pred, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
```

### Comparing `meta-core-3.7.21/metacore/app/segment.py` & `meta-core-3.7.22/metacore/app/segment.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/__init__.py` & `meta-core-3.7.22/metacore/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/coca_model.py` & `meta-core-3.7.22/metacore/open_clip/coca_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/factory.py` & `meta-core-3.7.22/metacore/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/hf_configs.py` & `meta-core-3.7.22/metacore/open_clip/hf_configs.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/hf_model.py` & `meta-core-3.7.22/metacore/open_clip/hf_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/loss.py` & `meta-core-3.7.22/metacore/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/model.py` & `meta-core-3.7.22/metacore/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/modified_resnet.py` & `meta-core-3.7.22/metacore/open_clip/modified_resnet.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/openai.py` & `meta-core-3.7.22/metacore/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/pretrained.py` & `meta-core-3.7.22/metacore/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/push_to_hf_hub.py` & `meta-core-3.7.22/metacore/open_clip/push_to_hf_hub.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/timm_model.py` & `meta-core-3.7.22/metacore/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/tokenizer.py` & `meta-core-3.7.22/metacore/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/transform.py` & `meta-core-3.7.22/metacore/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/transformer.py` & `meta-core-3.7.22/metacore/open_clip/transformer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/open_clip/utils.py` & `meta-core-3.7.22/metacore/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/utils/f3net.py` & `meta-core-3.7.22/metacore/utils/f3net.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/utils/model.py` & `meta-core-3.7.22/metacore/utils/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/metacore/utils/prompt_ensemble.py` & `meta-core-3.7.22/metacore/utils/prompt_ensemble.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.21/setup.py` & `meta-core-3.7.22/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     'opencv-python',
     'setuptools',
     'numpy',
     'pillow',
     'torch'
 ]
 
-__version__ = 'V3.07.21'
+__version__ = 'V3.07.22'
 
 setup(
     name='meta-core',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvreid',
```

