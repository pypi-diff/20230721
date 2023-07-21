# Comparing `tmp/st_track_analysis-0.0.1.tar.gz` & `tmp/st_track_analysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_track_analysis-0.0.1.tar", last modified: Fri Jul 21 11:09:45 2023, max compression
+gzip compressed data, was "st_track_analysis-0.0.2.tar", last modified: Fri Jul 21 18:15:16 2023, max compression
```

## Comparing `st_track_analysis-0.0.1.tar` & `st_track_analysis-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.193173 st_track_analysis-0.0.1/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-04 12:01:44.000000 st_track_analysis-0.0.1/LICENSE
--rw-r--r--   0 elliotglas   (501) staff       (20)       53 2023-07-21 10:04:23.000000 st_track_analysis-0.0.1/MANIFEST.in
--rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 11:09:45.192956 st_track_analysis-0.0.1/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 11:09:45.193231 st_track_analysis-0.0.1/setup.cfg
--rw-r--r--   0 elliotglas   (501) staff       (20)      663 2023-07-21 10:05:13.000000 st_track_analysis-0.0.1/setup.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.186031 st_track_analysis-0.0.1/st_track_analysis/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2645 2023-07-21 11:07:31.000000 st_track_analysis-0.0.1/st_track_analysis/__init__.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.184327 st_track_analysis-0.0.1/st_track_analysis/frontend/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.187702 st_track_analysis-0.0.1/st_track_analysis/frontend/build/
--rw-r--r--   0 elliotglas   (501) staff       (20)      879 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/asset-manifest.json
--rw-r--r--   0 elliotglas   (501) staff       (20)     2186 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/index.html
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.184801 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.188118 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/css/
--rw-r--r--   0 elliotglas   (501) staff       (20)      840 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css
--rw-r--r--   0 elliotglas   (501) staff       (20)     1567 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.192680 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/
--rw-r--r--   0 elliotglas   (501) staff       (20)   982744 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js.LICENSE.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)  4039604 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)    10934 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/main.1d17f984.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)    41286 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/main.1d17f984.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 11:09:10.000000 st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 11:09:45.187237 st_track_analysis-0.0.1/st_track_analysis.egg-info/
--rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 11:09:45.000000 st_track_analysis-0.0.1/st_track_analysis.egg-info/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)      980 2023-07-21 11:09:45.000000 st_track_analysis-0.0.1/st_track_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 11:09:45.000000 st_track_analysis-0.0.1/st_track_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 11:09:45.000000 st_track_analysis-0.0.1/st_track_analysis.egg-info/requires.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       18 2023-07-21 11:09:45.000000 st_track_analysis-0.0.1/st_track_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.170087 st_track_analysis-0.0.2/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-04 12:01:44.000000 st_track_analysis-0.0.2/LICENSE
+-rw-r--r--   0 elliotglas   (501) staff       (20)       53 2023-07-21 10:04:23.000000 st_track_analysis-0.0.2/MANIFEST.in
+-rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 18:15:16.169859 st_track_analysis-0.0.2/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 18:15:16.170152 st_track_analysis-0.0.2/setup.cfg
+-rw-r--r--   0 elliotglas   (501) staff       (20)      663 2023-07-21 18:13:03.000000 st_track_analysis-0.0.2/setup.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.161899 st_track_analysis-0.0.2/st_track_analysis/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2873 2023-07-21 18:12:54.000000 st_track_analysis-0.0.2/st_track_analysis/__init__.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.160533 st_track_analysis-0.0.2/st_track_analysis/frontend/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.163896 st_track_analysis-0.0.2/st_track_analysis/frontend/build/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      879 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/asset-manifest.json
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2186 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/index.html
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.160848 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.164329 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      840 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1567 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.169584 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   982743 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)  4039604 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)    11330 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)    41110 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.163402 st_track_analysis-0.0.2/st_track_analysis.egg-info/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)      980 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/requires.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       18 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/top_level.txt
```

### Comparing `st_track_analysis-0.0.1/LICENSE` & `st_track_analysis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.1/setup.py` & `st_track_analysis-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_track_analysis",
-    version="0.0.1",
+    version="0.0.2",
     author="Elliot Glas",
     author_email="elliot.glas@viscando.com",
     description="A tool to view tracks on an image",
     long_description="A tool to view tracks on an image",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_track_analysis-0.0.1/st_track_analysis/__init__.py` & `st_track_analysis-0.0.2/st_track_analysis/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,60 +18,85 @@
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("st_track_analysis", path=build_dir)
 
 
-def st_track_analysis(tracks, date, im, height, width):
+def st_track_analysis(tracks, date, im, height, width, key=None):
     buffer = BytesIO()
-    plt.imsave(buffer, im, cmap='gray', format='png')
+    plt.imsave(buffer, im, cmap="gray", format="png")
     base64_string = base64.b64encode(buffer.getvalue()).decode()
 
-    mime_type = 'image/png'
-    url_string = f'data:{mime_type};base64,{base64_string}'
-    component_value = _component_func(tracks=tracks, date=date, image=url_string, height=height, width=width, default=0)
+    mime_type = "image/png"
+    url_string = f"data:{mime_type};base64,{base64_string}"
+    component_value = _component_func(
+        tracks=tracks,
+        date=date,
+        image=url_string,
+        height=height,
+        width=width,
+        key=key,
+        default=0,
+    )
     return component_value
 
+
+def process_tracks(tracks):
+    time_strings = tracks["Time"].dt.strftime("%Y-%m-%dT%H:%M:%S.%f").tolist()
+    tracks = list(
+        zip(
+            tracks["ID"].tolist(),
+            tracks["X"].tolist(),
+            tracks["Y"].tolist(),
+            tracks["Type"].tolist(),
+            tracks["Estimated"].tolist(),
+            time_strings,
+        )
+    )
+    tracks = sorted(tracks, key=lambda x: x[5])
+    return tracks
+
+
 # Test code
 if not _RELEASE:
     import streamlit as st
 
     st.set_page_config(layout="wide")
     image = plt.imread("./frontend/src/assets/ground.png")
 
+    if "key" not in st.session_state:
+        st.session_state["key"] = "2023-05-04"
+
     folder_path = "./CSV2"
     csv_files = os.listdir(folder_path)
-    keys = list(map(lambda string: string.split("_")[0] ,csv_files))
-
-    if "key" not in st.session_state:
-      st.session_state["key"] = "2023-05-04"
+    keys = list(map(lambda string: string.split("_")[0], csv_files))
 
     if "track_data" not in st.session_state:
-      track_data = {}
+        print("Unnecessary reload")
+        track_data = {}
 
-      for file_name in csv_files:
-          if file_name.endswith(".csv"):
-              date_str = file_name.split("_")[0]
-              date_key = pd.to_datetime(date_str).date().isoformat()
-              file_path = os.path.join(folder_path, file_name)
-              tracks = pd.read_csv(file_path, sep=";", parse_dates=["Time"])
-              time_strings = tracks["Time"].dt.strftime("%Y-%m-%dT%H:%M:%S.%f").tolist()
-              tracks = list(
-                  zip(
-                      tracks["ID"].tolist(),
-                      tracks["X"].tolist(),
-                      tracks["Y"].tolist(),
-                      tracks["Type"].tolist(),
-                      tracks["Estimated"].tolist(),
-              time_strings
-                  )
-              )
-              tracks = sorted(tracks, key=lambda x: x[5])
-              track_data[date_key] = tracks
-      st.session_state["track_data"] = track_data
-    key = st_track_analysis(tracks=st.session_state.track_data[st.session_state.key], date=st.session_state.key, im=image, height=600, width=540)
-    if not st.session_state.key == key and key in keys:
+        for file_name in csv_files:
+            if file_name.endswith(".csv"):
+                date_str = file_name.split("_")[0]
+                date_key = pd.to_datetime(date_str).date().isoformat()
+                file_path = os.path.join(folder_path, file_name)
+                tracks = pd.read_csv(file_path, sep=";", parse_dates=["Time"])
+                track_data[date_key] = tracks
+        st.session_state["track_data"] = track_data
+    tracks = (
+        process_tracks(st.session_state.track_data[st.session_state.key])
+        if st.session_state.key in keys
+        else []
+    )
+    key = st_track_analysis(
+        tracks=tracks,
+        date=st.session_state.key,
+        im=image,
+        height=600,
+        width=540,
+    )
+    if not st.session_state.key == key and key != 0:
         st.session_state.key = key
         st.experimental_rerun()
     else:
         pass
