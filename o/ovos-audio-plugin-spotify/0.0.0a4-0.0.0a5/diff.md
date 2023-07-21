# Comparing `tmp/ovos_audio_plugin_spotify-0.0.0a4-py3-none-any.whl.zip` & `tmp/ovos_audio_plugin_spotify-0.0.0a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14172 bytes, number of entries: 9
--rw-r--r--  2.0 unx     3365 b- defN 23-Jul-21 11:46 ovos_audio_plugin_spotify/__init__.py
--rw-r--r--  2.0 unx    28703 b- defN 23-Jul-21 11:46 ovos_audio_plugin_spotify/spotify_client.py
--rw-r--r--  2.0 unx      177 b- defN 23-Jul-21 11:47 ovos_audio_plugin_spotify/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Jul-21 11:47 ovos_audio_plugin_spotify-0.0.0a4.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 23-Jul-21 11:47 ovos_audio_plugin_spotify-0.0.0a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 11:47 ovos_audio_plugin_spotify-0.0.0a4.dist-info/WHEEL
--rw-r--r--  2.0 unx      179 b- defN 23-Jul-21 11:47 ovos_audio_plugin_spotify-0.0.0a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 23-Jul-21 11:47 ovos_audio_plugin_spotify-0.0.0a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      889 b- defN 23-Jul-21 11:47 ovos_audio_plugin_spotify-0.0.0a4.dist-info/RECORD
-9 files, 45167 bytes uncompressed, 12596 bytes compressed:  72.1%
+Zip file size: 14198 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     3428 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify/__init__.py
+-rw-r--r--  2.0 unx    28703 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify/spotify_client.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify-0.0.0a5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      387 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify-0.0.0a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify-0.0.0a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      179 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify-0.0.0a5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify-0.0.0a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      889 b- defN 23-Jul-21 11:48 ovos_audio_plugin_spotify-0.0.0a5.dist-info/RECORD
+9 files, 45230 bytes uncompressed, 12622 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: ovos_audio_plugin_spotify/spotify_client.py
 Comment: 
 
 Filename: ovos_audio_plugin_spotify/version.py
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a4.dist-info/LICENSE
+Filename: ovos_audio_plugin_spotify-0.0.0a5.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a4.dist-info/METADATA
+Filename: ovos_audio_plugin_spotify-0.0.0a5.dist-info/METADATA
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a4.dist-info/WHEEL
+Filename: ovos_audio_plugin_spotify-0.0.0a5.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a4.dist-info/entry_points.txt
+Filename: ovos_audio_plugin_spotify-0.0.0a5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a4.dist-info/top_level.txt
+Filename: ovos_audio_plugin_spotify-0.0.0a5.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_audio_plugin_spotify-0.0.0a4.dist-info/RECORD
+Filename: ovos_audio_plugin_spotify-0.0.0a5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_audio_plugin_spotify/__init__.py

```diff
@@ -48,14 +48,15 @@
     def clear_list(self):
         self.tracks = []
         # TODO remove from spotify queue
         # Not available https://github.com/spotify/web-api/issues/462
         # once playback is started calling this will have no effect
 
     def add_list(self, tracks):
+        tracks = [t.replace("spotify://", "") for t in tracks]
         self.tracks += tracks
         LOG.info("Track list is " + str(tracks))
 
     def play(self, repeat=False):
         # TODO handle choose device (config / utterance ?)
         self.spotify.play(self.tracks, dev_id=self.device, repeat=repeat)
```

## ovos_audio_plugin_spotify/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 4
+VERSION_ALPHA = 5
 # END_VERSION_BLOCK
```

## Comparing `ovos_audio_plugin_spotify-0.0.0a4.dist-info/LICENSE` & `ovos_audio_plugin_spotify-0.0.0a5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_audio_plugin_spotify-0.0.0a4.dist-info/RECORD` & `ovos_audio_plugin_spotify-0.0.0a5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ovos_audio_plugin_spotify/__init__.py,sha256=KiuKT0K21LFJ7Z5-N0lQfn9Jnv0_K3pQbONyc9z6aFY,3365
+ovos_audio_plugin_spotify/__init__.py,sha256=QulkK97HHn8Bcl2QTajI-4rRP0dO-PUnx_s2fY_cCFs,3428
 ovos_audio_plugin_spotify/spotify_client.py,sha256=u_eQyvhKobVe7WFdR1t4K5f7Evx2u0xqPEKoQVsFG_E,28703
-ovos_audio_plugin_spotify/version.py,sha256=JN7aD_TugTLEaBIwM5kbDnKdd-QQQx3WIIaO6M_RM2s,177
-ovos_audio_plugin_spotify-0.0.0a4.dist-info/LICENSE,sha256=ntGHfW0JQ281uH6ycFGfAyFMCThkNAUM3r6HS2aPXA0,11349
-ovos_audio_plugin_spotify-0.0.0a4.dist-info/METADATA,sha256=IZFG-Z7mT6CD6l_7xAQ-QMbMNz4vdhtJf0y6G9JG-gI,387
-ovos_audio_plugin_spotify-0.0.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_audio_plugin_spotify-0.0.0a4.dist-info/entry_points.txt,sha256=eRqnpnbjSvjP2gy6-F4y1bj6PxZdk9bSuDQMZCg9YSo,179
-ovos_audio_plugin_spotify-0.0.0a4.dist-info/top_level.txt,sha256=61lSsvrOmPf1COig3R9LzTT5MQHYWehvB45eUgCNIZQ,26
-ovos_audio_plugin_spotify-0.0.0a4.dist-info/RECORD,,
+ovos_audio_plugin_spotify/version.py,sha256=hDOolhK88hLPyvV5m7E3osBHrG_NBU03rdk3-5YAKCA,177
+ovos_audio_plugin_spotify-0.0.0a5.dist-info/LICENSE,sha256=ntGHfW0JQ281uH6ycFGfAyFMCThkNAUM3r6HS2aPXA0,11349
+ovos_audio_plugin_spotify-0.0.0a5.dist-info/METADATA,sha256=4KhpQUpdjLM0j7WgXR5SinyXUg27dJm32GOTFAkHrNM,387
+ovos_audio_plugin_spotify-0.0.0a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_audio_plugin_spotify-0.0.0a5.dist-info/entry_points.txt,sha256=eRqnpnbjSvjP2gy6-F4y1bj6PxZdk9bSuDQMZCg9YSo,179
+ovos_audio_plugin_spotify-0.0.0a5.dist-info/top_level.txt,sha256=61lSsvrOmPf1COig3R9LzTT5MQHYWehvB45eUgCNIZQ,26
+ovos_audio_plugin_spotify-0.0.0a5.dist-info/RECORD,,
```

