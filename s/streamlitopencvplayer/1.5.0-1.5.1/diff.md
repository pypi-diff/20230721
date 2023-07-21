# Comparing `tmp/streamlitopencvplayer-1.5.0.tar.gz` & `tmp/streamlitopencvplayer-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.5.0.tar", last modified: Fri Jul 21 12:43:26 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.5.1.tar", last modified: Fri Jul 21 13:02:12 2023, max compression
```

## Comparing `streamlitopencvplayer-1.5.0.tar` & `streamlitopencvplayer-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.485322 streamlitopencvplayer-1.5.0/
--rw-rw-rw-   0        0        0      419 2023-07-21 12:43:26.484320 streamlitopencvplayer-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 12:43:26.486321 streamlitopencvplayer-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-21 12:43:21.000000 streamlitopencvplayer-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.457324 streamlitopencvplayer-1.5.0/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8513 2023-07-21 12:42:50.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.473324 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.480366 streamlitopencvplayer-1.5.0/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.0/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:02:12.152552 streamlitopencvplayer-1.5.1/
+-rw-rw-rw-   0        0        0      419 2023-07-21 13:02:12.151552 streamlitopencvplayer-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:02:12.153555 streamlitopencvplayer-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 13:02:08.000000 streamlitopencvplayer-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:02:12.124555 streamlitopencvplayer-1.5.1/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.1/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8591 2023-07-21 13:01:56.000000 streamlitopencvplayer-1.5.1/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:02:12.140553 streamlitopencvplayer-1.5.1/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-21 13:02:11.000000 streamlitopencvplayer-1.5.1/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-21 13:02:12.000000 streamlitopencvplayer-1.5.1/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:02:11.000000 streamlitopencvplayer-1.5.1/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 13:02:11.000000 streamlitopencvplayer-1.5.1/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 13:02:12.147550 streamlitopencvplayer-1.5.1/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.1/test/test.py
```

### Comparing `streamlitopencvplayer-1.5.0/README.md` & `streamlitopencvplayer-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.5.0/setup.py` & `streamlitopencvplayer-1.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.5.0' 
+VERSION = '1.5.1' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.5.0/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.5.1/streamlitopencvplayer/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
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
-
     # Draw detections on the frame
     for j in range(len(st.session_state['data'][i])):
         output = cv2.rectangle(frame, (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]), (
             st.session_state['data'][i][j][0][2], st.session_state['data'][i][j][0][3]), color=(128, 0, 0), thickness=2)
         output = cv2.putText(
             frame, st.session_state['data'][i][j][3], (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
     # Display the frame with detections
@@ -34,14 +35,15 @@
             st.session_state['capture'] = cv2.VideoCapture(video_path)
     else:
         # Check if the video URL has changed
         if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
             st.session_state['capture'] = cv2.VideoCapture(video_path)
             st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
 
+
     # Check if "fps" variable exists in session state
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
         st.write("No much video to open")
         exit()
```

### Comparing `streamlitopencvplayer-1.5.0/test/test.py` & `streamlitopencvplayer-1.5.1/test/test.py`

 * *Files identical despite different names*

