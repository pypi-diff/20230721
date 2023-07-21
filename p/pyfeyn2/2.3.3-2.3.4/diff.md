# Comparing `tmp/pyfeyn2-2.3.3.tar.gz` & `tmp/pyfeyn2-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.3.3.tar", max compression
+gzip compressed data, was "pyfeyn2-2.3.4.tar", max compression
```

## Comparing `pyfeyn2-2.3.3.tar` & `pyfeyn2-2.3.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35149 2023-05-27 22:06:11.091484 pyfeyn2-2.3.3/LICENSE
--rw-r--r--   0        0        0     3115 2023-05-27 22:06:11.091484 pyfeyn2-2.3.3/README.md
--rw-r--r--   0        0        0      154 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2838 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      647 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/diagram.py
--rw-r--r--   0        0        0      768 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0     2068 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0     3335 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2734 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0      279 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0      238 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0     2748 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3626 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3596 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     5926 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1617 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     6922 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     7036 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13245 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41394 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12740 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     9146 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2914 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     8914 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      863 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2364 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1701 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     2114 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      527 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3850 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1976 2023-05-27 22:06:11.171485 pyfeyn2-2.3.3/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2621 2023-05-27 22:06:13.151519 pyfeyn2-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 pyfeyn2-2.3.3/setup.py
--rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 pyfeyn2-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 11:06:02.341584 pyfeyn2-2.3.4/LICENSE
+-rw-r--r--   0        0        0     3115 2023-07-21 11:06:02.341584 pyfeyn2-2.3.4/README.md
+-rw-r--r--   0        0        0      154 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2838 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      647 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/diagram.py
+-rw-r--r--   0        0        0      768 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0     3068 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/auto/reshuffle.py
+-rw-r--r--   0        0        0     3336 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2734 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0      279 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0      238 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0     2911 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     3626 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3596 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     5926 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1617 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     7120 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     7036 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-07-21 11:06:02.421585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13245 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41394 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12740 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     9146 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     8914 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      863 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2364 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1701 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     2114 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      527 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3850 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1976 2023-07-21 11:06:02.425585 pyfeyn2-2.3.4/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2630 2023-07-21 11:06:04.625616 pyfeyn2-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 pyfeyn2-2.3.4/setup.py
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 pyfeyn2-2.3.4/PKG-INFO
```

### Comparing `pyfeyn2-2.3.3/LICENSE` & `pyfeyn2-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/README.md` & `pyfeyn2-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/auto/bend.py` & `pyfeyn2-2.3.4/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/auto/diagram.py` & `pyfeyn2-2.3.4/pyfeyn2/auto/diagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/auto/label.py` & `pyfeyn2-2.3.4/pyfeyn2/auto/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/auto/position.py` & `pyfeyn2-2.3.4/pyfeyn2/auto/position.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,53 @@
 from pyfeyn2.feynmandiagram import Propagator
 from pyfeyn2.interface.dot import dot_to_positions, feynman_to_dot
 
 
+def auto_position(fd, layout="neato", clear_vertices=True):
+    """Automatically position the vertices and legs."""
+    # fd = scale_positions(fd, 10)
+    fd = fd.with_style(f"layout : {layout}")
+    fd = incoming_to_left(fd)
+    fd = outgoing_to_right(fd)
+    fd = feynman_adjust_points(fd, size=5, clear_vertices=clear_vertices)
+    # fd = remove_unnecessary_vertices(fd)
+    return fd
+
+
+def incoming_to_left(fd):
+    """Set the incoming legs to the left."""
+    n = 0
+    for l in fd.legs:
+        if l.is_incoming():
+            l.x = -2
+            n = n + 1
+    i = 0
+    for l in fd.legs:
+        if l.is_incoming():
+            l.y = 4 / n * i
+            i = i + 1
+
+    return fd
+
+
+def outgoing_to_right(fd):
+    """Set the outgoing legs to the right."""
+    n = 0
+    for l in fd.legs:
+        if not l.is_incoming():
+            l.x = 2
+            n = n + 1
+    i = 0
+    for l in fd.legs:
+        if not l.is_incoming():
+            l.y = 4 / n * i
+            i = i + 1
+    return fd
+
+
 def scale_positions(fd, scale):
     """Scale the positions of the vertices and legs."""
     for v in fd.vertices:
         v.x *= scale
         v.y *= scale
     return fd
