# Comparing `tmp/st_track_analysis-0.0.2.tar.gz` & `tmp/st_track_analysis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_track_analysis-0.0.2.tar", last modified: Fri Jul 21 18:15:16 2023, max compression
+gzip compressed data, was "st_track_analysis-0.0.3.tar", last modified: Fri Jul 21 18:33:58 2023, max compression
```

## Comparing `st_track_analysis-0.0.2.tar` & `st_track_analysis-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.170087 st_track_analysis-0.0.2/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-04 12:01:44.000000 st_track_analysis-0.0.2/LICENSE
--rw-r--r--   0 elliotglas   (501) staff       (20)       53 2023-07-21 10:04:23.000000 st_track_analysis-0.0.2/MANIFEST.in
--rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 18:15:16.169859 st_track_analysis-0.0.2/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 18:15:16.170152 st_track_analysis-0.0.2/setup.cfg
--rw-r--r--   0 elliotglas   (501) staff       (20)      663 2023-07-21 18:13:03.000000 st_track_analysis-0.0.2/setup.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.161899 st_track_analysis-0.0.2/st_track_analysis/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2873 2023-07-21 18:12:54.000000 st_track_analysis-0.0.2/st_track_analysis/__init__.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.160533 st_track_analysis-0.0.2/st_track_analysis/frontend/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.163896 st_track_analysis-0.0.2/st_track_analysis/frontend/build/
--rw-r--r--   0 elliotglas   (501) staff       (20)      879 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/asset-manifest.json
--rw-r--r--   0 elliotglas   (501) staff       (20)     2186 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/index.html
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.160848 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.164329 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/
--rw-r--r--   0 elliotglas   (501) staff       (20)      840 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css
--rw-r--r--   0 elliotglas   (501) staff       (20)     1567 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.169584 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/
--rw-r--r--   0 elliotglas   (501) staff       (20)   982743 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)  4039604 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)    11330 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)    41110 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 18:14:26.000000 st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:15:16.163402 st_track_analysis-0.0.2/st_track_analysis.egg-info/
--rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)      980 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/requires.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       18 2023-07-21 18:15:16.000000 st_track_analysis-0.0.2/st_track_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.791003 st_track_analysis-0.0.3/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-04 12:01:44.000000 st_track_analysis-0.0.3/LICENSE
+-rw-r--r--   0 elliotglas   (501) staff       (20)       53 2023-07-21 10:04:23.000000 st_track_analysis-0.0.3/MANIFEST.in
+-rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 18:33:58.790805 st_track_analysis-0.0.3/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 18:33:58.791141 st_track_analysis-0.0.3/setup.cfg
+-rw-r--r--   0 elliotglas   (501) staff       (20)      663 2023-07-21 18:33:56.000000 st_track_analysis-0.0.3/setup.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.783213 st_track_analysis-0.0.3/st_track_analysis/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2873 2023-07-21 18:12:54.000000 st_track_analysis-0.0.3/st_track_analysis/__init__.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.782118 st_track_analysis-0.0.3/st_track_analysis/frontend/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.785098 st_track_analysis-0.0.3/st_track_analysis/frontend/build/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      879 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/asset-manifest.json
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2186 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/index.html
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.782409 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.785847 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/css/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      840 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1567 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.790547 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   982743 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)  4039604 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)    11378 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/main.56720d29.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)    40929 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/main.56720d29.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 18:33:18.000000 st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 18:33:58.784562 st_track_analysis-0.0.3/st_track_analysis.egg-info/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      292 2023-07-21 18:33:58.000000 st_track_analysis-0.0.3/st_track_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)      980 2023-07-21 18:33:58.000000 st_track_analysis-0.0.3/st_track_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 18:33:58.000000 st_track_analysis-0.0.3/st_track_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 18:33:58.000000 st_track_analysis-0.0.3/st_track_analysis.egg-info/requires.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       18 2023-07-21 18:33:58.000000 st_track_analysis-0.0.3/st_track_analysis.egg-info/top_level.txt
```

### Comparing `st_track_analysis-0.0.2/LICENSE` & `st_track_analysis-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/setup.py` & `st_track_analysis-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_track_analysis",
-    version="0.0.2",
+    version="0.0.3",
     author="Elliot Glas",
     author_email="elliot.glas@viscando.com",
     description="A tool to view tracks on an image",
     long_description="A tool to view tracks on an image",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_track_analysis-0.0.2/st_track_analysis/__init__.py` & `st_track_analysis-0.0.3/st_track_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/asset-manifest.json` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/asset-manifest.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'entrypoints'": "{insert: [(3, 'static/js/main.56720d29.chunk.js')], delete: [3]}",*

 * * "'files'": "{'main.js': './static/js/main.56720d29.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.56720d29.chunk.js.map'}"}*

```diff
@@ -1,19 +1,19 @@
 {
     "entrypoints": [
         "static/js/runtime-main.657b0728.js",
         "static/js/2.2edeab5c.chunk.js",
         "static/css/main.22919367.chunk.css",
-        "static/js/main.070b89e3.chunk.js"
+        "static/js/main.56720d29.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.22919367.chunk.css",
-        "main.js": "./static/js/main.070b89e3.chunk.js",
-        "main.js.map": "./static/js/main.070b89e3.chunk.js.map",
+        "main.js": "./static/js/main.56720d29.chunk.js",
+        "main.js.map": "./static/js/main.56720d29.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.657b0728.js",
         "runtime-main.js.map": "./static/js/runtime-main.657b0728.js.map",
         "static/css/main.22919367.chunk.css.map": "./static/css/main.22919367.chunk.css.map",
         "static/js/2.2edeab5c.chunk.js": "./static/js/2.2edeab5c.chunk.js",
         "static/js/2.2edeab5c.chunk.js.LICENSE.txt": "./static/js/2.2edeab5c.chunk.js.LICENSE.txt",
         "static/js/2.2edeab5c.chunk.js.map": "./static/js/2.2edeab5c.chunk.js.map"
     }
```

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/index.html` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style><link href="./static/css/main.22919367.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.2edeab5c.chunk.js"></script><script src="./static/js/main.070b89e3.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style><link href="./static/css/main.22919367.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.2edeab5c.chunk.js"></script><script src="./static/js/main.56720d29.chunk.js"></script></body></html>
```

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/main.56720d29.chunk.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -8,39 +8,45 @@
                 r = a.n(n),
                 c = a(46),
                 i = a.n(c),
                 o = a(96),
                 s = a(9),
                 l = a(19),
                 d = (a(196), a(25)),
-                u = ["red", "purple", "cyan", "green", "pink"],
+                u = new Map([
+                    [0, "green"],
+                    [1, "purple"],
+                    [4, "red"],
+                    [18, "cyan"],
+                    [34, "pink"]
+                ]),
                 j = ["Pedestrian", "Bicycle", "Light vehicle", "Heavy vehicle", "Unknown"];
 
-            function h(e, t, a, n, r, c) {
+            function b(e, t, a, n, r, c) {
                 var i, o = new Map,
                     l = Object(d.a)(e);
                 try {
                     for (l.s(); !(i = l.n()).done;) {
                         var u = Object(s.a)(i.value, 5),
-                            h = u[0],
-                            b = u[1],
+                            b = u[0],
+                            h = u[1],
                             m = u[2],
                             g = u[3],
                             f = u[4];
                         if (a.onlyConfirmed && 1 === f || -1 === t.indexOf(j[g]));
-                        else if (o.has(h)) {
-                            var O = o.get(h),
+                        else if (o.has(b)) {
+                            var O = o.get(b),
                                 x = Object(s.a)(O, 5),
                                 p = x[0],
-                                v = x[1],
-                                k = (x[2], x[3], x[4]);
-                            p.push(20 * b + 280), v.push(20 * m + 300), k.push(f)
-                        } else o.set(h, [
-                            [20 * b + 280],
-                            [20 * m + 300], g, h, [f]
+                                k = x[1],
+                                v = (x[2], x[3], x[4]);
+                            p.push(20 * h + 280), k.push(20 * m + 300), v.push(f)
+                        } else o.set(b, [
+                            [20 * h + 280],
+                            [20 * m + 300], g, b, [f]
                         ])
                     }
                 } catch (y) {
                     l.e(y)
                 } finally {
                     l.f()
                 }
@@ -60,65 +66,66 @@
                                 var i = l[n],
                                     o = "L ".concat(e, " ").concat(c[n]);
                                 if ((t && 0 === i || a && 1 === i && 0 !== n) && 0 !== n) {
                                     var s = 0 === i ? 6 : 3,
                                         d = [r[n - 1], c[n - 1]],
                                         u = d[0],
                                         j = d[1],
-                                        h = [e, c[n]],
-                                        b = h[0],
-                                        m = h[1],
-                                        g = Math.sqrt(Math.pow(b - u, 2) + Math.pow(m - j, 2)),
-                                        f = [(j - m) / g, (b - u) / g],
+                                        b = [e, c[n]],
+                                        h = b[0],
+                                        m = b[1],
+                                        g = Math.sqrt(Math.pow(h - u, 2) + Math.pow(m - j, 2)),
+                                        f = [(j - m) / g, (h - u) / g],
                                         O = .707,
                                         x = f[0] * O - f[1] * O,
                                         p = f[0] * O + f[1] * O;
                                     o += "L ".concat(e + x * s, " ").concat(c[n] + p * s, " L ").concat(e, " ").concat(c[n], " L ").concat(e - p * s, " ").concat(c[n] + x * s, " L ").concat(e, " ").concat(c[n])
                                 }
                                 return o
                             })).join(" ");
                         return ["M ".concat(r[0], " ").concat(c[0], " ").concat(j), i, o, d, u]
                     }(e, a.markMeasurements, a.markEstimated)
                 }))
             }
-            var b = a(2),
+            var h = a(2),
                 m = function(e) {
                     var t = e.WIDTH,
                         a = e.HEIGHT,
                         n = e.scale,
                         r = e.pathStrings,
                         c = e.showId,
                         i = e.selectedIndices,
                         o = e.vertices;
-                    return Object(b.jsxs)("svg", {
+                    return Object(h.jsxs)("svg", {
                         width: t * n,
                         height: a * n,
                         style: {
                             transform: "scale(".concat(n, ")"),
                             transformOrigin: "top left"
                         },
                         children: [r.map((function(e, t) {
-                            return i.has(t) ? Object(b.jsx)(b.Fragment, {}) : Object(b.jsxs)("g", {
-                                children: [Object(b.jsx)("path", {
+                            var a = u.get(e[1]);
+                            return i.has(t) ? Object(h.jsx)(h.Fragment, {}) : Object(h.jsxs)("g", {
+                                children: [Object(h.jsx)("path", {
                                     d: e[0],
-                                    stroke: u[e[1]],
+                                    stroke: a || "black",
                                     fill: "none"
-                                }), Object(b.jsx)("circle", {
+                                }), Object(h.jsx)("circle", {
                                     cx: e[3][0],
                                     cy: e[3][1],
                                     r: 4,
                                     fill: "green",
                                     strokeWidth: "4"
-                                }), Object(b.jsx)("circle", {
+                                }), Object(h.jsx)("circle", {
                                     cx: e[4][0],
                                     cy: e[4][1],
                                     r: 4,
                                     fill: "red",
                                     strokeWidth: "4"
-                                }), c && Object(b.jsx)("text", {
+                                }), c && Object(h.jsx)("text", {
                                     x: e[4][0],
                                     y: e[4][1],
                                     fill: "white",
                                     fontFamily: "sans-serif",
                                     fontSize: 10,
                                     children: e[2]
                                 })]
@@ -127,208 +134,207 @@
                     })
                 },
                 g = a(139),
                 f = a.n(g),
                 O = a(268),
                 x = a(270),
                 p = a(292),
-                v = a(307),
-                k = a(308),
+                k = a(307),
+                v = a(308),
                 y = a(273),
                 w = a(309),
                 C = a(310),
                 L = a(311),
                 M = a(294),
                 S = function(e) {
                     e.label;
-                    var t = e.image,
-                        a = e.WIDTH,
-                        r = e.HEIGHT,
-                        c = e.tracks,
-                        i = e.from,
-                        o = e.to,
-                        d = e.showType,
-                        u = e.filterLength,
-                        j = e.minLength,
-                        g = e.maxLength,
-                        S = Object(n.useState)(1),
-                        T = Object(s.a)(S, 2),
-                        I = T[0],
-                        D = T[1],
-                        F = Object(n.useState)({
+                    var t, a = e.image,
+                        r = e.WIDTH,
+                        c = e.HEIGHT,
+                        i = e.tracks,
+                        o = e.from,
+                        d = e.to,
+                        u = e.showType,
+                        j = e.filterLength,
+                        g = e.minLength,
+                        S = e.maxLength,
+                        T = Object(n.useState)(1),
+                        I = Object(s.a)(T, 2),
+                        D = I[0],
+                        F = I[1],
+                        H = Object(n.useState)({
                             markMeasurements: !1,
                             markEstimated: !1,
                             onlyConfirmed: !1,
                             trackId: !1,
                             showLines: !1
                         }),
-                        H = Object(s.a)(F, 2),
-                        E = H[0],
-                        N = H[1],
-                        R = Object(n.useState)(new Map),
-                        W = Object(s.a)(R, 2),
-                        Y = W[0],
-                        B = W[1],
-                        P = Object(n.useMemo)((function() {
-                            return h(c.slice(i, o), d, E, u, j, g)
-                        }), [i, o, d, E, u, j, g]),
-                        A = Object(b.jsx)(m, {
-                            WIDTH: a,
-                            HEIGHT: r,
-                            scale: I,
-                            pathStrings: P,
-                            showId: E.trackId,
-                            selectedIndices: Y,
+                        E = Object(s.a)(H, 2),
+                        N = E[0],
+                        R = E[1],
+                        W = Object(n.useState)(new Map),
+                        Y = Object(s.a)(W, 2),
+                        B = Y[0],
+                        P = Y[1],
+                        A = Object(n.useMemo)((function() {
+                            return b(i.slice(o, d), u, N, j, g, S)
+                        }), [o, d, u, N, j, g, S]),
+                        G = Object(h.jsx)(m, {
+                            WIDTH: r,
+                            HEIGHT: c,
+                            scale: D,
+                            pathStrings: A,
+                            showId: N.trackId,
+                            selectedIndices: B,
                             vertices: []
                         });
-                    var G;
-                    return Object(b.jsxs)("div", {
-                        children: [Object(b.jsx)("div", {
+                    return Object(h.jsxs)("div", {
+                        children: [Object(h.jsx)("div", {
                             className: "control-container",
-                            children: Object(b.jsx)(p.a, {
-                                value: I,
+                            children: Object(h.jsx)(p.a, {
+                                value: D,
                                 "aria-label": "Default",
                                 valueLabelDisplay: "auto",
                                 onChange: function(e, t) {
-                                    "number" === typeof t && D(t)
+                                    "number" === typeof t && F(t)
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
-                        }), Object(b.jsxs)("div", {
+                        }), Object(h.jsxs)("div", {
                             style: {
                                 overflow: "hidden",
                                 display: "flex"
                             },
-                            children: [Object(b.jsxs)("div", {
+                            children: [Object(h.jsxs)("div", {
                                 style: {
                                     display: "flex",
                                     flexDirection: "column"
                                 },
-                                children: [Object(b.jsx)(f.a, {
-                                    children: Object(b.jsx)("div", {
+                                children: [Object(h.jsx)(f.a, {
+                                    children: Object(h.jsx)("div", {
                                         className: "image-container",
                                         style: {
-                                            width: a * I,
-                                            height: r * I,
-                                            backgroundImage: "url(".concat(t, ")")
+                                            width: r * D,
+                                            height: c * D,
+                                            backgroundImage: "url(".concat(a, ")")
                                         },
-                                        children: A
+                                        children: G
                                     })
-                                }), Object(b.jsx)("div", {
+                                }), Object(h.jsx)("div", {
                                     style: {
                                         marginTop: 10
                                     },
-                                    children: Object(b.jsxs)(v.a, {
+                                    children: Object(h.jsxs)(k.a, {
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
-                                        subheader: Object(b.jsx)(k.a, {
+                                        subheader: Object(h.jsx)(v.a, {
                                             children: "Tracks"
                                         }),
                                         component: "nav",
                                         "aria-label": "main mailbox folders",
-                                        children: [Object(b.jsx)(y.a, {}), (G = P, G.map((function(e, t) {
-                                            return Object(b.jsxs)(O.a, {
-                                                selected: Y.has(t),
+                                        children: [Object(h.jsx)(y.a, {}), (t = A, t.map((function(e, t) {
+                                            return Object(h.jsxs)(O.a, {
+                                                selected: B.has(t),
                                                 onClick: function(e) {
-                                                    Y.has(t) ? B((function(e) {
+                                                    B.has(t) ? P((function(e) {
                                                         return e.delete(t), new Map(e)
                                                     })) : function(e, t) {
-                                                        B((function(e) {
+                                                        P((function(e) {
                                                             return new Map(e.set(t, !0))
                                                         }))
                                                     }(0, t)
                                                 },
-                                                children: [Object(b.jsx)(x.a, {
+                                                children: [Object(h.jsx)(x.a, {
                                                     primary: e[2]
-                                                }), Object(b.jsx)(x.a, {
+                                                }), Object(h.jsx)(x.a, {
                                                     primary: e[1]
                                                 })]
                                             }, t)
                                         })))]
                                     })
                                 })]
-                            }), Object(b.jsx)(w.a, {
+                            }), Object(h.jsx)(w.a, {
                                 sx: {
                                     margin: 0,
                                     marginLeft: 2
                                 },
                                 component: "fieldset",
                                 variant: "standard",
-                                children: Object(b.jsxs)(C.a, {
-                                    children: [Object(b.jsx)(L.a, {
-                                        control: Object(b.jsx)(M.a, {
-                                            checked: E.markMeasurements,
+                                children: Object(h.jsxs)(C.a, {
+                                    children: [Object(h.jsx)(L.a, {
+                                        control: Object(h.jsx)(M.a, {
+                                            checked: N.markMeasurements,
                                             onChange: function(e) {
-                                                N((function(t) {
+                                                R((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         markMeasurements: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Mark measurments"
-                                    }), Object(b.jsx)(L.a, {
-                                        control: Object(b.jsx)(M.a, {
-                                            checked: E.markEstimated,
+                                    }), Object(h.jsx)(L.a, {
+                                        control: Object(h.jsx)(M.a, {
+                                            checked: N.markEstimated,
                                             onChange: function(e) {
-                                                N((function(t) {
+                                                R((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         markEstimated: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Mark estimated"
-                                    }), Object(b.jsx)(L.a, {
-                                        control: Object(b.jsx)(M.a, {
-                                            checked: E.onlyConfirmed,
+                                    }), Object(h.jsx)(L.a, {
+                                        control: Object(h.jsx)(M.a, {
+                                            checked: N.onlyConfirmed,
                                             onChange: function(e) {
-                                                N((function(t) {
+                                                R((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         onlyConfirmed: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Show only confirmed"
-                                    }), Object(b.jsx)(L.a, {
-                                        control: Object(b.jsx)(M.a, {
-                                            checked: E.trackId,
+                                    }), Object(h.jsx)(L.a, {
+                                        control: Object(h.jsx)(M.a, {
+                                            checked: N.trackId,
                                             onChange: function(e) {
-                                                N((function(t) {
+                                                R((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         trackId: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Show track id"
-                                    }), Object(b.jsx)(L.a, {
-                                        control: Object(b.jsx)(M.a, {
-                                            checked: E.showLines,
+                                    }), Object(h.jsx)(L.a, {
+                                        control: Object(h.jsx)(M.a, {
+                                            checked: N.showLines,
                                             onChange: function(e) {
-                                                N((function(t) {
+                                                R((function(t) {
                                                     return Object(l.a)(Object(l.a)({}, t), {}, {
                                                         showLines: e.target.checked
                                                     })
                                                 }))
                                             }
                                         }),
                                         label: "Show lines"
@@ -359,127 +365,127 @@
                         c = e.setToTime,
                         i = e.interval,
                         o = e.setDir,
                         s = e.setInterval,
                         l = e.showType,
                         d = e.handleChange,
                         u = e.filterLength,
-                        h = e.setFilterLength,
+                        b = e.setFilterLength,
                         m = e.minLength,
                         g = e.setMinLength,
                         f = e.maxLength,
                         O = e.setMaxLength,
                         p = e.handleBackwardClick,
-                        v = e.handleForwardClick,
-                        k = {
+                        k = e.handleForwardClick,
+                        v = {
                             PaperProps: {
                                 style: {
                                     maxHeight: 224,
                                     width: 250
                                 }
                             }
                         };
-                    return console.log(l), Object(b.jsxs)("div", {
-                        children: [Object(b.jsxs)(Y.a, {
+                    return console.log(l), Object(h.jsxs)("div", {
+                        children: [Object(h.jsxs)(Y.a, {
                             dateAdapter: A.a,
-                            children: [Object(b.jsx)(B.a, {
+                            children: [Object(h.jsx)(B.a, {
                                 label: "Date",
                                 format: "YYYY-MM-DD",
                                 value: t,
                                 onChange: function(e) {
                                     e && a(e)
                                 },
                                 sx: {
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
                                     marginRight: 2
                                 }
-                            }), Object(b.jsx)(P.a, {
+                            }), Object(h.jsx)(P.a, {
                                 label: "From time",
                                 value: n,
                                 onChange: function(e) {
                                     e && (r(e), c(e.add(i, "minutes")), o(0))
                                 },
                                 ampm: !1,
                                 sx: {
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
                                     marginRight: 2
                                 }
                             })]
-                        }), Object(b.jsx)(F.a, {
+                        }), Object(h.jsx)(F.a, {
                             label: "Interval in minutes",
                             id: "outlined-start-adornment",
                             sx: {
                                 width: "25ch",
                                 backgroundColor: "background.default",
                                 borderRadius: 1,
                                 margin: 0,
                                 marginRight: 2
                             },
                             value: i,
                             onChange: function(e) {
                                 var t = Number(e.target.value);
                                 isNaN(t) || (s(t), c(n.add(t, "minutes")))
                             }
-                        }), Object(b.jsxs)(w.a, {
+                        }), Object(h.jsxs)(w.a, {
                             sx: {
                                 m: 1,
                                 width: 300,
                                 margin: 0
                             },
-                            children: [Object(b.jsx)(H.a, {
+                            children: [Object(h.jsx)(H.a, {
                                 id: "demo-multiple-name-label",
                                 children: "Show types"
-                            }), Object(b.jsx)(E.a, {
+                            }), Object(h.jsx)(E.a, {
                                 labelId: "demo-multiple-name-label",
                                 id: "demo-multiple-name",
                                 multiple: !0,
                                 value: l,
                                 onChange: d,
-                                input: Object(b.jsx)(N.a, {
+                                input: Object(h.jsx)(N.a, {
                                     label: "Show types"
                                 }),
                                 renderValue: function(e) {
                                     return e.join(", ")
                                 },
-                                MenuProps: k,
+                                MenuProps: v,
                                 sx: {
                                     backgroundColor: "background.default"
                                 },
                                 children: j.map((function(e) {
-                                    return Object(b.jsxs)(R.a, {
+                                    return Object(h.jsxs)(R.a, {
                                         value: e,
-                                        children: [Object(b.jsx)(M.a, {
+                                        children: [Object(h.jsx)(M.a, {
                                             checked: l.indexOf(e) > -1
-                                        }), Object(b.jsx)(x.a, {
+                                        }), Object(h.jsx)(x.a, {
                                             primary: e
                                         })]
                                     }, e)
                                 }))
                             })]
-                        }), Object(b.jsx)("div", {
-                            children: Object(b.jsx)(L.a, {
-                                control: Object(b.jsx)(M.a, {
+                        }), Object(h.jsx)("div", {
+                            children: Object(h.jsx)(L.a, {
+                                control: Object(h.jsx)(M.a, {
                                     checked: u,
                                     onChange: function(e) {
-                                        h(e.target.checked)
+                                        b(e.target.checked)
                                     }
                                 }),
                                 label: "Filter length",
                                 style: {
                                     margin: 0,
                                     marginTop: 10
                                 }
                             })
-                        }), u && Object(b.jsxs)("div", {
+                        }), u && Object(h.jsxs)("div", {
                             style: {
                                 marginTop: 10
                             },
-                            children: [Object(b.jsx)(F.a, {
+                            children: [Object(h.jsx)(F.a, {
                                 label: "Minimum length",
                                 id: "outlined-start-adornment",
                                 sx: {
                                     m: 1,
                                     width: "25ch",
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
@@ -487,15 +493,15 @@
                                     marginRight: 2
                                 },
                                 value: m,
                                 onChange: function(e) {
                                     var t = Number(e.target.value);
                                     isNaN(t) || g(t)
                                 }
-                            }), Object(b.jsx)(F.a, {
+                            }), Object(h.jsx)(F.a, {
                                 label: "Maximum length",
                                 id: "outlined-start-adornment",
                                 sx: {
                                     m: 1,
                                     width: "25ch",
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
@@ -504,35 +510,35 @@
                                 },
                                 value: f,
                                 onChange: function(e) {
                                     var t = Number(e.target.value);
                                     isNaN(t) || O(t)
                                 }
                             })]
-                        }), Object(b.jsxs)("div", {
+                        }), Object(h.jsxs)("div", {
                             style: {
                                 margin: 0,
                                 marginTop: 10
                             },
-                            children: [Object(b.jsx)(W.a, {
+                            children: [Object(h.jsx)(W.a, {
                                 sx: {
                                     marginRight: 2,
                                     backgroundColor: "background.default"
                                 },
                                 onClick: function() {
                                     return p()
                                 },
                                 children: "<"
-                            }), Object(b.jsx)(W.a, {
+                            }), Object(h.jsx)(W.a, {
                                 sx: {
                                     marginRight: 2,
                                     backgroundColor: "background.default"
                                 },
                                 onClick: function() {
-                                    return v()
+                                    return k()
                                 },
                                 children: ">"
                             })]
                         })]
                     })
                 },
                 V = function() {
@@ -540,23 +546,23 @@
                         t = Object(n.useState)(0),
                         a = Object(s.a)(t, 2),
                         c = a[0],
                         i = a[1],
                         l = Object(n.useState)(0),
                         d = Object(s.a)(l, 2),
                         u = d[0],
-                        h = d[1],
+                        b = d[1],
                         m = Object(n.useState)(0),
                         g = Object(s.a)(m, 2),
                         f = g[0],
                         O = g[1],
                         x = Object(n.useState)(I()(e.args.date)),
                         p = Object(s.a)(x, 2),
-                        v = p[0],
-                        k = p[1],
+                        k = p[0],
+                        v = p[1],
                         y = Object(n.useState)(I()(e.args.date)),
                         w = Object(s.a)(y, 2),
                         C = w[0],
                         L = w[1],
                         M = Object(n.useState)(I()(e.args.date)),
                         T = Object(s.a)(M, 2),
                         F = T[0],
@@ -584,63 +590,63 @@
                         te = Object(n.useState)(e.args.tracks),
                         ae = Object(s.a)(te, 2),
                         ne = ae[0],
                         re = (ae[1], e.args.image),
                         ce = e.args.height,
                         ie = e.args.width;
                     Object(n.useEffect)((function() {
-                        v.isValid() && D.Streamlit.setComponentValue(v.format("YYYY-MM-DD"))
-                    }), [v]), Object(n.useEffect)((function() {
+                        k.isValid() && D.Streamlit.setComponentValue(k.format("YYYY-MM-DD"))
+                    }), [k]), Object(n.useEffect)((function() {
                         ! function() {
                             var e, t;
                             if (0 === f) e = oe(C, 0, ne.length - 1), t = oe(F, 0, ne.length - 1);
                             else if (1 === f) {
                                 var a = e = u + 1;
                                 for (console.log("INDEX:", a, ne.length - 1, a < ne.length - 1); a < ne.length && I()(ne[a][5]).isBefore(F);) a++;
                                 t = a
                             } else {
                                 var n = t = c;
                                 for (console.log("INDEX:", n, ne.length); n > 0 && n < ne.length && C.isBefore(I()(ne[n][5]));) n--;
                                 e = n + 1
                             }
-                            i(e), h(t), console.log("First track:", ne[e]), console.log("Last track", ne[t - 1]), console.log("From ".concat(e, " to ").concat(t))
+                            i(e), b(t), console.log("First track:", ne[e]), console.log("Last track", ne[t - 1]), console.log("From ".concat(e, " to ").concat(t))
                         }()
                     }), [C, F]);
 
                     function oe(e, t, a) {
                         for (; t < a;) {
                             var n = Math.floor(t + a >>> 1);
                             if (0 === n) return 0;
                             var r = I()(ne[n][5]);
                             if (r.isAfter(e) && I()(ne[n - 1][5]).isBefore(e)) return n;
                             r.isAfter(e) ? a = n : t = n + 1
                         }
                         return t
                     }
-                    var se = [Object(b.jsx)(S, {
+                    var se = [Object(h.jsx)(S, {
                         image: re,
                         WIDTH: ie,
                         HEIGHT: ce,
                         tracks: ne,
                         from: c,
                         to: u,
                         label: "Version 1",
                         showType: P,
                         filterLength: J,
                         minLength: U,
                         maxLength: $
                     })];
-                    return Object(b.jsxs)("div", {
+                    return Object(h.jsxs)("div", {
                         style: {
                             flexDirection: "column",
                             marginTop: 30
                         },
-                        children: [Object(b.jsx)(G, {
-                            date: v,
-                            setDate: k,
+                        children: [Object(h.jsx)(G, {
+                            date: k,
+                            setDate: v,
                             fromTime: C,
                             setFromTime: L,
                             setToTime: H,
                             interval: R,
                             setDir: O,
                             setInterval: W,
                             showType: P,
@@ -664,27 +670,27 @@
                             handleForwardClick: function() {
                                 L((function(e) {
                                     return e.add(R, "minutes")
                                 })), H((function(e) {
                                     return e.add(R, "minutes")
                                 })), O(1)
                             }
-                        }), Object(b.jsx)("div", {
+                        }), Object(h.jsx)("div", {
                             style: {
                                 display: "flex",
                                 flexDirection: "row"
                             },
-                            children: Object(b.jsxs)("div", {
+                            children: Object(h.jsxs)("div", {
                                 style: {
                                     flexDirection: "row",
                                     flexWrap: "wrap"
                                 },
                                 children: [se.map((function(e) {
                                     return e
-                                })), Object(b.jsx)("div", {
+                                })), Object(h.jsx)("div", {
                                     style: {
                                         height: 1e4
                                     }
                                 })]
                             })
                         })]
                     })
@@ -712,22 +718,22 @@
                     },
                     background: {
                         default: "#262730",
                         paper: "#262730"
                     }
                 }
             });
-            i.a.render(Object(b.jsx)(r.a.StrictMode, {
-                children: Object(b.jsx)(o.StreamlitProvider, {
-                    children: Object(b.jsx)(J.a, {
+            i.a.render(Object(h.jsx)(r.a.StrictMode, {
+                children: Object(h.jsx)(o.StreamlitProvider, {
+                    children: Object(h.jsx)(J.a, {
                         theme: X,
-                        children: Object(b.jsx)(V, {})
+                        children: Object(h.jsx)(V, {})
                     })
                 })
             }), document.getElementById("root"))
         }
     },
     [
         [203, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.070b89e3.chunk.js.map
+//# sourceMappingURL=main.56720d29.chunk.js.map
```

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js.map` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/main.56720d29.chunk.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8037370792472833%*

 * *Differences: {"'file'": "'static/js/main.56720d29.chunk.js'",*

 * * "'mappings'": "'wPAAaA,EAA8B,IAAIC,IAAI,CACjD,CAAC,EAAG,SACJ,CAAC,EAAG,UACJ,CAAC,EAAG,OACJ,CAAC,GAAI,QACL,CAAC,GAAI,UAEMC,EAAQ,CACnB,aACA,UACA,gBACA,gBACA,WCJK,SAASC,EACdC,EACAC,EACAC,EACAC,EACAC,EACAC,GAEA,IACiDC,EAD3CC,EAAW,IAAIV,IAA4BW,EAAAC,YACPT,GAAO,IAAjD,IAAAQ,EAAAE,MAAAJ,EAAAE,EAAAG,KAAAC,MAAmD,CAAC,IAADC,EAAAC,YAAAR,EAAAS,MAAA,GAAvCC,EAAEH,EAAA,GAAEI,EAACJ,EAAA,GAAEK,EAACL,EAAA,GAAEM,EAAIN,EAAA,GAAEO,EAASP,EAAA,GACnC,GACGX,EAAQmB,eAA+B,IAAdD,IACS,IA […]*

```diff
@@ -1,23 +1,23 @@
 {
-    "file": "static/js/main.070b89e3.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.56720d29.chunk.js",
+    "mappings": "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",
     "names": [
         "colors",
+        "Map",
         "names",
         "pathStrings",
         "entries",
         "showType",
         "filters",
         "filterLength",
         "minLength",
         "maxLength",
         "_step",
         "trackMap",
-        "Map",
         "_iterator",
         "_createForOfIteratorHelper",
         "s",
         "n",
         "done",
         "_step$value",
         "_slicedToArray",
@@ -91,27 +91,29 @@
         "height",
         "style",
         "transform",
         "transformOrigin",
         "children",
         "path",
         "index",
+        "color",
         "_jsx",
         "_Fragment",
         "d",
         "stroke",
         "fill",
         "cx",
         "cy",
         "r",
         "strokeWidth",
         "fontFamily",
         "fontSize",
         "SourcePlotter",
         "label",
+        "rows",
         "image",
         "tracks",
         "to",
         "_useState",
         "useState",
         "_useState2",
         "setScale",
@@ -123,25 +125,23 @@
         "_useState5",
         "_useState6",
         "setSelectedIndices",
         "paths",
         "useMemo",
         "slice",
         "SVGLines",
-        "rows",
         "className",
         "Slider",
         "valueLabelDisplay",
         "onChange",
         "event",
         "newValue",
         "min",
         "max",
         "step",
-        "color",
         "margin",
         "overflow",
         "display",
         "flexDirection",
         "Draggable",
         "backgroundImage",
         "marginTop",
@@ -301,17 +301,17 @@
         "components/plotter/Lines.tsx",
         "components/plotter/SourcePlotter.tsx",
         "components/plotter/header/Header.tsx",
         "components/plotter/TrackAnalysis.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "export const colors = [\"red\", \"purple\", \"cyan\", \"green\", \"pink\"]\nexport const names = [\n  \"Pedestrian\",\n  \"Bicycle\",\n  \"Light vehicle\",\n  \"Heavy vehicle\",\n  \"Unknown\",\n]\n",
-        "import { Pos, TransformMatrix, transformPos } from \"./Matrix\"\nimport { names } from \"./consts\"\nimport { Show } from \"./types\"\n\nexport type Track = [number, number, number, number, number, string]\nexport type Path = [string, number, number, Pos, Pos]\ntype InternalTrack = [number[], number[], number, number, number[]]\n\nexport function pathStrings(\n  entries: Track[],\n  showType: string[],\n  filters: Show,\n  filterLength: boolean,\n  minLength: number,\n  maxLength: number\n): Path[] {\n  const trackMap = new Map<number, InternalTrack>()\n  for (const [id, x, y, type, estimated] of entries) {\n    if (\n      (filters.onlyConfirmed && estimated === 1) ||\n      showType.indexOf(names[type]) === -1\n    ) {\n    } else {\n      if (trackMap.has(id)) {\n        const [\n          xCoordinates,\n          yCoordinates,\n          existingType,\n          existingId,\n          estimates,\n        ] = trackMap.get(id)!\n        xCoordinates.push(x * 20 + 280)\n        yCoordinates.push(y * 20 + 300)\n        estimates.push(estimated)\n      } else {\n        trackMap.set(id, [\n          [x * 20 + 280],\n          [y * 20 + 300],\n          type,\n          id,\n          [estimated],\n        ])\n      }\n    }\n  }\n\n  trackMap.forEach((track, key) => {\n    if (\n      filterLength &&\n      (track[0].length < minLength || track[0].length > maxLength)\n    ) {\n      trackMap.delete(key)\n    }\n  })\n\n  return Array.from(trackMap.values(), (track) =>\n    createPath(track, filters.markMeasurements, filters.markEstimated)\n  )\n}\n\nfunction createPath(\n  track: InternalTrack,\n  markMeasured: boolean,\n  markEstimates: boolean\n): Path {\n  {\n    const [xs, ys, type, id, estimates] = track\n    const startPos: Pos = [xs[0], ys[0], 0]\n    const endPos: Pos = [xs[xs.length - 1], ys[ys.length - 1], 0]\n    const pathData = xs\n      .map((x, i) => {\n        const estimated = estimates[i]\n        let pathSegment = `L ${x} ${ys[i]}`\n        if (\n          ((markMeasured && estimated === 0) ||\n            (markEstimates && estimated === 1 && i !== 0)) &&\n          i !== 0\n        ) {\n          const size = estimated === 0 ? 6 : 3\n          const [x1, y1] = [xs[i - 1], ys[i - 1]]\n          const [x2, y2] = [x, ys[i]]\n          const length = Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2))\n          const perpendicularDir = [(y1 - y2) / length, (x2 - x1) / length]\n          const angle = 0.707\n          const offsetX =\n            perpendicularDir[0] * angle - perpendicularDir[1] * angle\n          const offsetY =\n            perpendicularDir[0] * angle + perpendicularDir[1] * angle\n          pathSegment += `L ${x + offsetX * size} ${\n            ys[i] + offsetY * size\n          } L ${x} ${ys[i]} L ${x - offsetY * size} ${\n            ys[i] + offsetX * size\n          } L ${x} ${ys[i]}`\n        }\n        return pathSegment\n      })\n      .join(\" \")\n    const pathString = `M ${xs[0]} ${ys[0]} ${pathData}`\n    return [pathString, type, id, startPos, endPos]\n  }\n}\n",
-        "import React from \"react\"\nimport { colors } from \"../../helpers/consts\"\nimport { Path } from \"../../helpers/Paths\"\n\ntype LinesProps = {\n  WIDTH: number\n  HEIGHT: number\n  scale: number\n  pathStrings: Path[]\n  showId: boolean\n  selectedIndices: Map<number, boolean>\n  vertices: JSX.Element[]\n}\n\nexport const Lines: React.FC<LinesProps> = ({\n  WIDTH,\n  HEIGHT,\n  scale,\n  pathStrings,\n  showId,\n  selectedIndices,\n  vertices,\n}) => {\n  return (\n    <svg\n      width={WIDTH * scale}\n      height={HEIGHT * scale}\n      style={{\n        transform: `scale(${scale})`,\n        transformOrigin: \"top left\", // Set the transformation origin\n      }}\n    >\n      {pathStrings.map((path, index) => {\n        /**\n         * The strings are of the format \"...L {x-ending point} {y-ending point},\n         * we want to get these coordinates to display the starting ids above\n         * the ending point\"\n         */\n        return !selectedIndices.has(index) ? (\n          <g key={path[0]}>\n            <path d={path[0]} stroke={colors[path[1]]} fill=\"none\" />\n            <circle\n              cx={path[3][0]}\n              cy={path[3][1]}\n              r={4}\n              fill=\"green\"\n              strokeWidth=\"4\"\n            />\n            <circle\n              cx={path[4][0]}\n              cy={path[4][1]}\n              r={4}\n              fill=\"red\"\n              strokeWidth=\"4\"\n            />\n            {showId && (\n              <text\n                x={path[4][0]}\n                y={path[4][1]}\n                fill=\"white\"\n                fontFamily=\"sans-serif\"\n                fontSize={10}\n              >\n                {path[2]}\n              </text>\n            )}\n          </g>\n        ) : (\n          <></>\n        )\n      })}\n      {vertices}\n    </svg>\n  )\n}\n",
-        "import React, { useState, useMemo } from \"react\"\nimport { TransformMatrix } from \"../../helpers/Matrix\"\nimport \"../../styles/styles.css\"\nimport { Path, Track, pathStrings } from \"../../helpers/Paths\"\nimport { Lines } from \"./Lines\"\nimport Draggable from \"react-draggable\"\nimport {\n  Box,\n  Checkbox,\n  Divider,\n  FormControl,\n  FormControlLabel,\n  FormGroup,\n  List,\n  ListItemButton,\n  ListItemIcon,\n  ListItemText,\n  ListSubheader,\n  Slider,\n} from \"@mui/material\"\nimport { Show } from \"../../helpers/types\"\n\ninterface SourcePlotterProps {\n  label: string\n  image: string\n  WIDTH: number\n  HEIGHT: number\n  filterLength: boolean\n  minLength: number\n  maxLength: number\n  tracks: Track[]\n  from: number\n  to: number\n  showType: string[]\n}\n\nconst SourcePlotter: React.FC<SourcePlotterProps> = ({\n  label,\n  image,\n  WIDTH,\n  HEIGHT,\n  tracks,\n  from,\n  to,\n  showType,\n  filterLength,\n  minLength,\n  maxLength,\n}) => {\n  const [scale, setScale] = useState<number>(1)\n  const [filters, setFilters] = useState<Show>({\n    markMeasurements: false,\n    markEstimated: false,\n    onlyConfirmed: false,\n    trackId: false,\n    showLines: false,\n  })\n  const [selectedIndices, setSelectedIndices] = useState<Map<number, boolean>>(\n    new Map()\n  )\n  /**\n   * Memoize the lines so we don't recalculate pathStrings everytime\n   * we rerender this component\n   */\n  const paths = useMemo(() => {\n    return pathStrings(\n      tracks.slice(from, to),\n      showType,\n      filters,\n      filterLength,\n      minLength,\n      maxLength\n    )\n  }, [from, to, showType, filters, filterLength, minLength, maxLength])\n\n  const handleSliderChange = (event: Event, newValue: number | number[]) => {\n    if (typeof newValue === \"number\") {\n      setScale(newValue)\n    }\n  }\n\n  const SVGLines = (\n    <Lines\n      WIDTH={WIDTH}\n      HEIGHT={HEIGHT}\n      scale={scale}\n      pathStrings={paths}\n      showId={filters.trackId}\n      selectedIndices={selectedIndices}\n      vertices={[]}\n    />\n  )\n\n  function sortedIndex(sortedArray: number[], value: number) {\n    let low = 0,\n      high = sortedArray.length\n\n    while (low < high) {\n      const mid = (low + high) >>> 1\n      if (sortedArray[mid] < value) low = mid + 1\n      else high = mid\n    }\n    return low\n  }\n\n  const handleListItemClick = (\n    event: React.MouseEvent<HTMLDivElement, MouseEvent>,\n    index: number\n  ) => {\n    setSelectedIndices((indices) => new Map(indices.set(index, true)))\n  }\n\n  const renderRows = (rows: Path[]) => {\n    return rows.map((path, index) => {\n      return (\n        <ListItemButton\n          key={index}\n          selected={selectedIndices.has(index)}\n          onClick={(event) => {\n            if (!selectedIndices.has(index)) handleListItemClick(event, index)\n            else\n              setSelectedIndices((indices) => {\n                indices.delete(index)\n                return new Map(indices)\n              })\n          }}\n        >\n          <ListItemText primary={path[2]} />\n          <ListItemText primary={path[1]} />\n        </ListItemButton>\n      )\n    })\n  }\n\n  return (\n    <div>\n      <div className=\"control-container\">\n        <Slider\n          value={scale}\n          aria-label=\"Default\"\n          valueLabelDisplay=\"auto\"\n          onChange={handleSliderChange}\n          min={0}\n          max={10}\n          step={0.01}\n          color=\"primary\"\n          className=\"slider\"\n          style={{ width: 300, margin: 0 }}\n        />\n      </div>\n      <div style={{ overflow: \"hidden\", display: \"flex\" }}>\n        <div style={{ display: \"flex\", flexDirection: \"column\" }}>\n          <Draggable>\n            <div\n              className=\"image-container\"\n              style={{\n                width: WIDTH * scale,\n                height: HEIGHT * scale,\n                backgroundImage: `url(${image})`,\n              }}\n            >\n              {SVGLines}\n            </div>\n          </Draggable>\n          <div style={{ marginTop: 10 }}>\n            <List\n              sx={{\n                width: \"100%\",\n                maxWidth: 360,\n                bgcolor: \"background.paper\",\n                position: \"relative\",\n                overflow: \"auto\",\n                maxHeight: 400,\n                \"& ul\": { padding: 0 },\n                borderRadius: 1,\n              }}\n              subheader={<ListSubheader>Tracks</ListSubheader>}\n              component=\"nav\"\n              aria-label=\"main mailbox folders\"\n            >\n              <Divider />\n              {renderRows(paths)}\n            </List>\n          </div>\n        </div>\n        <FormControl\n          sx={{ margin: 0, marginLeft: 2 }}\n          component=\"fieldset\"\n          variant=\"standard\"\n        >\n          <FormGroup>\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.markMeasurements}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      markMeasurements: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Mark measurments\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.markEstimated}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      markEstimated: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Mark estimated\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.onlyConfirmed}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      onlyConfirmed: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show only confirmed\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.trackId}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      trackId: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show track id\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.showLines}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      showLines: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show lines\"\n            />\n          </FormGroup>\n        </FormControl>\n      </div>\n    </div>\n  )\n}\n\nexport default SourcePlotter\n",
+        "export const colors: Map<number, string> = new Map([\n  [0, \"green\"],\n  [1, \"purple\"],\n  [4, \"red\"],\n  [18, \"cyan\"],\n  [34, \"pink\"],\n])\nexport const names = [\n  \"Pedestrian\",\n  \"Bicycle\",\n  \"Light vehicle\",\n  \"Heavy vehicle\",\n  \"Unknown\",\n]\n",
+        "import { Pos } from \"./Matrix\"\nimport { names } from \"./consts\"\nimport { Show } from \"./types\"\n\nexport type Track = [number, number, number, number, number, string]\nexport type Path = [string, number, number, Pos, Pos]\ntype InternalTrack = [number[], number[], number, number, number[]]\n\nexport function pathStrings(\n  entries: Track[],\n  showType: string[],\n  filters: Show,\n  filterLength: boolean,\n  minLength: number,\n  maxLength: number\n): Path[] {\n  const trackMap = new Map<number, InternalTrack>()\n  for (const [id, x, y, type, estimated] of entries) {\n    if (\n      (filters.onlyConfirmed && estimated === 1) ||\n      showType.indexOf(names[type]) === -1\n    ) {\n    } else {\n      if (trackMap.has(id)) {\n        const [\n          xCoordinates,\n          yCoordinates,\n          existingType,\n          existingId,\n          estimates,\n        ] = trackMap.get(id)!\n        xCoordinates.push(x * 20 + 280)\n        yCoordinates.push(y * 20 + 300)\n        estimates.push(estimated)\n      } else {\n        trackMap.set(id, [\n          [x * 20 + 280],\n          [y * 20 + 300],\n          type,\n          id,\n          [estimated],\n        ])\n      }\n    }\n  }\n\n  trackMap.forEach((track, key) => {\n    if (\n      filterLength &&\n      (track[0].length < minLength || track[0].length > maxLength)\n    ) {\n      trackMap.delete(key)\n    }\n  })\n\n  return Array.from(trackMap.values(), (track) =>\n    createPath(track, filters.markMeasurements, filters.markEstimated)\n  )\n}\n\nfunction createPath(\n  track: InternalTrack,\n  markMeasured: boolean,\n  markEstimates: boolean\n): Path {\n  {\n    const [xs, ys, type, id, estimates] = track\n    const startPos: Pos = [xs[0], ys[0], 0]\n    const endPos: Pos = [xs[xs.length - 1], ys[ys.length - 1], 0]\n    const pathData = xs\n      .map((x, i) => {\n        const estimated = estimates[i]\n        let pathSegment = `L ${x} ${ys[i]}`\n        if (\n          ((markMeasured && estimated === 0) ||\n            (markEstimates && estimated === 1 && i !== 0)) &&\n          i !== 0\n        ) {\n          const size = estimated === 0 ? 6 : 3\n          const [x1, y1] = [xs[i - 1], ys[i - 1]]\n          const [x2, y2] = [x, ys[i]]\n          const length = Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2))\n          const perpendicularDir = [(y1 - y2) / length, (x2 - x1) / length]\n          const angle = 0.707\n          const offsetX =\n            perpendicularDir[0] * angle - perpendicularDir[1] * angle\n          const offsetY =\n            perpendicularDir[0] * angle + perpendicularDir[1] * angle\n          pathSegment += `L ${x + offsetX * size} ${\n            ys[i] + offsetY * size\n          } L ${x} ${ys[i]} L ${x - offsetY * size} ${\n            ys[i] + offsetX * size\n          } L ${x} ${ys[i]}`\n        }\n        return pathSegment\n      })\n      .join(\" \")\n    const pathString = `M ${xs[0]} ${ys[0]} ${pathData}`\n    return [pathString, type, id, startPos, endPos]\n  }\n}\n",
+        "import React from \"react\"\nimport { colors } from \"../../helpers/consts\"\nimport { Path } from \"../../helpers/Paths\"\n\ntype LinesProps = {\n  WIDTH: number\n  HEIGHT: number\n  scale: number\n  pathStrings: Path[]\n  showId: boolean\n  selectedIndices: Map<number, boolean>\n  vertices: JSX.Element[]\n}\n\nexport const Lines: React.FC<LinesProps> = ({\n  WIDTH,\n  HEIGHT,\n  scale,\n  pathStrings,\n  showId,\n  selectedIndices,\n  vertices,\n}) => {\n  return (\n    <svg\n      width={WIDTH * scale}\n      height={HEIGHT * scale}\n      style={{\n        transform: `scale(${scale})`,\n        transformOrigin: \"top left\", // Set the transformation origin\n      }}\n    >\n      {pathStrings.map((path, index) => {\n        /**\n         * The strings are of the format \"...L {x-ending point} {y-ending point},\n         * we want to get these coordinates to display the starting ids above\n         * the ending point\"\n         */\n        const color = colors.get(path[1])\n        return !selectedIndices.has(index) ? (\n          <g key={path[0]}>\n            <path d={path[0]} stroke={color ? color : \"black\"} fill=\"none\" />\n            <circle\n              cx={path[3][0]}\n              cy={path[3][1]}\n              r={4}\n              fill=\"green\"\n              strokeWidth=\"4\"\n            />\n            <circle\n              cx={path[4][0]}\n              cy={path[4][1]}\n              r={4}\n              fill=\"red\"\n              strokeWidth=\"4\"\n            />\n            {showId && (\n              <text\n                x={path[4][0]}\n                y={path[4][1]}\n                fill=\"white\"\n                fontFamily=\"sans-serif\"\n                fontSize={10}\n              >\n                {path[2]}\n              </text>\n            )}\n          </g>\n        ) : (\n          <></>\n        )\n      })}\n      {vertices}\n    </svg>\n  )\n}\n",
+        "import React, { useState, useMemo } from \"react\"\nimport \"../../styles/styles.css\"\nimport { Path, Track, pathStrings } from \"../../helpers/Paths\"\nimport { Lines } from \"./Lines\"\nimport Draggable from \"react-draggable\"\nimport {\n  Checkbox,\n  Divider,\n  FormControl,\n  FormControlLabel,\n  FormGroup,\n  List,\n  ListItemButton,\n  ListItemText,\n  ListSubheader,\n  Slider,\n} from \"@mui/material\"\nimport { Show } from \"../../helpers/types\"\n\ninterface SourcePlotterProps {\n  label: string\n  image: string\n  WIDTH: number\n  HEIGHT: number\n  filterLength: boolean\n  minLength: number\n  maxLength: number\n  tracks: Track[]\n  from: number\n  to: number\n  showType: string[]\n}\n\nconst SourcePlotter: React.FC<SourcePlotterProps> = ({\n  label,\n  image,\n  WIDTH,\n  HEIGHT,\n  tracks,\n  from,\n  to,\n  showType,\n  filterLength,\n  minLength,\n  maxLength,\n}) => {\n  const [scale, setScale] = useState<number>(1)\n  const [filters, setFilters] = useState<Show>({\n    markMeasurements: false,\n    markEstimated: false,\n    onlyConfirmed: false,\n    trackId: false,\n    showLines: false,\n  })\n  const [selectedIndices, setSelectedIndices] = useState<Map<number, boolean>>(\n    new Map()\n  )\n  /**\n   * Memoize the lines so we don't recalculate pathStrings everytime\n   * we rerender this component\n   */\n  const paths = useMemo(() => {\n    return pathStrings(\n      tracks.slice(from, to),\n      showType,\n      filters,\n      filterLength,\n      minLength,\n      maxLength\n    )\n  }, [from, to, showType, filters, filterLength, minLength, maxLength])\n\n  const handleSliderChange = (event: Event, newValue: number | number[]) => {\n    if (typeof newValue === \"number\") {\n      setScale(newValue)\n    }\n  }\n\n  const SVGLines = (\n    <Lines\n      WIDTH={WIDTH}\n      HEIGHT={HEIGHT}\n      scale={scale}\n      pathStrings={paths}\n      showId={filters.trackId}\n      selectedIndices={selectedIndices}\n      vertices={[]}\n    />\n  )\n\n  const handleListItemClick = (\n    event: React.MouseEvent<HTMLDivElement, MouseEvent>,\n    index: number\n  ) => {\n    setSelectedIndices((indices) => new Map(indices.set(index, true)))\n  }\n\n  const renderRows = (rows: Path[]) => {\n    return rows.map((path, index) => {\n      return (\n        <ListItemButton\n          key={index}\n          selected={selectedIndices.has(index)}\n          onClick={(event) => {\n            if (!selectedIndices.has(index)) handleListItemClick(event, index)\n            else\n              setSelectedIndices((indices) => {\n                indices.delete(index)\n                return new Map(indices)\n              })\n          }}\n        >\n          <ListItemText primary={path[2]} />\n          <ListItemText primary={path[1]} />\n        </ListItemButton>\n      )\n    })\n  }\n\n  return (\n    <div>\n      <div className=\"control-container\">\n        <Slider\n          value={scale}\n          aria-label=\"Default\"\n          valueLabelDisplay=\"auto\"\n          onChange={handleSliderChange}\n          min={0}\n          max={10}\n          step={0.01}\n          color=\"primary\"\n          className=\"slider\"\n          style={{ width: 300, margin: 0 }}\n        />\n      </div>\n      <div style={{ overflow: \"hidden\", display: \"flex\" }}>\n        <div style={{ display: \"flex\", flexDirection: \"column\" }}>\n          <Draggable>\n            <div\n              className=\"image-container\"\n              style={{\n                width: WIDTH * scale,\n                height: HEIGHT * scale,\n                backgroundImage: `url(${image})`,\n              }}\n            >\n              {SVGLines}\n            </div>\n          </Draggable>\n          <div style={{ marginTop: 10 }}>\n            <List\n              sx={{\n                width: \"100%\",\n                maxWidth: 360,\n                bgcolor: \"background.paper\",\n                position: \"relative\",\n                overflow: \"auto\",\n                maxHeight: 400,\n                \"& ul\": { padding: 0 },\n                borderRadius: 1,\n              }}\n              subheader={<ListSubheader>Tracks</ListSubheader>}\n              component=\"nav\"\n              aria-label=\"main mailbox folders\"\n            >\n              <Divider />\n              {renderRows(paths)}\n            </List>\n          </div>\n        </div>\n        <FormControl\n          sx={{ margin: 0, marginLeft: 2 }}\n          component=\"fieldset\"\n          variant=\"standard\"\n        >\n          <FormGroup>\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.markMeasurements}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      markMeasurements: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Mark measurments\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.markEstimated}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      markEstimated: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Mark estimated\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.onlyConfirmed}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      onlyConfirmed: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show only confirmed\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.trackId}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      trackId: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show track id\"\n            />\n            <FormControlLabel\n              control={\n                <Checkbox\n                  checked={filters.showLines}\n                  onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                    setFilters((prevFilters) => ({\n                      ...prevFilters,\n                      showLines: event.target.checked,\n                    }))\n                  }}\n                />\n              }\n              label=\"Show lines\"\n            />\n          </FormGroup>\n        </FormControl>\n      </div>\n    </div>\n  )\n}\n\nexport default SourcePlotter\n",
         "import {\n  TextField,\n  FormControl,\n  InputLabel,\n  Select,\n  OutlinedInput,\n  MenuItem,\n  Checkbox,\n  ListItemText,\n  FormControlLabel,\n  Button,\n  SelectChangeEvent,\n} from \"@mui/material\"\nimport {\n  LocalizationProvider,\n  DatePicker,\n  TimePicker,\n} from \"@mui/x-date-pickers\"\nimport { AdapterDayjs } from \"@mui/x-date-pickers/AdapterDayjs\"\nimport { names } from \"../../../helpers/consts\"\nimport dayjs, { Dayjs } from \"dayjs\"\n\ninterface HeaderProps {\n  date: Dayjs\n  setDate: (value: React.SetStateAction<dayjs.Dayjs>) => void\n  fromTime: Dayjs\n  setFromTime: (value: React.SetStateAction<dayjs.Dayjs>) => void\n  setToTime: (value: React.SetStateAction<dayjs.Dayjs>) => void\n  interval: number\n  setDir: (value: React.SetStateAction<0 | 1 | -1>) => void\n  setInterval: (value: React.SetStateAction<number>) => void\n  showType: string[]\n  handleChange: (event: SelectChangeEvent<string[]>) => void\n  filterLength: boolean\n  setFilterLength: (value: React.SetStateAction<boolean>) => void\n  minLength: number\n  setMinLength: (value: React.SetStateAction<number>) => void\n  maxLength: number\n  setMaxLength: (value: React.SetStateAction<number>) => void\n  handleBackwardClick: () => void\n  handleForwardClick: () => void\n}\n\nexport const Header: React.FC<HeaderProps> = ({\n  date,\n  setDate,\n  fromTime,\n  setFromTime,\n  setToTime,\n  interval,\n  setDir,\n  setInterval,\n  showType,\n  handleChange,\n  filterLength,\n  setFilterLength,\n  minLength,\n  setMinLength,\n  maxLength,\n  setMaxLength,\n  handleBackwardClick,\n  handleForwardClick,\n}) => {\n  const ITEM_HEIGHT = 48\n  const ITEM_PADDING_TOP = 8\n  const MenuProps = {\n    PaperProps: {\n      style: {\n        maxHeight: ITEM_HEIGHT * 4.5 + ITEM_PADDING_TOP,\n        width: 250,\n      },\n    },\n  }\n  console.log(showType)\n  return (\n    <div>\n      <LocalizationProvider dateAdapter={AdapterDayjs}>\n        <DatePicker\n          label=\"Date\"\n          format=\"YYYY-MM-DD\"\n          value={date}\n          onChange={(newValue) => {\n            if (newValue) setDate(newValue)\n          }}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n        <TimePicker\n          label=\"From time\"\n          value={fromTime}\n          onChange={(newValue) => {\n            if (newValue) {\n              setFromTime(newValue)\n              setToTime(newValue.add(interval, \"minutes\"))\n              setDir(0)\n            }\n          }}\n          ampm={false}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n      </LocalizationProvider>\n      <TextField\n        label=\"Interval in minutes\"\n        id=\"outlined-start-adornment\"\n        sx={{\n          width: \"25ch\",\n          backgroundColor: \"background.default\",\n          borderRadius: 1,\n          margin: 0,\n          marginRight: 2,\n        }}\n        value={interval}\n        onChange={(newVal) => {\n          const val = Number(newVal.target.value)\n          if (!isNaN(val)) {\n            setInterval(val)\n            setToTime(fromTime.add(val, \"minutes\"))\n          }\n        }}\n      />\n      <FormControl sx={{ m: 1, width: 300, margin: 0 }}>\n        <InputLabel id=\"demo-multiple-name-label\">Show types</InputLabel>\n        <Select\n          labelId=\"demo-multiple-name-label\"\n          id=\"demo-multiple-name\"\n          multiple\n          value={showType}\n          onChange={handleChange}\n          input={<OutlinedInput label=\"Show types\" />}\n          renderValue={(selected) => selected.join(\", \")}\n          MenuProps={MenuProps}\n          sx={{ backgroundColor: \"background.default\" }}\n        >\n          {names.map((name) => (\n            <MenuItem key={name} value={name}>\n              <Checkbox checked={showType.indexOf(name) > -1} />\n              <ListItemText primary={name} />\n            </MenuItem>\n          ))}\n        </Select>\n      </FormControl>\n      <div>\n        <FormControlLabel\n          control={\n            <Checkbox\n              checked={filterLength}\n              onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                setFilterLength(event.target.checked)\n              }}\n            />\n          }\n          label=\"Filter length\"\n          style={{ margin: 0, marginTop: 10 }}\n        />\n      </div>\n      {filterLength && (\n        <div style={{ marginTop: 10 }}>\n          <TextField\n            label=\"Minimum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={minLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setMinLength(val)\n              }\n            }}\n          />\n          <TextField\n            label=\"Maximum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={maxLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setMaxLength(val)\n              }\n            }}\n          />\n        </div>\n      )}\n      <div style={{ margin: 0, marginTop: 10 }}>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleBackwardClick()}\n        >\n          {\"<\"}\n        </Button>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleForwardClick()}\n        >\n          {\">\"}\n        </Button>\n      </div>\n    </div>\n  )\n}\n",
         "import React, { useEffect, useState } from \"react\"\nimport SourcePlotter from \"./SourcePlotter\"\nimport { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport { Track } from \"../../helpers/Paths\"\nimport dayjs, { Dayjs } from \"dayjs\"\nimport { SelectChangeEvent } from \"@mui/material\"\nimport { names } from \"../../helpers/consts\"\nimport { Streamlit } from \"streamlit-component-lib\"\nimport { Header } from \"./header/Header\"\n\nconst TrackAnalysis: React.FC = () => {\n  const renderData = useRenderData()\n  const [from, setFrom] = useState(0)\n  const [to, setTo] = useState(0)\n  const [dir, setDir] = useState<0 | 1 | -1>(0)\n  const [date, setDate] = useState<Dayjs>(dayjs(renderData.args[\"date\"]))\n  const [fromTime, setFromTime] = useState<Dayjs>(\n    dayjs(renderData.args[\"date\"])\n  )\n  const [toTime, setToTime] = useState<Dayjs>(dayjs(renderData.args[\"date\"]))\n  const [interval, setInterval] = useState(1)\n  const [showType, setShowType] = React.useState<string[]>(names)\n  const [filterLength, setFilterLength] = useState(false)\n  const [minLength, setMinLength] = useState(0)\n  const [maxLength, setMaxLength] = useState(0)\n  const [tracks, setTracks] = useState<Track[]>(renderData.args[\"tracks\"])\n  const ground = renderData.args[\"image\"]\n  const height = renderData.args[\"height\"]\n  const width = renderData.args[\"width\"]\n\n  useEffect(() => {\n    if (date.isValid()) {\n      Streamlit.setComponentValue(date.format(\"YYYY-MM-DD\"))\n    }\n  }, [date])\n\n  useEffect(() => {\n    const setIndices = () => {\n      let fromIndex: number\n      let toIndex: number\n      if (dir === 0) {\n        fromIndex = binarySearch(fromTime, 0, tracks.length - 1)\n        toIndex = binarySearch(toTime, 0, tracks.length - 1)\n      } else if (dir === 1) {\n        fromIndex = to + 1\n        let i = fromIndex\n        console.log(\"INDEX:\", i, tracks.length - 1, i < tracks.length - 1)\n        while (i < tracks.length && dayjs(tracks[i][5]).isBefore(toTime)) {\n          i++\n        }\n        toIndex = i\n      } else {\n        toIndex = from\n        let i = toIndex\n        console.log(\"INDEX:\", i, tracks.length)\n        while (\n          i > 0 &&\n          i < tracks.length &&\n          fromTime.isBefore(dayjs(tracks[i][5]))\n        ) {\n          i--\n        }\n\n        fromIndex = i + 1\n      }\n      setFrom(fromIndex)\n      setTo(toIndex)\n      console.log(\"First track:\", tracks[fromIndex])\n      console.log(\"Last track\", tracks[toIndex - 1])\n      console.log(`From ${fromIndex} to ${toIndex}`)\n    }\n    setIndices()\n  }, [fromTime, toTime])\n\n  const handleBackwardClick = () => {\n    setFromTime((fromTime) => fromTime.subtract(interval, \"minutes\"))\n    setToTime((toTime) => toTime.subtract(interval, \"minutes\"))\n    setDir(-1)\n  }\n\n  const handleForwardClick = () => {\n    setFromTime((fromTime) => fromTime.add(interval, \"minutes\"))\n    setToTime((toTime) => toTime.add(interval, \"minutes\"))\n    setDir(1)\n  }\n\n  function binarySearch(time: Dayjs, low: number, high: number): number {\n    while (low < high) {\n      const mid = Math.floor((low + high) >>> 1)\n      if (mid === 0) return 0\n      const midTime = dayjs(tracks[mid][5])\n      if (midTime.isAfter(time) && dayjs(tracks[mid - 1][5]).isBefore(time)) {\n        return mid\n      } else if (midTime.isAfter(time)) {\n        high = mid\n      } else {\n        low = mid + 1\n      }\n    }\n    return low\n  }\n\n  const cameraPlots: JSX.Element[] = [\n    <SourcePlotter\n      image={ground}\n      WIDTH={width}\n      HEIGHT={height}\n      tracks={tracks}\n      from={from}\n      to={to}\n      label={\"Version 1\"}\n      showType={showType}\n      filterLength={filterLength}\n      minLength={minLength}\n      maxLength={maxLength}\n    />,\n  ]\n\n  const handleChange = (event: SelectChangeEvent<typeof showType>) => {\n    const {\n      target: { value },\n    } = event\n    setShowType(typeof value === \"string\" ? value.split(\",\") : value)\n  }\n\n  return (\n    <div style={{ flexDirection: \"column\", marginTop: 30 }}>\n      <Header\n        date={date}\n        setDate={setDate}\n        fromTime={fromTime}\n        setFromTime={setFromTime}\n        setToTime={setToTime}\n        interval={interval}\n        setDir={setDir}\n        setInterval={setInterval}\n        showType={showType}\n        handleChange={handleChange}\n        filterLength={filterLength}\n        setFilterLength={setFilterLength}\n        minLength={minLength}\n        setMinLength={setMinLength}\n        maxLength={maxLength}\n        setMaxLength={setMaxLength}\n        handleBackwardClick={handleBackwardClick}\n        handleForwardClick={handleForwardClick}\n      />\n      <div style={{ display: \"flex\", flexDirection: \"row\" }}>\n        <div\n          style={{\n            flexDirection: \"row\",\n            flexWrap: \"wrap\",\n          }}\n        >\n          {cameraPlots.map((plot) => plot)}\n          <div style={{ height: 10000 }} />\n        </div>\n      </div>\n    </div>\n  )\n}\n\nexport default TrackAnalysis\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport { StreamlitProvider } from \"streamlit-component-lib-react-hooks\"\nimport TrackAnalysis from \"./components/plotter/TrackAnalysis\"\nimport { ThemeProvider, createTheme } from \"@mui/material\"\n\n//Dirty dirty\nconsole.warn = () => {}\n\nconst theme = createTheme({\n  palette: {\n    primary: {\n      main: \"#F63366\",\n    },\n    common: {\n      black: \"#F63366\",\n    },\n    secondary: {\n      main: \"#F0F2F6\",\n    },\n    text: {\n      primary: \"#fff\",\n      secondary: \"#fff\",\n    },\n    action: {\n      active: \"#fff\",\n    },\n    background: {\n      default: \"#262730\",\n      paper: \"#262730\",\n    },\n  },\n})\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitProvider>\n      <ThemeProvider theme={theme}>\n        <TrackAnalysis />\n      </ThemeProvider>\n    </StreamlitProvider>\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map` & `st_track_analysis-0.0.3/st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map`

 * *Files identical despite different names*

### Comparing `st_track_analysis-0.0.2/st_track_analysis.egg-info/SOURCES.txt` & `st_track_analysis-0.0.3/st_track_analysis.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 st_track_analysis/frontend/build/asset-manifest.json
 st_track_analysis/frontend/build/index.html
 st_track_analysis/frontend/build/static/css/main.22919367.chunk.css
 st_track_analysis/frontend/build/static/css/main.22919367.chunk.css.map
 st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js
 st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.LICENSE.txt
 st_track_analysis/frontend/build/static/js/2.2edeab5c.chunk.js.map
-st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js
-st_track_analysis/frontend/build/static/js/main.070b89e3.chunk.js.map
+st_track_analysis/frontend/build/static/js/main.56720d29.chunk.js
+st_track_analysis/frontend/build/static/js/main.56720d29.chunk.js.map
 st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js
 st_track_analysis/frontend/build/static/js/runtime-main.657b0728.js.map
```

