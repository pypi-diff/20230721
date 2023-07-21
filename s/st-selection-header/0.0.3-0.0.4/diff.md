# Comparing `tmp/st-selection-header-0.0.3.tar.gz` & `tmp/st_selection_header-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-selection-header-0.0.3.tar", last modified: Fri Jul 21 16:27:03 2023, max compression
+gzip compressed data, was "st_selection_header-0.0.4.tar", last modified: Fri Jul 21 16:57:11 2023, max compression
```

## Comparing `st-selection-header-0.0.3.tar` & `st_selection_header-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:27:03.054044 st-selection-header-0.0.3/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-21 13:50:11.000000 st-selection-header-0.0.3/LICENSE
--rw-r--r--   0 elliotglas   (501) staff       (20)       55 2023-07-21 13:55:00.000000 st-selection-header-0.0.3/MANIFEST.in
--rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:27:03.053824 st-selection-header-0.0.3/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 16:27:03.054106 st-selection-header-0.0.3/setup.cfg
--rw-r--r--   0 elliotglas   (501) staff       (20)      645 2023-07-21 16:26:58.000000 st-selection-header-0.0.3/setup.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:27:03.046869 st-selection-header-0.0.3/st_selection_header/
--rw-r--r--   0 elliotglas   (501) staff       (20)      814 2023-07-21 16:18:00.000000 st-selection-header-0.0.3/st_selection_header/__init__.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:27:03.045715 st-selection-header-0.0.3/st_selection_header/frontend/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:27:03.048724 st-selection-header-0.0.3/st_selection_header/frontend/build/
--rw-r--r--   0 elliotglas   (501) staff       (20)      691 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/asset-manifest.json
--rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/index.html
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:27:03.045913 st-selection-header-0.0.3/st_selection_header/frontend/build/static/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:27:03.053535 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/
--rw-r--r--   0 elliotglas   (501) staff       (20)   924549 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)  3811745 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     4633 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/main.858e53a4.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)    14333 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/main.858e53a4.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 16:26:44.000000 st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:27:03.048276 st-selection-header-0.0.3/st_selection_header.egg-info/
--rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:27:02.000000 st-selection-header-0.0.3/st_selection_header.egg-info/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)      870 2023-07-21 16:27:03.000000 st-selection-header-0.0.3/st_selection_header.egg-info/SOURCES.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 16:27:02.000000 st-selection-header-0.0.3/st_selection_header.egg-info/dependency_links.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 16:27:02.000000 st-selection-header-0.0.3/st_selection_header.egg-info/requires.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       20 2023-07-21 16:27:02.000000 st-selection-header-0.0.3/st_selection_header.egg-info/top_level.txt
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:57:11.040448 st_selection_header-0.0.4/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-07-21 13:50:11.000000 st_selection_header-0.0.4/LICENSE
+-rw-r--r--   0 elliotglas   (501) staff       (20)       55 2023-07-21 13:55:00.000000 st_selection_header-0.0.4/MANIFEST.in
+-rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:57:11.040256 st_selection_header-0.0.4/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-07-21 16:57:11.040504 st_selection_header-0.0.4/setup.cfg
+-rw-r--r--   0 elliotglas   (501) staff       (20)      645 2023-07-21 16:56:42.000000 st_selection_header-0.0.4/setup.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:57:11.033840 st_selection_header-0.0.4/st_selection_header/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      814 2023-07-21 16:18:00.000000 st_selection_header-0.0.4/st_selection_header/__init__.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:57:11.032902 st_selection_header-0.0.4/st_selection_header/frontend/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:57:11.035713 st_selection_header-0.0.4/st_selection_header/frontend/build/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      691 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/asset-manifest.json
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/index.html
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:57:11.033088 st_selection_header-0.0.4/st_selection_header/frontend/build/static/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:57:11.039981 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   924549 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2484 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)  3811745 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     4624 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/main.2185bd8c.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)    14323 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/main.2185bd8c.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     8383 2023-07-21 16:56:21.000000 st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-07-21 16:57:11.035204 st_selection_header-0.0.4/st_selection_header.egg-info/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      274 2023-07-21 16:57:10.000000 st_selection_header-0.0.4/st_selection_header.egg-info/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)      870 2023-07-21 16:57:11.000000 st_selection_header-0.0.4/st_selection_header.egg-info/SOURCES.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-07-21 16:57:10.000000 st_selection_header-0.0.4/st_selection_header.egg-info/dependency_links.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-07-21 16:57:10.000000 st_selection_header-0.0.4/st_selection_header.egg-info/requires.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       20 2023-07-21 16:57:10.000000 st_selection_header-0.0.4/st_selection_header.egg-info/top_level.txt
```

### Comparing `st-selection-header-0.0.3/LICENSE` & `st_selection_header-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.3/setup.py` & `st_selection_header-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
-    name="st-selection-header",
-    version="0.0.3",
+    name="st_selection_header",
+    version="0.0.4",
     author="Elliot Glas",
     author_email="elliot.glas@viscando.com",
     description="Panel for changing data",
     long_description="Panel for changing data",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st-selection-header-0.0.3/st_selection_header/__init__.py` & `st_selection_header-0.0.4/st_selection_header/__init__.py`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/asset-manifest.json` & `st_selection_header-0.0.4/st_selection_header/frontend/build/asset-manifest.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.84375%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.2185bd8c.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.2185bd8c.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.2185bd8c.chunk.js.map'}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "entrypoints": [
         "static/js/runtime-main.39defc4e.js",
         "static/js/2.0a2a2974.chunk.js",
-        "static/js/main.858e53a4.chunk.js"
+        "static/js/main.2185bd8c.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.858e53a4.chunk.js",
-        "main.js.map": "./static/js/main.858e53a4.chunk.js.map",
+        "main.js": "./static/js/main.2185bd8c.chunk.js",
+        "main.js.map": "./static/js/main.2185bd8c.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.39defc4e.js",
         "runtime-main.js.map": "./static/js/runtime-main.39defc4e.js.map",
         "static/js/2.0a2a2974.chunk.js": "./static/js/2.0a2a2974.chunk.js",
         "static/js/2.0a2a2974.chunk.js.LICENSE.txt": "./static/js/2.0a2a2974.chunk.js.LICENSE.txt",
         "static/js/2.0a2a2974.chunk.js.map": "./static/js/2.0a2a2974.chunk.js.map"
     }
 }
```

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/index.html` & `st_selection_header-0.0.4/st_selection_header/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.0a2a2974.chunk.js"></script><script src="./static/js/main.858e53a4.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.0a2a2974.chunk.js"></script><script src="./static/js/main.2185bd8c.chunk.js"></script></body></html>
```

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js` & `st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt` & `st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map` & `st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/main.858e53a4.chunk.js` & `st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/main.2185bd8c.chunk.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,16 +5,16 @@
             n.r(t);
             var a = n(0),
                 r = n.n(a),
                 i = n(48),
                 o = n.n(i),
                 c = n(91),
                 l = n(19),
-                m = n(10),
-                u = n(288),
+                u = n(10),
+                m = n(288),
                 d = n(299),
                 s = n(289),
                 b = n(279),
                 g = n(292),
                 f = n(291),
                 h = n(284),
                 j = n(274),
@@ -40,21 +40,21 @@
                             filterLength: {
                                 filter: !1,
                                 minLength: 0,
                                 maxLength: 0
                             }
                         },
                         r = Object(a.useState)(n),
-                        i = Object(m.a)(r, 2),
+                        i = Object(u.a)(r, 2),
                         o = i[0],
                         T = i[1];
                     Object(a.useEffect)((function() {
                         o.date.isValid() && o.fromTime.isValid() && function() {
                             var e = Object(l.a)(Object(l.a)({}, o), {}, {
-                                date: o.date.format("YYYY-MM-DD HH:mm:ss"),
+                                date: o.date.format("YYYY-MM-DD"),
                                 fromTime: o.fromTime.format("YYYY-MM-DD HH:mm:ss")
                             });
                             L.Streamlit.setComponentValue(e)
                         }()
                     }), [o]);
                     var Y = {
                         PaperProps: {
@@ -95,15 +95,15 @@
                                 ampm: !1,
                                 sx: {
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
                                     marginRight: 2
                                 }
                             })]
-                        }), Object(R.jsx)(u.a, {
+                        }), Object(R.jsx)(m.a, {
                             label: "Interval in minutes",
                             id: "outlined-start-adornment",
                             sx: {
                                 width: "25ch",
                                 backgroundColor: "background.default",
                                 borderRadius: 1,
                                 margin: 0,
@@ -173,15 +173,15 @@
                                     marginTop: 10
                                 }
                             })
                         }), o.filterLength.filter && Object(R.jsxs)("div", {
                             style: {
                                 marginTop: 10
                             },
-                            children: [Object(R.jsx)(u.a, {
+                            children: [Object(R.jsx)(m.a, {
                                 label: "Minimum length",
                                 id: "outlined-start-adornment",
                                 sx: {
                                     m: 1,
                                     width: "25ch",
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
@@ -191,15 +191,15 @@
                                 value: o.filterLength.minLength,
                                 onChange: function(e) {
                                     var t = Number(e.target.value);
                                     isNaN(t) || T((function(e) {
                                         return e.filterLength.minLength = t, Object(l.a)({}, e)
                                     }))
                                 }
-                            }), Object(R.jsx)(u.a, {
+                            }), Object(R.jsx)(m.a, {
                                 label: "Maximum length",
                                 id: "outlined-start-adornment",
                                 sx: {
                                     m: 1,
                                     width: "25ch",
                                     backgroundColor: "background.default",
                                     borderRadius: 1,
@@ -286,8 +286,8 @@
             }), document.getElementById("root"))
         }
     },
     [
         [191, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.858e53a4.chunk.js.map
+//# sourceMappingURL=main.2185bd8c.chunk.js.map
```

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/main.858e53a4.chunk.js.map` & `st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/main.2185bd8c.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8214285714285714%*

 * *Differences: {"'file'": "'static/js/main.2185bd8c.chunk.js'",*

 * * "'mappings'": "'iWAAaA,EAAQ,CACnB,aACA,UACA,gBACA,gBACA,W,eCoRaC,EAzO0B,WACvC,IAAMC,EAAaC,0BACbC,EAAcC,IAAMH,EAAWI,KAAW,MAC1CC,EAAoB,CACxBC,KAAMJ,EACNK,SAAUL,EACVM,SAAU,EACVC,SAAUX,EACVY,aAAc,CACZC,QAAQ,EACRC,UAAW,EACXC,UAAW,IAGfC,EAAwBC,mBAAeV,GAAYW,EAAAC,YAAAH,EAAA,GAA5CI,EAAIF,EAAA,GAAEG,EAAOH,EAAA,GAEpBI,qBAAU,WASJF,EAAKZ,KAAKe,WAAaH,EAAKX,SAASc,WARrB,WAClB,IAAMC,EAAsBC,wBAAA,GACvBL,GAAI,IACPZ,KAAMY,EAAKZ,KAAKkB,OAAO,cACvBjB,SAAUW,EAAKX,SAASiB,OAAO,yBAEj […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.858e53a4.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.2185bd8c.chunk.js",
+    "mappings": "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",
     "names": [
         "names",
         "SelectionHeader",
         "renderData",
         "useRenderData",
         "initialDate",
         "dayjs",
@@ -123,12 +123,12 @@
     "sources": [
         "consts.ts",
         "SelectionHeader.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "export const names = [\n  \"Pedestrian\",\n  \"Bicycle\",\n  \"Light vehicle\",\n  \"Heavy vehicle\",\n  \"Unknown\",\n]\n",
-        "import {\n  TextField,\n  FormControl,\n  InputLabel,\n  Select,\n  OutlinedInput,\n  MenuItem,\n  Checkbox,\n  ListItemText,\n  FormControlLabel,\n  Button,\n  SelectChangeEvent,\n} from \"@mui/material\"\nimport {\n  LocalizationProvider,\n  DatePicker,\n  TimePicker,\n} from \"@mui/x-date-pickers\"\nimport { AdapterDayjs } from \"@mui/x-date-pickers/AdapterDayjs\"\nimport dayjs, { Dayjs } from \"dayjs\"\nimport React, { useEffect } from \"react\"\nimport { useState } from \"react\"\nimport { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport { names } from \"./consts\"\nimport { Streamlit } from \"streamlit-component-lib\"\n\ninterface Data {\n  date: Dayjs\n  fromTime: Dayjs\n  interval: number\n  showType: typeof names\n  filterLength: FilterLength\n}\n\ninterface FilterLength {\n  filter: boolean\n  minLength: number\n  maxLength: number\n}\n\ninterface ReturnData {\n  date: string\n  fromTime: string\n  interval: number\n  showType: typeof names\n  filterLength: FilterLength\n}\n\nexport const SelectionHeader: React.FC = () => {\n  const renderData = useRenderData()\n  const initialDate = dayjs(renderData.args[\"date\"])\n  const initialData: Data = {\n    date: initialDate,\n    fromTime: initialDate,\n    interval: 0,\n    showType: names,\n    filterLength: {\n      filter: false,\n      minLength: 0,\n      maxLength: 0,\n    },\n  }\n  const [data, setData] = useState<Data>(initialData)\n\n  useEffect(() => {\n    const returnValue = () => {\n      const returnData: ReturnData = {\n        ...data,\n        date: data.date.format(\"YYYY-MM-DD HH:mm:ss\"),\n        fromTime: data.fromTime.format(\"YYYY-MM-DD HH:mm:ss\"),\n      }\n      Streamlit.setComponentValue(returnData)\n    }\n    if (data.date.isValid() && data.fromTime.isValid()) returnValue()\n  }, [data])\n\n  const handleChange = (event: SelectChangeEvent<typeof names>) => {\n    const {\n      target: { value },\n    } = event\n    setData((data) => {\n      data.showType = typeof value === \"string\" ? value.split(\",\") : value\n      return { ...data }\n    })\n  }\n\n  const handleBackwardClick = () => {\n    setData((data) => {\n      data.fromTime = data.fromTime.subtract(data.interval, \"minutes\")\n      return { ...data }\n    })\n  }\n\n  const handleForwardClick = () => {\n    setData((data) => {\n      data.fromTime = data.fromTime.add(data.interval, \"minutes\")\n      return { ...data }\n    })\n  }\n\n  const ITEM_HEIGHT = 48\n  const ITEM_PADDING_TOP = 8\n  const MenuProps = {\n    PaperProps: {\n      style: {\n        maxHeight: ITEM_HEIGHT * 4.5 + ITEM_PADDING_TOP,\n        width: 250,\n      },\n    },\n  }\n\n  return (\n    <div style={{ marginTop: 30 }}>\n      <LocalizationProvider dateAdapter={AdapterDayjs}>\n        <DatePicker\n          label=\"Date\"\n          format=\"YYYY-MM-DD\"\n          value={data.date}\n          onChange={(newValue) => {\n            if (newValue)\n              setData((data) => {\n                data.date = newValue\n                if (newValue.isValid()) {\n                  data.fromTime = newValue\n                    .set(\"hour\", data.fromTime.hour())\n                    .set(\"minute\", data.fromTime.minute())\n                }\n                return { ...data }\n              })\n          }}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n        <TimePicker\n          label=\"From time\"\n          value={data.fromTime}\n          onChange={(newValue) => {\n            if (newValue) {\n              setData((data) => {\n                data.fromTime = newValue\n                return { ...data }\n              })\n            }\n          }}\n          ampm={false}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n      </LocalizationProvider>\n      <TextField\n        label=\"Interval in minutes\"\n        id=\"outlined-start-adornment\"\n        sx={{\n          width: \"25ch\",\n          backgroundColor: \"background.default\",\n          borderRadius: 1,\n          margin: 0,\n          marginRight: 2,\n        }}\n        value={data.interval}\n        onChange={(newVal) => {\n          const val = Number(newVal.target.value)\n          if (!isNaN(val)) {\n            setData((data) => {\n              data.interval = val\n              return { ...data }\n            })\n          }\n        }}\n      />\n      <FormControl sx={{ m: 1, width: 300, margin: 0 }}>\n        <InputLabel id=\"demo-multiple-name-label\">Show types</InputLabel>\n        <Select\n          labelId=\"demo-multiple-name-label\"\n          id=\"demo-multiple-name\"\n          multiple\n          value={data.showType}\n          onChange={handleChange}\n          input={<OutlinedInput label=\"Show types\" />}\n          renderValue={(selected) => selected.join(\", \")}\n          MenuProps={MenuProps}\n          sx={{ backgroundColor: \"background.default\" }}\n        >\n          {names.map((name) => (\n            <MenuItem key={name} value={name}>\n              <Checkbox checked={data.showType.indexOf(name) > -1} />\n              <ListItemText primary={name} />\n            </MenuItem>\n          ))}\n        </Select>\n      </FormControl>\n      <div>\n        <FormControlLabel\n          control={\n            <Checkbox\n              checked={data.filterLength.filter}\n              onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                setData((data) => {\n                  data.filterLength.filter = event.target.checked\n                  return { ...data }\n                })\n              }}\n            />\n          }\n          label=\"Filter length\"\n          style={{ margin: 0, marginTop: 10 }}\n        />\n      </div>\n      {data.filterLength.filter && (\n        <div style={{ marginTop: 10 }}>\n          <TextField\n            label=\"Minimum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={data.filterLength.minLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setData((data) => {\n                  data.filterLength.minLength = val\n                  return { ...data }\n                })\n              }\n            }}\n          />\n          <TextField\n            label=\"Maximum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={data.filterLength.maxLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setData((data) => {\n                  data.filterLength.maxLength = val\n                  return { ...data }\n                })\n              }\n            }}\n          />\n        </div>\n      )}\n      <div style={{ margin: 0, marginTop: 10 }}>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleBackwardClick()}\n        >\n          {\"<\"}\n        </Button>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleForwardClick()}\n        >\n          {\">\"}\n        </Button>\n      </div>\n      <div style={{ height: 100 }}></div>\n    </div>\n  )\n}\n\nexport default SelectionHeader\n",
+        "import {\n  TextField,\n  FormControl,\n  InputLabel,\n  Select,\n  OutlinedInput,\n  MenuItem,\n  Checkbox,\n  ListItemText,\n  FormControlLabel,\n  Button,\n  SelectChangeEvent,\n} from \"@mui/material\"\nimport {\n  LocalizationProvider,\n  DatePicker,\n  TimePicker,\n} from \"@mui/x-date-pickers\"\nimport { AdapterDayjs } from \"@mui/x-date-pickers/AdapterDayjs\"\nimport dayjs, { Dayjs } from \"dayjs\"\nimport React, { useEffect } from \"react\"\nimport { useState } from \"react\"\nimport { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport { names } from \"./consts\"\nimport { Streamlit } from \"streamlit-component-lib\"\n\ninterface Data {\n  date: Dayjs\n  fromTime: Dayjs\n  interval: number\n  showType: typeof names\n  filterLength: FilterLength\n}\n\ninterface FilterLength {\n  filter: boolean\n  minLength: number\n  maxLength: number\n}\n\ninterface ReturnData {\n  date: string\n  fromTime: string\n  interval: number\n  showType: typeof names\n  filterLength: FilterLength\n}\n\nexport const SelectionHeader: React.FC = () => {\n  const renderData = useRenderData()\n  const initialDate = dayjs(renderData.args[\"date\"])\n  const initialData: Data = {\n    date: initialDate,\n    fromTime: initialDate,\n    interval: 0,\n    showType: names,\n    filterLength: {\n      filter: false,\n      minLength: 0,\n      maxLength: 0,\n    },\n  }\n  const [data, setData] = useState<Data>(initialData)\n\n  useEffect(() => {\n    const returnValue = () => {\n      const returnData: ReturnData = {\n        ...data,\n        date: data.date.format(\"YYYY-MM-DD\"),\n        fromTime: data.fromTime.format(\"YYYY-MM-DD HH:mm:ss\"),\n      }\n      Streamlit.setComponentValue(returnData)\n    }\n    if (data.date.isValid() && data.fromTime.isValid()) returnValue()\n  }, [data])\n\n  const handleChange = (event: SelectChangeEvent<typeof names>) => {\n    const {\n      target: { value },\n    } = event\n    setData((data) => {\n      data.showType = typeof value === \"string\" ? value.split(\",\") : value\n      return { ...data }\n    })\n  }\n\n  const handleBackwardClick = () => {\n    setData((data) => {\n      data.fromTime = data.fromTime.subtract(data.interval, \"minutes\")\n      return { ...data }\n    })\n  }\n\n  const handleForwardClick = () => {\n    setData((data) => {\n      data.fromTime = data.fromTime.add(data.interval, \"minutes\")\n      return { ...data }\n    })\n  }\n\n  const ITEM_HEIGHT = 48\n  const ITEM_PADDING_TOP = 8\n  const MenuProps = {\n    PaperProps: {\n      style: {\n        maxHeight: ITEM_HEIGHT * 4.5 + ITEM_PADDING_TOP,\n        width: 250,\n      },\n    },\n  }\n\n  return (\n    <div style={{ marginTop: 30 }}>\n      <LocalizationProvider dateAdapter={AdapterDayjs}>\n        <DatePicker\n          label=\"Date\"\n          format=\"YYYY-MM-DD\"\n          value={data.date}\n          onChange={(newValue) => {\n            if (newValue)\n              setData((data) => {\n                data.date = newValue\n                if (newValue.isValid()) {\n                  data.fromTime = newValue\n                    .set(\"hour\", data.fromTime.hour())\n                    .set(\"minute\", data.fromTime.minute())\n                }\n                return { ...data }\n              })\n          }}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n        <TimePicker\n          label=\"From time\"\n          value={data.fromTime}\n          onChange={(newValue) => {\n            if (newValue) {\n              setData((data) => {\n                data.fromTime = newValue\n                return { ...data }\n              })\n            }\n          }}\n          ampm={false}\n          sx={{\n            backgroundColor: \"background.default\",\n            borderRadius: 1,\n            marginRight: 2,\n          }}\n        />\n      </LocalizationProvider>\n      <TextField\n        label=\"Interval in minutes\"\n        id=\"outlined-start-adornment\"\n        sx={{\n          width: \"25ch\",\n          backgroundColor: \"background.default\",\n          borderRadius: 1,\n          margin: 0,\n          marginRight: 2,\n        }}\n        value={data.interval}\n        onChange={(newVal) => {\n          const val = Number(newVal.target.value)\n          if (!isNaN(val)) {\n            setData((data) => {\n              data.interval = val\n              return { ...data }\n            })\n          }\n        }}\n      />\n      <FormControl sx={{ m: 1, width: 300, margin: 0 }}>\n        <InputLabel id=\"demo-multiple-name-label\">Show types</InputLabel>\n        <Select\n          labelId=\"demo-multiple-name-label\"\n          id=\"demo-multiple-name\"\n          multiple\n          value={data.showType}\n          onChange={handleChange}\n          input={<OutlinedInput label=\"Show types\" />}\n          renderValue={(selected) => selected.join(\", \")}\n          MenuProps={MenuProps}\n          sx={{ backgroundColor: \"background.default\" }}\n        >\n          {names.map((name) => (\n            <MenuItem key={name} value={name}>\n              <Checkbox checked={data.showType.indexOf(name) > -1} />\n              <ListItemText primary={name} />\n            </MenuItem>\n          ))}\n        </Select>\n      </FormControl>\n      <div>\n        <FormControlLabel\n          control={\n            <Checkbox\n              checked={data.filterLength.filter}\n              onChange={(event: React.ChangeEvent<HTMLInputElement>) => {\n                setData((data) => {\n                  data.filterLength.filter = event.target.checked\n                  return { ...data }\n                })\n              }}\n            />\n          }\n          label=\"Filter length\"\n          style={{ margin: 0, marginTop: 10 }}\n        />\n      </div>\n      {data.filterLength.filter && (\n        <div style={{ marginTop: 10 }}>\n          <TextField\n            label=\"Minimum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={data.filterLength.minLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setData((data) => {\n                  data.filterLength.minLength = val\n                  return { ...data }\n                })\n              }\n            }}\n          />\n          <TextField\n            label=\"Maximum length\"\n            id=\"outlined-start-adornment\"\n            sx={{\n              m: 1,\n              width: \"25ch\",\n              backgroundColor: \"background.default\",\n              borderRadius: 1,\n              margin: 0,\n              marginRight: 2,\n            }}\n            value={data.filterLength.maxLength}\n            onChange={(newVal) => {\n              const val = Number(newVal.target.value)\n              if (!isNaN(val)) {\n                setData((data) => {\n                  data.filterLength.maxLength = val\n                  return { ...data }\n                })\n              }\n            }}\n          />\n        </div>\n      )}\n      <div style={{ margin: 0, marginTop: 10 }}>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleBackwardClick()}\n        >\n          {\"<\"}\n        </Button>\n        <Button\n          sx={{ marginRight: 2, backgroundColor: \"background.default\" }}\n          onClick={() => handleForwardClick()}\n        >\n          {\">\"}\n        </Button>\n      </div>\n      <div style={{ height: 100 }}></div>\n    </div>\n  )\n}\n\nexport default SelectionHeader\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport { StreamlitProvider } from \"streamlit-component-lib-react-hooks\"\nimport SelectionHeader from \"./SelectionHeader\"\nimport { ThemeProvider, createTheme } from \"@mui/material\"\n\n//Dirty dirty\nconsole.warn = () => {}\n\nconst theme = createTheme({\n  palette: {\n    primary: {\n      main: \"#F63366\",\n    },\n    common: {\n      black: \"#F63366\",\n    },\n    secondary: {\n      main: \"#F0F2F6\",\n    },\n    text: {\n      primary: \"#fff\",\n      secondary: \"#fff\",\n    },\n    action: {\n      active: \"#fff\",\n    },\n    background: {\n      default: \"#262730\",\n      paper: \"#262730\",\n    },\n  },\n})\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitProvider>\n      <ThemeProvider theme={theme}>\n        <SelectionHeader />\n      </ThemeProvider>\n    </StreamlitProvider>\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js` & `st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.3/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map` & `st_selection_header-0.0.4/st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map`

 * *Files identical despite different names*

### Comparing `st-selection-header-0.0.3/st_selection_header.egg-info/SOURCES.txt` & `st_selection_header-0.0.4/st_selection_header.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 st_selection_header.egg-info/requires.txt
 st_selection_header.egg-info/top_level.txt
 st_selection_header/frontend/build/asset-manifest.json
 st_selection_header/frontend/build/index.html
 st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js
 st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.LICENSE.txt
 st_selection_header/frontend/build/static/js/2.0a2a2974.chunk.js.map
-st_selection_header/frontend/build/static/js/main.858e53a4.chunk.js
-st_selection_header/frontend/build/static/js/main.858e53a4.chunk.js.map
+st_selection_header/frontend/build/static/js/main.2185bd8c.chunk.js
+st_selection_header/frontend/build/static/js/main.2185bd8c.chunk.js.map
 st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js
 st_selection_header/frontend/build/static/js/runtime-main.39defc4e.js.map
```

