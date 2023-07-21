# Comparing `tmp/twirl-0.4.0.tar.gz` & `tmp/twirl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twirl-0.4.0.tar", max compression
+gzip compressed data, was "twirl-0.4.1.tar", max compression
```

## Comparing `twirl-0.4.0.tar` & `twirl-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4814 2023-06-15 12:56:06.841498 twirl-0.4.0/README.md
--rw-r--r--   0        0        0     2902 2023-06-15 12:56:06.849498 twirl-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5225 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/__init__.py
--rw-r--r--   0        0        0     4620 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/geometry.py
--rw-r--r--   0        0        0     4138 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/match.py
--rw-r--r--   0        0        0     2554 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/quads.py
--rw-r--r--   0        0        0     2174 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/triangles.py
--rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 twirl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4814 2023-07-21 14:51:59.780361 twirl-0.4.1/README.md
+-rw-r--r--   0        0        0     2902 2023-07-21 14:51:59.788361 twirl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5500 2023-07-21 14:51:59.788361 twirl-0.4.1/twirl/__init__.py
+-rw-r--r--   0        0        0     4620 2023-07-21 14:51:59.788361 twirl-0.4.1/twirl/geometry.py
+-rw-r--r--   0        0        0     4205 2023-07-21 14:51:59.788361 twirl-0.4.1/twirl/match.py
+-rw-r--r--   0        0        0     2554 2023-07-21 14:51:59.788361 twirl-0.4.1/twirl/quads.py
+-rw-r--r--   0        0        0     2174 2023-07-21 14:51:59.792361 twirl-0.4.1/twirl/triangles.py
+-rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 twirl-0.4.1/PKG-INFO
```

### Comparing `twirl-0.4.0/README.md` & `twirl-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `twirl-0.4.0/pyproject.toml` & `twirl-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twirl"
-version = "0.4.0"
+version = "0.4.1"
 description = "Astrometric plate solving in Python"
 authors = ["Lionel J. Garcia <lionel_garcia@live.fr>"]
 maintainers = [
   "Lionel J. Garcia <lionel_garcia@live.fr>",
   "Michael J. Roberts <michael@observerly.com>",
 ]
 license = "MIT"
```

### Comparing `twirl-0.4.0/twirl/__init__.py` & `twirl-0.4.1/twirl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,35 @@
         Number of sources to use for matching, by default 4
     min_match : int, optional
         Minimum number of matches required, by default None
 
     Returns
     -------
     astropy.wcs.WCS
-        WCS solution for the image
+        WCS solution for the image if a match can be computed, None otherwise.
+        A match is considered to be computed if at least one source and one target
+        star are located less than `tolerance` pixels away from each other.
     """
     M = find_transform(
         radecs,
         pixel_coords,
         tolerance=tolerance,
         asterism=asterism,
         min_match=min_match,
         quads_tolerance=quads_tolerance,
     )
-    radecs_xy = (M @ pad(radecs).T)[0:2].T
-    i, j = cross_match(pixel_coords, radecs_xy).T
-    M = get_transform_matrix(radecs[j], pixel_coords[i])
-    radecs_xy = (M @ pad(radecs).T)[0:2].T
-    i, j = cross_match(pixel_coords, radecs_xy).T
-    return fit_wcs_from_points(pixel_coords[i].T, SkyCoord(radecs[j], unit="deg"))
+    if M is None:
+        return None
+    else:
+        radecs_xy = (M @ pad(radecs).T)[0:2].T
+        i, j = cross_match(pixel_coords, radecs_xy).T
+        M = get_transform_matrix(radecs[j], pixel_coords[i])
+        radecs_xy = (M @ pad(radecs).T)[0:2].T
+        i, j = cross_match(pixel_coords, radecs_xy).T
+        return fit_wcs_from_points(pixel_coords[i].T, SkyCoord(radecs[j], unit="deg"))
 
 
 def gaia_radecs(
     center: Union[Tuple[float, float], SkyCoord],
     fov: Union[float, Quantity],
     limit: int = 10000,
     circular: bool = True,
```

### Comparing `twirl-0.4.0/twirl/geometry.py` & `twirl-0.4.1/twirl/geometry.py`

 * *Files identical despite different names*

### Comparing `twirl-0.4.0/twirl/match.py` & `twirl-0.4.1/twirl/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,11 +127,13 @@
         match = count_cross_match(pixels, test, tolerance)
         matches.append(match)
 
         if min_match is not None:
             if match >= min_match * len(pixels):
                 break
 
-    i, j = pairs[np.argmax(matches)]
-    M = get_transform_matrix(asterism_radecs[j], asterism_pixels[i])
-
-    return M
+    if len(matches) == 0:
+        return None
+    else:
+        i, j = pairs[np.argmax(matches)]
+        M = get_transform_matrix(asterism_radecs[j], asterism_pixels[i])
+        return M
```

### Comparing `twirl-0.4.0/twirl/quads.py` & `twirl-0.4.1/twirl/quads.py`

 * *Files identical despite different names*

### Comparing `twirl-0.4.0/twirl/triangles.py` & `twirl-0.4.1/twirl/triangles.py`

 * *Files identical despite different names*

### Comparing `twirl-0.4.0/PKG-INFO` & `twirl-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twirl
-Version: 0.4.0
+Version: 0.4.1
 Summary: Astrometric plate solving in Python
 Home-page: https://twirl.readthedocs.io
 License: MIT
 Keywords: astronomy,astrometry,plate-solving
 Author: Lionel J. Garcia
 Author-email: lionel_garcia@live.fr
 Maintainer: Lionel J. Garcia
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twirl Version: 0.4.0 Summary: Astrometric plate
+Metadata-Version: 2.1 Name: twirl Version: 0.4.1 Summary: Astrometric plate
 solving in Python Home-page: https://twirl.readthedocs.io License: MIT
 Keywords: astronomy,astrometry,plate-solving Author: Lionel J. Garcia Author-
 email: lionel_garcia@live.fr Maintainer: Lionel J. Garcia Maintainer-email:
 lionel_garcia@live.fr Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

