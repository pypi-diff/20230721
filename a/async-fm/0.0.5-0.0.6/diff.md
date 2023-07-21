# Comparing `tmp/async_fm-0.0.5.tar.gz` & `tmp/async_fm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_fm-0.0.5.tar", max compression
+gzip compressed data, was "async_fm-0.0.6.tar", max compression
```

## Comparing `async_fm-0.0.5.tar` & `async_fm-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-15 23:38:58.618624 async_fm-0.0.5/LICENSE
--rw-r--r--   0        0        0     1590 2023-06-15 23:38:58.618624 async_fm-0.0.5/README.md
--rw-r--r--   0        0        0      683 2023-06-15 23:38:58.618624 async_fm-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      130 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/__init__.py
--rw-r--r--   0        0        0     1264 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/api/__init__.py
--rw-r--r--   0        0        0    14965 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/api/user.py
--rw-r--r--   0        0        0     2403 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/exceptions.py
--rw-r--r--   0        0        0     1437 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/types.py
--rw-r--r--   0        0        0      208 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/utils.py
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 async_fm-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-21 00:07:29.766983 async_fm-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1590 2023-07-21 00:07:29.766983 async_fm-0.0.6/README.md
+-rw-r--r--   0        0        0      686 2023-07-21 00:07:29.766983 async_fm-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-07-21 00:07:29.766983 async_fm-0.0.6/src/asyncfm/__init__.py
+-rw-r--r--   0        0        0     1264 2023-07-21 00:07:29.766983 async_fm-0.0.6/src/asyncfm/api/__init__.py
+-rw-r--r--   0        0        0    15010 2023-07-21 00:07:29.766983 async_fm-0.0.6/src/asyncfm/api/user.py
+-rw-r--r--   0        0        0     2403 2023-07-21 00:07:29.766983 async_fm-0.0.6/src/asyncfm/exceptions.py
+-rw-r--r--   0        0        0     1480 2023-07-21 00:07:29.766983 async_fm-0.0.6/src/asyncfm/types.py
+-rw-r--r--   0        0        0      208 2023-07-21 00:07:29.766983 async_fm-0.0.6/src/asyncfm/utils.py
+-rw-r--r--   0        0        0     2267 1970-01-01 00:00:00.000000 async_fm-0.0.6/PKG-INFO
```

### Comparing `async_fm-0.0.5/LICENSE` & `async_fm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.5/README.md` & `async_fm-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.5/pyproject.toml` & `async_fm-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.poetry]
 name = "Async-FM"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python library for interacting with the Last.fm API asynchronously."
 authors = ["NachABR <nachabr@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "asyncfm", from = "src"}]
 homepage = "https://github.com/NachABR/async-fm"
 repository = "https://github.com/NachABR/async-fm.git"
 keywords = ["python", "lastfm", "aiohttp", "async"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10"
 aiohttp = ">=3.7"
-pydantic = "1.10.7"
-
+pydantic = ">=2.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.3.0"
-pylint = "2.17.2"
+black = "^23.3.0"
+pylint = "^2.17.2"
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `async_fm-0.0.5/src/asyncfm/api/__init__.py` & `async_fm-0.0.6/src/asyncfm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.5/src/asyncfm/api/user.py` & `async_fm-0.0.6/src/asyncfm/api/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
                 bootstrap=user_data.get("bootstrap"),
                 playcount=user_data.get("playcount"),
                 artist_count=user_data.get("artist_count"),
                 playlists=user_data.get("playlists"),
                 track_count=user_data.get("track_count"),
                 album_count=user_data.get("album_count"),
                 image=get_images_(user_data.get("image")),
-                registered=datetime.fromtimestamp(user_data["registered"]["unixtime"]),
+                registered=datetime.fromtimestamp(
+                    int(user_data["registered"]["unixtime"])
+                ),
                 country=user_data.get("country"),
                 gender=user_data.get("gender"),
                 url=user_data.get("url"),
                 type=user_data.get("type"),
             )
 
     async def get_recent_tracks(
@@ -270,16 +272,16 @@
             params["from"] = from_date.strftime("%Y-%m-%d")
         if to_date is not None:
             params["to"] = to_date.strftime("%Y-%m-%d")
 
         data = await self.api._make_request(params=params)
 
         if weekly_chart := data.get("weeklyartistchart"):
-            return Responses.Tracks(
-                tracks=list(
+            return Responses.Artists(
+                artists=list(
                     map(
                         lambda artist: Artist(
                             name=artist["name"],
                             playcount=artist["playcount"],
                             images=get_images_(images=images)
                             if (images := artist.get("image"))
                             else None,
```

### Comparing `async_fm-0.0.5/src/asyncfm/exceptions.py` & `async_fm-0.0.6/src/asyncfm/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.5/src/asyncfm/types.py` & `async_fm-0.0.6/src/asyncfm/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
 from typing import Optional, List
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 
 class Image(BaseModel):
     small: str
     medium: str
     large: str
-    extralarge: Optional[str]
+    extralarge: Optional[str] = None
 
 
 class User(BaseModel):
     name: str
     age: Optional[str]
     subscriber: Optional[int]
     realname: str
@@ -24,33 +24,32 @@
     image: Optional[Image]
     registered: datetime
     country: str
     gender: str
     url: str
     type: str
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class Track(BaseModel):
     artist: str
     title: str
-    album: Optional[str]
+    album: Optional[str] = None
     images: Optional[Image]
     now_playing: bool = False
-    rank: Optional[int]
-    playcount: Optional[int]
+    rank: Optional[int] = None
+    playcount: Optional[int] = None
 
 
 class Artist(BaseModel):
     name: str
-    images: Optional[Image]
+    images: Optional[Image] = None
     playcount: int
-    rank: Optional[int]
+    rank: Optional[int] = None
 
 
 class Album(BaseModel):
     artist: str
     title: str
     images: Optional[Image]
     rank: Optional[int]
```

### Comparing `async_fm-0.0.5/PKG-INFO` & `async_fm-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: async-fm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for interacting with the Last.fm API asynchronously.
 Home-page: https://github.com/NachABR/async-fm
 License: MIT
 Keywords: python,lastfm,aiohttp,async
 Author: NachABR
 Author-email: nachabr@protonmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7)
-Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: pydantic (>=2.0.0)
 Project-URL: Repository, https://github.com/NachABR/async-fm.git
 Description-Content-Type: text/markdown
 
 # AsyncFM
 
 Python library for interacting with the Last.fm API asynchronously.
```

