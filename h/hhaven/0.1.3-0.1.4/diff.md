# Comparing `tmp/hhaven-0.1.3.tar.gz` & `tmp/hhaven-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhaven-0.1.3.tar", last modified: Tue Jul 18 13:47:27 2023, max compression
+gzip compressed data, was "hhaven-0.1.4.tar", last modified: Fri Jul 21 14:53:01 2023, max compression
```

## Comparing `hhaven-0.1.3.tar` & `hhaven-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:47:27.697679 hhaven-0.1.3/
--rw-rw-rw-   0        0        0     1086 2023-07-17 11:16:45.000000 hhaven-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3772 2023-07-18 13:47:27.696681 hhaven-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2675 2023-07-18 13:41:36.000000 hhaven-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 13:47:27.688680 hhaven-0.1.3/hhaven/
--rw-rw-rw-   0        0        0      267 2023-07-18 13:47:20.000000 hhaven-0.1.3/hhaven/__init__.py
--rw-rw-rw-   0        0        0    10241 2023-07-17 16:00:30.000000 hhaven-0.1.3/hhaven/client.py
--rw-rw-rw-   0        0        0     1180 2023-07-17 15:43:02.000000 hhaven-0.1.3/hhaven/decorators.py
--rw-rw-rw-   0        0        0     2273 2023-07-17 15:12:47.000000 hhaven-0.1.3/hhaven/exceptions.py
--rw-rw-rw-   0        0        0    15853 2023-07-17 15:50:40.000000 hhaven-0.1.3/hhaven/models.py
--rw-rw-rw-   0        0        0      789 2023-07-17 16:05:23.000000 hhaven-0.1.3/hhaven/utility.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:47:27.695680 hhaven-0.1.3/hhaven.egg-info/
--rw-rw-rw-   0        0        0     3772 2023-07-18 13:47:27.000000 hhaven-0.1.3/hhaven.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-18 13:47:27.000000 hhaven-0.1.3/hhaven.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:47:27.000000 hhaven-0.1.3/hhaven.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-18 13:47:27.000000 hhaven-0.1.3/hhaven.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 13:47:27.000000 hhaven-0.1.3/hhaven.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1050 2023-07-18 13:47:20.000000 hhaven-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 13:47:27.697679 hhaven-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1505 2023-07-18 13:47:21.000000 hhaven-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:53:01.532967 hhaven-0.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-07-17 11:16:45.000000 hhaven-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3772 2023-07-21 14:53:01.531965 hhaven-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2675 2023-07-18 13:41:36.000000 hhaven-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 14:53:01.521964 hhaven-0.1.4/hhaven/
+-rw-rw-rw-   0        0        0      267 2023-07-21 14:47:34.000000 hhaven-0.1.4/hhaven/__init__.py
+-rw-rw-rw-   0        0        0    10241 2023-07-17 16:00:30.000000 hhaven-0.1.4/hhaven/client.py
+-rw-rw-rw-   0        0        0     1180 2023-07-17 15:43:02.000000 hhaven-0.1.4/hhaven/decorators.py
+-rw-rw-rw-   0        0        0     2273 2023-07-17 15:12:47.000000 hhaven-0.1.4/hhaven/exceptions.py
+-rw-rw-rw-   0        0        0    16064 2023-07-21 14:51:42.000000 hhaven-0.1.4/hhaven/models.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 20:32:41.000000 hhaven-0.1.4/hhaven/py.typed
+-rw-rw-rw-   0        0        0      789 2023-07-17 16:05:23.000000 hhaven-0.1.4/hhaven/utility.py
+drwxrwxrwx   0        0        0        0 2023-07-21 14:53:01.530969 hhaven-0.1.4/hhaven.egg-info/
+-rw-rw-rw-   0        0        0     3772 2023-07-21 14:53:01.000000 hhaven-0.1.4/hhaven.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-07-21 14:53:01.000000 hhaven-0.1.4/hhaven.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 14:53:01.000000 hhaven-0.1.4/hhaven.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-21 14:53:01.000000 hhaven-0.1.4/hhaven.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 14:53:01.000000 hhaven-0.1.4/hhaven.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1050 2023-07-21 14:47:34.000000 hhaven-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 14:53:01.532967 hhaven-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1505 2023-07-21 14:47:34.000000 hhaven-0.1.4/setup.py
```

### Comparing `hhaven-0.1.3/LICENSE` & `hhaven-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.3/PKG-INFO` & `hhaven-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhaven
-Version: 0.1.3
+Version: 0.1.4
 Summary: A well-documented and typed API wrapper for Hentai Haven.
 Home-page: https://github.com/jokelbaf/hhaven
 Author: jokelbaf
 Author-email: jokelbaf@gmail.com
 License: MIT
 Project-URL: Documentation, https://jokelbaf.github.io/hhaven
 Project-URL: API Reference, https://jokelbaf.github.io/hhaven-api-reference