```

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/index.html` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style><link href="./static/css/main.22919367.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.63817a12.chunk.js"></script><script src="./static/js/main.1d17f984.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style><link href="./static/css/main.22919367.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.2edeab5c.chunk.js"></script><script src="./static/js/main.070b89e3.chunk.js"></script></body></html>
```

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.63817a12.chunk.js.LICENSE.txt */
+/*! For license information please see 2.2edeab5c.chunk.js.LICENSE.txt */
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
         e.exports = n(187)
     }, function(e, t, n) {
         "use strict";
@@ -102,17 +102,17 @@
             return a
         })), t.default = a
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return o
         }));
-        var r = n(137);
+        var r = n(136);
         var a = n(73),
-            i = n(138);
+            i = n(137);
 
         function o(e, t) {
             return Object(r.a)(e) || function(e, t) {
                 var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                 if (null != n) {
                     var r, a, i, o, u = [],
                         c = !0,
@@ -138,15 +138,15 @@
         }
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return o
         }));
         var r = n(83);
-        var a = n(139),
+        var a = n(138),
             i = n(73);
 
         function o(e) {
             return function(e) {
                 if (Array.isArray(e)) return Object(r.a)(e)
             }(e) || Object(a.a)(e) || Object(i.a)(e) || function() {
                 throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
@@ -161,30 +161,30 @@
         }));
         var r = n(10),
             a = n(9),
             i = n(7),
             o = n(1),
             u = n(72),
             c = n(209),
-            s = n(152),
+            s = n(151),
             l = ["variant"];
 
         function f(e) {
             return 0 === e.length
         }
 
         function d(e) {
             var t = e.variant,
                 n = Object(i.a)(e, l),
                 r = t || "";
             return Object.keys(n).sort().forEach((function(t) {
                 r += "color" === t ? f(r) ? e[t] : Object(s.a)(e[t]) : "".concat(f(r) ? t : Object(s.a)(t)).concat(Object(s.a)(e[t].toString()))
             })), r
         }
-        var p = n(141),
+        var p = n(140),
             h = ["name", "slot", "skipVariantsResolver", "skipSx", "overridesResolver"];
 
         function b(e) {
             return "ownerState" !== e && "theme" !== e && "sx" !== e && "as" !== e
         }
         var v = Object(c.a)();
 
@@ -321,15 +321,15 @@
                 themeId: g.a,
                 defaultTheme: y.a,
                 rootShouldForwardProp: O
             });
         t.a = j
     }, function(e, t, n) {
         "use strict";
-        var r = n(142);
+        var r = n(141);
         t.a = function(e) {
             if ("string" !== typeof e) throw new Error(Object(r.a)(7));
             return e.charAt(0).toUpperCase() + e.slice(1)
         }
     }, function(e, t, n) {
         "use strict";
         n.d(t, "c", (function() {
@@ -341,15 +341,15 @@
         })), n.d(t, "b", (function() {
             return d
         })), n.d(t, "d", (function() {
             return p
         }));
         var r, a = n(1),
             i = n(0),
-            o = n(146),
+            o = n(145),
             u = {
                 previousMonth: "Previous month",
                 nextMonth: "Next month",
                 openPreviousView: "open previous view",
                 openNextView: "open next view",
                 calendarViewSwitchingButtonAriaLabel: function(e) {
                     return "year" === e ? "year view is open, switch to calendar view" : "calendar view is open, switch to year view"
@@ -701,15 +701,15 @@
         "use strict";
         n.d(t, "b", (function() {
             return o
         })), n.d(t, "c", (function() {
             return u
         }));
         var r = n(6),
-            a = n(152),
+            a = n(151),
             i = n(35);
 
         function o(e, t) {
             var n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
             if (!t || "string" !== typeof t) return null;
             if (e && e.vars && n) {
                 var r = "vars.".concat(t).split(".").reduce((function(e, t) {
@@ -2249,21 +2249,21 @@
         })), n.d(t, "a", (function() {
             return W
         }));
         var r = n(9),
             a = n(6),
             i = n(7),
             o = n(1),
-            u = n(142),
+            u = n(141),
             c = n(0),
             s = n(8),
             l = n(119),
             f = n(46),
-            d = n(153),
-            p = n(282);
+            d = n(152),
+            p = n(281);
         var h = n(122),
             b = n(2),
             v = ["onChange", "maxRows", "minRows", "style", "value"];
 
         function m(e) {
             return parseInt(e, 10) || 0
         }
@@ -2389,24 +2389,24 @@
                             paddingTop: 0,
                             paddingBottom: 0
                         })
                     })]
                 })
             })),
             w = O,
-            j = n(144),
+            j = n(143),
             k = n(38),
             x = n(62),
             S = n(34),
             T = n(11),
             _ = n(15),
             C = n(12),
             M = n(28),
             D = n(47),
-            I = n(281),
+            I = n(280),
             E = n(84);
         var P = function(e) {
                 var t = e.styles,
                     n = e.themeId,
                     r = e.defaultTheme,
                     a = void 0 === r ? {} : r,
                     i = Object(E.a)(a),
@@ -3260,15 +3260,15 @@
                 name: s,
                 styles: a,
                 next: d
             }
         }
     }, , function(e, t, n) {
         "use strict";
-        var r = n(151),
+        var r = n(150),
             a = Object(r.a)();
         t.a = a
     }, function(e, t, n) {
         "use strict";
         var r = n(0),
             a = r.createContext(void 0);
         t.a = a
@@ -3354,15 +3354,15 @@
             return l
         }));
         var r = n(33),
             a = n(0),
             i = n(44),
             o = n(56),
             u = n(59),
-            c = (n(103), n(136), n(82), n(80), Object(r.f)((function(e, t) {
+            c = (n(103), n(135), n(82), n(80), Object(r.f)((function(e, t) {
                 var n = e.styles,
                     c = Object(u.a)([n], void 0, a.useContext(r.b));
                 if (!r.e) {
                     for (var s, l = c.name, f = c.styles, d = c.next; void 0 !== d;) l += " " + d.name, f += d.styles, d = d.next;
                     var p = !0 === t.compat,
                         h = t.insert("", {
                             name: l,
@@ -3469,15 +3469,15 @@
                 var t = e.cache,
                     n = e.serialized,
                     r = e.isStringTag;
                 return Object(s.c)(t, n, r), Object(f.a)((function() {
                     return Object(s.b)(t, n, r)
                 })), null
             },
-            m = (n(136), function e(t, n) {
+            m = (n(135), function e(t, n) {
                 var i, o, u = t.__emotion_real === t,
                     f = u && t.__emotion_base || t;
                 void 0 !== n && (i = n.label, o = n.target);
                 var d = b(t, n, u),
                     p = d || h(f),
                     m = !p("as");
                 return function() {
@@ -3568,15 +3568,15 @@
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
         })), n.d(t, "b", (function() {
             return o
         }));
-        var r = n(154),
+        var r = n(153),
             a = n(205);
 
         function i(e) {
             return Object(r.a)("MuiPickersToolbar", e)
         }
         var o = Object(a.a)("MuiPickersToolbar", ["root", "content", "penIconButton", "penIconButtonLandscape"])
     }, function(e, t, n) {
@@ -20667,15 +20667,15 @@
             }
         }), Object.defineProperty(t, "StreamlitProvider", {
             enumerable: !0,
             get: function() {
                 return r(a).default
             }
         });
-        var i = n(133);
+        var i = n(132);
         Object.defineProperty(t, "useNullableRenderData", {
             enumerable: !0,
             get: function() {
                 return i.useNullableRenderData
             }
         })
     }, function(e, t, n) {
@@ -20766,15 +20766,15 @@
         var r = n(1),
             a = n(0),
             i = n(8),
             o = n(10),
             u = n(6),
             c = n(7),
             s = n(35),
-            l = n(272),
+            l = n(271),
             f = n(119),
             d = n(11),
             p = n(15),
             h = n(45);
         var b = a.createContext(),
             v = n(109),
             m = n(89);
@@ -21077,15 +21077,15 @@
                         className: Object(i.default)(W.root, s),
                         as: m,
                         ref: t
                     }, z))
                 })
             })),
             C = n(110),
-            M = n(277),
+            M = n(276),
             D = n(76),
             I = Object(d.a)("div", {
                 name: "MuiPickersToolbar",
                 slot: "Root",
                 overridesResolver: function(e, t) {
                     return t.root
                 }
@@ -21976,15 +21976,15 @@
         }
     }, function(e, t, n) {
         "use strict";
         var r = n(7),
             a = n(1),
             i = n(0),
             o = n(8),
-            u = n(272),
+            u = n(271),
             c = n(119),
             s = n(11),
             l = n(15),
             f = n(12),
             d = n(109),
             p = n(89);
 
@@ -22388,15 +22388,15 @@
                 u = Object(r.a)(o, 2),
                 c = u[0],
                 s = u[1];
             return [i ? t : c, a.useCallback((function(e) {
                 i || s(e)
             }), [])]
         }
-    }, , , , , , , , , function(e, t, n) {
+    }, , , , , , , , function(e, t, n) {
         "use strict";
         var r = Object.getOwnPropertySymbols,
             a = Object.prototype.hasOwnProperty,
             i = Object.prototype.propertyIsEnumerable;
         e.exports = function() {
             try {
                 if (!Object.assign) return !1;
@@ -22586,15 +22586,15 @@
         var r = n(197),
             a = r.default,
             i = r.DraggableCore;
         e.exports = a, e.exports.default = a, e.exports.DraggableCore = i
     }, function(e, t, n) {
         "use strict";
         var r = n(6),
-            a = n(152),
+            a = n(151),
             i = n(52),
             o = n(21),
             u = n(35),
             c = n(77);
         var s = function() {
             function e(e, t, n, i) {
                 var c, s = (c = {}, Object(r.a)(c, e, t), Object(r.a)(c, "theme", n), c),
@@ -23030,19 +23030,19 @@
             }
         }()
     }, function(e, t, n) {
         "use strict";
         var r = n(6),
             a = n(1),
             i = n(7),
-            o = n(142),
-            u = n(270),
+            o = n(141),
+            u = n(269),
             c = n(209),
             s = n(77),
-            l = n(141);
+            l = n(140);
 
         function f(e, t) {
             var n;
             return Object(a.a)({
                 toolbar: (n = {
                     minHeight: 56
                 }, Object(r.a)(n, e.up("xs"), {
@@ -23607,17 +23607,17 @@
             };
 
         function o(e, t) {
             var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "Mui",
                 r = i[t];
             return r ? "".concat(n, "-").concat(r) : "".concat(a.generate(e), "-").concat(t)
         }
-    }, , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , function(e, t, n) {
+    }, , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , function(e, t, n) {
         "use strict";
-        var r = n(132),
+        var r = n(131),
             a = "function" === typeof Symbol && Symbol.for,
             i = a ? Symbol.for("react.element") : 60103,
             o = a ? Symbol.for("react.portal") : 60106,
             u = a ? Symbol.for("react.fragment") : 60107,
             c = a ? Symbol.for("react.strict_mode") : 60108,
             s = a ? Symbol.for("react.profiler") : 60114,
             l = a ? Symbol.for("react.provider") : 60109,
@@ -23913,15 +23913,15 @@
             return V().useRef(e)
         }, t.useState = function(e) {
             return V().useState(e)
         }, t.version = "16.14.0"
     }, function(e, t, n) {
         "use strict";
         var r = n(0),
-            a = n(132),
+            a = n(131),
             i = n(189);
 
         function o(e) {
             for (var t = "https://reactjs.org/docs/error-decoder.html?invariant=" + e, n = 1; n < arguments.length; n++) t += "&args[]=" + encodeURIComponent(arguments[n]);
             return "Minified React error #" + e + "; visit " + t + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
         }
         if (!r) throw Error(o(227));
@@ -29460,15 +29460,15 @@
             };
         Object.defineProperty(t, "__esModule", {
             value: !0
         }), t.useRenderData = void 0;
         var c = n(2),
             s = o(n(0)),
             l = n(95),
-            f = n(133),
+            f = n(132),
             d = u(n(195)),
             p = s.default.createContext(void 0);
         t.useRenderData = function() {
             var e = (0, s.useContext)(p);
             if (null == e) throw new Error("useRenderData() must be used inside <StreamlitProvider />");
             return e
         };
@@ -29691,18 +29691,18 @@
                     } a.default = e, n && n.set(e, a);
                 return a
             }(n(0)),
             i = h(n(3)),
             o = h(n(46)),
             u = h(n(8)),
             c = n(115),
-            s = n(134),
+            s = n(133),
             l = n(94),
             f = h(n(201)),
-            d = h(n(135)),
+            d = h(n(134)),
             p = ["axis", "bounds", "children", "defaultPosition", "defaultClassName", "defaultClassNameDragging", "defaultClassNameDragged", "position", "positionOffset", "scale"];
 
         function h(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         }
@@ -30143,17 +30143,17 @@
                         u && (u.get || u.set) ? Object.defineProperty(a, o, u) : a[o] = e[o]
                     } a.default = e, n && n.set(e, a);
                 return a
             }(n(0)),
             i = f(n(3)),
             o = f(n(46)),
             u = n(115),
-            c = n(134),
+            c = n(133),
             s = n(94),
-            l = f(n(135));
+            l = f(n(134));
 
         function f(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         }
 
@@ -30531,15 +30531,15 @@
             a = "undefined" !== typeof window ? r.useLayoutEffect : r.useEffect;
         t.a = a
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return a
         }));
-        var r = n(154);
+        var r = n(153);
 
         function a(e, t) {
             var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "Mui",
                 a = {};
             return t.forEach((function(t) {
                 a[t] = Object(r.a)(e, t, n)
             })), a
@@ -30644,15 +30644,15 @@
         function S(e, t) {
             return t || (t = e.slice(0)), Object.freeze(Object.defineProperties(e, {
                 raw: {
                     value: Object.freeze(t)
                 }
             }))
         }
-        var T = n(317),
+        var T = n(316),
             _ = n(70),
             C = n(2);
         var M = function(e) {
                 var t = e.className,
                     n = e.classes,
                     a = e.pulsate,
                     i = void 0 !== a && a,
@@ -31083,15 +31083,15 @@
                     return Object(r.a)({}, e, Object(o.a)({}, t.key, t.val))
                 }), {})
             };
         var s = {
                 borderRadius: 4
             },
             l = n(16);
-        var f = n(141),
+        var f = n(140),
             d = n(77),
             p = ["breakpoints", "palette", "spacing", "shape"];
         t.a = function() {
             for (var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {}, t = e.breakpoints, n = void 0 === t ? {} : t, o = e.palette, h = void 0 === o ? {} : o, b = e.spacing, v = e.shape, m = void 0 === v ? {} : v, y = Object(a.a)(e, p), g = function(e) {
                     var t = e.values,
                         n = void 0 === t ? {
                             xs: 0,
@@ -31207,15 +31207,15 @@
             };
 
         function o(e, t) {
             var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "Mui",
                 r = i[t];
             return r ? "".concat(n, "-").concat(r) : "".concat(a.generate(e), "-").concat(t)
         }
-    }, , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , function(e, t, n) {
+    }, , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , , function(e, t, n) {
         "use strict";
         var r = n(6),
             a = n(7),
             i = n(1),
             o = n(0),
             u = n(8),
             c = n(119),
@@ -31542,15 +31542,15 @@
             a = n(1),
             i = n(0),
             o = n(8),
             u = n(119),
             c = n(88),
             s = n(11),
             l = n(15),
-            f = n(145),
+            f = n(144),
             d = n(2),
             p = ["absolute", "children", "className", "component", "flexItem", "light", "orientation", "role", "textAlign", "variant"],
             h = Object(s.a)("div", {
                 name: "MuiDivider",
                 slot: "Root",
                 overridesResolver: function(e, t) {
                     var n = e.ownerState;
@@ -31727,21 +31727,21 @@
         }));
         var r = n(9),
             a = n(5),
             i = n(4),
             o = n(1),
             u = n(29),
             c = n.n(u),
-            s = n(147),
+            s = n(146),
             l = n.n(s),
-            f = n(148),
+            f = n(147),
             d = n.n(f),
-            p = n(149),
+            p = n(148),
             h = n.n(p),
-            b = n(150),
+            b = n(149),
             v = n.n(b),
             m = n(97);
         c.a.extend(d.a), c.a.extend(h.a), c.a.extend(v.a);
         var y = Object(m.a)(["Your locale has not been found.", "Either the locale key is not a supported one. Locales supported by dayjs are available here: https://github.com/iamkun/dayjs/tree/dev/src/locale", "Or you forget to import the locale with `require('dayjs/locale/{localeUsed}')`", "fallback on English locale"]),
             g = {
                 YY: "year",
                 YYYY: {
@@ -32395,15 +32395,15 @@
             })), a
         }
     }, function(e, t, n) {
         "use strict";
         var r = n(9),
             a = n(0),
             i = n(46),
-            o = n(153),
+            o = n(152),
             u = n(122),
             c = n(107),
             s = n(2);
         var l = a.forwardRef((function(e, t) {
             var n = e.children,
                 l = e.container,
                 f = e.disablePortal,
@@ -32437,15 +32437,15 @@
                 children: b ? i.createPortal(n, b) : b
             })
         }));
         t.a = l
     }, function(e, t, n) {
         "use strict";
         var r = n(0),
-            a = n(153),
+            a = n(152),
             i = n(121),
             o = n(2),
             u = ["input", "select", "textarea", "a[href]", "button", "[tabindex]", "audio[controls]", "video[controls]", '[contenteditable]:not([contenteditable="false"])'].join(",");
 
         function c(e) {
             var t = [],
                 n = [];
@@ -32707,15 +32707,15 @@
         n.d(t, "a", (function() {
             return Tt
         }));
         var r = n(6),
             a = n(1),
             i = n(7),
             o = n(0),
-            u = n(299),
+            u = n(298),
             c = n(8),
             s = n(119),
             l = n(12),
             f = n(110),
             d = n(62),
             p = n(34),
             h = n(11),
@@ -32810,21 +32810,21 @@
                         }) : Object(w.jsx)(f.a, {
                             color: "text.secondary",
                             children: r
                         })
                     }))
                 })
             })),
-            S = n(313),
-            T = n(319),
-            _ = n(280),
+            S = n(312),
+            T = n(318),
+            _ = n(279),
             C = n(9),
-            M = n(287),
-            D = n(304),
-            I = n(153),
+            M = n(286),
+            D = n(303),
+            I = n(152),
             E = n(122),
             P = n(121);
 
         function A(e) {
             if (null == e) return window;
             if ("[object Window]" !== e.toString()) {
                 var t = e.ownerDocument;
@@ -33927,17 +33927,17 @@
                         }, t.attributes.popper = Object.assign({}, t.attributes.popper, {
                             "data-popper-reference-hidden": l,
                             "data-popper-escaped": f
                         })
                     }
                 }]
             }),
-            $e = n(285),
+            $e = n(284),
             Ke = n(210),
-            qe = n(284);
+            qe = n(283);
 
         function Ge(e) {
             return Object(Ke.a)("MuiPopper", e)
         }
         Object(qe.a)("MuiPopper", ["root"]);
         var Xe = n(99),
             Qe = ["anchorEl", "children", "direction", "disablePortal", "modifiers", "open", "placement", "popperOptions", "popperRef", "slotProps", "slots", "TransitionProps", "ownerState"],
@@ -34183,22 +34183,22 @@
                         root: S
                     },
                     slotProps: null != k ? k : l
                 }, T, {
                     ref: t
                 }))
             })),
-            ct = n(286),
-            st = n(277),
+            ct = n(285),
+            st = n(276),
             lt = n(67);
 
         function ft(e) {
             return e && e.ownerDocument || document
         }
-        var dt = n(154),
+        var dt = n(153),
             pt = n(205);
 
         function ht(e) {
             return Object(dt.a)("MuiPickersPopper", e)
         }
         Object(pt.a)("MuiPickersPopper", ["root", "paper"]);
         var bt = n(32),
@@ -34386,17 +34386,17 @@
                             }))
                         }))
                     }))
                 }
             }))
         }
         var gt = n(13),
-            Ot = n(298),
-            wt = n(146),
-            jt = n(292),
+            Ot = n(297),
+            wt = n(145),
+            jt = n(291),
             kt = ["props", "getOpenDialogAriaText"],
             xt = ["ownerState"],
             St = ["ownerState"],
             Tt = function(e) {
                 var t, n, c, s, l, f = e.props,
                     d = e.getOpenDialogAriaText,
                     p = Object(i.a)(e, kt),
@@ -34530,28 +34530,28 @@
         n.d(t, "a", (function() {
             return zt
         }));
         var r = n(1),
             a = n(7),
             i = n(0),
             o = n.n(i),
-            u = n(276),
+            u = n(275),
             c = n(15),
             s = n(3),
             l = n.n(s),
-            f = n(143),
+            f = n(142),
             d = n(24),
             p = n(13),
             h = n(41),
             b = n(17),
             v = n(110),
             m = n(11),
-            y = n(277),
+            y = n(276),
             g = n(102),
-            O = n(154),
+            O = n(153),
             w = n(205);
 
         function j(e) {
             return Object(O.a)("MuiDatePickerToolbar", e)
         }
         Object(w.a)("MuiDatePickerToolbar", ["root", "title"]);
         var k = n(2),
@@ -34685,19 +34685,19 @@
                         return "minDate";
                     case Boolean(d && r.utils.isAfterDay(n, d)):
                         return "maxDate";
                     default:
                         return null
                 }
             },
-            I = n(288),
+            I = n(287),
             E = n(57),
-            P = n(300),
-            A = n(299),
-            R = n(307),
+            P = n(299),
+            A = n(298),
+            R = n(306),
             L = n(100),
             N = function(e) {
                 var t = e.props,
                     n = e.inputRef,
                     a = function(e) {
                         var t, n, a, i = Object(p.e)(),
                             o = Object(p.a)();
@@ -34770,15 +34770,15 @@
                         onKeyDown: S,
                         ref: j
                     })
                 }))
             })),
             U = n(43),
             W = n(8),
-            H = n(280),
+            H = n(279),
             Y = n(67),
             $ = n(9),
             K = function(e) {
                 var t = e.shouldDisableDate,
                     n = e.shouldDisableMonth,
                     r = e.shouldDisableYear,
                     a = e.minDate,
@@ -34906,16 +34906,16 @@
                     changeMonth: _,
                     changeFocusedDay: D,
                     isDateDisabled: C,
                     onMonthSwitchingAnimationEnd: M,
                     handleChangeMonth: T
                 }
             },
-            X = n(279),
-            Q = n(317),
+            X = n(278),
+            Q = n(316),
             Z = function(e) {
                 return Object(O.a)("MuiPickersFadeTransitionGroup", e)
             },
             J = (Object(w.a)("MuiPickersFadeTransitionGroup", ["root"]), function(e) {
                 var t = e.classes;
                 return Object(y.a)({
                     root: ["root"]
@@ -34958,15 +34958,15 @@
                 }, i)
             })
         }
         var re = n(45),
             ae = n(123),
             ie = n(6),
             oe = n(208),
-            ue = n(319),
+            ue = n(318),
             ce = n(206),
             se = n(88),
             le = n(31);
 
         function fe(e) {
             return Object(O.a)("MuiPickersDay", e)
         }
@@ -36383,16 +36383,16 @@
                             yearsPerRow: D,
                             children: B.format(e, "year")
                         }, B.format(e, "year"))
                     }))
                 }))
             })),
             bt = n(51),
-            vt = n(313),
-            mt = n(318),
+            vt = n(312),
+            mt = n(317),
             yt = n(58),
             gt = function(e) {
                 return Object(O.a)("MuiPickersCalendarHeader", e)
             },
             Ot = Object(w.a)("MuiPickersCalendarHeader", ["root", "labelContainer", "label", "switchViewButton", "switchViewIcon"]),
             wt = ["ownerState"],
             jt = Object(m.a)("div", {
@@ -36573,15 +36573,15 @@
                         },
                         isNextDisabled: R,
                         nextLabel: i.nextMonth
                     })
                 })]
             })
         }
-        var Ct = n(278),
+        var Ct = n(277),
             Mt = "undefined" !== typeof navigator && /(android)/i.test(navigator.userAgent),
             Dt = function(e) {
                 return Object(O.a)("MuiDateCalendar", e)
             },
             It = (Object(w.a)("MuiDateCalendar", ["root", "viewTransitionContainer"]), ["autoFocus", "onViewChange", "value", "defaultValue", "referenceDate", "disableFuture", "disablePast", "defaultCalendarMonth", "onChange", "onYearChange", "onMonthChange", "reduceAnimations", "shouldDisableDate", "shouldDisableMonth", "shouldDisableYear", "view", "views", "openTo", "className", "disabled", "readOnly", "minDate", "maxDate", "disableHighlightToday", "focusedView", "onFocusedViewChange", "showDaysOutsideCurrentMonth", "fixedWeekNumber", "dayOfWeekFormatter", "components", "componentsProps", "slots", "slotProps", "loading", "renderLoading", "displayWeekNumber", "yearsPerRow", "monthsPerRow", "timezone"]);
         var Et = Object(m.a)(Ct.a, {
                 name: "MuiDateCalendar",
@@ -37042,15 +37042,15 @@
                 day: l.a.func,
                 month: l.a.func,
                 year: l.a.func
             }),
             views: l.a.arrayOf(l.a.oneOf(["day", "month", "year"]).isRequired),
             yearsPerRow: l.a.oneOf([3, 4])
         };
-        var Nt = n(294),
+        var Nt = n(293),
             Ft = i.forwardRef((function(e, t) {
                 var n, a = Object(p.b)(),
                     i = Object(p.e)(),
                     o = M(e, "MuiMobileDatePicker"),
                     u = Object(r.a)({
                         day: Rt,
                         month: Rt,
@@ -37168,24 +37168,24 @@
         "use strict";
         n.d(t, "a", (function() {
             return Mt
         }));
         var r = n(1),
             a = n(7),
             i = n(0),
-            o = n(276),
+            o = n(275),
             u = n(15),
             c = n(10),
             s = n(3),
             l = n.n(s),
-            f = n(143),
+            f = n(142),
             d = n(24),
-            p = n(300),
-            h = n(299),
-            b = n(307),
+            p = n(299),
+            h = n(298),
+            b = n(306),
             v = n(27),
             m = function(e) {
                 var t = e.adapter,
                     n = e.value,
                     r = e.props;
                 if (null === n) return null;
                 var a = r.minTime,
@@ -37306,18 +37306,18 @@
                         ref: M
                     })
                 }))
             })),
             T = n(6),
             _ = n(11),
             C = n(45),
-            M = n(277),
+            M = n(276),
             D = n(8),
             I = n(110),
-            E = n(154),
+            E = n(153),
             P = n(205);
 
         function A(e) {
             return Object(E.a)("MuiPickersToolbarText", e)
         }
         var R = Object(P.a)("MuiPickersToolbarText", ["root", "selected"]),
             L = ["className", "selected", "value"],
@@ -37355,15 +37355,15 @@
                     ref: t,
                     className: Object(D.default)(i, s.root),
                     component: "span"
                 }, c, {
                     children: o
                 }))
             })),
-            B = n(302),
+            B = n(301),
             V = n(76),
             z = ["align", "className", "selected", "typographyClassName", "value", "variant", "width"],
             U = Object(_.a)(B.a, {
                 name: "MuiPickersToolbarButton",
                 slot: "Root",
                 overridesResolver: function(e, t) {
                     return t.root
@@ -37637,26 +37637,26 @@
                         ampm: d,
                         ampmInClock: f.ampmInClock
                     }, null == b ? void 0 : b.toolbar)
                 })
             })
         }
         var ie = n(57),
-            oe = n(288),
+            oe = n(287),
             ue = n(43),
-            ce = n(280),
-            se = n(318),
+            ce = n(279),
+            se = n(317),
             le = n(51),
-            fe = n(278);
+            fe = n(277);
 
         function de(e) {
             return Object(E.a)("MuiTimeClock", e)
         }
         Object(P.a)("MuiTimeClock", ["root", "arrowSwitcher"]);
-        var pe = n(313),
+        var pe = n(312),
             he = n(206),
             be = 220,
             ve = 36,
             me = {
                 x: be / 2,
                 y: be / 2
             },
@@ -38465,17 +38465,17 @@
                         nextLabel: ie.openNextView,
                         ownerState: je
                     })]
                 }))
             })),
             Je = n(88),
             et = n(67),
-            tt = n(306),
-            nt = n(305),
-            rt = n(319);
+            tt = n(305),
+            nt = n(304),
+            rt = n(318);
 
         function at(e) {
             return Object(E.a)("MuiDigitalClock", e)
         }
         Object(P.a)("MuiDigitalClock", ["root", "list", "item"]);
         var it = n(31),
             ot = ["ampm", "timeStep", "autoFocus", "components", "componentsProps", "slots", "slotProps", "value", "defaultValue", "referenceDate", "disableIgnoringDatePartForTimeValidation", "maxTime", "minTime", "disableFuture", "disablePast", "minutesStep", "shouldDisableClock", "shouldDisableTime", "onChange", "view", "openTo", "onViewChange", "focusedView", "onFocusedViewChange", "className", "disabled", "readOnly", "views", "skipDisabled", "timezone"],
@@ -39436,15 +39436,15 @@
                 hours: l.a.func,
                 meridiem: l.a.func,
                 minutes: l.a.func,
                 seconds: l.a.func
             }),
             views: l.a.arrayOf(l.a.oneOf(["hours", "minutes", "seconds"]).isRequired)
         };
-        var Tt = n(294),
+        var Tt = n(293),
             _t = i.forwardRef((function(e, t) {
                 var n, a, i = Object(y.b)(),
                     o = Object(y.e)(),
                     u = ae(e, "MuiMobileTimePicker"),
                     c = Object(r.a)({
                         hours: jt,
                         minutes: jt,
@@ -39552,24 +39552,24 @@
             }))
     }, function(e, t, n) {
         "use strict";
         var r = n(1),
             a = n(7),
             i = n(0),
             o = n(8),
-            u = n(270),
+            u = n(269),
             c = n(9),
             s = n(6),
-            l = n(142),
+            l = n(141),
             f = (n(116), n(119)),
             d = n(65),
             p = n(12),
-            h = n(305),
-            b = n(299),
-            v = n(144),
+            h = n(304),
+            b = n(298),
+            v = n(143),
             m = n(11),
             y = n(15);
         var g = function(e) {
                 var t, n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 166;
 
                 function r() {
                     for (var r = this, a = arguments.length, i = new Array(a), o = 0; o < a; o++) i[o] = arguments[o];
@@ -39582,17 +39582,17 @@
                 }, r
             },
             O = n(207);
         var w = function(e) {
                 return Object(O.a)(e).defaultView || window
             },
             j = n(28),
-            k = n(287),
-            x = n(296),
-            S = n(304),
+            k = n(286),
+            x = n(295),
+            S = n(303),
             T = n(109),
             _ = n(89);
 
         function C(e) {
             return Object(_.a)("MuiPopover", e)
         }
         Object(T.a)("MuiPopover", ["root", "paper"]);
@@ -40427,17 +40427,17 @@
             })),
             ve = n(38),
             me = n(34),
             ye = n(36),
             ge = Object(ye.a)(Object(M.jsx)("path", {
                 d: "M7 10l5 5 5-5z"
             }), "ArrowDropDown"),
-            Oe = n(314),
-            we = n(315),
-            je = n(303),
+            Oe = n(313),
+            we = n(314),
+            je = n(302),
             ke = ["autoWidth", "children", "classes", "className", "defaultOpen", "displayEmpty", "IconComponent", "id", "input", "inputProps", "label", "labelId", "MenuProps", "multiple", "native", "onClose", "onOpen", "open", "renderValue", "SelectDisplayProps", "variant"],
             xe = {
                 name: "MuiSelect",
                 overridesResolver: function(e, t) {
                     return t.root
                 },
                 shouldForwardProp: function(e) {
@@ -40559,26 +40559,26 @@
         var r = n(6),
             a = n(0),
             i = n(3),
             o = n.n(i),
             u = n(8),
             c = n(11),
             s = n(15),
-            l = n(277),
-            f = n(154),
+            l = n(276),
+            f = n(153),
             d = n(205);
 
         function p(e) {
             return Object(f.a)("MuiPickersLayout", e)
         }
         var h = Object(d.a)("MuiPickersLayout", ["root", "landscape", "contentWrapper", "toolbar", "actionBar", "shortcuts"]),
             b = n(1),
-            v = n(299),
+            v = n(298),
             m = n(7),
-            y = n(302),
+            y = n(301),
             g = n(119),
             O = n(109),
             w = n(89);
 
         function j(e) {
             return Object(w.a)("MuiDialogActions", e)
         }
@@ -40670,16 +40670,16 @@
                 }
             }));
             return Object(k.jsx)(T, Object(b.a)({}, o, {
                 children: c
             }))
         }
         var D = n(10),
-            I = n(308),
-            E = n(144),
+            I = n(307),
+            E = n(143),
             P = n(88),
             A = n(208),
             R = n(79),
             L = n(47),
             N = n(28),
             F = n(40);
 
@@ -41463,16 +41463,16 @@
         "use strict";
         var r = n(6),
             a = n(7),
             i = n(1),
             o = n(0),
             u = n(8),
             c = n(119),
-            s = n(299),
-            l = n(144),
+            s = n(298),
+            l = n(143),
             f = n(10),
             d = n(9),
             p = n(121);
         var h, b = !0,
             v = !1,
             m = {
                 text: !0,
@@ -41529,17 +41529,17 @@
                     return !!t.current && (v = !0, window.clearTimeout(h), h = window.setTimeout((function() {
                         v = !1
                     }), 100), t.current = !1, !0)
                 },
                 ref: e
             }
         }
-        var k = n(153),
+        var k = n(152),
             x = n(122),
-            S = n(273),
+            S = n(272),
             T = {
                 border: 0,
                 clip: "rect(0 0 0 0)",
                 height: "1px",
                 margin: -1,
                 overflow: "hidden",
                 padding: 0,
@@ -42623,17 +42623,17 @@
         "use strict";
         n.d(t, "a", (function() {
             return G
         }));
         var r = n(1),
             a = n(7),
             i = n(0),
-            o = n(299),
-            u = n(319),
-            c = n(280),
+            o = n(298),
+            u = n(318),
+            c = n(279),
             s = n(6),
             l = n(8),
             f = n(119),
             d = n(11),
             p = n(15),
             h = n(109),
             b = n(89);
@@ -42689,26 +42689,26 @@
                     }(s);
                 return Object(y.jsx)(O, Object(r.a)({
                     className: Object(l.default)(d.root, i),
                     ownerState: s,
                     ref: t
                 }, c))
             })),
-            j = n(279),
-            k = n(283),
+            j = n(278),
+            k = n(282),
             x = n(12),
-            S = n(296),
-            T = n(304);
+            S = n(295),
+            T = n(303);
 
         function _(e) {
             return Object(b.a)("MuiDialog", e)
         }
         var C = Object(h.a)("MuiDialog", ["root", "scrollPaper", "scrollBody", "container", "paper", "paperScrollPaper", "paperScrollBody", "paperWidthFalse", "paperWidthXs", "paperWidthSm", "paperWidthMd", "paperWidthLg", "paperWidthXl", "paperFullWidth", "paperFullScreen"]);
         var M, D = i.createContext({}),
-            I = n(316),
+            I = n(315),
             E = n(45),
             P = ["aria-describedby", "aria-labelledby", "BackdropComponent", "BackdropProps", "children", "className", "disableEscapeKeyDown", "fullScreen", "fullWidth", "maxWidth", "onBackdropClick", "onClose", "open", "PaperComponent", "PaperProps", "scroll", "TransitionComponent", "transitionDuration", "TransitionProps"],
             A = Object(d.a)(I.a, {
                 name: "MuiDialog",
                 slot: "Backdrop",
                 overrides: function(e, t) {
                     return t.backdrop
@@ -42956,19 +42956,19 @@
                 PaperComponent: null == u ? void 0 : u.mobilePaper,
                 PaperProps: null == c ? void 0 : c.mobilePaper,
                 children: Object(y.jsx)(z, {
                     children: a
                 })
             }))
         }
-        var W = n(298),
+        var W = n(297),
             H = n(32),
             Y = n(13),
-            $ = n(146),
-            K = n(292),
+            $ = n(145),
+            K = n(291),
             q = ["props", "getOpenDialogAriaText"],
             G = function(e) {
                 var t, n, s, l = e.props,
                     f = e.getOpenDialogAriaText,
                     d = Object(a.a)(e, q),
                     p = l.slots,
                     h = l.slotProps,
@@ -43311,40 +43311,40 @@
     }, function(e, t, n) {
         "use strict";
         var r = n(9),
             a = n(7),
             i = n(1),
             o = n(0),
             u = n(8),
-            c = n(284),
+            c = n(283),
             s = n(210);
 
         function l(e) {
             return Object(s.a)("MuiModal", e)
         }
         Object(c.a)("MuiModal", ["root", "hidden", "backdrop"]);
-        var f = n(153),
+        var f = n(152),
             d = n(121),
-            p = n(273);
+            p = n(272);
 
         function h() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
             return t.reduce((function(e, t) {
                 return null == t ? e : function() {
                     for (var n = arguments.length, r = new Array(n), a = 0; a < n; a++) r[a] = arguments[a];
                     e.apply(this, r), t.apply(this, r)
                 }
             }), (function() {}))
         }
         var b = n(119),
-            v = n(285),
+            v = n(284),
             m = n(4),
             y = n(5),
             g = n(10),
-            O = n(282);
+            O = n(281);
 
         function w(e, t) {
             t ? e.setAttribute("aria-hidden", "true") : e.removeAttribute("aria-hidden")
         }
 
         function j(e) {
             return parseInt(Object(O.a)(e).getComputedStyle(e).paddingRight, 10) || 0
@@ -43482,16 +43482,16 @@
                 }, {
                     key: "isTopModal",
                     value: function(e) {
                         return this.modals.length > 0 && this.modals[this.modals.length - 1] === e
                     }
                 }]), e
             }(),
-            _ = n(286),
-            C = n(299),
+            _ = n(285),
+            C = n(298),
             M = n(99),
             D = n(2),
             I = ["children", "closeAfterTransition", "container", "disableAutoFocus", "disableEnforceFocus", "disableEscapeKeyDown", "disablePortal", "disableRestoreFocus", "disableScrollLock", "hideBackdrop", "keepMounted", "manager", "onBackdropClick", "onClose", "onKeyDown", "open", "onTransitionEnter", "onTransitionExited", "slotProps", "slots"];
         var E = new T,
             P = o.forwardRef((function(e, t) {
                 var n, u, c = e.children,
                     s = e.closeAfterTransition,
@@ -43637,19 +43637,19 @@
                             isEnabled: be,
                             open: K,
                             children: o.cloneElement(c, Oe)
                         })]
                     }))
                 }) : null
             })),
-            A = n(143),
-            R = n(144),
+            A = n(142),
+            R = n(143),
             L = n(11),
             N = n(15),
-            F = n(316),
+            F = n(315),
             B = ["BackdropComponent", "BackdropProps", "classes", "className", "closeAfterTransition", "children", "container", "component", "components", "componentsProps", "disableAutoFocus", "disableEnforceFocus", "disableEscapeKeyDown", "disablePortal", "disableRestoreFocus", "disableScrollLock", "hideBackdrop", "keepMounted", "onBackdropClick", "onClose", "open", "slotProps", "slots", "theme"],
             V = Object(L.a)("div", {
                 name: "MuiModal",
                 slot: "Root",
                 overridesResolver: function(e, t) {
                     var n = e.ownerState;
                     return [t.root, !n.open && n.exited && t.hidden]
@@ -44293,16 +44293,16 @@
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return d
         }));
         var r = n(1),
             a = n(7),
-            i = n(153),
-            o = n(144);
+            i = n(152),
+            o = n(143);
         var u = n(8);
 
         function c(e) {
             if (void 0 === e) return {};
             var t = {};
             return Object.keys(e).filter((function(t) {
                 return !(t.match(/^on[A-Z]/) && "function" === typeof e[t])
@@ -44343,15 +44343,15 @@
                 m = Object(r.a)({}, null == b ? void 0 : b.style, null == n ? void 0 : n.style, null == i ? void 0 : i.style, null == a ? void 0 : a.style),
                 y = Object(r.a)({}, b, n, h, p);
             return v.length > 0 && (y.className = v), Object.keys(m).length > 0 && (y.style = m), {
                 props: y,
                 internalRef: b.ref
             }
         }
-        var l = n(143),
+        var l = n(142),
             f = ["elementType", "externalSlotProps", "ownerState", "skipResolvingSlotProps"];
 
         function d(e) {
             var t, n = e.elementType,
                 u = e.externalSlotProps,
                 c = e.ownerState,
                 d = e.skipResolvingSlotProps,
@@ -44376,22 +44376,22 @@
     }, function(e, t, n) {
         "use strict";
         var r = n(1),
             a = n(7),
             i = n(0),
             o = n(8),
             u = n(119),
-            c = n(283),
+            c = n(282),
             s = n(11),
             l = n(15),
-            f = n(314),
-            d = n(315),
-            p = n(303),
-            h = n(301),
-            b = n(310),
+            f = n(313),
+            d = n(314),
+            p = n(302),
+            h = n(300),
+            b = n(309),
             v = n(6),
             m = n(38),
             y = n(34),
             g = n(12),
             O = n(109),
             w = n(89);
 
@@ -44479,15 +44479,15 @@
                 }, d, {
                     children: " " === i ? k || (k = Object(S.jsx)("span", {
                         className: "notranslate",
                         children: "\u200b"
                     })) : i
                 }))
             })),
-            M = n(291);
+            M = n(290);
 
         function D(e) {
             return Object(w.a)("MuiTextField", e)
         }
         Object(O.a)("MuiTextField", ["root"]);
         var I = ["autoComplete", "autoFocus", "children", "className", "color", "defaultValue", "disabled", "error", "FormHelperTextProps", "fullWidth", "helperText", "id", "InputLabelProps", "inputProps", "InputProps", "inputRef", "label", "maxRows", "minRows", "multiline", "name", "onBlur", "onChange", "onClick", "onFocus", "placeholder", "required", "rows", "select", "SelectProps", "type", "value", "variant"],
             E = {
@@ -45501,15 +45501,15 @@
         t.a = y
     }, function(e, t, n) {
         "use strict";
         var r = n(1),
             a = n(7),
             i = n(0),
             o = (n(116), n(65)),
-            u = n(308);
+            u = n(307);
         var c = function(e) {
                 var t = e.documentElement.clientWidth;
                 return Math.abs(window.innerWidth - t)
             },
             s = n(28),
             l = n(47),
             f = n(2),
@@ -45629,15 +45629,15 @@
             s = n(88),
             l = n(11),
             f = n(15),
             d = n(40),
             p = n(208),
             h = n(47),
             b = n(28),
-            v = n(145),
+            v = n(144),
             m = n(109),
             y = n(89);
         var g = Object(m.a)("MuiListItemIcon", ["root", "alignItemsFlexStart"]),
             O = n(106);
 
         function w(e) {
             return Object(y.a)("MuiMenuItem", e)
@@ -45791,15 +45791,15 @@
             return j
         }));
         var r = n(1),
             a = n(7),
             i = n(0),
             o = n(206),
             u = n(67),
-            c = n(319),
+            c = n(318),
             s = n(45),
             l = n(101),
             f = n(13),
             d = n(26),
             p = n(10),
             h = n(9),
             b = n(123),
@@ -47134,15 +47134,15 @@
         "use strict";
         var r = n(6),
             a = n(10),
             i = n(7),
             o = n(1),
             u = n(0),
             c = n(119),
-            s = n(270),
+            s = n(269),
             l = n(42),
             f = n(11),
             d = n(15),
             p = n(109),
             h = n(89),
             b = n(87);
 
@@ -47278,15 +47278,15 @@
     }, function(e, t, n) {
         "use strict";
         var r = n(6),
             a = n(10),
             i = n(7),
             o = n(1),
             u = n(0),
-            c = n(270),
+            c = n(269),
             s = n(119),
             l = n(42),
             f = n(11),
             d = n(15),
             p = n(109),
             h = n(89),
             b = n(87);
@@ -47503,15 +47503,15 @@
         var r = n(7),
             a = n(1),
             i = n(0),
             o = n(8),
             u = n(119),
             c = n(11),
             s = n(15),
-            l = n(279),
+            l = n(278),
             f = n(109),
             d = n(89);
 
         function p(e) {
             return Object(d.a)("MuiBackdrop", e)
         }
         Object(f.a)("MuiBackdrop", ["root", "invisible"]);
@@ -47744,19 +47744,19 @@
             i = n(1),
             o = n(0),
             u = n(8),
             c = n(110),
             s = n(11),
             l = n(45),
             f = n(15),
-            d = n(277),
-            p = n(299),
-            h = n(313),
+            d = n(276),
+            p = n(298),
+            h = n(312),
             b = n(57),
-            v = n(154),
+            v = n(153),
             m = n(205);
 
         function y(e) {
             return Object(v.a)("MuiPickersArrowSwitcher", e)
         }
         Object(m.a)("MuiPickersArrowSwitcher", ["root", "spacer", "button"]);
         var g = n(2),
@@ -47931,8 +47931,8 @@
                         }(t, e)
                     }))
                 }
             }), t)
         }
     }]
 ]);
-//# sourceMappingURL=2.63817a12.chunk.js.map
+//# sourceMappingURL=2.2edeab5c.chunk.js.map
```

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js.LICENSE.txt` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js.map` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'static/js/2.2edeab5c.chunk.js'",*

 * * "'mappings'": "';0IAGEA,EAAOC,QAAUC,EAAQ,I,+BCHZ,SAASC,IAYtB,OAXAA,EAAWC,OAAOC,OAASD,OAAOC,OAAOC,OAAS,SAAUC,GAC1D,IAAK,IAAIC,EAAI,EAAGA,EAAIC,UAAUC,OAAQF,IAAK,CACzC,IAAIG,EAASF,UAAUD,GACvB,IAAK,IAAII,KAAOD,EACVP,OAAOS,UAAUC,eAAeC,KAAKJ,EAAQC,KAC/CL,EAAOK,GAAOD,EAAOC,GAG3B,CACA,OAAOL,CACT,EACOJ,EAASa,MAAMC,KAAMR,UAC9B,CAbA,iC,+BCGET,EAAOC,QAAUC,EAAQ,I,kBCczBF,EAAOC,QAAUC,EAAQ,IAARA,E,+BCjBJ,SAASgB,EAAgBC,EAAUC,GAChD,KAAMD,aAAoBC,GACxB,MAAM,IAAIC,UAAU,oCAExB,CAJA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.63817a12.chunk.js",
