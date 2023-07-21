# Comparing `tmp/selectable_text-0.0.1.tar.gz` & `tmp/selectable_text-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selectable_text-0.0.1.tar", last modified: Fri Jul 21 20:12:58 2023, max compression
+gzip compressed data, was "selectable_text-0.0.2.tar", last modified: Fri Jul 21 20:29:21 2023, max compression
```

## Comparing `selectable_text-0.0.1.tar` & `selectable_text-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:12:58.172139 selectable_text-0.0.1/
--rw-r--r--   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:00:05.000000 selectable_text-0.0.1/LICENSE
--rw-r--r--   0 johnlithio   (501) staff       (20)      383 2023-07-21 20:00:05.000000 selectable_text-0.0.1/MANIFEST.in
--rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-21 20:12:58.171995 selectable_text-0.0.1/PKG-INFO
--rw-r--r--   0 johnlithio   (501) staff       (20)     3665 2023-07-21 20:00:05.000000 selectable_text-0.0.1/README.md
--rw-r--r--   0 johnlithio   (501) staff       (20)     1749 2023-07-21 20:00:36.000000 selectable_text-0.0.1/package.json
-drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:12:58.171234 selectable_text-0.0.1/selectable_text/
--rw-r--r--   0 johnlithio   (501) staff       (20)     1531 2023-07-21 20:09:14.000000 selectable_text-0.0.1/selectable_text/SelectableText.py
--rw-r--r--   0 johnlithio   (501) staff       (20)     2259 2023-07-21 20:00:05.000000 selectable_text-0.0.1/selectable_text/__init__.py
--rw-r--r--   0 johnlithio   (501) staff       (20)       78 2023-07-21 20:09:14.000000 selectable_text-0.0.1/selectable_text/_imports_.py
--rw-r--r--   0 johnlithio   (501) staff       (20)     1132 2023-07-21 20:09:14.000000 selectable_text-0.0.1/selectable_text/metadata.json
--rw-r--r--   0 johnlithio   (501) staff       (20)     1749 2023-07-21 20:09:13.000000 selectable_text-0.0.1/selectable_text/package-info.json
--rw-r--r--   0 johnlithio   (501) staff       (20)     3791 2023-07-21 20:09:13.000000 selectable_text-0.0.1/selectable_text/selectable_text.min.js
--rw-r--r--   0 johnlithio   (501) staff       (20)     7891 2023-07-21 20:09:13.000000 selectable_text-0.0.1/selectable_text/selectable_text.min.js.map
-drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:12:58.171811 selectable_text-0.0.1/selectable_text.egg-info/
--rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-21 20:12:58.000000 selectable_text-0.0.1/selectable_text.egg-info/PKG-INFO
--rw-r--r--   0 johnlithio   (501) staff       (20)      444 2023-07-21 20:12:58.000000 selectable_text-0.0.1/selectable_text.egg-info/SOURCES.txt
--rw-r--r--   0 johnlithio   (501) staff       (20)        1 2023-07-21 20:12:58.000000 selectable_text-0.0.1/selectable_text.egg-info/dependency_links.txt
--rw-r--r--   0 johnlithio   (501) staff       (20)       16 2023-07-21 20:12:58.000000 selectable_text-0.0.1/selectable_text.egg-info/top_level.txt
--rw-r--r--   0 johnlithio   (501) staff       (20)       38 2023-07-21 20:12:58.172184 selectable_text-0.0.1/setup.cfg
--rw-r--r--   0 johnlithio   (501) staff       (20)      510 2023-07-21 20:00:05.000000 selectable_text-0.0.1/setup.py
+drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:29:21.015452 selectable_text-0.0.2/
+-rw-r--r--   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:00:05.000000 selectable_text-0.0.2/LICENSE
+-rw-r--r--   0 johnlithio   (501) staff       (20)      383 2023-07-21 20:00:05.000000 selectable_text-0.0.2/MANIFEST.in
+-rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-21 20:29:21.015283 selectable_text-0.0.2/PKG-INFO
+-rw-r--r--   0 johnlithio   (501) staff       (20)     3665 2023-07-21 20:00:05.000000 selectable_text-0.0.2/README.md
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1748 2023-07-21 20:29:06.000000 selectable_text-0.0.2/package.json
+drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:29:21.014402 selectable_text-0.0.2/selectable_text/
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1515 2023-07-21 20:29:16.000000 selectable_text-0.0.2/selectable_text/SelectableText.py
+-rw-r--r--   0 johnlithio   (501) staff       (20)     2259 2023-07-21 20:00:05.000000 selectable_text-0.0.2/selectable_text/__init__.py
+-rw-r--r--   0 johnlithio   (501) staff       (20)       78 2023-07-21 20:29:16.000000 selectable_text-0.0.2/selectable_text/_imports_.py
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1854 2023-07-21 20:29:16.000000 selectable_text-0.0.2/selectable_text/metadata.json
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1748 2023-07-21 20:29:15.000000 selectable_text-0.0.2/selectable_text/package-info.json
+-rw-r--r--   0 johnlithio   (501) staff       (20)     4550 2023-07-21 20:29:15.000000 selectable_text-0.0.2/selectable_text/selectable_text.min.js
+-rw-r--r--   0 johnlithio   (501) staff       (20)     9479 2023-07-21 20:29:15.000000 selectable_text-0.0.2/selectable_text/selectable_text.min.js.map
+drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:29:21.015091 selectable_text-0.0.2/selectable_text.egg-info/
+-rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-21 20:29:20.000000 selectable_text-0.0.2/selectable_text.egg-info/PKG-INFO
+-rw-r--r--   0 johnlithio   (501) staff       (20)      444 2023-07-21 20:29:20.000000 selectable_text-0.0.2/selectable_text.egg-info/SOURCES.txt
+-rw-r--r--   0 johnlithio   (501) staff       (20)        1 2023-07-21 20:29:20.000000 selectable_text-0.0.2/selectable_text.egg-info/dependency_links.txt
+-rw-r--r--   0 johnlithio   (501) staff       (20)       16 2023-07-21 20:29:20.000000 selectable_text-0.0.2/selectable_text.egg-info/top_level.txt
+-rw-r--r--   0 johnlithio   (501) staff       (20)       38 2023-07-21 20:29:21.015502 selectable_text-0.0.2/setup.cfg
+-rw-r--r--   0 johnlithio   (501) staff       (20)      510 2023-07-21 20:00:05.000000 selectable_text-0.0.2/setup.py
```

### Comparing `selectable_text-0.0.1/README.md` & `selectable_text-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `selectable_text-0.0.1/package.json` & `selectable_text-0.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.2'"}*

```diff
@@ -42,9 +42,9 @@
         "build:backends": "dash-generate-components ./src/lib/components selectable_text -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.0.2"
 }