```

### Comparing `hhaven-0.1.3/README.md` & `hhaven-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.3/hhaven/client.py` & `hhaven-0.1.4/hhaven/client.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.3/hhaven/decorators.py` & `hhaven-0.1.4/hhaven/decorators.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.3/hhaven/exceptions.py` & `hhaven-0.1.4/hhaven/exceptions.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.3/hhaven/models.py` & `hhaven-0.1.4/hhaven/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,23 @@
     """
     Raw title.
     
     Example: episode-1
     """
     date: datetime
     """Datetime object representing episode upload date."""
+    content: str
+    """
+    Url to m3u8 file of the episode. Usually contains multiple quality levels:
+    - 480p
+    - 720p
+    - 1080p
+    
+    Example: https://example.com/episode-name.m3u8
+    """
     thumbnail: str
     """
     Episode thumbnail url.
     
     Example: https://example.com/episode_thumbnail.jpg
     """
     hentai_id: int
@@ -343,17 +352,17 @@
                     else:
                         data["next_episode"][key] = value
                     
         if data["prev_episode"] is not None:
             for key, value in data.items():
                 if key not in ("id", "name", "thumbnail", "date", "slug"):
                     if key == "next_episode" or key == "prev_episode":
-                        data["next_episode"][key] = None
+                        data["prev_episode"][key] = None
                     else:
-                        data["next_episode"][key] = value
+                        data["prev_episode"][key] = value
                         
         for genre in processed["hentai_genres"]:
             genre["client"] = data.get("client")
         
         super().__init__(**processed)
```

### Comparing `hhaven-0.1.3/hhaven/utility.py` & `hhaven-0.1.4/hhaven/utility.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.3/hhaven.egg-info/PKG-INFO` & `hhaven-0.1.4/hhaven.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhaven
-Version: 0.1.3
+Version: 0.1.4
 Summary: A well-documented and typed API wrapper for Hentai Haven.
 Home-page: https://github.com/jokelbaf/hhaven
 Author: jokelbaf
 Author-email: jokelbaf@gmail.com
 License: MIT
 Project-URL: Documentation, https://jokelbaf.github.io/hhaven
 Project-URL: API Reference, https://jokelbaf.github.io/hhaven-api-reference
```

### Comparing `hhaven-0.1.3/pyproject.toml` & `hhaven-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hhaven"
 license = "MIT"
-version = "0.1.3"
+version = "0.1.4"
 description = "A well-documented and typed API wrapper for Hentai Haven."
 authors = [
     "JokelBaf <jokelbaf@gmail.com>",
 ]
 maintainers = [
     "JokelBaf <jokelbaf@gmail.com>",
 ]
```

### Comparing `hhaven-0.1.3/setup.py` & `hhaven-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Run setuptools."""
 from setuptools import find_packages, setup
 
 setup(
     name = "hhaven",
-    version = "0.1.3",
+    version = "0.1.4",
     author = "jokelbaf",
     author_email = "jokelbaf@gmail.com",
     description = "A well-documented and typed API wrapper for Hentai Haven.",
     keywords = "hentai-haven hentai".split(),
     url = "https://github.com/jokelbaf/hhaven",
     project_urls = {
         "Documentation": "https://jokelbaf.github.io/hhaven",
```

