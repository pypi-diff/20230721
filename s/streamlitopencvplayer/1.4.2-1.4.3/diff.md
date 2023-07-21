# Comparing `tmp/streamlitopencvplayer-1.4.2.tar.gz` & `tmp/streamlitopencvplayer-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.4.2.tar", last modified: Fri Jul 21 00:39:20 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.4.3.tar", last modified: Fri Jul 21 00:46:56 2023, max compression
```

## Comparing `streamlitopencvplayer-1.4.2.tar` & `streamlitopencvplayer-1.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 00:39:20.812276 streamlitopencvplayer-1.4.2/
--rw-rw-rw-   0        0        0      419 2023-07-21 00:39:20.810161 streamlitopencvplayer-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 00:39:20.813295 streamlitopencvplayer-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-21 00:39:15.000000 streamlitopencvplayer-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 00:39:20.777988 streamlitopencvplayer-1.4.2/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.2/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     8596 2023-07-21 00:19:52.000000 streamlitopencvplayer-1.4.2/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 00:39:20.798293 streamlitopencvplayer-1.4.2/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-21 00:39:20.000000 streamlitopencvplayer-1.4.2/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-21 00:39:20.000000 streamlitopencvplayer-1.4.2/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 00:39:20.000000 streamlitopencvplayer-1.4.2/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 00:39:20.000000 streamlitopencvplayer-1.4.2/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 00:39:20.805163 streamlitopencvplayer-1.4.2/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.2/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.787798 streamlitopencvplayer-1.4.3/
+-rw-rw-rw-   0        0        0      419 2023-07-21 00:46:56.785795 streamlitopencvplayer-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 00:46:56.788678 streamlitopencvplayer-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 00:46:48.000000 streamlitopencvplayer-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.755237 streamlitopencvplayer-1.4.3/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8593 2023-07-21 00:46:02.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.773489 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 00:46:56.000000 streamlitopencvplayer-1.4.3/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 00:46:56.782328 streamlitopencvplayer-1.4.3/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.3/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.3/test/test.py
```

### Comparing `streamlitopencvplayer-1.4.2/README.md` & `streamlitopencvplayer-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.4.2/setup.py` & `streamlitopencvplayer-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.2' 
+VERSION = '1.4.3' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.4.2/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.4.3/streamlitopencvplayer/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if "data" not in st.session_state:
     st.session_state['data'] = []
 
 
 # Function to display video in the Streamlit app
 
 
-def draw_detections(stframe, frame, i):
+def draw_on_frames(stframe, frame, i):
     st.write(st.session_state["capture"].get(
         cv2.CAP_PROP_POS_FRAMES))
     # Draw detections on the frame
     for j in range(len(st.session_state['data'][i])):
         output = cv2.rectangle(frame, (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]), (
             st.session_state['data'][i][j][0][2], st.session_state['data'][i][j][0][3]), color=(128, 0, 0), thickness=2)
         output = cv2.putText(
@@ -104,15 +104,15 @@
             if button_value == 1:
                 st.session_state["resume"] = True
                 # Set the video capture position to the selected alert frame
                 st.session_state["capture"].set(
                     cv2.CAP_PROP_POS_FRAMES, st.session_state['alerts'][int(button_label)]-1)
                 ret, frame = st.session_state["capture"].read()
                 if draw_detections:
-                    draw_detections(stframe, frame, int(button_label))
+                    draw_on_frames(stframe, frame, int(button_label))
                 else:
                     stframe.image(frame, caption='', width=500)
 
                 # st.write(st.session_state['alerts'][int(button_label)])
                 # st.write(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))
                 # Set "resume" to True to stop the video playback from the selected alert
                 #  add read
@@ -144,15 +144,15 @@
 
         if draw_detections:
             # Perform actions on the frame
             for i in range(len(st.session_state['data'])):
 
                 # Check if the current frame matches an alert frame
                 if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(st.session_state['alerts'][i]):
-                    draw_detections(stframe, frame, i)
+                    draw_on_frames(stframe, frame, i)
         # Display the original frame
         stframe.image(
             frame, caption='', width=500)
         time.sleep(0.05)
 
         # Handle button clicks
         if pause:
```

### Comparing `streamlitopencvplayer-1.4.2/test/test.py` & `streamlitopencvplayer-1.4.3/test/test.py`

 * *Files identical despite different names*

