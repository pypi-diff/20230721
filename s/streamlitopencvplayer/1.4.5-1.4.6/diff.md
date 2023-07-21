# Comparing `tmp/streamlitopencvplayer-1.4.5.tar.gz` & `tmp/streamlitopencvplayer-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.4.5.tar", last modified: Fri Jul 21 08:09:54 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.4.6.tar", last modified: Fri Jul 21 08:13:12 2023, max compression
```

## Comparing `streamlitopencvplayer-1.4.5.tar` & `streamlitopencvplayer-1.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:09:54.773632 streamlitopencvplayer-1.4.5/
--rw-rw-rw-   0        0        0      419 2023-07-21 08:09:54.771633 streamlitopencvplayer-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 08:09:54.774632 streamlitopencvplayer-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-21 08:09:45.000000 streamlitopencvplayer-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:09:54.740732 streamlitopencvplayer-1.4.5/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.5/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     7652 2023-07-21 08:09:39.000000 streamlitopencvplayer-1.4.5/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:09:54.759155 streamlitopencvplayer-1.4.5/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-21 08:09:54.000000 streamlitopencvplayer-1.4.5/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-21 08:09:54.000000 streamlitopencvplayer-1.4.5/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:09:54.000000 streamlitopencvplayer-1.4.5/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 08:09:54.000000 streamlitopencvplayer-1.4.5/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 08:09:54.767157 streamlitopencvplayer-1.4.5/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.5/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:13:12.828365 streamlitopencvplayer-1.4.6/
+-rw-rw-rw-   0        0        0      419 2023-07-21 08:13:12.826360 streamlitopencvplayer-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:13:12.829360 streamlitopencvplayer-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 08:13:05.000000 streamlitopencvplayer-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:13:12.794917 streamlitopencvplayer-1.4.6/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.4.6/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8204 2023-07-21 08:12:46.000000 streamlitopencvplayer-1.4.6/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:13:12.814926 streamlitopencvplayer-1.4.6/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-21 08:13:12.000000 streamlitopencvplayer-1.4.6/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-21 08:13:12.000000 streamlitopencvplayer-1.4.6/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:13:12.000000 streamlitopencvplayer-1.4.6/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 08:13:12.000000 streamlitopencvplayer-1.4.6/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 08:13:12.822837 streamlitopencvplayer-1.4.6/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.4.6/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.4.6/test/test.py
```

### Comparing `streamlitopencvplayer-1.4.5/README.md` & `streamlitopencvplayer-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.4.5/setup.py` & `streamlitopencvplayer-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.5' 
+VERSION = '1.4.6' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.4.5/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.4.6/streamlitopencvplayer/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     st.session_state['data'] = []
 st.session_state['name_vid_sel'] = "1689004947.7068138_1689004953.7068138"
 
 # Function to display video in the Streamlit app
 
 
 def draw_on_frames(stframe, frame, i):
-    st.write(st.session_state["capture"].get(
-        cv2.CAP_PROP_POS_FRAMES))
     # Draw detections on the frame
     for j in range(len(st.session_state['data'][i])):
         output = cv2.rectangle(frame, (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]), (
             st.session_state['data'][i][j][0][2], st.session_state['data'][i][j][0][3]), color=(128, 0, 0), thickness=2)
         output = cv2.putText(
             frame, st.session_state['data'][i][j][3], (st.session_state['data'][i][j][0][0], st.session_state['data'][i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
     # Display the frame with detections
@@ -93,15 +91,25 @@
         # Display the buttons and update their values
         for button_label, button_value in button_values.items():
             if st.button(str('Alert ')+button_label):
                 # Set the selected button to 1, others to 0
                 button_values = {label: 1 if label ==
                                  button_label else 0 for label in button_values}
         # Perform actions based on the button values
-
+        for button_label, button_value in button_values.items():
+            if button_value == 1:
+                st.session_state["resume"] = True
+                # Set the video capture position to the selected alert frame
+                st.session_state["capture"].set(
+                    cv2.CAP_PROP_POS_FRAMES, st.session_state['alerts'][int(button_label)]-1)
+                ret, frame = st.session_state["capture"].read()
+                if draw_detections:
+                    draw_on_frames(stframe, frame, int(button_label))
+                else:
+                    stframe.image(frame, caption='', width=500)
 
                 # st.write(st.session_state['alerts'][int(button_label)])
                 # st.write(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))
                 # Set "resume" to True to stop the video playback from the selected alert
                 #  add read
 
     # Buttons and zone of display
```

### Comparing `streamlitopencvplayer-1.4.5/test/test.py` & `streamlitopencvplayer-1.4.6/test/test.py`

 * *Files identical despite different names*

