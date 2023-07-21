# Comparing `tmp/spotify_dl-8.8.1.tar.gz` & `tmp/spotify_dl-8.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_dl-8.8.1.tar", last modified: Fri May 12 15:34:10 2023, max compression
+gzip compressed data, was "spotify_dl-8.8.2.tar", last modified: Fri Jul 21 00:45:41 2023, max compression
```

## Comparing `spotify_dl-8.8.1.tar` & `spotify_dl-8.8.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/spotify_dl/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/spotify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6663 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/spotify_dl.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/spotify_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:45:41.939548 spotify_dl-8.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-21 00:45:41.939548 spotify_dl-8.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 00:45:41.939548 spotify_dl-8.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:45:41.935548 spotify_dl-8.8.2/spotify_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/spotify_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/spotify_dl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/spotify_dl/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/spotify_dl/spotify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6667 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/spotify_dl/spotify_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/spotify_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-07-21 00:45:26.000000 spotify_dl-8.8.2/spotify_dl/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:45:41.939548 spotify_dl-8.8.2/spotify_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-21 00:45:41.000000 spotify_dl-8.8.2/spotify_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-21 00:45:41.000000 spotify_dl-8.8.2/spotify_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:45:41.000000 spotify_dl-8.8.2/spotify_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 00:45:41.000000 spotify_dl-8.8.2/spotify_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 00:45:41.000000 spotify_dl-8.8.2/spotify_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 00:45:41.000000 spotify_dl-8.8.2/spotify_dl.egg-info/top_level.txt
```

### Comparing `spotify_dl-8.8.1/LICENSE` & `spotify_dl-8.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.1/PKG-INFO` & `spotify_dl-8.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_dl
-Version: 8.8.1
+Version: 8.8.2
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spotify_dl-8.8.1/README.md` & `spotify_dl-8.8.2/README.md`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.1/setup.py` & `spotify_dl-8.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.1/spotify_dl/scaffold.py` & `spotify_dl-8.8.2/spotify_dl/scaffold.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.1/spotify_dl/spotify.py` & `spotify_dl-8.8.2/spotify_dl/spotify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import sys
 from spotify_dl.scaffold import log
 from spotify_dl.utils import sanitize
 from rich.progress import Progress
 
 
-def fetch_tracks(sp, item_type, url):
+def fetch_tracks(sp, item_type, item_id):
     """
-    Fetches tracks from the provided URL.
+    Fetches tracks from the provided item_id.
     :param sp: Spotify client
     :param item_type: Type of item being requested for: album/playlist/track
-    :param url: URL of the item
+    :param item_id: id of the item
     :return Dictionary of song and artist
     """
     songs_list = []
     offset = 0
     songs_fetched = 0
 
     if item_type == "playlist":
         with Progress() as progress:
             songs_task = progress.add_task(description="Fetching songs from playlist..")
             while True:
                 items = sp.playlist_items(
-                    playlist_id=url,
+                    playlist_id=item_id,
                     fields="items.track.name,items.track.artists(name, uri),"
                     "items.track.album(name, release_date, total_tracks, images),"
                     "items.track.track_number,total, next,offset,"
                     "items.track.id",
                     additional_types=["track"],
                     offset=offset,
                 )
@@ -107,16 +107,16 @@
 
     elif item_type == "album":
         with Progress() as progress:
             album_songs_task = progress.add_task(
                 description="Fetching songs from the album.."
             )
             while True:
-                album_info = sp.album(album_id=url)
-                items = sp.album_tracks(album_id=url, offset=offset)
+                album_info = sp.album(album_id=item_id)
+                items = sp.album_tracks(album_id=item_id, offset=offset)
                 total_songs = items.get("total")
                 track_album = album_info.get("name")
                 track_year = (
                     album_info.get("release_date")[:4]
                     if album_info.get("release_date")
                     else ""
                 )
@@ -164,15 +164,15 @@
                     advance=offset,
                     total=album_total,
                 )
                 if album_total == offset:
                     break
 
     elif item_type == "track":
-        items = sp.track(track_id=url)
+        items = sp.track(track_id=item_id)
         track_name = items.get("name")
         album_info = items.get("album")
         track_artist = ", ".join([artist["name"] for artist in items["artists"]])
         if album_info:
             track_album = album_info.get("name")
             track_year = (
                 album_info.get("release_date")[:4]
@@ -215,17 +215,18 @@
     :param url: URL to be parsed
 
     :return tuple indicating the type and id of the item
     """
     if url.startswith("spotify:"):
         log.error("Spotify URI was provided instead of a playlist/album/track URL.")
         sys.exit(1)
-    parsed_url = url.replace("https://open.spotify.com/", "").split("?")[0]
-    item_type = parsed_url.split("/")[0]
-    item_id = parsed_url.split("/")[1]
+    parsed_url = url.replace("https://open.spotify.com/", "").split("?")[0].split("/")
+    index_adjustment = 1 if parsed_url[0].startswith("intl") else 0
+    item_type = parsed_url[0+index_adjustment]
+    item_id = parsed_url[1+index_adjustment]
     return item_type, item_id
 
 
 def get_item_name(sp, item_type, item_id):
     """
     Fetch the name of the item.
     :param sp: Spotify Client
```

### Comparing `spotify_dl-8.8.1/spotify_dl/spotify_dl.py` & `spotify_dl-8.8.2/spotify_dl/spotify_dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         item_type, item_id = parse_spotify_url(url)
         directory_name = get_item_name(sp, item_type, item_id)
         url_dict["save_path"] = Path(
             PurePath.joinpath(Path(args.output), Path(directory_name))
         )
         url_dict["save_path"].mkdir(parents=True, exist_ok=True)
         log.info("Saving songs to %s directory", directory_name)
-        url_dict["songs"] = fetch_tracks(sp, item_type, url)
+        url_dict["songs"] = fetch_tracks(sp, item_type, item_id)
         url_data["urls"].append(url_dict.copy())
     if args.dump_json is True:
         dump_json(url_dict["songs"])
     elif args.download is True:
         file_name_f = default_filename
         if args.keep_playlist_order:
             file_name_f = playlist_num_filename
```

### Comparing `spotify_dl-8.8.1/spotify_dl/youtube.py` & `spotify_dl-8.8.2/spotify_dl/youtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 int(temp[-1].replace("\n", "")),
             )
 
             query = f"{artist} - {name} Lyrics".replace(":", "").replace('"', "")
             print(f"Initiating download for {query}.")
 
             file_name = kwargs["file_name_f"](
-                name=name, artist=artist, track_num=kwargs["track_db"][i].get("num")
+                name=name, artist=artist, track_num=kwargs["track_db"][i].get("playlist_num")
             )
 
             if kwargs["use_sponsorblock"][0].lower() == "y":
                 sponsorblock_postprocessor = [
                     {
                         "key": "SponsorBlock",
                         "categories": ["skip_non_music_sections"],
```

### Comparing `spotify_dl-8.8.1/spotify_dl.egg-info/PKG-INFO` & `spotify_dl-8.8.2/spotify_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-dl
-Version: 8.8.1
+Version: 8.8.2
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

