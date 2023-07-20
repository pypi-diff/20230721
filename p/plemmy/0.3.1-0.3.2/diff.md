# Comparing `tmp/plemmy-0.3.1.tar.gz` & `tmp/plemmy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.3.1.tar", last modified: Tue Jul 11 14:30:07 2023, max compression
+gzip compressed data, was "plemmy-0.3.2.tar", last modified: Thu Jul 20 23:47:13 2023, max compression
```

## Comparing `plemmy-0.3.1.tar` & `plemmy-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-11 14:30:07.064181 plemmy-0.3.1/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.3.1/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-11 14:30:07.064025 plemmy-0.3.1/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     2372 2023-07-08 04:32:47.000000 plemmy-0.3.1/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-11 14:30:07.062904 plemmy-0.3.1/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-08 04:04:32.000000 plemmy-0.3.1/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-08 03:39:07.000000 plemmy-0.3.1/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    13987 2023-07-11 14:28:15.000000 plemmy-0.3.1/plemmy/objects.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    19156 2023-07-08 04:04:32.000000 plemmy-0.3.1/plemmy/responses.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.3.1/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-11 14:29:11.000000 plemmy-0.3.1/plemmy/version.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-08 04:04:32.000000 plemmy-0.3.1/plemmy/views.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-11 14:30:07.063800 plemmy-0.3.1/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-11 14:30:07.064227 plemmy-0.3.1/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.3.1/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-20 23:47:13.810187 plemmy-0.3.2/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-07-20 23:46:22.000000 plemmy-0.3.2/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-20 23:47:13.810017 plemmy-0.3.2/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2372 2023-07-20 23:46:22.000000 plemmy-0.3.2/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-20 23:47:13.808878 plemmy-0.3.2/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    13987 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/objects.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    19231 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/responses.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-20 23:46:37.000000 plemmy-0.3.2/plemmy/version.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/views.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-20 23:47:13.809794 plemmy-0.3.2/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-20 23:47:13.810240 plemmy-0.3.2/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-07-20 23:46:22.000000 plemmy-0.3.2/setup.py
```

### Comparing `plemmy-0.3.1/LICENSE` & `plemmy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.1/PKG-INFO` & `plemmy-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.3.1/README.md` & `plemmy-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.1/plemmy/lemmyhttp.py` & `plemmy-0.3.2/plemmy/lemmyhttp.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.1/plemmy/objects.py` & `plemmy-0.3.2/plemmy/objects.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.1/plemmy/responses.py` & `plemmy-0.3.2/plemmy/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     """https://join-lemmy.org/api/interfaces/GetPostResponse.html"""
 
     def __init__(self, api_response: requests.Response) -> None:
 
         response = api_response.json()
         self.community_view = CommunityView(response["community_view"])
         self.cross_posts = [PostView(p) for p in response["cross_posts"]]
-        self.moderators = CommunityModeratorView(response["moderators"])
+        self.moderators = [CommunityModeratorView(m) for m in response["moderators"]]
         self.post_view = PostView(response["post_view"])
 
 
 class GetPostsResponse(object):
     """https://join-lemmy.org/api/interfaces/GetPostsResponse.html"""
 
     def __init__(self, api_response: requests.Response) -> None:
@@ -314,15 +314,16 @@
     """https://join-lemmy.org/api/interfaces/GetSiteResponse.html"""
 
     def __init__(self, api_response: requests.Response) -> None:
 
         response = api_response.json()
         self.admins = [PersonView(a) for a in response["admins"]]
         self.all_languages = [Language(**lang)
-                              for lang in response["discussion_languages"]]
+                              for lang in response["all_languages"]]
+        self.discussion_languages = response["discussion_languages"]
         if "my_user" in response.keys():
             self.my_user = response["my_user"]
         else:
             self.my_user = None
         self.site_view = SiteView(response["site_view"])
         self.taglines = [Tagline(**t) for t in response["taglines"]]
         self.version = response["version"]
```

### Comparing `plemmy-0.3.1/plemmy/utils.py` & `plemmy-0.3.2/plemmy/utils.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.1/plemmy/views.py` & `plemmy-0.3.2/plemmy/views.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.1/plemmy.egg-info/PKG-INFO` & `plemmy-0.3.2/plemmy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.3.1/setup.py` & `plemmy-0.3.2/setup.py`

 * *Files identical despite different names*

