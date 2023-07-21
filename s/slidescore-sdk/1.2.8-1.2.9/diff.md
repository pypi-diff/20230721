# Comparing `tmp/slidescore-sdk-1.2.8.tar.gz` & `tmp/slidescore-sdk-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\slidescore-sdk-1.2.8.tar", last modified: Tue May 17 11:51:05 2022, max compression
+gzip compressed data, was "slidescore-sdk-1.2.9.tar", last modified: Sat May 21 22:00:32 2022, max compression
```

## Comparing `slidescore-sdk-1.2.8.tar` & `slidescore-sdk-1.2.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-05-17 11:51:05.000000 slidescore-sdk-1.2.8/
--rw-rw-rw-   0        0        0      868 2022-05-17 11:51:05.000000 slidescore-sdk-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      207 2019-10-24 20:00:11.000000 slidescore-sdk-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2022-05-17 11:51:05.000000 slidescore-sdk-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      926 2022-05-17 11:50:24.000000 slidescore-sdk-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-17 11:51:05.000000 slidescore-sdk-1.2.8/slidescore/
--rw-rw-rw-   0        0        0       25 2020-04-28 18:50:14.000000 slidescore-sdk-1.2.8/slidescore/__init__.py
--rw-rw-rw-   0        0        0    14286 2022-05-17 11:50:33.000000 slidescore-sdk-1.2.8/slidescore/slidescore.py
-drwxrwxrwx   0        0        0        0 2022-05-17 11:51:05.000000 slidescore-sdk-1.2.8/slidescore_sdk.egg-info/
--rw-rw-rw-   0        0        0      868 2022-05-17 11:51:04.000000 slidescore-sdk-1.2.8/slidescore_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2022-05-17 11:51:04.000000 slidescore-sdk-1.2.8/slidescore_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-17 11:51:04.000000 slidescore-sdk-1.2.8/slidescore_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-05-17 11:51:04.000000 slidescore-sdk-1.2.8/slidescore_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-05-17 11:51:04.000000 slidescore-sdk-1.2.8/slidescore_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-21 22:00:32.689754 slidescore-sdk-1.2.9/
+-rw-rw-rw-   0        0        0     1091 2019-10-24 20:00:11.000000 slidescore-sdk-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      858 2022-05-21 22:00:32.688835 slidescore-sdk-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2019-10-24 20:00:11.000000 slidescore-sdk-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-05-21 22:00:32.689754 slidescore-sdk-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      926 2022-05-21 21:57:39.000000 slidescore-sdk-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-21 22:00:32.665579 slidescore-sdk-1.2.9/slidescore/
+-rw-rw-rw-   0        0        0       25 2020-04-28 18:50:14.000000 slidescore-sdk-1.2.9/slidescore/__init__.py
+-rw-rw-rw-   0        0        0    14952 2022-05-21 21:57:27.000000 slidescore-sdk-1.2.9/slidescore/slidescore.py
+drwxrwxrwx   0        0        0        0 2022-05-21 22:00:32.687303 slidescore-sdk-1.2.9/slidescore_sdk.egg-info/
+-rw-rw-rw-   0        0        0      858 2022-05-21 22:00:32.000000 slidescore-sdk-1.2.9/slidescore_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2022-05-21 22:00:32.000000 slidescore-sdk-1.2.9/slidescore_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-21 22:00:32.000000 slidescore-sdk-1.2.9/slidescore_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2022-05-21 22:00:32.000000 slidescore-sdk-1.2.9/slidescore_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-05-21 22:00:32.000000 slidescore-sdk-1.2.9/slidescore_sdk.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `slidescore-sdk-1.2.8/setup.py` & `slidescore-sdk-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="slidescore-sdk",
-    version="1.2.8",
+    version="1.2.9",
     author="Slide Score B.V.",
     author_email="info@slidescore.com",
     description="SDK for using the API of Slide Score",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/slide-score/SlideScore-python-sdk",
     packages=setuptools.find_packages(),
```

### Comparing `slidescore-sdk-1.2.8/slidescore/slidescore.py` & `slidescore-sdk-1.2.9/slidescore/slidescore.py`

 * *Files 4% similar despite different names*

```diff
@@ -363,8 +363,20 @@
         if response.text[0] == '"':
             raise SlideScoreErrorException("Failed reimporting: " + response.text);
         rjson=response.json()
         if not rjson["success"]:
             raise SlideScoreErrorException("Failed reimporting: " + rjson["log"]);
         return { "id": rjson['id'], "log": rjson["log"]}
         
-  
+    def get_slide_path(self, image_id):
+        response = self.perform_request("GetSlidePath", {"imageId": image_id}, method="GET")
+        rjson = response.json()
+        if not rjson["success"]:
+            raise SlideScoreErrorException("Failed getting slide path: " + response.text);
+        return rjson['path'] 
+        
+
+    def update_slide_path(self, image_id, new_path):
+        response = self.perform_request("UpdateSlidePath", {"imageId": image_id, "newPath": new_path}, method="POST")
+        rjson = response.json()
+        if not rjson["success"]:
+            raise SlideScoreErrorException("Failed updating slide path: " + response.text);
```

