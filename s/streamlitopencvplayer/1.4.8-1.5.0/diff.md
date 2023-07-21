# Comparing `tmp/streamlitopencvplayer-1.4.8.tar.gz` & `tmp/streamlitopencvplayer-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.4.8.tar", last modified: Fri Jul 21 12:35:52 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.5.0.tar", last modified: Fri Jul 21 12:43:26 2023, max compression
```

## Comparing `streamlitopencvplayer-1.4.8.tar` & `streamlitopencvplayer-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:35:52.011635 streamlitopencvplayer-1.4.8/
--rw-rw-rw-   0        0        0      419 2023-07-21 12:35:52.010634 streamlitopencvplayer-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 12:35:52.012634 streamlitopencvplayer-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-21 12:35:46.000000 streamlitopencvplayer-1.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:35:51.982636 streamlitopencvplayer-1.4.8/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8150 2023-07-21 12:34:24.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:35:51.997635 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 12:35:51.000000 streamlitopencvplayer-1.4.8/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 12:35:52.006634 streamlitopencvplayer-1.4.8/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.8/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.485322 streamlitopencvplayer-1.5.0/
+-rw-rw-rw-   0        0        0      419 2023-07-21 12:43:26.484320 streamlitopencvplayer-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:43:26.486321 streamlitopencvplayer-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 12:43:21.000000 streamlitopencvplayer-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.457324 streamlitopencvplayer-1.5.0/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8513 2023-07-21 12:42:50.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.473324 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 12:43:26.000000 streamlitopencvplayer-1.5.0/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 12:43:26.480366 streamlitopencvplayer-1.5.0/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.0/test/test.py
```

### Comparing `streamlitopencvplayer-1.4.8/README.md` & `streamlitopencvplayer-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.4.8/setup.py` & `streamlitopencvplayer-1.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.8' 
+VERSION = '1.5.0' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.4.8/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.5.0/streamlitopencvplayer/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import json
 import time
 import urllib.request
 
 import cv2
 import streamlit as st
-
-
 if "alerts" not in st.session_state:
-    alerts = []
+    st.session_state['alerts'] = []
 if "data" not in st.session_state:
-    data = []
+    st.session_state['data'] = []
+
 
 # Function to display video in the Streamlit app
 
 
-def draw_on_frames(stframe, frame, i,data):
+def draw_on_frames(stframe, frame, i):
+
     # Draw detections on the frame
-    for j in range(len(data[i])):
-        output = cv2.rectangle(frame, (data[i][j][0][0], data[i][j][0][1]), (
-            data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
+    for j in range(len(st.session_state['data'][i])):
+        output = cv2.rectangle(frame, (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]), (
+            st.session_state['data'][i][j][0][2], st.session_state['data'][i][j][0][3]), color=(128, 0, 0), thickness=2)
         output = cv2.putText(
-            frame, data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
+            frame, st.session_state['data'][i][j][3], (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
     # Display the frame with detections
     stframe.image(output, caption='', width=500)
     time.sleep(0.05)
 
 
 def display_video(video_path, json_file):
     # Check if video_url variables exists in session state
@@ -34,15 +34,14 @@
             st.session_state['capture'] = cv2.VideoCapture(video_path)
     else:
         # Check if the video URL has changed
         if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
             st.session_state['capture'] = cv2.VideoCapture(video_path)
             st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
 
-
     # Check if "fps" variable exists in session state
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
         st.write("No much video to open")
         exit()
@@ -62,38 +61,38 @@
         for alert in fileReader["alerts"]:
             list_ts.append(alert["timestamp"])
             list_data.append(alert["data"])
 
         # Store the timestamps and data in the session state
         st.session_state['alerts_list'] = list_ts
 
-        alerts = []
-        data = []
+        st.session_state['alerts'] = []
+        st.session_state['data'] = []
 
         # Calculate the frame positions for each alert
         for x in range(len(list_ts)):
             # Calculate the time difference between the alert timestamp and the selected video timestamp start
             time_alert = float(list_ts[x])-float(
                 st.session_state['name_vid_sel'].partition('_')[0])
             # Convert the time difference to frame position by multiplying with the FPS
-            alerts.append(
+            st.session_state['alerts'].append(
                 int((time_alert)*st.session_state['fps']))
-            data.append(list_data[x])
+            st.session_state['data'].append(list_data[x])
 
     # checkbox to enable detections
     draw_detections = st.checkbox("Draw detections", value=True)
     column1, column2, column3 = st.columns([1, 2, 1])
     with column1:
         # zone to display images
         stframe = st.empty()
     with column3:
         # Create buttons for alerts
         st.subheader('Alerts :')
         # Determine the number of buttons based on the number of alerts
-        num_buttons = len(alerts)
+        num_buttons = len(st.session_state['alerts'])
         # Create a dictionary to store the button values
         button_values = {f'{i}': 0 for i in range(num_buttons)}
 
         # Display the buttons and update their values
         for button_label, button_value in button_values.items():
             if st.button(str('Alert ')+button_label):
                 # Set the selected button to 1, others to 0
@@ -101,22 +100,22 @@
                                  button_label else 0 for label in button_values}
         # Perform actions based on the button values
         for button_label, button_value in button_values.items():
             if button_value == 1:
                 st.session_state["resume"] = True
                 # Set the video capture position to the selected alert frame
                 st.session_state["capture"].set(
-                    cv2.CAP_PROP_POS_FRAMES, alerts[int(button_label)]-1)
+                    cv2.CAP_PROP_POS_FRAMES, st.session_state['alerts'][int(button_label)]-1)
                 ret, frame = st.session_state["capture"].read()
                 if draw_detections:
-                    draw_on_frames(stframe, frame, int(button_label),data)
+                    draw_on_frames(stframe, frame, int(button_label))
                 else:
                     stframe.image(frame, caption='', width=500)
 
-                # st.write(alerts[int(button_label)])
+                # st.write(st.session_state['alerts'][int(button_label)])
                 # st.write(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))
                 # Set "resume" to True to stop the video playback from the selected alert
                 #  add read
 
     # Buttons and zone of display
     col1, col2, col3, col4, col5, col6, col7 = st.columns(7, gap="small")
     with col1:
@@ -140,19 +139,19 @@
         # for x in range(int(st.session_state['fps'])):
         # Read the next frame from the video capture
         ret, frame = st.session_state["capture"].read()
         # Update the current frame in session state
 
         if draw_detections:
             # Perform actions on the frame
-            for i in range(len(data)):
+            for i in range(len(st.session_state['data'])):
 
                 # Check if the current frame matches an alert frame
-                if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(alerts[i]):
-                    draw_on_frames(stframe, frame, i,data)
+                if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(st.session_state['alerts'][i]):
+                    draw_on_frames(stframe, frame, i)
         # Display the original frame
         stframe.image(
             frame, caption='', width=500)
         time.sleep(0.05)
 
         # Handle button clicks
         if pause:
```

### Comparing `streamlitopencvplayer-1.4.8/test/test.py` & `streamlitopencvplayer-1.5.0/test/test.py`

 * *Files identical despite different names*

