# Comparing `tmp/streamlitopencvplayer-1.4.3.tar.gz` & `tmp/streamlitopencvplayer-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.4.3.tar", last modified: Fri Jul 21 00:46:56 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.4.4.tar", last modified: Fri Jul 21 01:13:31 2023, max compression
```

## Comparing `streamlitopencvplayer-1.4.3.tar` & `streamlitopencvplayer-1.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.787798 streamlitopencvplayer-1.4.3/
--rw-rw-rw-   0        0        0      419 2023-07-21 00:46:56.785795 streamlitopencvplayer-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 00:46:56.788678 streamlitopencvplayer-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-21 00:46:48.000000 streamlitopencvplayer-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.755237 streamlitopencvplayer-1.4.3/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8593 2023-07-21 00:46:02.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.773489 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.782328 streamlitopencvplayer-1.4.3/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.3/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.3/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:13:31.548943 streamlitopencvplayer-1.4.4/
+-rw-rw-rw-   0        0        0      419 2023-07-21 01:13:31.547515 streamlitopencvplayer-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 01:13:31.548943 streamlitopencvplayer-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 01:13:24.000000 streamlitopencvplayer-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:13:31.516726 streamlitopencvplayer-1.4.4/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.4/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8270 2023-07-21 01:13:20.000000 streamlitopencvplayer-1.4.4/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:13:31.535420 streamlitopencvplayer-1.4.4/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-21 01:13:31.000000 streamlitopencvplayer-1.4.4/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-21 01:13:31.000000 streamlitopencvplayer-1.4.4/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 01:13:31.000000 streamlitopencvplayer-1.4.4/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 01:13:31.000000 streamlitopencvplayer-1.4.4/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 01:13:31.543170 streamlitopencvplayer-1.4.4/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.4/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.4/test/test.py
```

### Comparing `streamlitopencvplayer-1.4.3/README.md` & `streamlitopencvplayer-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.4.3/setup.py` & `streamlitopencvplayer-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.3' 
+VERSION = '1.4.4' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.4.3/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.4.4/streamlitopencvplayer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 import time
 import urllib.request
 
 import cv2
 import streamlit as st
+
+
 if "alerts" not in st.session_state:
     st.session_state['alerts'] = []
 if "data" not in st.session_state:
     st.session_state['data'] = []
-
+st.session_state['name_vid_sel'] = "1689004947.7068138_1689004953.7068138"
 
 # Function to display video in the Streamlit app
 
 
 def draw_on_frames(stframe, frame, i):
     st.write(st.session_state["capture"].get(
         cv2.CAP_PROP_POS_FRAMES))
@@ -25,23 +27,18 @@
     # Display the frame with detections
     stframe.image(output, caption='', width=500)
     time.sleep(0.05)
 
 
 def display_video(video_path, json_file):
     # Check if video_url variables exists in session state
-    if "name_vid_old" not in st.session_state and "name_vid_sel" not in st.session_state:
-        if "capture" not in st.session_state:
+    if "capture" not in st.session_state:
             # Open the video file
             st.session_state['capture'] = cv2.VideoCapture(video_path)
-    else:
-        # Check if the video URL has changed
-        if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
-            st.session_state['capture'] = cv2.VideoCapture(video_path)
-            st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
+
 
     # Check if "fps" variable exists in session state
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
         st.write("No much video to open")
@@ -104,15 +101,15 @@
             if button_value == 1:
                 st.session_state["resume"] = True
                 # Set the video capture position to the selected alert frame
                 st.session_state["capture"].set(
                     cv2.CAP_PROP_POS_FRAMES, st.session_state['alerts'][int(button_label)]-1)
                 ret, frame = st.session_state["capture"].read()
                 if draw_detections:
-                    draw_on_frames(stframe, frame, int(button_label))
+                    draw_on_frames(stframe, frame, 0)
                 else:
                     stframe.image(frame, caption='', width=500)
 
                 # st.write(st.session_state['alerts'][int(button_label)])
                 # st.write(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))
                 # Set "resume" to True to stop the video playback from the selected alert
                 #  add read
```

### Comparing `streamlitopencvplayer-1.4.3/test/test.py` & `streamlitopencvplayer-1.4.4/test/test.py`

 * *Files identical despite different names*

