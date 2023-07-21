# Comparing `tmp/chromahacker-0.2.3.tar.gz` & `tmp/chromahacker-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahacker-0.2.3.tar", max compression
+gzip compressed data, was "chromahacker-0.2.4.tar", max compression
```

## Comparing `chromahacker-0.2.3.tar` & `chromahacker-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-06 19:05:27.000000 chromahacker-0.2.3/README.md
--rw-r--r--   0        0        0     6148 2023-06-06 20:17:27.000000 chromahacker-0.2.3/chromahacker/.DS_Store
--rw-r--r--   0        0        0       89 2023-06-08 16:47:40.000000 chromahacker-0.2.3/chromahacker/__init__.py
--rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.000000 chromahacker-0.2.3/chromahacker/color_input.py
--rw-r--r--   0        0        0      543 2023-07-21 17:18:42.338101 chromahacker-0.2.3/chromahacker/palettize.py
--rw-r--r--   0        0        0      266 2023-06-09 00:21:03.000000 chromahacker-0.2.3/chromahacker/process_image.py
--rw-r--r--   0        0        0      469 2023-07-21 16:56:05.933097 chromahacker-0.2.3/chromahacker/spline.py
--rw-r--r--   0        0        0      337 2023-07-21 17:20:13.765508 chromahacker-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 19:05:27.000000 chromahacker-0.2.4/README.md
+-rw-r--r--   0        0        0     6148 2023-06-06 20:17:27.000000 chromahacker-0.2.4/chromahacker/.DS_Store
+-rw-r--r--   0        0        0       89 2023-06-08 16:47:40.000000 chromahacker-0.2.4/chromahacker/__init__.py
+-rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.000000 chromahacker-0.2.4/chromahacker/color_input.py
+-rw-r--r--   0        0        0      547 2023-07-21 17:43:55.100337 chromahacker-0.2.4/chromahacker/palettize.py
+-rw-r--r--   0        0        0      266 2023-06-09 00:21:03.000000 chromahacker-0.2.4/chromahacker/process_image.py
+-rw-r--r--   0        0        0      469 2023-07-21 17:43:15.983637 chromahacker-0.2.4/chromahacker/spline.py
+-rw-r--r--   0        0        0      337 2023-07-21 17:44:24.869993 chromahacker-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.2.4/PKG-INFO
```

### Comparing `chromahacker-0.2.3/chromahacker/.DS_Store` & `chromahacker-0.2.4/chromahacker/.DS_Store`

 * *Files identical despite different names*

### Comparing `chromahacker-0.2.3/chromahacker/color_input.py` & `chromahacker-0.2.4/chromahacker/color_input.py`

 * *Files identical despite different names*

### Comparing `chromahacker-0.2.3/chromahacker/palettize.py` & `chromahacker-0.2.4/chromahacker/palettize.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 from chromahacker.process_image import url_to_image
 
 def palettize(url, output, *args, accurate=False):
     np_array = url_to_image(url)
 
     img = cv2.cvtColor(np_array, cv2.COLOR_RGB2GRAY)
 
-    fn = spline_from(*args)
+    fn = spline_from(*args, accurate=accurate)
 
     if accurate:
-        display = np.array([[fn(j, accurate=True) for j in i] for i in img])
+        display = np.array([[fn(j) for j in i] for i in img])
     else:
         display = np.rint(fn(img)).astype(np.uint8)
     cv2.imwrite('wallpaper.' + output, display)
```