+    "file": "static/js/2.2edeab5c.chunk.js",
     "names": [
         "module",
         "exports",
         "require",
         "_extends",
         "Object",
         "assign",
```

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/main.1d17f984.chunk.js` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,332 +1,332 @@
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [0], {
         196: function(e, t, a) {},
         203: function(e, t, a) {
             "use strict";
             a.r(t);
             var n = a(0),
-                c = a.n(n),
-                r = a(46),
-                i = a.n(r),
+                r = a.n(n),
+                c = a(46),
+                i = a.n(c),
                 o = a(96),
                 s = a(9),
                 l = a(19),
-                u = (a(196), a(25)),
-                d = ["red", "purple", "cyan", "green", "pink"],
+                d = (a(196), a(25)),
+                u = ["red", "purple", "cyan", "green", "pink"],
                 j = ["Pedestrian", "Bicycle", "Light vehicle", "Heavy vehicle", "Unknown"];
 
-            function b(e, t, a, n, c, r) {
+            function h(e, t, a, n, r, c) {
                 var i, o = new Map,
-                    l = Object(u.a)(e);
+                    l = Object(d.a)(e);
                 try {
                     for (l.s(); !(i = l.n()).done;) {
-                        var d = Object(s.a)(i.value, 5),
-                            b = d[0],
-                            h = d[1],
-                            m = d[2],
-                            f = d[3],
-                            g = d[4];
-                        if (a.onlyConfirmed && 1 === g || -1 === t.indexOf(j[f]));
-                        else if (o.has(b)) {
-                            var O = o.get(b),
+                        var u = Object(s.a)(i.value, 5),
+                            h = u[0],
+                            b = u[1],
+                            m = u[2],
+                            g = u[3],
+                            f = u[4];
+                        if (a.onlyConfirmed && 1 === f || -1 === t.indexOf(j[g]));
+                        else if (o.has(h)) {
+                            var O = o.get(h),
                                 x = Object(s.a)(O, 5),
                                 p = x[0],
                                 v = x[1],
                                 k = (x[2], x[3], x[4]);
-                            p.push(h), v.push(m), k.push(g)
-                        } else o.set(b, [
-                            [h],
-                            [m], f, b, [g]
+                            p.push(20 * b + 280), v.push(20 * m + 300), k.push(f)
+                        } else o.set(h, [
+                            [20 * b + 280],
+                            [20 * m + 300], g, h, [f]
                         ])
                     }
                 } catch (y) {
                     l.e(y)
                 } finally {
                     l.f()
                 }
                 return o.forEach((function(e, t) {
-                    n && (e[0].length < c || e[0].length > r) && o.delete(t)
+                    n && (e[0].length < r || e[0].length > c) && o.delete(t)
                 })), Array.from(o.values(), (function(e) {
                     return function(e, t, a) {
                         var n = Object(s.a)(e, 5),
-                            c = n[0],
-                            r = n[1],
+                            r = n[0],
+                            c = n[1],
                             i = n[2],
                             o = n[3],
                             l = n[4],
-                            u = [c[0], r[0], 0],
-                            d = [c[c.length - 1], r[r.length - 1], 0],
-                            j = c.map((function(e, n) {
+                            d = [r[0], c[0], 0],
+                            u = [r[r.length - 1], c[c.length - 1], 0],
+                            j = r.map((function(e, n) {
                                 var i = l[n],
-                                    o = "L ".concat(e, " ").concat(r[n]);
+                                    o = "L ".concat(e, " ").concat(c[n]);
                                 if ((t && 0 === i || a && 1 === i && 0 !== n) && 0 !== n) {
                                     var s = 0 === i ? 6 : 3,
-                                        u = [c[n - 1], r[n - 1]],
-                                        d = u[0],
-                                        j = u[1],
-                                        b = [e, r[n]],
-                                        h = b[0],
-                                        m = b[1],
-                                        f = Math.sqrt(Math.pow(h - d, 2) + Math.pow(m - j, 2)),
-                                        g = [(j - m) / f, (h - d) / f],
+                                        d = [r[n - 1], c[n - 1]],
+                                        u = d[0],
+                                        j = d[1],
+                                        h = [e, c[n]],
+                                        b = h[0],
+                                        m = h[1],
+                                        g = Math.sqrt(Math.pow(b - u, 2) + Math.pow(m - j, 2)),
+                                        f = [(j - m) / g, (b - u) / g],
                                         O = .707,
-                                        x = g[0] * O - g[1] * O,
-                                        p = g[0] * O + g[1] * O;
-                                    o += "L ".concat(e + x * s, " ").concat(r[n] + p * s, " L ").concat(e, " ").concat(r[n], " L ").concat(e - p * s, " ").concat(r[n] + x * s, " L ").concat(e, " ").concat(r[n])
+                                        x = f[0] * O - f[1] * O,
+                                        p = f[0] * O + f[1] * O;
+                                    o += "L ".concat(e + x * s, " ").concat(c[n] + p * s, " L ").concat(e, " ").concat(c[n], " L ").concat(e - p * s, " ").concat(c[n] + x * s, " L ").concat(e, " ").concat(c[n])
                                 }
                                 return o
                             })).join(" ");
-                        return ["M ".concat(c[0], " ").concat(r[0], " ").concat(j), i, o, u, d]
+                        return ["M ".concat(r[0], " ").concat(c[0], " ").concat(j), i, o, d, u]
                     }(e, a.markMeasurements, a.markEstimated)
                 }))
             }
-            var h = a(2),
+            var b = a(2),
                 m = function(e) {
                     var t = e.WIDTH,
                         a = e.HEIGHT,
                         n = e.scale,
-                        c = e.pathStrings,
-                        r = e.showId,
+                        r = e.pathStrings,
+                        c = e.showId,
                         i = e.selectedIndices,
                         o = e.vertices;
-                    return Object(h.jsxs)("svg", {
+                    return Object(b.jsxs)("svg", {
                         width: t * n,
                         height: a * n,
                         style: {
                             transform: "scale(".concat(n, ")"),
                             transformOrigin: "top left"
                         },
-                        children: [c.map((function(e, t) {
-                            return i.has(t) ? Object(h.jsx)(h.Fragment, {}) : Object(h.jsxs)("g", {
-                                children: [Object(h.jsx)("path", {
+                        children: [r.map((function(e, t) {
+                            return i.has(t) ? Object(b.jsx)(b.Fragment, {}) : Object(b.jsxs)("g", {
+                                children: [Object(b.jsx)("path", {
                                     d: e[0],
-                                    stroke: d[e[1]],
+                                    stroke: u[e[1]],
                                     fill: "none"
-                                }), Object(h.jsx)("circle", {
+                                }), Object(b.jsx)("circle", {
                                     cx: e[3][0],
                                     cy: e[3][1],
                                     r: 4,
                                     fill: "green",
                                     strokeWidth: "4"
-                                }), Object(h.jsx)("circle", {
+                                }), Object(b.jsx)("circle", {
                                     cx: e[4][0],
                                     cy: e[4][1],
                                     r: 4,
                                     fill: "red",
                                     strokeWidth: "4"
-                                }), r && Object(h.jsx)("text", {
+                                }), c && Object(b.jsx)("text", {
                                     x: e[4][0],
                                     y: e[4][1],
                                     fill: "white",
                                     fontFamily: "sans-serif",
                                     fontSize: 10,
                                     children: e[2]
                                 })]
                             }, e[0])
                         })), o]
                     })
                 },
-                f = a(140),
-                g = a.n(f),
-                O = a(269),
-                x = a(271),
-                p = a(293),
-                v = a(308),
-                k = a(309),
-                y = a(274),
-                w = a(310),
-                C = a(311),
-                S = a(312),
-                M = a(295),
-                I = function(e) {
+                g = a(139),
+                f = a.n(g),
+                O = a(268),
+                x = a(270),
+                p = a(292),
+                v = a(307),
+                k = a(308),
+                y = a(273),
+                w = a(309),
+                C = a(310),
+                L = a(311),
+                M = a(294),
+                S = function(e) {
                     e.label;
                     var t = e.image,
                         a = e.WIDTH,
-                        c = e.HEIGHT,
-                        r = e.tracks,
+                        r = e.HEIGHT,
+                        c = e.tracks,
                         i = e.from,
                         o = e.to,
-                        u = e.showType,
-                        d = e.filterLength,
+                        d = e.showType,
+                        u = e.filterLength,
                         j = e.minLength,
-                        f = e.maxLength,
-                        I = Object(n.useState)(1),
-                        L = Object(s.a)(I, 2),
-                        D = L[0],
-                        T = L[1],
-                        E = Object(n.useState)({
+                        g = e.maxLength,
+                        S = Object(n.useState)(1),
+                        T = Object(s.a)(S, 2),
+                        I = T[0],
+                        D = T[1],
+                        F = Object(n.useState)({
                             markMeasurements: !1,
                             markEstimated: !1,
                             onlyConfirmed: !1,
                             trackId: !1,
                             showLines: !1
                         }),
-                        H = Object(s.a)(E, 2),
-                        R = H[0],
+                        H = Object(s.a)(F, 2),
+                        E = H[0],
                         N = H[1],
-                        F = Object(n.useState)(new Map),
-                        W = Object(s.a)(F, 2),
+                        R = Object(n.useState)(new Map),
+                        W = Object(s.a)(R, 2),
                         Y = W[0],
-                        A = W[1],
-                        B = Object(n.useMemo)((function() {
-                            return b(r.slice(i, o), u, R, d, j, f)
-                        }), [i, o, u, R, d, j, f]),
-                        P = Object(h.jsx)(m, {
+                        B = W[1],
+                        P = Object(n.useMemo)((function() {
+                            return h(c.slice(i, o), d, E, u, j, g)
+                        }), [i, o, d, E, u, j, g]),
+                        A = Object(b.jsx)(m, {
                             WIDTH: a,
-                            HEIGHT: c,
-                            scale: D,
-                            pathStrings: B,
-                            showId: R.trackId,
+                            HEIGHT: r,
+                            scale: I,
+                            pathStrings: P,
+                            showId: E.trackId,
                             selectedIndices: Y,
                             vertices: []
                         });
                     var G;
-                    return Object(h.jsxs)("div", {
-                        children: [Object(h.jsx)("div", {
+                    return Object(b.jsxs)("div", {
+                        children: [Object(b.jsx)("div", {
                             className: "control-container",
-                            children: Object(h.jsx)(p.a, {
-                                value: D,
+                            children: Object(b.jsx)(p.a, {
+                                value: I,
                                 "aria-label": "Default",
                                 valueLabelDisplay: "auto",
                                 onChange: function(e, t) {
-                                    "number" === typeof t && T(t)
+                                    "number" === typeof t && D(t)
                                 },
                                 min: 0,
                                 max: 10,
                                 step: .01,
                                 color: "primary",
                                 className: "slider",
                                 style: {
                                     width: 300,
                                     margin: 0
                                 }
                             })
-                        }), Object(h.jsxs)("div", {
+                        }), Object(b.jsxs)("div", {
                             style: {
                                 overflow: "hidden",
                                 display: "flex"
                             },
-                            children: [Object(h.jsxs)("div", {
+                            children: [Object(b.jsxs)("div", {
                                 style: {
                                     display: "flex",
                                     flexDirection: "column"
                                 },
-                                children: [Object(h.jsx)(g.a, {
-                                    children: Object(h.jsx)("div", {
+                                children: [Object(b.jsx)(f.a, {
+                                    children: Object(b.jsx)("div", {
                                         className: "image-container",
                                         style: {
-                                            width: a * D,
-                                            height: c * D,
+                                            width: a * I,
+                                            height: r * I,
                                             backgroundImage: "url(".concat(t, ")")
                                         },
-                                        children: P
+                                        children: A
                                     })
-                                }), Object(h.jsx)("div", {
+                                }), Object(b.jsx)("div", {
                                     style: {
                                         marginTop: 10
                                     },
-                                    children: Object(h.jsxs)(v.a, {
+                                    children: Object(b.jsxs)(v.a, {
                                         sx: {
                                             width: "100%",
                                             maxWidth: 360,
                                             bgcolor: "background.paper",
                                             position: "relative",
                                             overflow: "auto",
                                             maxHeight: 400,
                                             "& ul": {
                                                 padding: 0
                                             },
                                             borderRadius: 1
                                         },
-                                        subheader: Object(h.jsx)(k.a, {
+                                        subheader: Object(b.jsx)(k.a, {
                                             children: "Tracks"
                                         }),
                                         component: "nav",
                                         "aria-label": "main mailbox folders",
-                                        children: [Object(h.jsx)(y.a, {}), (G = B, G.map((function(e, t) {
-                                            return Object(h.jsxs)(O.a, {
+                                        children: [Object(b.jsx)(y.a, {}), (G = P, G.map((function(e, t) {
+                                            return Object(b.jsxs)(O.a, {
                                                 selected: Y.has(t),
                                                 onClick: function(e) {
-                                                    Y.has(t) ? A((function(e) {
+                                                    Y.has(t) ? B((function(e) {
                                                         return e.delete(t), new Map(e)
                                                     })) : function(e, t) {
-                                                        A((function(e) {
+                                                        B((function(e) {
                                                             return new Map(e.set(t, !0))
                                                         }))
                                                     }(0, t)
                                                 },
-                                                children: [Object(h.jsx)(x.a, {
+                                                children: [Object(b.jsx)(x.a, {
                                                     primary: e[2]
-                                                }), Object(h.jsx)(x.a, {
+                                                }), Object(b.jsx)(x.a, {
                                                     primary: e[1]
                                                 })]
                                             }, t)
                                         })))]
                                     })
                                 })]
-                            }), Object(h.jsx)(w.a, {
+                            }), Object(b.jsx)(w.a, {
                                 sx: {
                                     margin: 0,
                                     marginLeft: 2
                                 },
                                 component: "fieldset",
                                 variant: "standard",
-                                children: Object(h.jsxs)(C.a, {
-                                    children: [Object(h.jsx)(S.a, {
-                                        control: Object(h.jsx)(M.a, {
-                                            checked: R.markMeasurements,
+                                children: Object(b.jsxs)(C.a, {
+                                    children: [Object(b.jsx)(L.a, {
+                                        control: Object(b.jsx)(M.a, {
+                                            checked: E.markMeasurements,
                                             onChange: function(e) {
                                                 N((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         markMeasurements: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Mark measurments"
-                                    }), Object(h.jsx)(S.a, {
-                                        control: Object(h.jsx)(M.a, {
-                                            checked: R.markEstimated,
+                                    }), Object(b.jsx)(L.a, {
+                                        control: Object(b.jsx)(M.a, {
+                                            checked: E.markEstimated,
                                             onChange: function(e) {
                                                 N((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         markEstimated: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Mark estimated"
-                                    }), Object(h.jsx)(S.a, {
-                                        control: Object(h.jsx)(M.a, {
-                                            checked: R.onlyConfirmed,
+                                    }), Object(b.jsx)(L.a, {
+                                        control: Object(b.jsx)(M.a, {
+                                            checked: E.onlyConfirmed,
                                             onChange: function(e) {
                                                 N((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         onlyConfirmed: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Show only confirmed"
-                                    }), Object(h.jsx)(S.a, {
-                                        control: Object(h.jsx)(M.a, {
-                                            checked: R.trackId,
+                                    }), Object(b.jsx)(L.a, {
+                                        control: Object(b.jsx)(M.a, {
+                                            checked: E.trackId,
                                             onChange: function(e) {
                                                 N((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         trackId: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Show track id"
-                                    }), Object(h.jsx)(S.a, {
-                                        control: Object(h.jsx)(M.a, {
-                                            checked: R.showLines,
+                                    }), Object(b.jsx)(L.a, {
+                                        control: Object(b.jsx)(M.a, {
+                                            checked: E.showLines,
                                             onChange: function(e) {
                                                 N((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         showLines: e.target.checked
                                                     })
                                                 }))
                                             }
@@ -334,337 +334,369 @@
                                         label: "Show lines"
                                     })]
                                 })
                             })]
                         })]
                     })
                 },
-                L = a(146),
-                D = a(275),
-                T = a(290),
-                E = a(289),
-                H = a(29),
-                R = a.n(H),
-                N = a(300),
-                F = a(301),
-                W = a(291),
-                Y = a(303),
-                A = a(306),
-                B = a(302),
-                P = a(95),
-                G = function() {
-                    var e = Object(o.useRenderData)(),
-                        t = Object(n.useState)(0),
-                        a = Object(s.a)(t, 2),
-                        r = a[0],
-                        i = a[1],
-                        l = Object(n.useState)(0),
-                        u = Object(s.a)(l, 2),
-                        d = u[0],
-                        b = u[1],
-                        m = Object(n.useState)(0),
-                        f = Object(s.a)(m, 2),
-                        g = f[0],
-                        O = f[1],
-                        p = Object(n.useState)(R()(e.args.date)),
-                        v = Object(s.a)(p, 2),
-                        k = v[0],
-                        y = v[1],
-                        C = Object(n.useState)(R()(e.args.date)),
-                        H = Object(s.a)(C, 2),
-                        G = H[0],
-                        V = H[1],
-                        _ = Object(n.useState)(R()(e.args.date)),
-                        J = Object(s.a)(_, 2),
-                        q = J[0],
-                        z = J[1],
-                        U = Object(n.useState)(1),
-                        K = Object(s.a)(U, 2),
-                        Q = K[0],
-                        X = K[1],
-                        Z = c.a.useState(j),
-                        $ = Object(s.a)(Z, 2),
-                        ee = $[0],
-                        te = $[1],
-                        ae = Object(n.useState)(!1),
-                        ne = Object(s.a)(ae, 2),
-                        ce = ne[0],
-                        re = ne[1],
-                        ie = Object(n.useState)(0),
-                        oe = Object(s.a)(ie, 2),
-                        se = oe[0],
-                        le = oe[1],
-                        ue = Object(n.useState)(0),
-                        de = Object(s.a)(ue, 2),
-                        je = de[0],
-                        be = de[1],
-                        he = Object(n.useState)(e.args.tracks),
-                        me = Object(s.a)(he, 2),
-                        fe = me[0],
-                        ge = (me[1], e.args.image),
-                        Oe = e.args.height,
-                        xe = e.args.width;
-                    console.log(ge);
-                    Object(n.useEffect)((function() {
-                        k.isValid() && P.Streamlit.setComponentValue(k.format("YYYY-MM-DD"))
-                    }), [k]), Object(n.useEffect)((function() {
-                        ! function() {
-                            var e, t;
-                            if (0 === g) e = ke(G, 0, fe.length - 1), t = ke(q, 0, fe.length - 1);
-                            else if (1 === g) {
-                                for (var a = e = d + 1; a < fe.length - 1 && R()(fe[a][5]).isBefore(q);) a++;
-                                t = a
-                            } else {
-                                console.log("Backwards", r, fe[r][5], G.toISOString());
-                                for (var n = t = r; n > 0 && G.isBefore(R()(fe[n][5]));) n--;
-                                e = n + 1
-                            }
-                            i(e), b(t), console.log("First track:", fe[e]), console.log("Last track", fe[t - 1]), console.log("From ".concat(e, " to ").concat(t))
-                        }()
-                    }), [G, q]);
-                    var pe = function() {
-                            V((function(e) {
-                                return e.subtract(Q, "minutes")
-                            })), z((function(e) {
-                                return e.subtract(Q, "minutes")
-                            })), O(-1)
-                        },
-                        ve = function() {
-                            V((function(e) {
-                                return e.add(Q, "minutes")
-                            })), z((function(e) {
-                                return e.add(Q, "minutes")
-                            })), O(1)
-                        };
-
-                    function ke(e, t, a) {
-                        if (t < a) {
-                            var n = Math.floor((t + a) / 2);
-                            if (0 === n) return 0;
-                            var c = R()(fe[n][5]);
-                            return c.isAfter(e) && R()(fe[n - 1][5]).isBefore(e) ? n : c.isAfter(e) ? ke(e, t, n) : ke(e, n + 1, a)
-                        }
-                        return t === a ? t : -1
-                    }
-                    Object(n.useEffect)((function() {
-                        var e = function(e) {
-                            "ArrowRight" === e.key ? ve() : "ArrowLeft" === e.key && pe()
-                        };
-                        return document.addEventListener("keydown", e),
-                            function() {
-                                document.removeEventListener("keydown", e)
-                            }
-                    }), [Q]);
-                    var ye = [Object(h.jsx)(I, {
-                            image: ge,
-                            WIDTH: xe,
-                            HEIGHT: Oe,
-                            tracks: fe,
-                            from: r,
-                            to: d,
-                            label: "Version 1",
-                            showType: ee,
-                            filterLength: ce,
-                            minLength: se,
-                            maxLength: je
-                        })],
-                        we = {
+                T = a(29),
+                I = a.n(T),
+                D = a(95),
+                F = a(299),
+                H = a(300),
+                E = a(290),
+                N = a(302),
+                R = a(305),
+                W = a(301),
+                Y = a(145),
+                B = a(288),
+                P = a(289),
+                A = a(274),
+                G = function(e) {
+                    var t = e.date,
+                        a = e.setDate,
+                        n = e.fromTime,
+                        r = e.setFromTime,
+                        c = e.setToTime,
+                        i = e.interval,
+                        o = e.setDir,
+                        s = e.setInterval,
+                        l = e.showType,
+                        d = e.handleChange,
+                        u = e.filterLength,
+                        h = e.setFilterLength,
+                        m = e.minLength,
+                        g = e.setMinLength,
+                        f = e.maxLength,
+                        O = e.setMaxLength,
+                        p = e.handleBackwardClick,
+                        v = e.handleForwardClick,
+                        k = {
                             PaperProps: {
                                 style: {
                                     maxHeight: 224,
                                     width: 250
                                 }
                             }
                         };
-                    return Object(h.jsxs)("div", {
-                        style: {
-                            flexDirection: "column",
-                            marginTop: 30
-                        },
-                        children: [Object(h.jsxs)(L.a, {
-                            dateAdapter: D.a,
-                            children: [Object(h.jsx)(E.a, {
+                    return console.log(l), Object(b.jsxs)("div", {
+                        children: [Object(b.jsxs)(Y.a, {
+                            dateAdapter: A.a,
+                            children: [Object(b.jsx)(B.a, {
                                 label: "Date",
                                 format: "YYYY-MM-DD",
-                                value: k,
+                                value: t,
                                 onChange: function(e) {
-                                    e && y(e)
+                                    e && a(e)
                                 },
                                 sx: {
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
                                     marginRight: 2
                                 }
-                            }), Object(h.jsx)(T.a, {
+                            }), Object(b.jsx)(P.a, {
                                 label: "From time",
-                                value: G,
+                                value: n,
                                 onChange: function(e) {
-                                    e && (V(e), z(e.add(Q, "minutes")), O(0))
+                                    e && (r(e), c(e.add(i, "minutes")), o(0))
                                 },
                                 ampm: !1,
                                 sx: {
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
                                     marginRight: 2
                                 }
                             })]
-                        }), Object(h.jsx)(N.a, {
+                        }), Object(b.jsx)(F.a, {
                             label: "Interval in minutes",
                             id: "outlined-start-adornment",
                             sx: {
                                 width: "25ch",
                                 backgroundColor: "background.default",
                                 borderRadius: 1,
                                 margin: 0,
                                 marginRight: 2
                             },
-                            value: Q,
+                            value: i,
                             onChange: function(e) {
                                 var t = Number(e.target.value);
-                                isNaN(t) || (X(t), z(G.add(t, "minutes")))
+                                isNaN(t) || (s(t), c(n.add(t, "minutes")))
                             }
-                        }), Object(h.jsxs)(w.a, {
+                        }), Object(b.jsxs)(w.a, {
                             sx: {
                                 m: 1,
                                 width: 300,
                                 margin: 0
                             },
-                            children: [Object(h.jsx)(F.a, {
+                            children: [Object(b.jsx)(H.a, {
                                 id: "demo-multiple-name-label",
                                 children: "Show types"
-                            }), Object(h.jsx)(W.a, {
+                            }), Object(b.jsx)(E.a, {
                                 labelId: "demo-multiple-name-label",
                                 id: "demo-multiple-name",
                                 multiple: !0,
-                                value: ee,
-                                onChange: function(e) {
-                                    var t = e.target.value;
-                                    te("string" === typeof t ? t.split(",") : t)
-                                },
-                                input: Object(h.jsx)(Y.a, {
+                                value: l,
+                                onChange: d,
+                                input: Object(b.jsx)(N.a, {
                                     label: "Show types"
                                 }),
                                 renderValue: function(e) {
                                     return e.join(", ")
                                 },
-                                MenuProps: we,
+                                MenuProps: k,
                                 sx: {
                                     backgroundColor: "background.default"
                                 },
                                 children: j.map((function(e) {
-                                    return Object(h.jsxs)(A.a, {
+                                    return Object(b.jsxs)(R.a, {
                                         value: e,
-                                        children: [Object(h.jsx)(M.a, {
-                                            checked: ee.indexOf(e) > -1
-                                        }), Object(h.jsx)(x.a, {
+                                        children: [Object(b.jsx)(M.a, {
+                                            checked: l.indexOf(e) > -1
+                                        }), Object(b.jsx)(x.a, {
                                             primary: e
                                         })]
                                     }, e)
                                 }))
                             })]
-                        }), Object(h.jsx)("div", {
-                            children: Object(h.jsx)(S.a, {
-                                control: Object(h.jsx)(M.a, {
-                                    checked: ce,
+                        }), Object(b.jsx)("div", {
+                            children: Object(b.jsx)(L.a, {
+                                control: Object(b.jsx)(M.a, {
+                                    checked: u,
                                     onChange: function(e) {
-                                        re(e.target.checked)
+                                        h(e.target.checked)
                                     }
                                 }),
                                 label: "Filter length",
                                 style: {
                                     margin: 0,
                                     marginTop: 10
                                 }
                             })
-                        }), ce && Object(h.jsxs)("div", {
+                        }), u && Object(b.jsxs)("div", {
                             style: {
                                 marginTop: 10
                             },
-                            children: [Object(h.jsx)(N.a, {
+                            children: [Object(b.jsx)(F.a, {
                                 label: "Minimum length",
                                 id: "outlined-start-adornment",
                                 sx: {
                                     m: 1,
                                     width: "25ch",
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
                                     margin: 0,
                                     marginRight: 2
                                 },
-                                value: se,
+                                value: m,
                                 onChange: function(e) {
                                     var t = Number(e.target.value);
-                                    isNaN(t) || le(t)
+                                    isNaN(t) || g(t)
                                 }
-                            }), Object(h.jsx)(N.a, {
+                            }), Object(b.jsx)(F.a, {
                                 label: "Maximum length",
                                 id: "outlined-start-adornment",
                                 sx: {
                                     m: 1,
                                     width: "25ch",
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
                                     margin: 0,
                                     marginRight: 2
                                 },
-                                value: je,
+                                value: f,
                                 onChange: function(e) {
                                     var t = Number(e.target.value);
-                                    isNaN(t) || be(t)
+                                    isNaN(t) || O(t)
                                 }
                             })]
-                        }), Object(h.jsxs)("div", {
+                        }), Object(b.jsxs)("div", {
                             style: {
                                 margin: 0,
                                 marginTop: 10
                             },
-                            children: [Object(h.jsx)(B.a, {
+                            children: [Object(b.jsx)(W.a, {
                                 sx: {
                                     marginRight: 2,
                                     backgroundColor: "background.default"
                                 },
                                 onClick: function() {
-                                    return pe()
+                                    return p()
                                 },
                                 children: "<"
-                            }), Object(h.jsx)(B.a, {
+                            }), Object(b.jsx)(W.a, {
                                 sx: {
                                     marginRight: 2,
                                     backgroundColor: "background.default"
                                 },
                                 onClick: function() {
-                                    return ve()
+                                    return v()
                                 },
                                 children: ">"
                             })]
-                        }), Object(h.jsx)("div", {
+                        })]
+                    })
+                },
+                V = function() {
+                    var e = Object(o.useRenderData)(),
+                        t = Object(n.useState)(0),
+                        a = Object(s.a)(t, 2),
+                        c = a[0],
+                        i = a[1],
+                        l = Object(n.useState)(0),
+                        d = Object(s.a)(l, 2),
+                        u = d[0],
+                        h = d[1],
+                        m = Object(n.useState)(0),
+                        g = Object(s.a)(m, 2),
+                        f = g[0],
+                        O = g[1],
+                        x = Object(n.useState)(I()(e.args.date)),
+                        p = Object(s.a)(x, 2),
+                        v = p[0],
+                        k = p[1],
+                        y = Object(n.useState)(I()(e.args.date)),
+                        w = Object(s.a)(y, 2),
+                        C = w[0],
+                        L = w[1],
+                        M = Object(n.useState)(I()(e.args.date)),
+                        T = Object(s.a)(M, 2),
+                        F = T[0],
+                        H = T[1],
+                        E = Object(n.useState)(1),
+                        N = Object(s.a)(E, 2),
+                        R = N[0],
+                        W = N[1],
+                        Y = r.a.useState(j),
+                        B = Object(s.a)(Y, 2),
+                        P = B[0],
+                        A = B[1],
+                        V = Object(n.useState)(!1),
+                        _ = Object(s.a)(V, 2),
+                        J = _[0],
+                        X = _[1],
+                        q = Object(n.useState)(0),
+                        z = Object(s.a)(q, 2),
+                        U = z[0],
+                        K = z[1],
+                        Q = Object(n.useState)(0),
+                        Z = Object(s.a)(Q, 2),
+                        $ = Z[0],
+                        ee = Z[1],
+                        te = Object(n.useState)(e.args.tracks),
+                        ae = Object(s.a)(te, 2),
+                        ne = ae[0],
+                        re = (ae[1], e.args.image),
+                        ce = e.args.height,
+                        ie = e.args.width;
+                    Object(n.useEffect)((function() {
+                        v.isValid() && D.Streamlit.setComponentValue(v.format("YYYY-MM-DD"))
+                    }), [v]), Object(n.useEffect)((function() {
+                        ! function() {
+                            var e, t;
+                            if (0 === f) e = oe(C, 0, ne.length - 1), t = oe(F, 0, ne.length - 1);
+                            else if (1 === f) {
+                                var a = e = u + 1;
+                                for (console.log("INDEX:", a, ne.length - 1, a < ne.length - 1); a < ne.length && I()(ne[a][5]).isBefore(F);) a++;
+                                t = a
+                            } else {
+                                var n = t = c;
+                                for (console.log("INDEX:", n, ne.length); n > 0 && n < ne.length && C.isBefore(I()(ne[n][5]));) n--;
+                                e = n + 1
+                            }
+                            i(e), h(t), console.log("First track:", ne[e]), console.log("Last track", ne[t - 1]), console.log("From ".concat(e, " to ").concat(t))
+                        }()
+                    }), [C, F]);
+
+                    function oe(e, t, a) {
+                        for (; t < a;) {
+                            var n = Math.floor(t + a >>> 1);
+                            if (0 === n) return 0;
+                            var r = I()(ne[n][5]);
+                            if (r.isAfter(e) && I()(ne[n - 1][5]).isBefore(e)) return n;
+                            r.isAfter(e) ? a = n : t = n + 1
+                        }
+                        return t
+                    }
+                    var se = [Object(b.jsx)(S, {
+                        image: re,
+                        WIDTH: ie,
+                        HEIGHT: ce,
+                        tracks: ne,
+                        from: c,
+                        to: u,
+                        label: "Version 1",
+                        showType: P,
+                        filterLength: J,
+                        minLength: U,
+                        maxLength: $
+                    })];
+                    return Object(b.jsxs)("div", {
+                        style: {
+                            flexDirection: "column",
+                            marginTop: 30
+                        },
+                        children: [Object(b.jsx)(G, {
+                            date: v,
+                            setDate: k,
+                            fromTime: C,
+                            setFromTime: L,
+                            setToTime: H,
+                            interval: R,
+                            setDir: O,
+                            setInterval: W,
+                            showType: P,
+                            handleChange: function(e) {
+                                var t = e.target.value;
+                                A("string" === typeof t ? t.split(",") : t)
+                            },
+                            filterLength: J,
+                            setFilterLength: X,
+                            minLength: U,
+                            setMinLength: K,
+                            maxLength: $,
+                            setMaxLength: ee,
+                            handleBackwardClick: function() {
+                                L((function(e) {
+                                    return e.subtract(R, "minutes")
+                                })), H((function(e) {
+                                    return e.subtract(R, "minutes")
+                                })), O(-1)
+                            },
+                            handleForwardClick: function() {
+                                L((function(e) {
+                                    return e.add(R, "minutes")
+                                })), H((function(e) {
+                                    return e.add(R, "minutes")
+                                })), O(1)
+                            }
+                        }), Object(b.jsx)("div", {
                             style: {
                                 display: "flex",
                                 flexDirection: "row"
                             },
-                            children: Object(h.jsxs)("div", {
+                            children: Object(b.jsxs)("div", {
                                 style: {
                                     flexDirection: "row",
                                     flexWrap: "wrap"
                                 },
-                                children: [ye.map((function(e) {
+                                children: [se.map((function(e) {
                                     return e
-                                })), Object(h.jsx)("div", {
+                                })), Object(b.jsx)("div", {
                                     style: {
                                         height: 1e4
                                     }
                                 })]
                             })
                         })]
                     })
                 },
-                V = a(151),
-                _ = a(297);
+                _ = a(150),
+                J = a(296);
             console.warn = function() {};
-            var J = Object(V.a)({
+            var X = Object(_.a)({
                 palette: {
                     primary: {
                         main: "#F63366"
                     },
                     common: {
                         black: "#F63366"
                     },
@@ -680,22 +712,22 @@
                     },
                     background: {
                         default: "#262730",
                         paper: "#262730"
                     }
                 }
             });
-            i.a.render(Object(h.jsx)(c.a.StrictMode, {
-                children: Object(h.jsx)(o.StreamlitProvider, {
-                    children: Object(h.jsx)(_.a, {
-                        theme: J,
-                        children: Object(h.jsx)(G, {})
+            i.a.render(Object(b.jsx)(r.a.StrictMode, {
+                children: Object(b.jsx)(o.StreamlitProvider, {
+                    children: Object(b.jsx)(J.a, {
+                        theme: X,
+                        children: Object(b.jsx)(V, {})
                     })
                 })
             }), document.getElementById("root"))
         }
     },
     [
         [203, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.1d17f984.chunk.js.map
+//# sourceMappingURL=main.070b89e3.chunk.js.map
```

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/main.1d17f984.chunk.js.map` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js.map`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7867283765901277%*

 * *Differences: {"'file'": "'static/js/main.070b89e3.chunk.js'",*

 * * "'mappings'": "'wPAAaA,EAAS,CAAC,MAAO,SAAU,OAAQ,QAAS,QAC5CC,EAAQ,CACnB,aACA,UACA,gBACA,gBACA,WCEK,SAASC,EACdC,EACAC,EACAC,EACAC,EACAC,EACAC,GAEA,IACiDC,EAD3CC,EAAW,IAAIC,IAA4BC,EAAAC,YACPV,GAAO,IAAjD,IAAAS,EAAAE,MAAAL,EAAAG,EAAAG,KAAAC,MAAmD,CAAC,IAADC,EAAAC,YAAAT,EAAAU,MAAA,GAAvCC,EAAEH,EAAA,GAAEI,EAACJ,EAAA,GAAEK,EAACL,EAAA,GAAEM,EAAIN,EAAA,GAAEO,EAASP,EAAA,GACnC,GACGZ,EAAQoB,eAA+B,IAAdD,IACS,IAAnCpB,EAASsB,QAAQzB,EAAMsB,UAGvB,GAAIb,EAASiB,IAAIP,GAAK,CACpB […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.1d17f984.chunk.js",
-    "mappings": "wPAAaA,EAAS,CAAC,MAAO,SAAU,OAAQ,QAAS,QAC5CC,EAAQ,CACnB,aACA,UACA,gBACA,gBACA,WCEK,SAASC,EACdC,EACAC,EACAC,EACAC,EACAC,EACAC,GAEA,IACiDC,EAD3CC,EAAW,IAAIC,IAA4BC,EAAAC,YACPV,GAAO,IAAjD,IAAAS,EAAAE,MAAAL,EAAAG,EAAAG,KAAAC,MAAmD,CAAC,IAADC,EAAAC,YAAAT,EAAAU,MAAA,GAAvCC,EAAEH,EAAA,GAAEI,EAACJ,EAAA,GAAEK,EAACL,EAAA,GAAEM,EAAIN,EAAA,GAAEO,EAASP,EAAA,GACnC,GACGZ,EAAQoB,eAA+B,IAAdD,IACS,IAAnCpB,EAASsB,QAAQzB,EAAMsB,UAGvB,GAAIb,EAASiB,IAAIP,GAAK,CACpB,IAAAQ,EAMIlB,EAASmB,IAAIT,GAAGU,EAAAZ,YAAAU,EAAA,GALlBG,EAAYD,EAAA,GACZE,EAAYF,EAAA,GAGZG,GAFYH,EAAA,GACFA,EAAA,GACDA,EAAA,IAEXC,EAAaG,KAAKb,GAClBW,EAAaE,KAAKZ,GAClBW,EAAUC,KAAKV,EACjB,MACEd,EAASyB,IAAIf,EAAI,CAAC,CAACC,GAAI,CAACC,GAAIC,EAAMH,EAAI,CAACI,IAG7C,CAAC,OAAAY,GAAAxB,EAAAyB,EAAAD,EAAA,SAAAxB,EAAA0B,GAAA,CAWD,OATA5B,EAAS6B,SAAQ,SAACC,EAAOC,GAErBnC,IACCkC,EAAM,GAAGE,OAASnC,GAAaiC,EAAM,GAAGE,OAASlC,IAElDE,EAASiC,OAAOF,EAEpB,IAEOG,MAAMC,KAAKnC,EAASoC,UAAU,SAACN,GAAK,OAK7C,SACEA,EACAO,EACAC,GAGE,IAAAC,EAAA/B,YAAsCsB,EAAK,GAApCU,EAAED,EAAA,GAAEE,EAAEF,EAAA,GAAE1B,EAAI0B,EAAA,GAAE7B,EAAE6B,EAAA,GAAEhB,EAASgB,EAAA,GAC5BG,EAAgB,CAACF,EAAG,GAAIC,EAAG,GAAI,GAC/BE,EAAc,CAACH,EAAGA,EAAGR,OAAS,GAAIS,EAAGA,EAAGT,OAAS,GAAI,GACrDY,EAAWJ,EACdK,KAAI,SAAClC,EAAGmC,GACP,IAAMhC,EAAYS,EAAUuB,GACxBC,EAAW,KAAAC,OAAQrC,EAAC,KAAAqC,OAAIP,EAAGK,IAC/B,IACIT,GAA8B,IAAdvB,GACfwB,GAA+B,IAAdxB,GAAyB,IAANgC,IACjC,IAANA,EACA,CACA,IAAMG,EAAqB,IAAdnC,EAAkB,EAAI,EACnCoC,EAAiB,CAACV,EAAGM,EAAI,GAAIL,EAAGK,EAAI,IAA7BK,EAAED,EAAA,GAAEE,EAAEF,EAAA,GACbG,EAAiB,CAAC1C,EAAG8B,EAAGK,IAAjBQ,EAAED,EAAA,GAAEE,EAAEF,EAAA,GACPrB,EAASwB,KAAKC,KAAKD,KAAKE,IAAIJ,EAAKH,EAAI,GAAKK,KAAKE,IAAIH,EAAKH,EAAI,IAC5DO,EAAmB,EAAEP,EAAKG,GAAMvB,GAASsB,EAAKH,GAAMnB,GACpD4B,EAAQ,KACRC,EACJF,EAAiB,GAAKC,EAAQD,EAAiB,GAAKC,EAChDE,EACJH,EAAiB,GAAKC,EAAQD,EAAiB,GAAKC,EACtDb,GAAW,KAAAC,OAASrC,EAAIkD,EAAUZ,EAAI,KAAAD,OACpCP,EAAGK,GAAKgB,EAAUb,EAAI,OAAAD,OAClBrC,EAAC,KAAAqC,OAAIP,EAAGK,GAAE,OAAAE,OAAMrC,EAAImD,EAAUb,EAAI,KAAAD,OACtCP,EAAGK,GAAKe,EAAUZ,EAAI,OAAAD,OAClBrC,EAAC,KAAAqC,OAAIP,EAAGK,GAChB,CACA,OAAOC,CACT,IACCgB,KAAK,KAER,MAAO,CADS,KAAAf,OAAQR,EAAG,GAAE,KAAAQ,OAAIP,EAAG,GAAE,KAAAO,OAAIJ,GACtB/B,EAAMH,EAAIgC,EAAUC,EAE5C,CA5CIqB,CAAWlC,EAAOnC,EAAQsE,iBAAkBtE,EAAQuE,cAAc,GAEtE,C,WCtCaC,EAA8B,SAAHjD,GAQjC,IAPLkD,EAAKlD,EAALkD,MACAC,EAAMnD,EAANmD,OACAC,EAAKpD,EAALoD,MACA9E,EAAW0B,EAAX1B,YACA+E,EAAMrD,EAANqD,OACAC,EAAetD,EAAfsD,gBACAC,EAAQvD,EAARuD,SAEA,OACEC,eAAA,OACEC,MAAOP,EAAQE,EACfM,OAAQP,EAASC,EACjBO,MAAO,CACLC,UAAU,SAAD9B,OAAWsB,EAAK,KACzBS,gBAAiB,YACjBC,SAAA,CAEDxF,EAAYqD,KAAI,SAACoC,EAAMC,GAMtB,OAAQV,EAAgBvD,IAAIiE,GA8B1BC,cAAAC,WAAA,IA7BAV,eAAA,KAAAM,SAAA,CACEG,cAAA,QAAME,EAAGJ,EAAK,GAAIK,OAAQhG,EAAO2F,EAAK,IAAKM,KAAK,SAChDJ,cAAA,UACEK,GAAIP,EAAK,GAAG,GACZQ,GAAIR,EAAK,GAAG,GACZS,EAAG,EACHH,KAAK,QACLI,YAAY,MAEdR,cAAA,UACEK,GAAIP,EAAK,GAAG,GACZQ,GAAIR,EAAK,GAAG,GACZS,EAAG,EACHH,KAAK,MACLI,YAAY,MAEbpB,GACCY,cAAA,QACExE,EAAGsE,EAAK,GAAG,GACXrE,EAAGqE,EAAK,GAAG,GACXM,KAAK,QACLK,WAAW,aACXC,SAAU,GAAGb,SAEZC,EAAK,OAxBJA,EAAK,GA+BjB,IACCR,IAGP,E,4GCkMeqB,EAxOqC,SAAH5E,GAC1CA,EAAL6E,MAWK,IAVLC,EAAK9E,EAAL8E,MACA5B,EAAKlD,EAALkD,MACAC,EAAMnD,EAANmD,OACA4B,EAAM/E,EAAN+E,OACA9D,EAAIjB,EAAJiB,KACA+D,EAAEhF,EAAFgF,GACAxG,EAAQwB,EAARxB,SACAE,EAAYsB,EAAZtB,aACAC,EAASqB,EAATrB,UACAC,EAASoB,EAATpB,UAEAqG,EAA0BC,mBAAiB,GAAEC,EAAA7F,YAAA2F,EAAA,GAAtC7B,EAAK+B,EAAA,GAAEC,EAAQD,EAAA,GACtBE,EAA8BH,mBAAe,CAC3CnC,kBAAkB,EAClBC,eAAe,EACfnD,eAAe,EACfyF,SAAS,EACTC,WAAW,IACXC,EAAAlG,YAAA+F,EAAA,GANK5G,EAAO+G,EAAA,GAAEC,EAAUD,EAAA,GAO1BE,EAA8CR,mBAC5C,IAAInG,KACL4G,EAAArG,YAAAoG,EAAA,GAFMpC,EAAeqC,EAAA,GAAEC,EAAkBD,EAAA,GAOpCE,EAAQC,mBAAQ,WACpB,OAAOxH,EACLyG,EAAOgB,MAAM9E,EAAM+D,GACnBxG,EACAC,EACAC,EACAC,EACAC,EAEJ,GAAG,CAACqC,EAAM+D,EAAIxG,EAAUC,EAASC,EAAcC,EAAWC,IAQpDoH,EACJ/B,cAAChB,EAAK,CACJC,MAAOA,EACPC,OAAQA,EACRC,MAAOA,EACP9E,YAAauH,EACbxC,OAAQ5E,EAAQ6G,QAChBhC,gBAAiBA,EACjBC,SAAU,KAgBd,IAOoB0C,EAsBpB,OACEzC,eAAA,OAAAM,SAAA,CACEG,cAAA,OAAKiC,UAAU,oBAAmBpC,SAChCG,cAACkC,IAAM,CACL5G,MAAO6D,EACP,aAAW,UACXgD,kBAAkB,OAClBC,SAlEmB,SAACC,EAAcC,GAChB,kBAAbA,GACTnB,EAASmB,EAEb,EA+DQC,IAAK,EACLC,IAAK,GACLC,KAAM,IACNC,MAAM,UACNT,UAAU,SACVvC,MAAO,CAAEF,MAAO,IAAKmD,OAAQ,OAGjCpD,eAAA,OAAKG,MAAO,CAAEkD,SAAU,SAAUC,QAAS,QAAShD,SAAA,CAClDN,eAAA,OAAKG,MAAO,CAAEmD,QAAS,OAAQC,cAAe,UAAWjD,SAAA,CACvDG,cAAC+C,IAAS,CAAAlD,SACRG,cAAA,OACEiC,UAAU,kBACVvC,MAAO,CACLF,MAAOP,EAAQE,EACfM,OAAQP,EAASC,EACjB6D,gBAAgB,OAADnF,OAASgD,EAAK,MAC7BhB,SAEDkC,MAGL/B,cAAA,OAAKN,MAAO,CAAEuD,UAAW,IAAKpD,SAC5BN,eAAC2D,IAAI,CACHC,GAAI,CACF3D,MAAO,OACP4D,SAAU,IACVC,QAAS,mBACTC,SAAU,WACVV,SAAU,OACVW,UAAW,IACX,OAAQ,CAAEC,QAAS,GACnBC,aAAc,GAEhBC,UAAW1D,cAAC2D,IAAa,CAAA9D,SAAC,WAC1B+D,UAAU,MACV,aAAW,uBAAsB/D,SAAA,CAEjCG,cAAC6D,IAAO,KApEA7B,EAqEIJ,EApEfI,EAAKtE,KAAI,SAACoC,EAAMC,GACrB,OACER,eAACuE,IAAc,CAEbC,SAAU1E,EAAgBvD,IAAIiE,GAC9BiE,QAAS,SAAC3B,GACHhD,EAAgBvD,IAAIiE,GAEvB4B,GAAmB,SAACsC,GAElB,OADAA,EAAQnH,OAAOiD,GACR,IAAIjF,IAAImJ,EACjB,IAnBgB,SAC1B5B,EACAtC,GAEA4B,GAAmB,SAACsC,GAAO,OAAK,IAAInJ,IAAImJ,EAAQ3H,IAAIyD,GAAO,GAAM,GACnE,CAS2CmE,CAAoB7B,EAAOtC,EAM9D,EAAEF,SAAA,CAEFG,cAACmE,IAAY,CAACC,QAAStE,EAAK,KAC5BE,cAACmE,IAAY,CAACC,QAAStE,EAAK,OAZvBC,EAeX,aAsDIC,cAACqE,IAAW,CACVlB,GAAI,CAAER,OAAQ,EAAG2B,WAAY,GAC7BV,UAAU,WACVW,QAAQ,WAAU1E,SAElBN,eAACiF,IAAS,CAAA3E,SAAA,CACRG,cAACyE,IAAgB,CACfC,QACE1E,cAAC2E,IAAQ,CACPC,QAASpK,EAAQsE,iBACjBsD,SAAU,SAACC,GACTb,GAAW,SAACqD,GAAW,OAAAC,wBAAA,GAClBD,GAAW,IACd/F,iBAAkBuD,EAAM0C,OAAOH,SAAO,GAE1C,IAGJhE,MAAM,qBAERZ,cAACyE,IAAgB,CACfC,QACE1E,cAAC2E,IAAQ,CACPC,QAASpK,EAAQuE,cACjBqD,SAAU,SAACC,GACTb,GAAW,SAACqD,GAAW,OAAAC,wBAAA,GAClBD,GAAW,IACd9F,cAAesD,EAAM0C,OAAOH,SAAO,GAEvC,IAGJhE,MAAM,mBAERZ,cAACyE,IAAgB,CACfC,QACE1E,cAAC2E,IAAQ,CACPC,QAASpK,EAAQoB,cACjBwG,SAAU,SAACC,GACTb,GAAW,SAACqD,GAAW,OAAAC,wBAAA,GAClBD,GAAW,IACdjJ,cAAeyG,EAAM0C,OAAOH,SAAO,GAEvC,IAGJhE,MAAM,wBAERZ,cAACyE,IAAgB,CACfC,QACE1E,cAAC2E,IAAQ,CACPC,QAASpK,EAAQ6G,QACjBe,SAAU,SAACC,GACTb,GAAW,SAACqD,GAAW,OAAAC,wBAAA,GAClBD,GAAW,IACdxD,QAASgB,EAAM0C,OAAOH,SAAO,GAEjC,IAGJhE,MAAM,kBAERZ,cAACyE,IAAgB,CACfC,QACE1E,cAAC2E,IAAQ,CACPC,QAASpK,EAAQ8G,UACjBc,SAAU,SAACC,GACTb,GAAW,SAACqD,GAAW,OAAAC,wBAAA,GAClBD,GAAW,IACdvD,UAAWe,EAAM0C,OAAOH,SAAO,GAEnC,IAGJhE,MAAM,yBAOpB,E,mHCgGeoE,EAjViB,WAC9B,IAAMC,EAAaC,0BACnBlE,EAAwBC,mBAAS,GAAEC,EAAA7F,YAAA2F,EAAA,GAA5BhE,EAAIkE,EAAA,GAAEiE,EAAOjE,EAAA,GACpBE,EAAoBH,mBAAS,GAAEM,EAAAlG,YAAA+F,EAAA,GAAxBL,EAAEQ,EAAA,GAAE6D,EAAK7D,EAAA,GAChBE,EAAsBR,mBAAqB,GAAES,EAAArG,YAAAoG,EAAA,GAAtC4D,EAAG3D,EAAA,GAAE4D,EAAM5D,EAAA,GAClB6D,EAAwBtE,mBAAgBuE,IAAMP,EAAWQ,KAAW,OAAGC,EAAArK,YAAAkK,EAAA,GAAhEI,EAAID,EAAA,GAAEE,EAAOF,EAAA,GACpBG,EAAgC5E,mBAC9BuE,IAAMP,EAAWQ,KAAW,OAC7BK,EAAAzK,YAAAwK,EAAA,GAFME,EAAQD,EAAA,GAAEE,EAAWF,EAAA,GAG5BG,EAA4BhF,mBAAgBuE,IAAMP,EAAWQ,KAAW,OAAGS,EAAA7K,YAAA4K,EAAA,GAApEE,EAAMD,EAAA,GAAEE,EAASF,EAAA,GACxBG,EAAgCpF,mBAAS,GAAEqF,EAAAjL,YAAAgL,EAAA,GAApCE,EAAQD,EAAA,GAAEE,EAAWF,EAAA,GAC5BG,EAAgCC,IAAMzF,SAAmB7G,GAAMuM,EAAAtL,YAAAoL,EAAA,GAAxDlM,GAAQoM,EAAA,GAAEC,GAAWD,EAAA,GAC5BE,GAAwC5F,oBAAS,GAAM6F,GAAAzL,YAAAwL,GAAA,GAAhDpM,GAAYqM,GAAA,GAAEC,GAAeD,GAAA,GACpCE,GAAkC/F,mBAAS,GAAEgG,GAAA5L,YAAA2L,GAAA,GAAtCtM,GAASuM,GAAA,GAAEC,GAAYD,GAAA,GAC9BE,GAAkClG,mBAAS,GAAEmG,GAAA/L,YAAA8L,GAAA,GAAtCxM,GAASyM,GAAA,GAAEC,GAAYD,GAAA,GAC9BE,GAA4BrG,mBAAkBgE,EAAWQ,KAAa,QAAE8B,GAAAlM,YAAAiM,GAAA,GAAjExG,GAAMyG,GAAA,GACPC,IADkBD,GAAA,GACTtC,EAAWQ,KAAY,OAChChG,GAASwF,EAAWQ,KAAa,OACjCjG,GAAQyF,EAAWQ,KAAY,MACrCgC,QAAQC,IAAIF,IAkCZG,qBAAU,WACJhC,EAAKiC,WACPC,YAAUC,kBAAkBnC,EAAKoC,OAAO,cAE5C,GAAG,CAACpC,IAEJgC,qBAAU,YACW,WACjB,IAAIK,EACAC,EACJ,GAAY,IAAR5C,EACF2C,EAAYE,GAAanC,EAAU,EAAGjF,GAAOjE,OAAS,GACtDoL,EAAUC,GAAa/B,EAAQ,EAAGrF,GAAOjE,OAAS,QAC7C,GAAY,IAARwI,EAAW,CAGpB,IADA,IAAI1H,EADJqK,EAAYjH,EAAK,EAEVpD,EAAImD,GAAOjE,OAAS,GAAK2I,IAAM1E,GAAOnD,GAAG,IAAIwK,SAAShC,IAC3DxI,IAEFsK,EAAUtK,CACZ,KAAO,CACL8J,QAAQC,IAAI,YAAa1K,EAAM8D,GAAO9D,GAAM,GAAI+I,EAASqC,eAGzD,IADA,IAAIzK,EADJsK,EAAUjL,EAEHW,EAAI,GAAKoI,EAASoC,SAAS3C,IAAM1E,GAAOnD,GAAG,MAChDA,IAGFqK,EAAYrK,EAAI,CAClB,CACAwH,EAAQ6C,GACR5C,EAAM6C,GACNR,QAAQC,IAAI,eAAgB5G,GAAOkH,IACnCP,QAAQC,IAAI,aAAc5G,GAAOmH,EAAU,IAC3CR,QAAQC,IAAI,QAAD7J,OAASmK,EAAS,QAAAnK,OAAOoK,GACtC,CACAI,EACF,GAAG,CAACtC,EAAUI,IAEd,IAAMmC,GAAsB,WAC1BtC,GAAY,SAACD,GAAQ,OAAKA,EAASwC,SAAShC,EAAU,UAAU,IAChEH,GAAU,SAACD,GAAM,OAAKA,EAAOoC,SAAShC,EAAU,UAAU,IAC1DjB,GAAQ,EACV,EAEMkD,GAAqB,WACzBxC,GAAY,SAACD,GAAQ,OAAKA,EAAS0C,IAAIlC,EAAU,UAAU,IAC3DH,GAAU,SAACD,GAAM,OAAKA,EAAOsC,IAAIlC,EAAU,UAAU,IACrDjB,EAAO,EACT,EAqBA,SAAS4C,GAAaQ,EAAaC,EAAaC,GAC9C,GAAID,EAAMC,EAAM,CACd,IAAMC,EAAMxK,KAAKyK,OAAOH,EAAMC,GAAQ,GACtC,GAAY,IAARC,EAAW,OAAO,EACtB,IAAME,EAAUvD,IAAM1E,GAAO+H,GAAK,IAClC,OAAIE,EAAQC,QAAQN,IAASlD,IAAM1E,GAAO+H,EAAM,GAAG,IAAIV,SAASO,GACvDG,EACEE,EAAQC,QAAQN,GAClBR,GAAaQ,EAAMC,EAAKE,GAExBX,GAAaQ,EAAMG,EAAM,EAAGD,EAEvC,CAAO,OAAID,IAAQC,EACVD,GAED,CACV,CAnCAhB,qBAAU,WACR,IAAMsB,EAAgB,SAAC5G,GACH,eAAdA,EAAMzF,IACR4L,KACuB,cAAdnG,EAAMzF,KACf0L,IAEJ,EAIA,OAFAY,SAASC,iBAAiB,UAAWF,GAE9B,WACLC,SAASE,oBAAoB,UAAWH,EAC1C,CACF,GAAG,CAAC1C,IAuBJ,IAAM8C,GAA6B,CACjCrJ,cAACW,EAAa,CACZE,MAAO2G,GACPvI,MAAOO,GACPN,OAAQO,GACRqB,OAAQA,GACR9D,KAAMA,EACN+D,GAAIA,EACJH,MAAO,YACPrG,SAAUA,GACVE,aAAcA,GACdC,UAAWA,GACXC,UAAWA,MAgBT2O,GAAY,CAChBC,WAAY,CACV7J,MAAO,CACL6D,UAAWiG,IACXhK,MAAO,OAKb,OACED,eAAA,OAAKG,MAAO,CAAEoD,cAAe,SAAUG,UAAW,IAAKpD,SAAA,CACrDN,eAACkK,IAAoB,CAACC,YAAaC,IAAa9J,SAAA,CAC9CG,cAAC4J,IAAU,CACThJ,MAAM,OACNmH,OAAO,aACPzM,MAAOqK,EACPvD,SAAU,SAACE,GACLA,GAAUsD,EAAQtD,EACxB,EACAa,GAAI,CACF0G,gBAAiB,qBACjBpG,aAAc,EACdqG,YAAa,KAGjB9J,cAAC+J,IAAU,CACTnJ,MAAM,YACNtF,MAAOyK,EACP3D,SAAU,SAACE,GACLA,IACF0D,EAAY1D,GACZ8D,EAAU9D,EAASmG,IAAIlC,EAAU,YACjCjB,EAAO,GAEX,EACA0E,MAAM,EACN7G,GAAI,CACF0G,gBAAiB,qBACjBpG,aAAc,EACdqG,YAAa,QAInB9J,cAACiK,IAAS,CACRrJ,MAAM,sBACNrF,GAAG,2BACH4H,GAAI,CACF3D,MAAO,OACPqK,gBAAiB,qBACjBpG,aAAc,EACdd,OAAQ,EACRmH,YAAa,GAEfxO,MAAOiL,EACPnE,SAAU,SAAC8H,GACT,IAAMC,EAAMC,OAAOF,EAAOnF,OAAOzJ,OAC5B+O,MAAMF,KACT3D,EAAY2D,GACZ/D,EAAUL,EAAS0C,IAAI0B,EAAK,YAEhC,IAEF5K,eAAC8E,IAAW,CAAClB,GAAI,CAAEmH,EAAG,EAAG9K,MAAO,IAAKmD,OAAQ,GAAI9C,SAAA,CAC/CG,cAACuK,IAAU,CAAChP,GAAG,2BAA0BsE,SAAC,eAC1CG,cAACwK,IAAM,CACLC,QAAQ,2BACRlP,GAAG,qBACHmP,UAAQ,EACRpP,MAAOf,GACP6H,SAjFa,SAACC,GACpB,IACY/G,EACR+G,EADF0C,OAAUzJ,MAEZsL,GAEmB,kBAAVtL,EAAqBA,EAAMqP,MAAM,KAAOrP,EAEnD,EA0EQsP,MAAO5K,cAAC6K,IAAa,CAACjK,MAAM,eAC5BkK,YAAa,SAAC/G,GAAQ,OAAKA,EAASnF,KAAK,KAAK,EAC9C0K,UAAWA,GACXnG,GAAI,CAAE0G,gBAAiB,sBAAuBhK,SAE7CzF,EAAMsD,KAAI,SAACqN,GAAI,OACdxL,eAACyL,IAAQ,CAAY1P,MAAOyP,EAAKlL,SAAA,CAC/BG,cAAC2E,IAAQ,CAACC,QAASrK,GAASsB,QAAQkP,IAAS,IAC7C/K,cAACmE,IAAY,CAACC,QAAS2G,MAFVA,EAGJ,SAIjB/K,cAAA,OAAAH,SACEG,cAACyE,IAAgB,CACfC,QACE1E,cAAC2E,IAAQ,CACPC,QAASnK,GACT2H,SAAU,SAACC,GACT0E,GAAgB1E,EAAM0C,OAAOH,QAC/B,IAGJhE,MAAM,gBACNlB,MAAO,CAAEiD,OAAQ,EAAGM,UAAW,QAGlCxI,IACC8E,eAAA,OAAKG,MAAO,CAAEuD,UAAW,IAAKpD,SAAA,CAC5BG,cAACiK,IAAS,CACRrJ,MAAM,iBACNrF,GAAG,2BACH4H,GAAI,CACFmH,EAAG,EACH9K,MAAO,OACPqK,gBAAiB,qBACjBpG,aAAc,EACdd,OAAQ,EACRmH,YAAa,GAEfxO,MAAOZ,GACP0H,SAAU,SAAC8H,GACT,IAAMC,EAAMC,OAAOF,EAAOnF,OAAOzJ,OAC5B+O,MAAMF,IACTjD,GAAaiD,EAEjB,IAEFnK,cAACiK,IAAS,CACRrJ,MAAM,iBACNrF,GAAG,2BACH4H,GAAI,CACFmH,EAAG,EACH9K,MAAO,OACPqK,gBAAiB,qBACjBpG,aAAc,EACdd,OAAQ,EACRmH,YAAa,GAEfxO,MAAOX,GACPyH,SAAU,SAAC8H,GACT,IAAMC,EAAMC,OAAOF,EAAOnF,OAAOzJ,OAC5B+O,MAAMF,IACT9C,GAAa8C,EAEjB,OAIN5K,eAAA,OAAKG,MAAO,CAAEiD,OAAQ,EAAGM,UAAW,IAAKpD,SAAA,CACvCG,cAACiL,IAAM,CACL9H,GAAI,CAAE2G,YAAa,EAAGD,gBAAiB,sBACvC7F,QAAS,kBAAMsE,IAAqB,EAACzI,SAEpC,MAEHG,cAACiL,IAAM,CACL9H,GAAI,CAAE2G,YAAa,EAAGD,gBAAiB,sBACvC7F,QAAS,kBAAMwE,IAAoB,EAAC3I,SAEnC,SAGLG,cAAA,OAAKN,MAAO,CAAEmD,QAAS,OAAQC,cAAe,OAAQjD,SACpDN,eAAA,OACEG,MAAO,CACLoD,cAAe,MACfoI,SAAU,QACVrL,SAAA,CAEDwJ,GAAY3L,KAAI,SAACyN,GAAI,OAAKA,CAAI,IAC/BnL,cAAA,OAAKN,MAAO,CAAED,OAAQ,cAKhC,E,kBCjWAgI,QAAQ2D,KAAO,WAAO,EAEtB,IAAMC,EAAQC,YAAY,CACxBC,QAAS,CACPnH,QAAS,CACPoH,KAAM,WAERC,OAAQ,CACNC,MAAO,WAETC,UAAW,CACTH,KAAM,WAERI,KAAM,CACJxH,QAAS,OACTuH,UAAW,QAEbE,OAAQ,CACNC,OAAQ,QAEVC,WAAY,CACVC,QAAS,UACTC,MAAO,cAKbC,IAASC,OACPnM,cAAC0G,IAAM0F,WAAU,CAAAvM,SACfG,cAACqM,oBAAiB,CAAAxM,SAChBG,cAACsM,IAAa,CAACjB,MAAOA,EAAMxL,SAC1BG,cAACgF,EAAa,UAIpBkE,SAASqD,eAAe,Q",
+    "file": "static/js/main.070b89e3.chunk.js",
+    "mappings": "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",
     "names": [
         "colors",
         "names",
         "pathStrings",
         "entries",
         "showType",
         "filters",
@@ -171,112 +171,109 @@
         "FormControlLabel",
         "control",
         "Checkbox",
         "checked",
         "prevFilters",
         "_objectSpread",
         "target",
+        "Header",
+        "date",
+        "setDate",
+        "fromTime",
+        "setFromTime",
+        "setToTime",
+        "interval",
+        "setDir",
+        "setInterval",
+        "handleChange",
+        "setFilterLength",
+        "setMinLength",
+        "setMaxLength",
+        "handleBackwardClick",
+        "handleForwardClick",
+        "MenuProps",
+        "PaperProps",
+        "ITEM_HEIGHT",
+        "console",
+        "log",
+        "LocalizationProvider",
+        "dateAdapter",
+        "AdapterDayjs",
+        "DatePicker",
+        "format",
+        "backgroundColor",
+        "marginRight",
+        "TimePicker",
+        "add",
+        "ampm",
+        "TextField",
+        "newVal",
+        "val",
+        "Number",
+        "isNaN",
+        "m",
+        "InputLabel",
+        "Select",
+        "labelId",
+        "multiple",
+        "input",
+        "OutlinedInput",
+        "renderValue",
+        "name",
+        "MenuItem",
+        "Button",
         "TrackAnalysis",
         "renderData",
         "useRenderData",
         "setFrom",
         "setTo",
         "dir",
-        "setDir",
         "_useState7",
         "dayjs",
         "args",
         "_useState8",
-        "date",
-        "setDate",
         "_useState9",
         "_useState10",
-        "fromTime",
-        "setFromTime",
         "_useState11",
         "_useState12",
         "toTime",
-        "setToTime",
         "_useState13",
         "_useState14",
-        "interval",
-        "setInterval",
         "_React$useState",
         "React",
         "_React$useState2",
         "setShowType",
         "_useState15",
         "_useState16",
-        "setFilterLength",
         "_useState17",
         "_useState18",
-        "setMinLength",
         "_useState19",
         "_useState20",
-        "setMaxLength",
         "_useState21",
         "_useState22",
         "ground",
-        "console",
-        "log",
         "useEffect",
         "isValid",
         "Streamlit",
         "setComponentValue",
-        "format",
         "fromIndex",
         "toIndex",
         "binarySearch",
         "isBefore",
-        "toISOString",
         "setIndices",
-        "handleBackwardClick",
-        "subtract",
-        "handleForwardClick",
-        "add",
         "time",
         "low",
         "high",
         "mid",
         "floor",
         "midTime",
         "isAfter",
-        "handleKeyDown",
-        "document",
-        "addEventListener",
-        "removeEventListener",
         "cameraPlots",
-        "MenuProps",
-        "PaperProps",
-        "ITEM_HEIGHT",
-        "LocalizationProvider",
-        "dateAdapter",
-        "AdapterDayjs",
-        "DatePicker",
-        "backgroundColor",
-        "marginRight",
-        "TimePicker",
-        "ampm",
-        "TextField",
-        "newVal",
-        "val",
-        "Number",
-        "isNaN",
-        "m",
-        "InputLabel",
-        "Select",
-        "labelId",
-        "multiple",
         "split",
-        "input",
-        "OutlinedInput",
-        "renderValue",
-        "name",
-        "MenuItem",
-        "Button",
+        "subtract",
         "flexWrap",
         "plot",
         "warn",
         "theme",
         "createTheme",
         "palette",
         "main",
@@ -290,28 +287,31 @@
         "default",
         "paper",
         "ReactDOM",
         "render",
         "StrictMode",
         "StreamlitProvider",
         "ThemeProvider",
+        "document",
         "getElementById"
     ],
     "sourceRoot": "",
     "sources": [
         "helpers/consts.ts",
         "helpers/Paths.ts",
         "components/plotter/Lines.tsx",
         "components/plotter/SourcePlotter.tsx",
+        "components/plotter/header/Header.tsx",
         "components/plotter/TrackAnalysis.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "export const colors = [\"red\", \"purple\", \"cyan\", \"green\", \"pink\"]\nexport const names = [\n  \"Pedestrian\",\n  \"Bicycle\",\n  \"Light vehicle\",\n  \"Heavy vehicle\",\n  \"Unknown\",\n]\n",
-        "import { Pos, TransformMatrix, transformPos } from \"./Matrix\"\nimport { names } from \"./consts\"\nimport { Show } from \"./types\"\n\nexport type Track = [number, number, number, number, number, string]\nexport type Path = [string, number, number, Pos, Pos]\ntype InternalTrack = [number[], number[], number, number, number[]]\n\nexport function pathStrings(\n  entries: Track[],\n  showType: string[],\n  filters: Show,\n  filterLength: boolean,\n  minLength: number,\n  maxLength: number\n): Path[] {\n  const trackMap = new Map<number, InternalTrack>()\n  for (const [id, x, y, type, estimated] of entries) {\n    if (\n      (filters.onlyConfirmed && estimated === 1) ||\n      showType.indexOf(names[type]) === -1\n    ) {\n    } else {\n      if (trackMap.has(id)) {\n        const [\n          xCoordinates,\n          yCoordinates,\n          existingType,\n          existingId,\n          estimates,\n        ] = trackMap.get(id)!\n        xCoordinates.push(x)\n        yCoordinates.push(y)\n        estimates.push(estimated)\n      } else {\n        trackMap.set(id, [[x], [y], type, id, [estimated]])\n      }\n    }\n  }\n\n  trackMap.forEach((track, key) => {\n    if (\n      filterLength &&\n      (track[0].length < minLength || track[0].length > maxLength)\n    ) {\n      trackMap.delete(key)\n    }\n  })\n\n  return Array.from(trackMap.values(), (track) =>\n    createPath(track, filters.markMeasurements, filters.markEstimated)\n  )\n}\n\nfunction createPath(\n  track: InternalTrack,\n  markMeasured: boolean,\n  markEstimates: boolean\n): Path {\n  {\n    const [xs, ys, type, id, estimates] = track\n    const startPos: Pos = [xs[0], ys[0], 0]\n    const endPos: Pos = [xs[xs.length - 1], ys[ys.length - 1], 0]\n    const pathData = xs\n      .map((x, i) => {\n        const estimated = estimates[i]\n        let pathSegment = `L ${x} ${ys[i]}`\n        if (\n          ((markMeasured && estimated === 0) ||\n            (markEstimates && estimated === 1 && i !== 0)) &&\n          i !== 0\n        ) {\n          const size = estimated === 0 ? 6 : 3\n          const [x1, y1] = [xs[i - 1], ys[i - 1]]\n          const [x2, y2] = [x, ys[i]]\n          const length = Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2))\n          const perpendicularDir = [(y1 - y2) / length, (x2 - x1) / length]\n          const angle = 0.707\n          const offsetX =\n            perpendicularDir[0] * angle - perpendicularDir[1] * angle\n          const offsetY =\n            perpendicularDir[0] * angle + perpendicularDir[1] * angle\n          pathSegment += `L ${x + offsetX * size} ${\n            ys[i] + offsetY * size\n          } L ${x} ${ys[i]} L ${x - offsetY * size} ${\n            ys[i] + offsetX * size\n          } L ${x} ${ys[i]}`\n        }\n        return pathSegment\n      })\n      .join(\" \")\n    const pathString = `M ${xs[0]} ${ys[0]} ${pathData}`\n    return [pathString, type, id, startPos, endPos]\n  }\n}\n",
+        "import { Pos, TransformMatrix, transformPos } from \"./Matrix\"\nimport { names } from \"./consts\"\nimport { Show } from \"./types\"\n\nexport type Track = [number, number, number, number, number, string]\nexport type Path = [string, number, number, Pos, Pos]\ntype InternalTrack = [number[], number[], number, number, number[]]\n\nexport function pathStrings(\n  entries: Track[],\n  showType: string[],\n  filters: Show,\n  filterLength: boolean,\n  minLength: number,\n  maxLength: number\n): Path[] {\n  const trackMap = new Map<number, InternalTrack>()\n  for (const [id, x, y, type, estimated] of entries) {\n    if (\n      (filters.onlyConfirmed && estimated === 1) ||\n      showType.indexOf(names[type]) === -1\n    ) {\n    } else {\n      if (trackMap.has(id)) {\n        const [\n          xCoordinates,\n          yCoordinates,\n          existingType,\n          existingId,\n          estimates,\n        ] = trackMap.get(id)!\n        xCoordinates.push(x * 20 + 280)\n        yCoordinates.push(y * 20 + 300)\n        estimates.push(estimated)\n      } else {\n        trackMap.set(id, [\n          [x * 20 + 280],\n          [y * 20 + 300],\n          type,\n          id,\n          [estimated],\n        ])\n      }\n    }\n  }\n\n  trackMap.forEach((track, key) => {\n    if (\n      filterLength &&\n      (track[0].length < minLength || track[0].length > maxLength)\n    ) {\n      trackMap.delete(key)\n    }\n  })\n\n  return Array.from(trackMap.values(), (track) =>\n    createPath(track, filters.markMeasurements, filters.markEstimated)\n  )\n}\n\nfunction createPath(\n  track: InternalTrack,\n  markMeasured: boolean,\n  markEstimates: boolean\n): Path {\n  {\n    const [xs, ys, type, id, estimates] = track\n    const startPos: Pos = [xs[0], ys[0], 0]\n    const endPos: Pos = [xs[xs.length - 1], ys[ys.length - 1], 0]\n    const pathData = xs\n      .map((x, i) => {\n        const estimated = estimates[i]\n        let pathSegment = `L ${x} ${ys[i]}`\n        if (\n          ((markMeasured && estimated === 0) ||\n            (markEstimates && estimated === 1 && i !== 0)) &&\n          i !== 0\n        ) {\n          const size = estimated === 0 ? 6 : 3\n          const [x1, y1] = [xs[i - 1], ys[i - 1]]\n          const [x2, y2] = [x, ys[i]]\n          const length = Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2))\n          const perpendicularDir = [(y1 - y2) / length, (x2 - x1) / length]\n          const angle = 0.707\n          const offsetX =\n            perpendicularDir[0] * angle - perpendicularDir[1] * angle\n          const offsetY =\n            perpendicularDir[0] * angle + perpendicularDir[1] * angle\n          pathSegment += `L ${x + offsetX * size} ${\n            ys[i] + offsetY * size\n          } L ${x} ${ys[i]} L ${x - offsetY * size} ${\n            ys[i] + offsetX * size\n          } L ${x} ${ys[i]}`\n        }\n        return pathSegment\n      })\n      .join(\" \")\n    const pathString = `M ${xs[0]} ${ys[0]} ${pathData}`\n    return [pathString, type, id, startPos, endPos]\n  }\n}\n",
         "import React from \"react\"\nimport { colors } from \"../../helpers/consts\"\nimport { Path } from \"../../helpers/Paths\"\n\ntype LinesProps = {\n  WIDTH: number\n  HEIGHT: number\n  scale: number\n  pathStrings: Path[]\n  showId: boolean\n  selectedIndices: Map<number, boolean>\n  vertices: JSX.Element[]\n}\n\nexport const Lines: React.FC<LinesProps> = ({\n  WIDTH,\n  HEIGHT,\n  scale,\n  pathStrings,\n  showId,\n  selectedIndices,\n  vertices,\n}) => {\n  return (\n    <svg\n      width={WIDTH * scale}\n      height={HEIGHT * scale}\n      style={{\n        transform: `scale(${scale})`,\n        transformOrigin: \"top left\", // Set the transformation origin\n      }}\n    >\n      {pathStrings.map((path, index) => {\n        /**\n         * The strings are of the format \"...L {x-ending point} {y-ending point},\n         * we want to get these coordinates to display the starting ids above\n         * the ending point\"\n         */\n        return !selectedIndices.has(index) ? (\n          <g key={path[0]}>\n            <path d={path[0]} stroke={colors[path[1]]} fill=\"none\" />\n            <circle\n              cx={path[3][0]}\n              cy={path[3][1]}\n              r={4}\n              fill=\"green\"\n              strokeWidth=\"4\"\n            />\n            <circle\n              cx={path[4][0]}\n              cy={path[4][1]}\n              r={4}\n              fill=\"red\"\n              strokeWidth=\"4\"\n            />\n            {showId && (\n              <text\n                x={path[4][0]}\n                y={path[4][1]}\n                fill=\"white\"\n                fontFamily=\"sans-serif\"\n                fontSize={10}\n              >\n                {path[2]}\n              </text>\n            )}\n          </g>\n        ) : (\n          <></>\n        )\n      })}\n      {vertices}\n    </svg>\n  )\n}\n",
         "import React, { useState, useMemo } from \"react\"\nimport { TransformMatrix } from \"../../helpers/Matrix\"\nimport \"../../styles/styles.css\"\nimport { Path, Track, pathStrings } from \"../../helpers/Paths\"\nimport { Lines } from \"./Lines\"\nimport Draggable from \"react-draggable\"\nimport {\n  Box,\n  Checkbox,\n  Divider,\n  FormControl,\n  FormControlLabel,\n  FormGroup,\n  List,\n  ListItemButton,\n  ListItemIcon,\n  ListItemText,\n  ListSubheader,\n  Slider,\n} from \"@mui/material\"\nimport { Show } from \"../../helpers/types\"\n\ninterface SourcePlotterProps {\n  label: string\n  image: string\n  WIDTH: number\n  HEIGHT: number\n  filterLength: boolean\n  minLength: number\n  maxLength: number\n  tracks: Track[]\n  from: number\n  to: number\n  showType: string[]\n}\n\nconst SourcePlotter: React.FC<SourcePlotterProps> = ({\n  label,\n  image,\n  WIDTH,\n  HEIGHT,\n  tracks,\n  from,\n  to,\n  showType,\n  filterLength,\n  minLength,\n  maxLength,\n}) => {\n  const [scale, setScale] = useState<number>(1)\n  const [filters, setFilters] = useState<Show>({\n    markMeasurements: false,\n    markEstimated: false,\n    onlyConfirmed: false,\n    trackId: false,\n    showLines: false,\n  })\n  const [selectedIndices, setSelectedIndices] = useState<Map<number, boolean>>(\n    new Map()\n  )\n  /**\n   * Memoize the lines so we don't recalculate pathStrings everytime\n   * we rerender this component\n   */\n  const paths = useMemo(() => {\n    return pathStrings(\n      tracks.slice(from, to),\n      showType,\n      filters,\n      filterLength,\n      minLength,\n      maxLength\n    )\n  }, [from, to, showType, filters, filterLength, minLength, maxLength])\n\n  const handleSliderChange = (event: Event, newValue: number | number[]) => {\n    if (typeof newValue === \"number\") {\n      setScale(newValue)\n    }\n  }\n\n  const SVGLines = (\n    <Lines\n      WIDTH={WIDTH}\n      HEIGHT={HEIGHT}\n      scale={scale}\n      pathStrings={paths}\n      showId={filters.trackId}\n      selectedIndices={selectedIndices}\n      vertices={[]}\n    />\n  )\n\n  function sortedIndex(sortedArray: number[], value: number) {\n    let low = 0,\n      high = sortedArray.length\n\n    while (low < high) {\n      const mid = (low + high) >>> 1\n      if (sortedArray[mid] < value) low = mid + 1\n      else high = mid\n    }\n    return low\n  }\n\n  const handleListItemClick = (\n    event: React.MouseEvent<HTMLDivElement, MouseEvent>,\n    index: number\n  ) => {\n    setSelectedIndices((indices) => new Map(indices.set(index, true)))\n  }\n\n  const renderRows = (rows: Path[]) => {\n    return rows.map((path, index) => {\n      return (\n        <ListItemButton\n          key={index}\n          selected={selectedIndices.has(index)}\n          onClick={(event) => {\n            if (!selectedIndices.has(index)) handleListItemClick(event, index)\n            else\n              setSelectedIndices((indices) => {\n                indices.delete(index)\n                return new Map(indices)\n              })\n          }}\n        >\n          <ListItemText primary={path[2]} />\n          <ListItemText primary={path[1]} />\n        </ListItemButton>\n      )\n    })\n  }\n\n  return (\n    <div>\n      <div className=\"control-container\">\n        <Slider\n          value={scale}\n          aria-label=\"Default\"\n          valueLabelDisplay=\"auto\"\n          onChange={handleSliderChange}\n          min={0}\n          max={10}\n          step={0.01}\n          color=\"primary\"\n          className=\"slider\"\n          style={{ width: 300, margin: 0 }}\n        />\n      </div>\n      <div style={{ overflow: \"hidden\", display: \"flex\" }}>\n        <div style={{ display: \"flex\", flexDirection: \"column\" }}>\n          <Draggable>\n            <div\n              className=\"image-container\"\n              style={{\n                width: WIDTH * scale,\n                height: HEIGHT * scale,\n                backgroundImage: `url(${image})`,\n              }}\n            >\n              {SVGLines}\n            </div>\n          </Draggable>\n          <div style={{ marginTop: 10 }}>\n            <List\n              sx={{\n                width: \"100%\",\n                maxWidth: 360,\n                bgcolor: \"background.paper\",\n                position: \"relative\",\n                overflow: \"auto\",\n                maxHeight: 400,\n                \"& ul\": { padding: 0 },\n                borderRadius: 1,\n              }}\n              subheader={<ListSubheader>Tracks</ListSubheader>}\n              component=\"nav\"\n              aria-label=\"main mailbox folders\"\n            >\n              <Divider />\n              {renderRows(paths)}\n            </List>\n          </div>\n        </div>\n        <FormControl\n          sx={{ margin: 0, marginLeft: 2 }}\n          component=\"fieldset\"\n          variant=\"standard\"\n        >\n          <FormGroup>\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.markMeasurements}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      markMeasurements: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Mark measurments\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.markEstimated}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      markEstimated: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Mark estimated\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.onlyConfirmed}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      onlyConfirmed: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show only confirmed\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.trackId}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      trackId: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show track id\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.showLines}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      showLines: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show lines\"\n            />\n          </FormGroup>\n        </FormControl>\n      </div>\n    </div>\n  )\n}\n\nexport default SourcePlotter\n",
-        "import React, { useEffect, useState } from \"react\"\nimport SourcePlotter from \"./SourcePlotter\"\nimport { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport { Track } from \"../../helpers/Paths\"\nimport { LocalizationProvider } from \"@mui/x-date-pickers/LocalizationProvider\"\nimport { AdapterDayjs } from \"@mui/x-date-pickers/AdapterDayjs\"\nimport { TimePicker } from \"@mui/x-date-pickers/TimePicker\"\nimport { DatePicker } from \"@mui/x-date-pickers\"\nimport dayjs, { Dayjs } from \"dayjs\"\nimport {\n  Button,\n  Checkbox,\n  FormControl,\n  FormControlLabel,\n  InputLabel,\n  ListItemText,\n  MenuItem,\n  OutlinedInput,\n  Select,\n  SelectChangeEvent,\n  TextField,\n} from \"@mui/material\"\nimport { names } from \"../../helpers/consts\"\nimport { Streamlit } from \"streamlit-component-lib\"\n\nconst TrackAnalysis: React.FC = () => {\n  const renderData = useRenderData()\n  const [from, setFrom] = useState(0)\n  const [to, setTo] = useState(0)\n  const [dir, setDir] = useState<0 | 1 | -1>(0)\n  const [date, setDate] = useState<Dayjs>(dayjs(renderData.args[\"date\"]))\n  const [fromTime, setFromTime] = useState<Dayjs>(\n    dayjs(renderData.args[\"date\"])\n  )\n  const [toTime, setToTime] = useState<Dayjs>(dayjs(renderData.args[\"date\"]))\n  const [interval, setInterval] = useState(1)\n  const [showType, setShowType] = React.useState<string[]>(names)\n  const [filterLength, setFilterLength] = useState(false)\n  const [minLength, setMinLength] = useState(0)\n  const [maxLength, setMaxLength] = useState(0)\n  const [tracks, setTracks] = useState<Track[]>(renderData.args[\"tracks\"])\n  const ground = renderData.args[\"image\"]\n  const height = renderData.args[\"height\"]\n  const width = renderData.args[\"width\"]\n  console.log(ground)\n\n  const extraTrack: Track[] = [\n    [100002336, 110.397, 21.156, 1, 0, \"2023-05-04T20:08:08.520000\"],\n    [100002336, 103.7364, 35.958, 1, 0, \"2023-05-04T20:08:08.600000\"],\n    [100002336, 92.1048, 48.942, 1, 0, \"2023-05-04T20:08:08.680000\"],\n    [100002336, 96.94, 62.928, 1, 0, \"2023-05-04T20:08:08.760000\"],\n    [100002336, 102.676, 77.818, 1, 0, \"2023-05-04T20:08:08.840000\"],\n    [100002336, 105.7234, 91.916, 1, 0, \"2023-05-04T20:08:08.920000\"],\n    [100002336, 108.2698, 107.1402, 1, 0, \"2023-05-04T20:08:09.000000\"],\n    [100002336, 107.503, 119.1164, 1, 0, \"2023-05-04T20:08:09.080000\"],\n    [100002336, 110.0692, 132.6774, 1, 0, \"2023-05-04T20:08:09.160000\"],\n    [100002336, 110.8798, 145.8788, 1, 0, \"2023-05-04T20:08:09.240000\"],\n    [100002336, 112.1886, 159.5174, 1, 0, \"2023-05-04T20:08:09.320000\"],\n    [100002336, 112.9392, 173.068, 1, 0, \"2023-05-04T20:08:09.400000\"],\n    [100002336, 113.8368, 186.516, 1, 0, \"2023-05-04T20:08:09.480000\"],\n    [100002336, 115.2658, 200.6134, 1, 0, \"2023-05-04T20:08:09.560000\"],\n    [100002336, 116.1722, 214.6188, 1, 0, \"2023-05-04T20:08:09.640000\"],\n    [100002336, 117.9876, 228.8156, 1, 0, \"2023-05-04T20:08:09.720000\"],\n    [100002336, 120.4566, 243.051, 1, 0, \"2023-05-04T20:08:09.800000\"],\n    [100002336, 121.117, 256.325, 1, 0, \"2023-05-04T20:08:09.880000\"],\n    [100002336, 123.0336, 270.032, 1, 0, \"2023-05-04T20:08:09.960000\"],\n    [100002336, 125.427, 284.2901, 1, 0, \"2023-05-04T20:08:10.040000\"],\n    [100002336, 126.1348, 297.724616, 1, 0, \"2023-05-04T20:08:10.120000\"],\n    [100002336, 127.0122, 311.13014, 1, 0, \"2023-05-04T20:08:10.200000\"],\n    [100002336, 129.2824, 325.196, 1, 0, \"2023-05-04T20:08:10.280000\"],\n    [100002336, 129.79, 338.5664, 1, 0, \"2023-05-04T20:08:10.360000\"],\n    [100002336, 120.595, 522.766, 1, 0, \"2023-05-04T20:08:11.560000\"],\n    [100002336, 119.2942, 536.064, 1, 0, \"2023-05-04T20:08:11.640000\"],\n    [100002336, 116.86, 549.226, 1, 0, \"2023-05-04T20:08:11.720000\"],\n    [100002336, 111.6988, 574.988, 1, 0, \"2023-05-04T20:08:11.800000\"],\n    [100002336, 106.179, 587.106, 1, 0, \"2023-05-04T20:08:11.880000\"],\n  ]\n\n  useEffect(() => {\n    if (date.isValid()) {\n      Streamlit.setComponentValue(date.format(\"YYYY-MM-DD\"))\n    }\n  }, [date])\n\n  useEffect(() => {\n    const setIndices = () => {\n      let fromIndex: number\n      let toIndex: number\n      if (dir === 0) {\n        fromIndex = binarySearch(fromTime, 0, tracks.length - 1)\n        toIndex = binarySearch(toTime, 0, tracks.length - 1)\n      } else if (dir === 1) {\n        fromIndex = to + 1\n        let i = fromIndex\n        while (i < tracks.length - 1 && dayjs(tracks[i][5]).isBefore(toTime)) {\n          i++\n        }\n        toIndex = i\n      } else {\n        console.log(\"Backwards\", from, tracks[from][5], fromTime.toISOString())\n        toIndex = from\n        let i = toIndex\n        while (i > 0 && fromTime.isBefore(dayjs(tracks[i][5]))) {\n          i--\n        }\n\n        fromIndex = i + 1\n      }\n      setFrom(fromIndex)\n      setTo(toIndex)\n      console.log(\"First track:\", tracks[fromIndex])\n      console.log(\"Last track\", tracks[toIndex - 1])\n      console.log(`From ${fromIndex} to ${toIndex}`)\n    }\n    setIndices()\n  }, [fromTime, toTime])\n\n  const handleBackwardClick = () => {\n    setFromTime((fromTime) => fromTime.subtract(interval, \"minutes\"))\n    setToTime((toTime) => toTime.subtract(interval, \"minutes\"))\n    setDir(-1)\n  }\n\n  const handleForwardClick = () => {\n    setFromTime((fromTime) => fromTime.add(interval, \"minutes\"))\n    setToTime((toTime) => toTime.add(interval, \"minutes\"))\n    setDir(1)\n  }\n\n  useEffect(() => {\n    const handleKeyDown = (event: KeyboardEvent) => {\n      if (event.key === \"ArrowRight\") {\n        handleForwardClick()\n      } else if (event.key === \"ArrowLeft\") {\n        handleBackwardClick()\n      }\n    }\n\n    document.addEventListener(\"keydown\", handleKeyDown)\n\n    return () => {\n      document.removeEventListener(\"keydown\", handleKeyDown)\n    }\n  }, [interval])\n\n  /**\n   * OPTIMISE THIS! >>> 1 for halving and unrecurse it with a while loop\n   */\n  function binarySearch(time: Dayjs, low: number, high: number): number {\n    if (low < high) {\n      const mid = Math.floor((low + high) / 2)\n      if (mid === 0) return 0\n      const midTime = dayjs(tracks[mid][5])\n      if (midTime.isAfter(time) && dayjs(tracks[mid - 1][5]).isBefore(time)) {\n        return mid\n      } else if (midTime.isAfter(time)) {\n        return binarySearch(time, low, mid)\n      } else {\n        return binarySearch(time, mid + 1, high)\n      }\n    } else if (low === high) {\n      return low\n    }\n    return -1\n  }\n\n  const cameraPlots: JSX.Element[] = [\n    <SourcePlotter\n      image={ground}\n      WIDTH={width}\n      HEIGHT={height}\n      tracks={tracks}\n      from={from}\n      to={to}\n      label={\"Version 1\"}\n      showType={showType}\n      filterLength={filterLength}\n      minLength={minLength}\n      maxLength={maxLength}\n    />,\n  ]\n\n  const handleChange = (event: SelectChangeEvent<typeof showType>) => {\n    const {\n      target: { value },\n    } = event\n    setShowType(\n      // On autofill we get a stringified value.\n      typeof value === \"string\" ? value.split(\",\") : value\n    )\n  }\n\n  const ITEM_HEIGHT = 48\n  const ITEM_PADDING_TOP = 8\n  const MenuProps = {\n    PaperProps: {\n      style: {\n        maxHeight: ITEM_HEIGHT * 4.5 + ITEM_PADDING_TOP,\n        width: 250,\n      },\n    },\n  }\n\n  return (\n    <div style={{ flexDirection: \"column\", marginTop: 30 }}>\n      <LocalizationProvider dateAdapter={AdapterDayjs}>\n        <DatePicker\n          label=\"Date\"\n          format=\"YYYY-MM-DD\"\n          value={date}\n          onChange={(newValue) => {\n            if (newValue) setDate(newValue)\n          }}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n        <TimePicker\n          label=\"From time\"\n          value={fromTime}\n          onChange={(newValue) => {\n            if (newValue) {\n              setFromTime(newValue)\n              setToTime(newValue.add(interval, \"minutes\"))\n              setDir(0)\n            }\n          }}\n          ampm={false}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n      </LocalizationProvider>\n      <TextField\n        label=\"Interval in minutes\"\n        id=\"outlined-start-adornment\"\n        sx={{\n          width: \"25ch\",\n          backgroundColor: \"background.default\",\n          borderRadius: 1,\n          margin: 0,\n          marginRight: 2,\n        }}\n        value={interval}\n        onChange={(newVal) => {\n          const val = Number(newVal.target.value)\n          if (!isNaN(val)) {\n            setInterval(val)\n            setToTime(fromTime.add(val, \"minutes\"))\n          }\n        }}\n      />\n      <FormControl sx={{ m: 1, width: 300, margin: 0 }}>\n        <InputLabel id=\"demo-multiple-name-label\">Show types</InputLabel>\n        <Select\n          labelId=\"demo-multiple-name-label\"\n          id=\"demo-multiple-name\"\n          multiple\n          value={showType}\n          onChange={handleChange}\n          input={<OutlinedInput label=\"Show types\" />}\n          renderValue={(selected) => selected.join(\", \")}\n          MenuProps={MenuProps}\n          sx={{ backgroundColor: \"background.default\" }}\n        >\n          {names.map((name) => (\n            <MenuItem key={name} value={name}>\n              <Checkbox checked={showType.indexOf(name) > -1} />\n              <ListItemText primary={name} />\n            </MenuItem>\n          ))}\n        </Select>\n      </FormControl>\n      <div>\n        <FormControlLabel\n          control={\n            <Checkbox\n              checked={filterLength}\n              onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                setFilterLength(event.target.checked)\n              }}\n            />\n          }\n          label=\"Filter length\"\n          style={{ margin: 0, marginTop: 10 }}\n        />\n      </div>\n      {filterLength && (\n        <div style={{ marginTop: 10 }}>\n          <TextField\n            label=\"Minimum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={minLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setMinLength(val)\n              }\n            }}\n          />\n          <TextField\n            label=\"Maximum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={maxLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setMaxLength(val)\n              }\n            }}\n          />\n        </div>\n      )}\n      <div style={{ margin: 0, marginTop: 10 }}>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleBackwardClick()}\n        >\n          {\"<\"}\n        </Button>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleForwardClick()}\n        >\n          {\">\"}\n        </Button>\n      </div>\n      <div style={{ display: \"flex\", flexDirection: \"row\" }}>\n        <div\n          style={{\n            flexDirection: \"row\",\n            flexWrap: \"wrap\",\n          }}\n        >\n          {cameraPlots.map((plot) => plot)}\n          <div style={{ height: 10000 }} />\n        </div>\n      </div>\n    </div>\n  )\n}\n\nexport default TrackAnalysis\n",
+        "import {\n  TextField,\n  FormControl,\n  InputLabel,\n  Select,\n  OutlinedInput,\n  MenuItem,\n  Checkbox,\n  ListItemText,\n  FormControlLabel,\n  Button,\n  SelectChangeEvent,\n} from \"@mui/material\"\nimport {\n  LocalizationProvider,\n  DatePicker,\n  TimePicker,\n} from \"@mui/x-date-pickers\"\nimport { AdapterDayjs } from \"@mui/x-date-pickers/AdapterDayjs\"\nimport { names } from \"../../../helpers/consts\"\nimport dayjs, { Dayjs } from \"dayjs\"\n\ninterface HeaderProps {\n  date: Dayjs\n  setDate: (value: React.SetStateAction<dayjs.Dayjs>) => void\n  fromTime: Dayjs\n  setFromTime: (value: React.SetStateAction<dayjs.Dayjs>) => void\n  setToTime: (value: React.SetStateAction<dayjs.Dayjs>) => void\n  interval: number\n  setDir: (value: React.SetStateAction<0 | 1 | -1>) => void\n  setInterval: (value: React.SetStateAction<number>) => void\n  showType: string[]\n  handleChange: (event: SelectChangeEvent<string[]>) => void\n  filterLength: boolean\n  setFilterLength: (value: React.SetStateAction<boolean>) => void\n  minLength: number\n  setMinLength: (value: React.SetStateAction<number>) => void\n  maxLength: number\n  setMaxLength: (value: React.SetStateAction<number>) => void\n  handleBackwardClick: () => void\n  handleForwardClick: () => void\n}\n\nexport const Header: React.FC<HeaderProps> = ({\n  date,\n  setDate,\n  fromTime,\n  setFromTime,\n  setToTime,\n  interval,\n  setDir,\n  setInterval,\n  showType,\n  handleChange,\n  filterLength,\n  setFilterLength,\n  minLength,\n  setMinLength,\n  maxLength,\n  setMaxLength,\n  handleBackwardClick,\n  handleForwardClick,\n}) => {\n  const ITEM_HEIGHT = 48\n  const ITEM_PADDING_TOP = 8\n  const MenuProps = {\n    PaperProps: {\n      style: {\n        maxHeight: ITEM_HEIGHT * 4.5 + ITEM_PADDING_TOP,\n        width: 250,\n      },\n    },\n  }\n  console.log(showType)\n  return (\n    <div>\n      <LocalizationProvider dateAdapter={AdapterDayjs}>\n        <DatePicker\n          label=\"Date\"\n          format=\"YYYY-MM-DD\"\n          value={date}\n          onChange={(newValue) => {\n            if (newValue) setDate(newValue)\n          }}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n        <TimePicker\n          label=\"From time\"\n          value={fromTime}\n          onChange={(newValue) => {\n            if (newValue) {\n              setFromTime(newValue)\n              setToTime(newValue.add(interval, \"minutes\"))\n              setDir(0)\n            }\n          }}\n          ampm={false}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n      </LocalizationProvider>\n      <TextField\n        label=\"Interval in minutes\"\n        id=\"outlined-start-adornment\"\n        sx={{\n          width: \"25ch\",\n          backgroundColor: \"background.default\",\n          borderRadius: 1,\n          margin: 0,\n          marginRight: 2,\n        }}\n        value={interval}\n        onChange={(newVal) => {\n          const val = Number(newVal.target.value)\n          if (!isNaN(val)) {\n            setInterval(val)\n            setToTime(fromTime.add(val, \"minutes\"))\n          }\n        }}\n      />\n      <FormControl sx={{ m: 1, width: 300, margin: 0 }}>\n        <InputLabel id=\"demo-multiple-name-label\">Show types</InputLabel>\n        <Select\n          labelId=\"demo-multiple-name-label\"\n          id=\"demo-multiple-name\"\n          multiple\n          value={showType}\n          onChange={handleChange}\n          input={<OutlinedInput label=\"Show types\" />}\n          renderValue={(selected) => selected.join(\", \")}\n          MenuProps={MenuProps}\n          sx={{ backgroundColor: \"background.default\" }}\n        >\n          {names.map((name) => (\n            <MenuItem key={name} value={name}>\n              <Checkbox checked={showType.indexOf(name) > -1} />\n              <ListItemText primary={name} />\n            </MenuItem>\n          ))}\n        </Select>\n      </FormControl>\n      <div>\n        <FormControlLabel\n          control={\n            <Checkbox\n              checked={filterLength}\n              onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                setFilterLength(event.target.checked)\n              }}\n            />\n          }\n          label=\"Filter length\"\n          style={{ margin: 0, marginTop: 10 }}\n        />\n      </div>\n      {filterLength && (\n        <div style={{ marginTop: 10 }}>\n          <TextField\n            label=\"Minimum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={minLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setMinLength(val)\n              }\n            }}\n          />\n          <TextField\n            label=\"Maximum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={maxLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setMaxLength(val)\n              }\n            }}\n          />\n        </div>\n      )}\n      <div style={{ margin: 0, marginTop: 10 }}>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleBackwardClick()}\n        >\n          {\"<\"}\n        </Button>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleForwardClick()}\n        >\n          {\">\"}\n        </Button>\n      </div>\n    </div>\n  )\n}\n",
+        "import React, { useEffect, useState } from \"react\"\nimport SourcePlotter from \"./SourcePlotter\"\nimport { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport { Track } from \"../../helpers/Paths\"\nimport dayjs, { Dayjs } from \"dayjs\"\nimport { SelectChangeEvent } from \"@mui/material\"\nimport { names } from \"../../helpers/consts\"\nimport { Streamlit } from \"streamlit-component-lib\"\nimport { Header } from \"./header/Header\"\n\nconst TrackAnalysis: React.FC = () => {\n  const renderData = useRenderData()\n  const [from, setFrom] = useState(0)\n  const [to, setTo] = useState(0)\n  const [dir, setDir] = useState<0 | 1 | -1>(0)\n  const [date, setDate] = useState<Dayjs>(dayjs(renderData.args[\"date\"]))\n  const [fromTime, setFromTime] = useState<Dayjs>(\n    dayjs(renderData.args[\"date\"])\n  )\n  const [toTime, setToTime] = useState<Dayjs>(dayjs(renderData.args[\"date\"]))\n  const [interval, setInterval] = useState(1)\n  const [showType, setShowType] = React.useState<string[]>(names)\n  const [filterLength, setFilterLength] = useState(false)\n  const [minLength, setMinLength] = useState(0)\n  const [maxLength, setMaxLength] = useState(0)\n  const [tracks, setTracks] = useState<Track[]>(renderData.args[\"tracks\"])\n  const ground = renderData.args[\"image\"]\n  const height = renderData.args[\"height\"]\n  const width = renderData.args[\"width\"]\n\n  useEffect(() => {\n    if (date.isValid()) {\n      Streamlit.setComponentValue(date.format(\"YYYY-MM-DD\"))\n    }\n  }, [date])\n\n  useEffect(() => {\n    const setIndices = () => {\n      let fromIndex: number\n      let toIndex: number\n      if (dir === 0) {\n        fromIndex = binarySearch(fromTime, 0, tracks.length - 1)\n        toIndex = binarySearch(toTime, 0, tracks.length - 1)\n      } else if (dir === 1) {\n        fromIndex = to + 1\n        let i = fromIndex\n        console.log(\"INDEX:\", i, tracks.length - 1, i < tracks.length - 1)\n        while (i < tracks.length && dayjs(tracks[i][5]).isBefore(toTime)) {\n          i++\n        }\n        toIndex = i\n      } else {\n        toIndex = from\n        let i = toIndex\n        console.log(\"INDEX:\", i, tracks.length)\n        while (\n          i > 0 &&\n          i < tracks.length &&\n          fromTime.isBefore(dayjs(tracks[i][5]))\n        ) {\n          i--\n        }\n\n        fromIndex = i + 1\n      }\n      setFrom(fromIndex)\n      setTo(toIndex)\n      console.log(\"First track:\", tracks[fromIndex])\n      console.log(\"Last track\", tracks[toIndex - 1])\n      console.log(`From ${fromIndex} to ${toIndex}`)\n    }\n    setIndices()\n  }, [fromTime, toTime])\n\n  const handleBackwardClick = () => {\n    setFromTime((fromTime) => fromTime.subtract(interval, \"minutes\"))\n    setToTime((toTime) => toTime.subtract(interval, \"minutes\"))\n    setDir(-1)\n  }\n\n  const handleForwardClick = () => {\n    setFromTime((fromTime) => fromTime.add(interval, \"minutes\"))\n    setToTime((toTime) => toTime.add(interval, \"minutes\"))\n    setDir(1)\n  }\n\n  function binarySearch(time: Dayjs, low: number, high: number): number {\n    while (low < high) {\n      const mid = Math.floor((low + high) >>> 1)\n      if (mid === 0) return 0\n      const midTime = dayjs(tracks[mid][5])\n      if (midTime.isAfter(time) && dayjs(tracks[mid - 1][5]).isBefore(time)) {\n        return mid\n      } else if (midTime.isAfter(time)) {\n        high = mid\n      } else {\n        low = mid + 1\n      }\n    }\n    return low\n  }\n\n  const cameraPlots: JSX.Element[] = [\n    <SourcePlotter\n      image={ground}\n      WIDTH={width}\n      HEIGHT={height}\n      tracks={tracks}\n      from={from}\n      to={to}\n      label={\"Version 1\"}\n      showType={showType}\n      filterLength={filterLength}\n      minLength={minLength}\n      maxLength={maxLength}\n    />,\n  ]\n\n  const handleChange = (event: SelectChangeEvent<typeof showType>) => {\n    const {\n      target: { value },\n    } = event\n    setShowType(typeof value === \"string\" ? value.split(\",\") : value)\n  }\n\n  return (\n    <div style={{ flexDirection: \"column\", marginTop: 30 }}>\n      <Header\n        date={date}\n        setDate={setDate}\n        fromTime={fromTime}\n        setFromTime={setFromTime}\n        setToTime={setToTime}\n        interval={interval}\n        setDir={setDir}\n        setInterval={setInterval}\n        showType={showType}\n        handleChange={handleChange}\n        filterLength={filterLength}\n        setFilterLength={setFilterLength}\n        minLength={minLength}\n        setMinLength={setMinLength}\n        maxLength={maxLength}\n        setMaxLength={setMaxLength}\n        handleBackwardClick={handleBackwardClick}\n        handleForwardClick={handleForwardClick}\n      />\n      <div style={{ display: \"flex\", flexDirection: \"row\" }}>\n        <div\n          style={{\n            flexDirection: \"row\",\n            flexWrap: \"wrap\",\n          }}\n        >\n          {cameraPlots.map((plot) => plot)}\n          <div style={{ height: 10000 }} />\n        </div>\n      </div>\n    </div>\n  )\n}\n\nexport default TrackAnalysis\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport { StreamlitProvider } from \"streamlit-component-lib-react-hooks\"\nimport TrackAnalysis from \"./components/plotter/TrackAnalysis\"\nimport { ThemeProvider, createTheme } from \"@mui/material\"\n\n//Dirty dirty\nconsole.warn = () => {}\n\nconst theme = createTheme({\n  palette: {\n    primary: {\n      main: \"#F63366\",\n    },\n    common: {\n      black: \"#F63366\",\n    },\n    secondary: {\n      main: \"#F0F2F6\",\n    },\n    text: {\n      primary: \"#fff\",\n      secondary: \"#fff\",\n    },\n    action: {\n      active: \"#fff\",\n    },\n    background: {\n      default: \"#262730\",\n      paper: \"#262730\",\n    },\n  },\n})\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitProvider>\n      <ThemeProvider theme={theme}>\n        <TrackAnalysis />\n      </ThemeProvider>\n    </StreamlitProvider>\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.1/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map` & `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.1/st_track_analysis.egg-info/SOURCES.txt` & `st_track_analysis-0.0.2/st_track_analysis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 st_track_analysis.egg-info/dependency_links.txt
 st_track_analysis.egg-info/requires.txt
 st_track_analysis.egg-info/top_level.txt
 st_track_analysis/frontend/build/asset-manifest.json
 st_track_analysis/frontend/build/index.html
 st_track_analysis/frontend/build/static/css/main.22919367.chunk.css
 st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map
-st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js
-st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js.LICENSE.txt
-st_track_analysis/frontend/build/static/js/2.63817a12.chunk.js.map
-st_track_analysis/frontend/build/static/js/main.1d17f984.chunk.js
-st_track_analysis/frontend/build/static/js/main.1d17f984.chunk.js.map
+st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js
+st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt
+st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map
+st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js
+st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js.map
 st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js
 st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map
```
