# Comparing `tmp/streamlitopencvplayer-1.5.2.tar.gz` & `tmp/streamlitopencvplayer-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.5.2.tar", last modified: Fri Jul 21 13:06:46 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.5.3.tar", last modified: Fri Jul 21 13:10:01 2023, max compression
```

## Comparing `streamlitopencvplayer-1.5.2.tar` & `streamlitopencvplayer-1.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:06:46.724054 streamlitopencvplayer-1.5.2/
--rw-rw-rw-   0        0        0      419 2023-07-21 13:06:46.723051 streamlitopencvplayer-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 13:06:46.725051 streamlitopencvplayer-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-21 13:06:42.000000 streamlitopencvplayer-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:06:46.697052 streamlitopencvplayer-1.5.2/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.2/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     7859 2023-07-21 13:06:31.000000 streamlitopencvplayer-1.5.2/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:06:46.713055 streamlitopencvplayer-1.5.2/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-21 13:06:46.000000 streamlitopencvplayer-1.5.2/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-21 13:06:46.000000 streamlitopencvplayer-1.5.2/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:06:46.000000 streamlitopencvplayer-1.5.2/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 13:06:46.000000 streamlitopencvplayer-1.5.2/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 13:06:46.720051 streamlitopencvplayer-1.5.2/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.2/test/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:10:01.013304 streamlitopencvplayer-1.5.3/
+-rw-rw-rw-   0        0        0      419 2023-07-21 13:10:01.011304 streamlitopencvplayer-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:10:01.014306 streamlitopencvplayer-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-21 13:09:54.000000 streamlitopencvplayer-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:10:00.986267 streamlitopencvplayer-1.5.3/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.5.3/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     8491 2023-07-21 13:09:24.000000 streamlitopencvplayer-1.5.3/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:10:01.000310 streamlitopencvplayer-1.5.3/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-21 13:10:00.000000 streamlitopencvplayer-1.5.3/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-21 13:10:00.000000 streamlitopencvplayer-1.5.3/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:10:00.000000 streamlitopencvplayer-1.5.3/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 13:10:00.000000 streamlitopencvplayer-1.5.3/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 13:10:01.008306 streamlitopencvplayer-1.5.3/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.5.3/test/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-07-16 23:22:17.000000 streamlitopencvplayer-1.5.3/test/test.py
```

### Comparing `streamlitopencvplayer-1.5.2/README.md` & `streamlitopencvplayer-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.5.2/setup.py` & `streamlitopencvplayer-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.5.2' 
+VERSION = '1.5.3' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.5.2/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.5.3/streamlitopencvplayer/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,71 +25,76 @@
     # Display the frame with detections
     stframe.image(output, caption='', width=500)
     time.sleep(0.05)
 
 
 def display_video(video_path, json_file):
     # Check if video_url variables exists in session state
-
-    if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
+    if "name_vid_old" not in st.session_state and "name_vid_sel" not in st.session_state:
+        if "capture" not in st.session_state:
+            # Open the video file
+            st.session_state['capture'] = cv2.VideoCapture(video_path)
+    else:
+        # Check if the video URL has changed
+        if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
             st.session_state['capture'] = cv2.VideoCapture(video_path)
-            #st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
+            st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
 
 
     # Check if "fps" variable exists in session state
     if "fps" not in st.session_state:
         st.session_state['fps'] = st.session_state['capture'].get(
             cv2.CAP_PROP_FPS)
     if not st.session_state["capture"].isOpened():
         st.write("No much video to open")
         exit()
     # Check if "resume" variable exists in session state
     if "resume" not in st.session_state:
         st.session_state["resume"] = False
 
     # Opening JSON file and returns JSON object as a dictionnary
-    if json_file is not None and st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
+    if json_file is not None:
         # Open and read the JSON file from the given URL
         response = urllib.request.urlopen(json_file)
         fileReader = json.loads(response.read())
         list_ts = []
         list_data = []
 
         # Extract the timestamp and data from each alert in the JSON file
         for alert in fileReader["alerts"]:
             list_ts.append(alert["timestamp"])
             list_data.append(alert["data"])
 
         # Store the timestamps and data in the session state
         st.session_state['alerts_list'] = list_ts
 
-        st.session_state['alerts'] = []
+        alerts = []
         st.session_state['data'] = []
 
         # Calculate the frame positions for each alert
         for x in range(len(list_ts)):
             # Calculate the time difference between the alert timestamp and the selected video timestamp start
             time_alert = float(list_ts[x])-float(
                 st.session_state['name_vid_sel'].partition('_')[0])
             # Convert the time difference to frame position by multiplying with the FPS
-            st.session_state['alerts'].append(
+            alerts.append(
                 int((time_alert)*st.session_state['fps']))
             st.session_state['data'].append(list_data[x])
 
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
-        num_buttons = len(st.session_state['alerts'])
+        num_buttons = len(alerts)
         # Create a dictionary to store the button values
         button_values = {f'{i}': 0 for i in range(num_buttons)}
 
         # Display the buttons and update their values
         for button_label, button_value in button_values.items():
             if st.button(str('Alert ')+button_label):
                 # Set the selected button to 1, others to 0
@@ -97,22 +102,22 @@
                                  button_label else 0 for label in button_values}
         # Perform actions based on the button values
         for button_label, button_value in button_values.items():
             if button_value == 1:
                 st.session_state["resume"] = True
                 # Set the video capture position to the selected alert frame
                 st.session_state["capture"].set(
-                    cv2.CAP_PROP_POS_FRAMES, st.session_state['alerts'][int(button_label)]-1)
+                    cv2.CAP_PROP_POS_FRAMES, alerts[int(button_label)]-1)
                 ret, frame = st.session_state["capture"].read()
                 if draw_detections:
                     draw_on_frames(stframe, frame, int(button_label))
                 else:
                     stframe.image(frame, caption='', width=500)
 
-                # st.write(st.session_state['alerts'][int(button_label)])
+                # st.write(alerts[int(button_label)])
                 # st.write(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))
                 # Set "resume" to True to stop the video playback from the selected alert
                 #  add read
 
     # Buttons and zone of display
     col1, col2, col3, col4, col5, col6, col7 = st.columns(7, gap="small")
     with col1:
@@ -172,9 +177,19 @@
 
     # Perform actions when "resume" is True
     if st.session_state["resume"]:
         # Clear the container
         container_2.empty()
         pause = container_2.button('▶')
         st.session_state["resume"] = False
-    if st.session_state['name_vid_old'] != st.session_state['name_vid_sel']:
-        st.session_state['name_vid_old'] = st.session_state['name_vid_sel']
+
+
+def main():
+
+    video_path = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138.webm?sv=2021-10-04&st=2023-07-11T15%3A21%3A27Z&se=2023-07-26T15%3A21%3A00Z&sr=b&sp=r&sig=u6uuOUo9wvn5KJFNUnUR3axYtC815SUQBuDqNIC4L%2Bw%3D"
+    down_json = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138_global.json?sv=2021-10-04&st=2023-07-11T15%3A22%3A03Z&se=2023-07-26T15%3A22%3A00Z&sr=b&sp=r&sig=qSHWvDUIOOT%2F%2Bff270JVX7ucSRn5Lylgw5%2Fh9iTa4BY%3D"
+    if video_path is not None:
+        display_video(video_path, down_json)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `streamlitopencvplayer-1.5.2/test/test.py` & `streamlitopencvplayer-1.5.3/test/test.py`

 * *Files identical despite different names*

