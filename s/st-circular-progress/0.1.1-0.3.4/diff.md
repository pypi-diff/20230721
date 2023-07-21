# Comparing `tmp/st_circular_progress-0.1.1.tar.gz` & `tmp/st_circular_progress-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_circular_progress-0.1.1.tar", last modified: Fri Jul 21 01:23:35 2023, max compression
+gzip compressed data, was "st_circular_progress-0.3.4.tar", last modified: Fri Jul 21 15:49:28 2023, max compression
```

## Comparing `st_circular_progress-0.1.1.tar` & `st_circular_progress-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,26 @@
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:23:35.012142 st_circular_progress-0.1.1/
--rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.1.1/LICENSE
--rw-rw-r--   0 cserrano   (501) staff       (20)       43 2023-07-12 21:17:31.000000 st_circular_progress-0.1.1/MANIFEST.in
--rw-r--r--   0 cserrano   (501) staff       (20)      317 2023-07-21 01:23:35.011797 st_circular_progress-0.1.1/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 01:23:35.012255 st_circular_progress-0.1.1/setup.cfg
--rw-rw-r--   0 cserrano   (501) staff       (20)      539 2023-07-21 01:23:29.000000 st_circular_progress-0.1.1/setup.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:23:35.008226 st_circular_progress-0.1.1/st_circular_progress/
--rw-rw-r--   0 cserrano   (501) staff       (20)     2707 2023-07-21 00:01:57.000000 st_circular_progress-0.1.1/st_circular_progress/__init__.py
-drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 01:23:35.011004 st_circular_progress-0.1.1/st_circular_progress.egg-info/
--rw-r--r--   0 cserrano   (501) staff       (20)      317 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/PKG-INFO
--rw-r--r--   0 cserrano   (501) staff       (20)      280 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/SOURCES.txt
--rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/dependency_links.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       16 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/requires.txt
--rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 01:23:34.000000 st_circular_progress-0.1.1/st_circular_progress.egg-info/top_level.txt
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 15:49:28.762932 st_circular_progress-0.3.4/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     1063 2023-07-12 21:17:31.000000 st_circular_progress-0.3.4/LICENSE
+-rw-rw-r--   0 cserrano   (501) staff       (20)       89 2023-07-21 15:17:58.000000 st_circular_progress-0.3.4/MANIFEST.in
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 15:49:28.762591 st_circular_progress-0.3.4/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)     2874 2023-07-21 15:48:57.000000 st_circular_progress-0.3.4/README.md
+-rw-r--r--   0 cserrano   (501) staff       (20)       38 2023-07-21 15:49:28.763043 st_circular_progress-0.3.4/setup.cfg
+-rw-rw-r--   0 cserrano   (501) staff       (20)      633 2023-07-21 15:49:22.000000 st_circular_progress-0.3.4/setup.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 15:49:28.751961 st_circular_progress-0.3.4/st_circular_progress/
+-rw-rw-r--   0 cserrano   (501) staff       (20)     3683 2023-07-21 15:38:05.000000 st_circular_progress-0.3.4/st_circular_progress/__init__.py
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 15:49:28.747490 st_circular_progress-0.3.4/st_circular_progress/frontend/
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 15:49:28.758415 st_circular_progress-0.3.4/st_circular_progress/frontend/build/
+-rw-r--r--   0 cserrano   (501) staff       (20)      221 2023-07-21 15:10:53.000000 st_circular_progress-0.3.4/st_circular_progress/frontend/build/asset-manifest.json
+-rw-rw-r--   0 cserrano   (501) staff       (20)   197459 2023-07-21 15:10:47.000000 st_circular_progress-0.3.4/st_circular_progress/frontend/build/bootstrap.min.css
+-rw-r--r--   0 cserrano   (501) staff       (20)      194 2023-07-21 15:10:53.000000 st_circular_progress-0.3.4/st_circular_progress/frontend/build/index.html
+-rw-r--r--   0 cserrano   (501) staff       (20)     1663 2023-07-21 15:10:47.000000 st_circular_progress-0.3.4/st_circular_progress/frontend/build/progress.css
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 15:49:28.748289 st_circular_progress-0.3.4/st_circular_progress/frontend/build/static/
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 15:49:28.760799 st_circular_progress-0.3.4/st_circular_progress/frontend/build/static/js/
+-rw-r--r--   0 cserrano   (501) staff       (20)   254162 2023-07-21 15:10:53.000000 st_circular_progress-0.3.4/st_circular_progress/frontend/build/static/js/main.8241ff8d.js
+-rw-r--r--   0 cserrano   (501) staff       (20)      692 2023-07-21 15:10:53.000000 st_circular_progress-0.3.4/st_circular_progress/frontend/build/static/js/main.8241ff8d.js.LICENSE.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)  1042955 2023-07-21 15:10:53.000000 st_circular_progress-0.3.4/st_circular_progress/frontend/build/static/js/main.8241ff8d.js.map
+drwxr-xr-x   0 cserrano   (501) staff       (20)        0 2023-07-21 15:49:28.755141 st_circular_progress-0.3.4/st_circular_progress.egg-info/
+-rw-r--r--   0 cserrano   (501) staff       (20)      411 2023-07-21 15:49:28.000000 st_circular_progress-0.3.4/st_circular_progress.egg-info/PKG-INFO
+-rw-r--r--   0 cserrano   (501) staff       (20)      701 2023-07-21 15:49:28.000000 st_circular_progress-0.3.4/st_circular_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)        1 2023-07-21 15:49:28.000000 st_circular_progress-0.3.4/st_circular_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       18 2023-07-21 15:49:28.000000 st_circular_progress-0.3.4/st_circular_progress.egg-info/requires.txt
+-rw-r--r--   0 cserrano   (501) staff       (20)       21 2023-07-21 15:49:28.000000 st_circular_progress-0.3.4/st_circular_progress.egg-info/top_level.txt
```

### Comparing `st_circular_progress-0.1.1/LICENSE` & `st_circular_progress-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st_circular_progress-0.1.1/setup.py` & `st_circular_progress-0.3.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 setuptools.setup(
     name="st_circular_progress",
-    version="0.1.1",
+    version="0.3.4",
     author="Carlos D Serrano",
     author_email="sqlinsights@gmail.com",
     description="Circular progress wheel for Streamlit",
-    long_description="",
+    long_description="Streamlit custom component based in VanillaJs that generates a Circular Shaped progress bar.",
     long_description_content_type="text/plain",
     url="https://github.com/sqlinsights/st-circular-progress",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.6",
     install_requires=[
-        "streamlit >= 0.63",
+        "streamlit >= 1.20.0",
     ],
 )