```

### Comparing `selectable_text-0.0.1/selectable_text/__init__.py` & `selectable_text-0.0.2/selectable_text/__init__.py`

 * *Files identical despite different names*

### Comparing `selectable_text-0.0.1/selectable_text/package-info.json` & `selectable_text-0.0.2/selectable_text/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.2'"}*

```diff
@@ -42,9 +42,9 @@
         "build:backends": "dash-generate-components ./src/lib/components selectable_text -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.0.2"
 }
```

### Comparing `selectable_text-0.0.1/selectable_text/selectable_text.min.js` & `selectable_text-0.0.2/selectable_text/selectable_text.min.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,168 +1,197 @@
 (() => {
     "use strict";
-    var e, t = {
-            n: e => {
-                var r = e && e.__esModule ? () => e.default : () => e;
-                return t.d(r, {
-                    a: r
-                }), r
+    var t, e = {
+            n: t => {
+                var n = t && t.__esModule ? () => t.default : () => t;
+                return e.d(n, {
+                    a: n
+                }), n
             },
-            d: (e, r) => {
-                for (var n in r) t.o(r, n) && !t.o(e, n) && Object.defineProperty(e, n, {
+            d: (t, n) => {
+                for (var r in n) e.o(n, r) && !e.o(t, r) && Object.defineProperty(t, r, {
                     enumerable: !0,
-                    get: r[n]
+                    get: n[r]
                 })
             },
-            o: (e, t) => Object.prototype.hasOwnProperty.call(e, t),
-            r: e => {
-                "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
+            o: (t, e) => Object.prototype.hasOwnProperty.call(t, e),
+            r: t => {
+                "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
                     value: "Module"
-                }), Object.defineProperty(e, "__esModule", {
+                }), Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
             }
         },
-        r = function() {
-            var e = document.currentScript;
-            if (!e) {
-                for (var t = document.getElementsByTagName("script"), r = [], n = 0; n < t.length; n++) r.push(t[n]);
-                e = (r = r.filter((function(e) {
-                    return !e.async && !e.text && !e.textContent
+        n = function() {
+            var t = document.currentScript;
+            if (!t) {
+                for (var e = document.getElementsByTagName("script"), n = [], r = 0; r < e.length; r++) n.push(e[r]);
+                t = (n = n.filter((function(t) {
+                    return !t.async && !t.text && !t.textContent
                 }))).slice(-1)[0]
             }
-            return e
+            return t
         };
-    if (Object.defineProperty(t, "p", {
-            get: (e = r().src.split("/").slice(0, -1).join("/") + "/", function() {
-                return e
+    if (Object.defineProperty(e, "p", {
+            get: (t = n().src.split("/").slice(0, -1).join("/") + "/", function() {
+                return t
             })
         }), "undefined" != typeof jsonpScriptSrc) {
-        var n = jsonpScriptSrc;
-        jsonpScriptSrc = function(e) {
-            var t, o = (t = r(), /\/_dash-component-suites\//.test(t.src)),
-                i = n(e);
+        var r = jsonpScriptSrc;
+        jsonpScriptSrc = function(t) {
+            var e, o = (e = n(), /\/_dash-component-suites\//.test(e.src)),
+                i = r(t);
             if (!o) return i;
             var c = i.split("/"),
                 u = c.slice(-1)[0].split(".");
-            return u.splice(1, 0, "v0_0_1m1689970153"), c.splice(-1, 1, u.join(".")), c.join("/")
+            return u.splice(1, 0, "v0_0_2m1689971355"), c.splice(-1, 1, u.join(".")), c.join("/")
         }
     }
     var o = {};
-    t.r(o), t.d(o, {
-        SelectableText: () => y
+    e.r(o), e.d(o, {
+        SelectableText: () => d
     });
     const i = window.React;
-    var c = t.n(i);
+    var c = e.n(i);
     const u = window.PropTypes;
-    var f = t.n(u);
+    var s = e.n(u);
 
-    function l(e) {
-        return l = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-            return typeof e
-        } : function(e) {
-            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, l(e)
+    function l(t) {
+        return l = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+            return typeof t
+        } : function(t) {
+            return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
+        }, l(t)
     }
 
-    function a(e, t) {
-        for (var r = 0; r < t.length; r++) {
-            var n = t[r];
-            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, (void 0, o = function(e, t) {
-                if ("object" !== l(e) || null === e) return e;
-                var r = e[Symbol.toPrimitive];
-                if (void 0 !== r) {
-                    var n = r.call(e, "string");
-                    if ("object" !== l(n)) return n;
+    function p(t, e) {
+        for (var n = 0; n < e.length; n++) {
+            var r = e[n];
+            r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(t, (void 0, o = function(t, e) {
+                if ("object" !== l(t) || null === t) return t;
+                var n = t[Symbol.toPrimitive];
+                if (void 0 !== n) {
+                    var r = n.call(t, "string");
+                    if ("object" !== l(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
-                return String(e)
-            }(n.key), "symbol" === l(o) ? o : String(o)), n)
+                return String(t)
+            }(r.key), "symbol" === l(o) ? o : String(o)), r)
         }
         var o
     }
 
-    function p(e, t) {
-        return p = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
-            return e.__proto__ = t, e
-        }, p(e, t)
+    function f(t, e) {
+        return f = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(t, e) {
+            return t.__proto__ = e, t
+        }, f(t, e)
     }
 
-    function s(e) {
-        return s = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
-            return e.__proto__ || Object.getPrototypeOf(e)
-        }, s(e)
+    function a(t) {
+        return a = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
+            return t.__proto__ || Object.getPrototypeOf(t)
+        }, a(t)
     }
-    var y = function(e) {
-        ! function(e, t) {
-            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-            e.prototype = Object.create(t && t.prototype, {
+    var d = function(t) {
+        ! function(t, e) {
+            if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function");
+            t.prototype = Object.create(e && e.prototype, {
                 constructor: {
-                    value: e,
+                    value: t,
                     writable: !0,
                     configurable: !0
                 }
-            }), Object.defineProperty(e, "prototype", {
+            }), Object.defineProperty(t, "prototype", {
                 writable: !1
-            }), t && p(e, t)
-        }(u, e);
-        var t, r, n, o, i = (n = u, o = function() {
+            }), e && f(t, e)
+        }(u, t);
+        var e, n, r, o, i = (r = u, o = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-            } catch (e) {
+            } catch (t) {
                 return !1
             }
         }(), function() {
-            var e, t = s(n);
+            var t, e = a(r);
             if (o) {
-                var r = s(this).constructor;
-                e = Reflect.construct(t, arguments, r)
-            } else e = t.apply(this, arguments);
-            return function(e, t) {
-                if (t && ("object" === l(t) || "function" == typeof t)) return t;
-                if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                return function(e) {
-                    if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                    return e
-                }(e)
-            }(this, e)
+                var n = a(this).constructor;
+                t = Reflect.construct(e, arguments, n)
+            } else t = e.apply(this, arguments);
+            return function(t, e) {
+                if (e && ("object" === l(e) || "function" == typeof e)) return e;
+                if (void 0 !== e) throw new TypeError("Derived constructors may only return object or undefined");
+                return function(t) {
+                    if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                    return t
+                }(t)
+            }(this, t)
         });
 
         function u() {
-            return function(e, t) {
-                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+            return function(t, e) {
+                if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
             }(this, u), i.apply(this, arguments)
         }
-        return t = u, (r = [{
+        return e = u, n = [{
+            key: "mouseEvent",
+            value: function() {
+                var t = "";
+                if (window.getSelection && (t = window.getSelection().toString()), !t || !t.length) return !1;
+                this.props.setProps({
+                    selected_text: t,
+                    selection_start: window.getSelection().anchorOffset
+                })
+            }
+        }, {
+            key: "onMouseUp",
+            value: function(t) {
+                var e, n, r = this;
+                (e = function() {
+                    r.doucleckicked ? (r.doucleckicked = !1, r.dismissMouseUp++) : r.dismissMouseUp > 0 ? r.dismissMouseUp-- : r.mouseEvent.bind(r)()
+                }, 200, function() {
+                    var t = this,
+                        r = arguments;
+                    clearTimeout(n), n = setTimeout((function() {
+                        n = null, e.apply(t, r)
+                    }), 200)
+                }).bind(this)()
+            }
+        }, {
+            key: "onDoubleClick",
+            value: function(t) {
+                t.stopPropagation(), this.doucleckicked = !0, this.mouseEvent.bind(this)()
+            }
+        }, {
             key: "render",
             value: function() {
-                var e = this.props,
-                    t = e.id,
-                    r = e.label,
-                    n = e.setProps,
-                    o = e.value;
                 return c().createElement("div", {
-                    id: t
-                }, "ExampleComponent: ", r, " ", c().createElement("input", {
-                    value: o,
-                    onChange: function(e) {
-                        return n({
-                            value: e.target.value
-                        })
-                    }
-                }))
+                    id: this.props.id,
+                    style: {
+                        whiteSpace: "pre-wrap",
+                        display: "inline-block",
+                        verticalAlign: "text-top",
+                        margin: "10px",
+                        width: this.props.width
+                    },
+                    onMouseUp: this.onMouseUp.bind(this),
+                    onDoubleClick: this.onDoubleClick.bind(this)
+                }, this.props.text)
             }
-        }]) && a(t.prototype, r), Object.defineProperty(t, "prototype", {
+        }], n && p(e.prototype, n), Object.defineProperty(e, "prototype", {
             writable: !1
         }), u
     }(i.Component);
-    y.defaultProps = {}, y.propTypes = {
-        id: f().string,
-        label: f().string.isRequired,
-        value: f().string,
-        setProps: f().func
+    d.defaultProps = {}, d.propTypes = {
+        id: s().string,
+        width: s().string,
+        text: s().string.isRequired,
+        selected_text: s().string,
+        selection_start: s().number,
+        selection_end: s().number,
+        setProps: s().func
     }, window.selectable_text = o
 })();
 //# sourceMappingURL=selectable_text.min.js.map
```

### Comparing `selectable_text-0.0.1/selectable_text/selectable_text.min.js.map` & `selectable_text-0.0.2/selectable_text/selectable_text.min.js.map`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.878087598675834%*

 * *Differences: {"'mappings'": "'mBACA,IC2BYA,ED3BRC,EAAsB,CEA1BA,EAAyBC,IACxB,IAAIC,EAASD,GAAUA,EAAOE,WAC7B,IAAOF,EAAiB,QACxB,IAAM,EAEP,OADAD,EAAoBI,EAAEF,EAAQ,CAAEG,EAAGH,IAC5BA,CAAM,ECLdF,EAAwB,CAACM,EAASC,KACjC,IAAI,IAAIC,KAAOD,EACXP,EAAoBS,EAAEF,EAAYC,KAASR,EAAoBS,EAAEH,EAASE,IAC5EE,OAAOC,eAAeL,EAASE,EAAK,CAAEI,YAAY,EAAMC,IAAKN,EAAWC,IAE1E,ECNDR,EAAwB,CAACc,EAAKC,IAAUL,OAAOM,UAAUC,eAAeC,KAAKJ,EAAKC,GCClFf,EAAyBM,IACH,oBAAXa,QAA0BA,OAAOC,aAC1CV,OAAOC,eAAeL,EAASa,OAAOC,YAAa,CAAEC,MAAO,WAE7DX,OAAOC,eAAeL,EAAS,aAAc,CAAEe, […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "selectable_text.min.js",
-    "mappings": "mBACA,IC2BYA,ED3BRC,EAAsB,CEA1BA,EAAyBC,IACxB,IAAIC,EAASD,GAAUA,EAAOE,WAC7B,IAAOF,EAAiB,QACxB,IAAM,EAEP,OADAD,EAAoBI,EAAEF,EAAQ,CAAEG,EAAGH,IAC5BA,CAAM,ECLdF,EAAwB,CAACM,EAASC,KACjC,IAAI,IAAIC,KAAOD,EACXP,EAAoBS,EAAEF,EAAYC,KAASR,EAAoBS,EAAEH,EAASE,IAC5EE,OAAOC,eAAeL,EAASE,EAAK,CAAEI,YAAY,EAAMC,IAAKN,EAAWC,IAE1E,ECNDR,EAAwB,CAACc,EAAKC,IAAUL,OAAOM,UAAUC,eAAeC,KAAKJ,EAAKC,GCClFf,EAAyBM,IACH,oBAAXa,QAA0BA,OAAOC,aAC1CV,OAAOC,eAAeL,EAASa,OAAOC,YAAa,CAAEC,MAAO,WAE7DX,OAAOC,eAAeL,EAAS,aAAc,CAAEe,OAAO,GAAO,GJL1DC,EAAmB,WACnB,IAAIC,EAASC,SAASC,cACtB,IAAKF,EAAQ,CAOT,IAHA,IAAIG,EAAcF,SAASG,qBAAqB,UAC5CC,EAAU,GAELC,EAAI,EAAGA,EAAIH,EAAYI,OAAQD,IACpCD,EAAQG,KAAKL,EAAYG,IAI7BN,GADAK,EAAUA,EAAQI,QAAO,SAASC,GAAK,OAAQA,EAAEC,QAAUD,EAAEE,OAASF,EAAEG,WAAa,KACpEC,OAAO,GAAG,EAC/B,CAEA,OAAOd,CACX,EAkBA,GAZAb,OAAOC,eAAeX,EAAqB,IAAK,CAC5Ca,KAGQd,EAFSuB,IAEIgB,IAAIC,MAAM,KAAKF,MAAM,GAAI,GAAGG,KAAK,KAAO,IAElD,WACH,OAAOzC,CACX,KAIsB,oBAAnB0C,eAAgC,CACvC,IAAIC,EAAqBD,eACzBA,eAAiB,SAASE,GACtB,IAnBqBpB,EAoBjBqB,GApBiBrB,EAmBRD,IAlBV,6BAA6BuB,KAAKtB,EAAOe,MAqBxCA,EAAMI,EAAmBC,GAE7B,IAAIC,EACA,OAAON,EAGX,IAAIQ,EAAeR,EAAIC,MAAM,KACzBQ,EAAgBD,EAAaT,OAAO,GAAG,GAAGE,MAAM,KAKpD,OAHAQ,EAAcC,OAAO,EAAG,EAAG,qBAC3BF,EAAaE,QAAQ,EAAG,EAAGD,EAAcP,KAAK,MAEvCM,EAAaN,KAAK,IAC7B,CACJ,C,8CKxDA,MAAM,EAA+BS,OAAc,M,aCAnD,MAAM,EAA+BA,OAAkB,U,k7BCGvD,IAOqBC,EAAc,SAAAC,I,qRAAAC,CAAAF,EAAAC,GAAA,I,QAAAE,G,EAAAH,E,qrBAAA,SAAAA,IAAA,O,4FAAAI,CAAA,KAAAJ,GAAAG,EAAAE,MAAA,KAAAC,UAAA,CAwB9B,O,EAxB8BN,G,EAAA,EAAA1C,IAAA,SAAAa,MAC/B,WACI,IAAAoC,EAAuCC,KAAKC,MAApCC,EAAEH,EAAFG,GAAIC,EAAKJ,EAALI,MAAOC,EAAQL,EAARK,SAAUzC,EAAKoC,EAALpC,MAE7B,OACI0C,IAAAA,cAAA,OAAKH,GAAIA,GAAI,qBACUC,EAAM,IACzBE,IAAAA,cAAA,SACI1C,MAAOA,EACP2C,SAUI,SAAAC,GAAC,OAAIH,EAAS,CAAEzC,MAAO4C,EAAEC,OAAO7C,OAAQ,IAK5D,M,oEAAC6B,CAAA,CAxB8B,CAASiB,EAAAA,WA2B5CjB,EAAekB,aAAe,CAAC,EAE/BlB,EAAemB,UAAY,CAIvBT,GAAIU,IAAAA,OAKJT,MAAOS,IAAAA,OAAiBC,WAKxBlD,MAAOiD,IAAAA,OAMPR,SAAUQ,IAAAA,M",
+    "mappings": "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",
     "names": [
         "url",
         "__webpack_require__",
         "module",
         "getter",
         "__esModule",
         "d",
@@ -56,29 +56,52 @@
         "SelectableText",
         "_Component",
         "_inherits",
         "_super",
         "_classCallCheck",
         "apply",
         "arguments",
-        "_this$props",
+        "getSelection",
+        "toString",
         "this",
         "props",
-        "id",
-        "label",
         "setProps",
+        "selected_text",
+        "selection_start",
+        "anchorOffset",
+        "event",
+        "func",
+        "timeout",
+        "_this",
+        "doucleckicked",
+        "dismissMouseUp",
+        "mouseEvent",
+        "bind",
+        "context",
+        "args",
+        "clearTimeout",
+        "setTimeout",
+        "debounce",
+        "stopPropagation",
         "React",
-        "onChange",
-        "e",
-        "target",
+        "id",
+        "style",
+        "whiteSpace",
+        "display",
+        "verticalAlign",
+        "margin",
+        "width",
+        "onMouseUp",
+        "onDoubleClick",
         "Component",
         "defaultProps",
         "propTypes",
         "PropTypes",
-        "isRequired"
+        "isRequired",
+        "selection_end"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///webpack/bootstrap",
         "webpack:///webpack/runtime/compat",
         "webpack:///webpack/runtime/compat get default export",
         "webpack:///webpack/runtime/define property getters",
@@ -86,18 +109,18 @@
         "webpack:///webpack/runtime/make namespace object",
         "webpack:///external window \"React\"",
         "webpack:///external window \"PropTypes\"",
         "webpack:///./src/lib/components/SelectableText.react.js"
     ],
     "sourcesContent": [
         "// The require scope\nvar __webpack_require__ = {};\n\n",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_1m1689970153\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_2m1689971355\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"React\"];",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
-        "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * ExampleComponent is an example component.\n * It takes a property, `label`, and\n * displays it.\n * It renders an input with the property `value`\n * which is editable by the user.\n */\nexport default class SelectableText extends Component {\n    render() {\n        const { id, label, setProps, value } = this.props;\n\n        return (\n            <div id={id}>\n                ExampleComponent: {label}&nbsp;\n                <input\n                    value={value}\n                    onChange={\n                        /*\n                         * Send the new value to the parent component.\n                         * setProps is a prop that is automatically supplied\n                         * by dash's front-end (\"dash-renderer\").\n                         * In a Dash app, this will update the component's\n                         * props and send the data back to the Python Dash\n                         * app server if a callback uses the modified prop as\n                         * Input or State.\n                         */\n                        e => setProps({ value: e.target.value })\n                    }\n                />\n            </div>\n        );\n    }\n}\n\nSelectableText.defaultProps = {};\n\nSelectableText.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * A label that will be printed when this component is rendered.\n     */\n    label: PropTypes.string.isRequired,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.string,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n"
+        "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n\nfunction debounce(func, wait, immediate) {\n    let timeout;\n\n    return function () {\n        const context = this, args = arguments;\n        const later = () => {\n            timeout = null;\n            if (!immediate) func.apply(context, args);\n        };\n        const callNow = immediate && !timeout;\n\n        clearTimeout(timeout);\n        timeout = setTimeout(later, wait);\n        if (callNow) func.apply(context, args);\n    };\n}\n\n\nexport default class SelectableText extends Component {\n\n    mouseEvent() {\n\n        let text = '';\n\n        if (window.getSelection) {\n            text = window.getSelection().toString();\n        }\n\n        if (!text || !text.length) {\n            return false;\n        }\n\n        this.props.setProps({\n            selected_text: text,\n            selection_start: window.getSelection().anchorOffset,\n        })\n    }\n\n    onMouseUp(event) {\n        debounce(() => {\n            if (this.doucleckicked) {\n                this.doucleckicked = false;\n                this.dismissMouseUp++;\n            } else if (this.dismissMouseUp > 0) {\n                this.dismissMouseUp--;\n            } else {\n                this.mouseEvent.bind(this)();\n            }\n        }, 200).bind(this)();\n    }\n\n    onDoubleClick(event) {\n        event.stopPropagation();\n\n        this.doucleckicked = true;\n        this.mouseEvent.bind(this)();\n    }\n\n    render() {\n        return (\n            <div id={this.props.id}\n                style={{\n                    whiteSpace: 'pre-wrap',\n                    display: 'inline-block',\n                    verticalAlign: 'text-top',\n                    margin: '10px',\n                    width: this.props.width\n                }}\n                onMouseUp={this.onMouseUp.bind(this)}\n                onDoubleClick={this.onDoubleClick.bind(this)}>\n                {this.props.text}\n            </div>\n        );\n    }\n}\n\nSelectableText.defaultProps = {};\n\nSelectableText.propTypes = {\n    id: PropTypes.string,\n    width: PropTypes.string,\n    text: PropTypes.string.isRequired,\n    selected_text: PropTypes.string,\n    selection_start: PropTypes.number,\n    selection_end: PropTypes.number,\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};"
     ],
     "version": 3
 }
```