```

### Comparing `pyfeyn2-2.3.3/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.3.4/pyfeyn2/feynmandiagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,9 +109,9 @@
 class FeynML(FeynML_):
     """FeynML with pyfeyn2 meta tag."""
 
     class Meta(FeynML_.Meta):
         pass
 
     def __post_init__(self):
-        self.head.metas.append(Meta("pyfeyn2", version("pyfeyn2")))
+        self.head.metas.append(Meta_("pyfeyn2", version("pyfeyn2")))
         return super().__post_init__()
```

### Comparing `pyfeyn2-2.3.3/pyfeyn2/interface/dot.py` & `pyfeyn2-2.3.4/pyfeyn2/interface/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/mkfeyndiag.py` & `pyfeyn2-2.3.4/pyfeyn2/mkfeyndiag.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,21 @@
         help="CSS like Style file to use.",
     )
     parser.add_argument(
         "--show",
         action="store_true",
         help="Show the output file.",
     )
+    parser.add_argument(
+        "--diagram",
+        metavar="DIAGRAM",
+        default=None,
+        type=str,
+        help="Diagram id to render.",
+    )
 
     args = parser.parse_args()
 
     arenderer = args.renderer
     renderer = None
     if arenderer is None:
         pass
@@ -88,10 +95,10 @@
         arenderer = fml.head.get_meta_dict()["renderer"]
         renderer = renderer_from_string(arenderer)
     if args.style is not None:
         style_string = Path(args.style).read_text()
         for diagram in fml.diagrams:
             diagram.external_sheet = cssutils.parseString(style_string)
 
-    # TODO think about how to handle multiple diagrams
     for i, d in enumerate(fml.diagrams):
-        renderer(d).render(file=args.output + f"_{i}", show=args.show)
+        if args.diagram is None or args.diagram == d.id:
+            renderer(d).render(file=args.output + f"_{i}", show=args.show)
```

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/all.py` & `pyfeyn2-2.3.4/pyfeyn2/render/all.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.3.4/pyfeyn2/render/latex/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.3.4/pyfeyn2/render/latex/feynmp.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.3.4/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.3.4/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.3.4/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,21 @@
 
 def stylize_connect(fd: FeynmanDiagram, c: Connector):
     style = fd.get_style(c)
     ret = ""
     if style.getProperty("line") is not None:
         ret += type_map[style.getProperty("line").value]
     else:
-        ret += type_map[c.type]  # fallback to type if no style
+        if c.type is not None:
+            ret += type_map[c.type]  # fallback to type if no style
+        else:
+            warnings.warn(
+                f"No type or style set for connector  {c.id} {c.type} {c.pdgid}"
+            )
+            ret += "plain"
 
     if c.label is not None:
         ret += ",edge label=" + c.label
     # if c.edge_label_ is not None: style += ",edge label'=" + c.edge_label_
     if (
         style.getProperty("momentum-arrow") is not None
         and style.getProperty("momentum-arrow").value == "true"
```

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.3.4/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/lines.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/pyxrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.3.4/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/render.py` & `pyfeyn2-2.3.4/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/ascii.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/label.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/line.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/plainpdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/point.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/point.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/style.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.3.4/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.3/pyproject.toml` & `pyfeyn2-2.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.3.3"
+version = "2.3.4"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -64,15 +64,15 @@
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.20,<4.0"
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.1"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.26.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `pyfeyn2-2.3.3/setup.py` & `pyfeyn2-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.3.3',
+    'version': '2.3.4',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
     'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (graphviz)\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
```

### Comparing `pyfeyn2-2.3.3/PKG-INFO` & `pyfeyn2-2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.3.3
+Version: 2.3.4
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

