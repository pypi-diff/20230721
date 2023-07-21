# Comparing `tmp/streamlitopencvplayer-1.4.7.tar.gz` & `tmp/streamlitopencvplayer-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.4.7.tar", last modified: Fri Jul 21 12:32:28 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.4.8.tar", last modified: Fri Jul 21 12:35:52 2023, max compression
```

## Comparing `streamlitopencvplayer-1.4.7.tar` & `streamlitopencvplayer-1.4.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:32:28.269410 streamlitopencvplayer-1.4.7/
--rw-rw-rw-   0        0        0      419 2023-07-21 12:32:28.268406 streamlitopencvplayer-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 12:32:28.270406 streamlitopencvplayer-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-21 12:32:22.000000 streamlitopencvplayer-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:32:28.239404 streamlitopencvplayer-1.4.7/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.7/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     7839 2023-07-21 12:31:53.000000 streamlitopencvplayer-1.4.7/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:32:28.256405 streamlitopencvplayer-1.4.7/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-21 12:32:27.000000 streamlitopencvplayer-1.4.7/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-21 12:32:28.000000 streamlitopencvplayer-1.4.7/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:32:27.000000 streamlitopencvplayer-1.4.7/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 12:32:27.000000 streamlitopencvplayer-1.4.7/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 12:32:28.264405 streamlitopencvplayer-1.4.7/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.7/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:35:52.011635 streamlitopencvplayer-1.4.8/
+-rw-rw-rw-   0        0        0      419 2023-07-21 12:35:52.010634 streamlitopencvplayer-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:35:52.012634 streamlitopencvplayer-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 12:35:46.000000 streamlitopencvplayer-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:35:51.982636 streamlitopencvplayer-1.4.8/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8150 2023-07-21 12:34:24.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:35:51.997635 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 12:35:52.006634 streamlitopencvplayer-1.4.8/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.8/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.8/test/test.py
```

### Comparing `streamlitopencvplayer-1.4.7/README.md` & `streamlitopencvplayer-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.4.7/setup.py` & `streamlitopencvplayer-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.7' 
+VERSION = '1.4.8' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.4.7/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.4.8/streamlitopencvplayer/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import streamlit as st
 
 
 if "alerts" not in st.session_state:
     alerts = []
 if "data" not in st.session_state:
     data = []
-st.session_state['name_vid_sel'] = "1689004947.7068138_1689004953.7068138"
 
 # Function to display video in the Streamlit app
 
 
 def draw_on_frames(stframe, frame, i,data):
     # Draw detections on the frame
     for j in range(len(data[i])):
@@ -25,17 +24,23 @@
     # Display the frame with detections
     stframe.image(output, caption='', width=500)
     time.sleep(0.05)
 
 
 def display_video(video_path, json_file):
     # Check if video_url variables exists in session state
-    if "capture" not in st.session_state:
+    if "name_vid_old" not in st.session_state and "name_vid_sel" not in st.session_state:
+        if "capture" not in st.session_state:
             # Open the video file
             st.session_state['capture'] = cv2.VideoCapture(video_path)
+    else:
+        # Check if the video URL has changed
+        if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
+            st.session_state['capture'] = cv2.VideoCapture(video_path)
+            st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
 
 
     # Check if "fps" variable exists in session state
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
```

### Comparing `streamlitopencvplayer-1.4.7/test/test.py` & `streamlitopencvplayer-1.4.8/test/test.py`

 * *Files identical despite different names*