```

### Comparing `st_circular_progress-0.1.1/st_circular_progress/__init__.py` & `st_circular_progress-0.3.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,115 @@
-import os
-import streamlit.components.v1 as components
-import streamlit as st
+# Streamlit Circular Progress Component
+> Author: Carlos D. Serrano
 
-_RELEASE = True
+## Installation and Usage Sample:
 
+### Install using PIP
+```
+pip install st-circular-progress
+```
+## Creating an instance
+Each circular slider must be initialized by calling the CircularProgress class, which requires the following attributes:
+- Label
+- Value
+- Key
+- size [optional] defaults to "medium"
+- track_color [optional] defaults to "lightgray"
+- color [optional] defaults to "blue"
+
+**Example**
+```python
+my_circular_progress = CircularProgress(
+    label="Sample Bar",
+    value=55,
+    key="my_circular_progress").st_circular_progress()
+```
+or 
+
+```python
+my_circular_progress = CircularProgress(
+    label="Sample Bar",
+    value=55,
+    key="my_circular_progress")
+
+my_circular_progress.st_circular_progress()
+```
+
+## Updating Values
+This widget uses session states and there are two ways of refreshing its state:
+- Use a callback function on your widget causing the change (not the circular progress)
+- Use Re-Run to reload
+
+An `update_value()` function has been provided to facilitate updating the value of a pre-defined `CircularProgress`
+
+**Example**
+```python
+my_circular_progress.update_values(progress=100)
+```
+### Sample Code
+
+```python
+
+ import streamlit as st
+    import pandas as pd
+    import numpy as np
+
+    st.title("Circular Progress Component")
+
+    def calculate_progress():
+        if "slider" in st.session_state:
+            cp.update_value(progress=st.session_state["slider"])
 
-if not _RELEASE:
-    _st_circular_progress_component = components.declare_component(
-        "st_circular_progress",
-        url="http://localhost:3001",
-    )
-else:
-    parent_dir = os.path.dirname(os.path.abspath(__file__))
-    build_dir = os.path.join(parent_dir, "frontend/build")
-    _st_circular_progress_component = components.declare_component(
-        "st_circular_progress", path=build_dir
-    )
-
-
-class CircularProgressBarError(Exception):
-    pass
+    columns = st.columns((1, 2))
 
+    with columns[0]:
+        cp = CircularProgress(
+            value=0,
+            label="Progress Indicator",
+            size="Large",
+            key="circular_progress_total",
+        )
+        cp.st_circular_progress()
+    with columns[1]:
+        st.slider(
+            "Change progress to",
+            min_value=0,
+            max_value=100,
+            on_change=calculate_progress,
+            key="slider",
+        )
 
-class CircularProgress:
-    """Uses a callback function to update the value. Keep label under 50 characters"""
+    data = [
+        ["Feature #126", 55],
+        ["Feature #95", 100],
+        ["Feature #134", 24],
+        ["Feature #77", 98],
+        ["Feature #98", 32],
+    ]
+    project_data = pd.DataFrame(data=data, columns=["Project Name", "Completion"])
+    project_data["color"] = project_data.apply(
+        lambda x: "red"
+        if x["Completion"] < 25
+        else "orange"
+        if x["Completion"] < 75
+        else "green",
+        axis=1,
+    )
 
-    def __init__(
-        self,
-        label: str,
-        value: int = None,
-        size: str = "medium",
-        track_color: str = "lightgray",
-        color: str = "blue",
-        key: str = None,
-    ):
-        self.value = value
-        self.size = size.lower()
-        self.label = label
-        self.track_color = track_color
-        self.color = color
-        self.key = key or label
-
-    def st_circular_progress(self):
-        if f"cp_{self.key}" not in st.session_state:
-            st.session_state[f"cp_{self.key}"] = self.value
-        if self.size not in ["small", "medium", "large"]:
-            raise CircularProgressBarError("Size must be small, medium or large")
-        if len(self.label) > 50:
-            raise CircularProgressBarError("Label can't be longer than 50 characters")
-        if self.value < 0 or self.value > 100:
-            raise CircularProgressBarError("Value must be between 0 and 100")
-        component_value = _st_circular_progress_component(
-            label=self.label,
-            value=st.session_state[f"cp_{self.key}"],
-            size=self.size,
-            color=self.color,
-            track_color=self.track_color,
-            key=self.key,
-        )
-        return component_value
+    widgets = {}
+    dashboard = st.columns(5)
+    for k, v in project_data.iterrows():
+        with dashboard[k]:
+            widgets[k] = CircularProgress(
+                value=v["Completion"],
+                label=v["Project Name"],
+                size="Medium",
+                key=f"dsh_{k}",
+                color=v["color"],
+            ).st_circular_progress()
 
-    def update_value(self, progress):
-        st.session_state[f"cp_{self.key}"] = progress
 
+```
 
-if not _RELEASE:
-    import streamlit as st
+## Sample App 
+[Click Here for a sample app](https://st-circular-progress-demo.streamlit.app)
 
-    columns = st.columns(4)
-    with columns[0]:
-        cp = CircularProgress(
-            value=89,
-            label="Lorem ipsum dolor sit amet, consectetuer adipiscin",
-            size="small",
-            key="1",
-        ).st_circular_progress()
-        cp2 = CircularProgress(
-            value=25,
-            label="Short Text, but can be a very very long text",
-            size="medium",
-            key="2",
-        ).st_circular_progress()
-        cp3 = CircularProgress(
-            value=50,
-            label="Short Text, but can be a very very long text,",
-            size="large",
-            key="3",
-        ).st_circular_progress()
```

