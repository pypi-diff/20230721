# Comparing `tmp/cupcake_editor-0.25.5.tar.gz` & `tmp/cupcake-editor-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake_editor-0.25.5.tar", max compression
+gzip compressed data, was "cupcake-editor-0.5.1.tar", max compression
```

## Comparing `cupcake_editor-0.25.5.tar` & `cupcake-editor-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,64 @@
--rw-r--r--   0        0        0     4480 2023-07-21 13:02:10.728378 cupcake_editor-0.25.5/cupcake/__init__.py
--rw-r--r--   0        0        0     1000 2023-07-21 12:43:34.872738 cupcake_editor-0.25.5/cupcake/breadcrumbs/__init__.py
--rw-r--r--   0        0        0     1287 2023-07-21 12:43:34.873741 cupcake_editor-0.25.5/cupcake/breadcrumbs/pathview.py
--rw-r--r--   0        0        0     1012 2023-07-21 12:43:34.874740 cupcake_editor-0.25.5/cupcake/config/__init__.py
--rw-r--r--   0        0        0     3035 2023-07-21 12:43:34.889740 cupcake_editor-0.25.5/cupcake/config/dark.toml
--rw-r--r--   0        0        0     3017 2023-07-21 12:58:47.832566 cupcake_editor-0.25.5/cupcake/config/light.toml
--rw-r--r--   0        0        0      518 2023-07-21 12:43:34.902739 cupcake_editor-0.25.5/cupcake/config/stipple.xbm
--rw-r--r--   0        0        0     5585 2023-07-21 12:43:34.903739 cupcake_editor-0.25.5/cupcake/config/styles.py
--rw-r--r--   0        0        0     5625 2023-07-21 12:43:34.912736 cupcake_editor-0.25.5/cupcake/diffeditor/__init__.py
--rw-r--r--   0        0        0      283 2023-07-21 12:43:34.914746 cupcake_editor-0.25.5/cupcake/diffeditor/differ.py
--rw-r--r--   0        0        0      376 2023-07-21 12:43:34.915743 cupcake_editor-0.25.5/cupcake/diffeditor/pane.py
--rw-r--r--   0        0        0      513 2023-07-21 12:43:34.916744 cupcake_editor-0.25.5/cupcake/editor.py
--rw-r--r--   0        0        0      634 2023-07-21 12:43:34.917741 cupcake_editor-0.25.5/cupcake/imageviewer/__init__.py
--rw-r--r--   0        0        0    13726 2023-07-21 12:43:34.948833 cupcake_editor-0.25.5/cupcake/languages.py
--rw-r--r--   0        0        0     7305 2023-07-21 12:43:34.949832 cupcake_editor-0.25.5/cupcake/texteditor/__init__.py
--rw-r--r--   0        0        0     4736 2023-07-21 12:43:34.966831 cupcake_editor-0.25.5/cupcake/texteditor/autocomplete/__init__.py
--rw-r--r--   0        0        0     2576 2023-07-21 12:43:34.976991 cupcake_editor-0.25.5/cupcake/texteditor/autocomplete/item.py
--rw-r--r--   0        0        0     1251 2023-07-21 12:43:34.978009 cupcake_editor-0.25.5/cupcake/texteditor/autocomplete/kind.py
--rw-r--r--   0        0        0     6472 2023-07-21 12:43:34.989742 cupcake_editor-0.25.5/cupcake/texteditor/autocomplete/kinds.py
--rw-r--r--   0        0        0     2221 2023-07-21 12:43:35.012762 cupcake_editor-0.25.5/cupcake/texteditor/highlighter.py
--rw-r--r--   0        0        0     2031 2023-07-21 12:43:35.015768 cupcake_editor-0.25.5/cupcake/texteditor/linenumbers/__init__.py
--rw-r--r--   0        0        0     1252 2023-07-21 12:43:35.016764 cupcake_editor-0.25.5/cupcake/texteditor/linenumbers/breakpoint.py
--rw-r--r--   0        0        0     3021 2023-07-21 12:43:35.017763 cupcake_editor-0.25.5/cupcake/texteditor/minimap.py
--rw-r--r--   0        0        0      193 2023-07-21 12:43:35.019763 cupcake_editor-0.25.5/cupcake/texteditor/syntax.py
--rw-r--r--   0        0        0    17076 2023-07-21 12:43:35.033060 cupcake_editor-0.25.5/cupcake/texteditor/text.py
--rw-r--r--   0        0        0      521 2023-07-21 12:43:35.034060 cupcake_editor-0.25.5/cupcake/utils/__init__.py
--rw-r--r--   0        0        0      216 2023-07-21 12:43:35.035063 cupcake_editor-0.25.5/cupcake/utils/canvas.py
--rw-r--r--   0        0        0     3289 2023-07-21 12:43:35.046217 cupcake_editor-0.25.5/cupcake/utils/directorytree.py
--rw-r--r--   0        0        0      234 2023-07-21 12:43:35.047211 cupcake_editor-0.25.5/cupcake/utils/filetype.py
--rw-r--r--   0        0        0      279 2023-07-21 12:43:35.049212 cupcake_editor-0.25.5/cupcake/utils/frame.py
--rw-r--r--   0        0        0      214 2023-07-21 12:43:35.050206 cupcake_editor-0.25.5/cupcake/utils/label.py
--rw-r--r--   0        0        0      224 2023-07-21 12:43:35.051208 cupcake_editor-0.25.5/cupcake/utils/menubutton.py
--rw-r--r--   0        0        0     1503 2023-07-21 12:43:35.053210 cupcake_editor-0.25.5/cupcake/utils/scrollableframe.py
--rw-r--r--   0        0        0      263 2023-07-21 12:43:35.054209 cupcake_editor-0.25.5/cupcake/utils/scrollbar.py
--rw-r--r--   0        0        0      270 2023-07-21 12:43:35.055208 cupcake_editor-0.25.5/cupcake/utils/text.py
--rw-r--r--   0        0        0      220 2023-07-21 12:43:35.055208 cupcake_editor-0.25.5/cupcake/utils/toplevel.py
--rw-r--r--   0        0        0     2886 2023-07-21 12:43:35.057214 cupcake_editor-0.25.5/cupcake/utils/tree.py
--rw-r--r--   0        0        0     1093 2023-07-20 17:23:12.850580 cupcake_editor-0.25.5/LICENSE
--rw-r--r--   0        0        0      548 2023-07-21 13:36:31.300349 cupcake_editor-0.25.5/pyproject.toml
--rw-r--r--   0        0        0     2486 2023-07-21 12:45:54.091252 cupcake_editor-0.25.5/README.md
--rw-r--r--   0        0        0     2945 1970-01-01 00:00:00.000000 cupcake_editor-0.25.5/PKG-INFO
+-rw-r--r--   0        0        0       53 2022-06-15 20:37:25.646469 cupcake-editor-0.5.1/cupcake/__init__.py
+-rw-r--r--   0        0        0      228 2022-06-15 20:20:04.770629 cupcake-editor-0.5.1/cupcake/config/__init__.py
+-rw-r--r--   0        0        0      574 2022-05-21 11:11:55.024996 cupcake-editor-0.5.1/cupcake/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       54 2022-05-21 11:11:16.714520 cupcake-editor-0.5.1/cupcake/config/languages/__init__.py
+-rw-r--r--   0        0        0      235 2022-05-21 11:11:55.118136 cupcake-editor-0.5.1/cupcake/config/languages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2212 2022-05-21 11:11:55.138206 cupcake-editor-0.5.1/cupcake/config/languages/__pycache__/cpp.cpython-310.pyc
+-rw-r--r--   0        0        0      416 2022-05-21 11:11:55.120883 cupcake-editor-0.5.1/cupcake/config/languages/__pycache__/language.cpython-310.pyc
+-rw-r--r--   0        0        0     2828 2022-05-21 11:11:16.716515 cupcake-editor-0.5.1/cupcake/config/languages/cpp.py
+-rw-r--r--   0        0        0       95 2022-05-21 11:11:16.716515 cupcake-editor-0.5.1/cupcake/config/languages/language.py
+-rw-r--r--   0        0        0     2662 2022-06-15 20:20:04.771628 cupcake-editor-0.5.1/cupcake/editor/__init__.py
+-rw-r--r--   0        0        0     2736 2022-05-25 08:02:10.370766 cupcake-editor-0.5.1/cupcake/editor/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      871 2022-05-25 07:37:38.467977 cupcake-editor-0.5.1/cupcake/editor/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0        0        0     1720 2022-05-21 11:11:55.163188 cupcake-editor-0.5.1/cupcake/editor/__pycache__/highlighter.cpython-310.pyc
+-rw-r--r--   0        0        0     3111 2022-05-25 07:37:38.475973 cupcake-editor-0.5.1/cupcake/editor/__pycache__/minimap.cpython-310.pyc
+-rw-r--r--   0        0        0     2876 2022-05-25 07:37:38.479969 cupcake-editor-0.5.1/cupcake/editor/__pycache__/scrollbar.cpython-310.pyc
+-rw-r--r--   0        0        0    10965 2022-06-15 19:12:04.211093 cupcake-editor-0.5.1/cupcake/editor/__pycache__/text.cpython-310.pyc
+-rw-r--r--   0        0        0     3702 2022-05-21 11:11:55.285705 cupcake-editor-0.5.1/cupcake/editor/__pycache__/textw.cpython-310.pyc
+-rw-r--r--   0        0        0     5005 2022-06-15 20:20:04.772629 cupcake-editor-0.5.1/cupcake/editor/autocomplete/__init__.py
+-rw-r--r--   0        0        0     6042 2022-05-25 09:12:44.839979 cupcake-editor-0.5.1/cupcake/editor/autocomplete/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4160 2022-05-21 11:11:55.201143 cupcake-editor-0.5.1/cupcake/editor/autocomplete/__pycache__/item.cpython-310.pyc
+-rw-r--r--   0        0        0     6623 2022-05-21 11:11:55.186977 cupcake-editor-0.5.1/cupcake/editor/autocomplete/__pycache__/itemkinds.cpython-310.pyc
+-rw-r--r--   0        0        0     3726 2022-05-21 11:11:16.718512 cupcake-editor-0.5.1/cupcake/editor/autocomplete/item.py
+-rw-r--r--   0        0        0     6472 2022-05-21 11:11:16.719510 cupcake-editor-0.5.1/cupcake/editor/autocomplete/itemkinds.py
+-rw-r--r--   0        0        0      404 2022-06-15 20:20:04.773627 cupcake-editor-0.5.1/cupcake/editor/events.py
+-rw-r--r--   0        0        0     1993 2022-06-15 20:20:04.774626 cupcake-editor-0.5.1/cupcake/editor/find_replace/__init__.py
+-rw-r--r--   0        0        0     2630 2022-05-21 11:11:55.301204 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1710 2022-05-21 11:11:55.331600 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0        0        0     3713 2022-05-21 11:11:55.361456 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/container.cpython-310.pyc
+-rw-r--r--   0        0        0     1676 2022-05-21 11:11:55.319712 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/entrybox.cpython-310.pyc
+-rw-r--r--   0        0        0     9862 2022-05-25 07:37:38.565916 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/find_replace.cpython-310.pyc
+-rw-r--r--   0        0        0     2340 2022-05-21 11:11:55.348512 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/findbox.cpython-310.pyc
+-rw-r--r--   0        0        0     1675 2022-05-21 11:11:55.351766 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/replacebox.cpython-310.pyc
+-rw-r--r--   0        0        0     1069 2022-05-21 11:11:55.354409 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/results.cpython-310.pyc
+-rw-r--r--   0        0        0     2703 2022-05-21 11:11:55.358004 cupcake-editor-0.5.1/cupcake/editor/find_replace/__pycache__/togglew.cpython-310.pyc
+-rw-r--r--   0        0        0     1189 2022-05-21 11:11:16.722513 cupcake-editor-0.5.1/cupcake/editor/find_replace/button.py
+-rw-r--r--   0        0        0     3821 2022-05-21 11:11:16.723512 cupcake-editor-0.5.1/cupcake/editor/find_replace/container.py
+-rw-r--r--   0        0        0     1218 2022-05-21 11:11:16.724511 cupcake-editor-0.5.1/cupcake/editor/find_replace/entrybox.py
+-rw-r--r--   0        0        0    10482 2022-06-15 20:20:04.775625 cupcake-editor-0.5.1/cupcake/editor/find_replace/find_replace.py
+-rw-r--r--   0        0        0     2108 2022-05-21 11:11:16.727507 cupcake-editor-0.5.1/cupcake/editor/find_replace/findbox.py
+-rw-r--r--   0        0        0     1318 2022-05-21 11:11:16.728507 cupcake-editor-0.5.1/cupcake/editor/find_replace/replacebox.py
+-rw-r--r--   0        0        0      580 2022-05-21 11:11:16.730508 cupcake-editor-0.5.1/cupcake/editor/find_replace/results.py
+-rw-r--r--   0        0        0     1409 2022-05-21 11:11:16.730508 cupcake-editor-0.5.1/cupcake/editor/find_replace/toggle.py
+-rw-r--r--   0        0        0     2402 2022-05-21 11:11:16.731506 cupcake-editor-0.5.1/cupcake/editor/find_replace/togglew.py
+-rw-r--r--   0        0        0     1674 2022-05-21 11:11:16.732503 cupcake-editor-0.5.1/cupcake/editor/highlighter.py
+-rw-r--r--   0        0        0       34 2022-05-21 11:11:16.733503 cupcake-editor-0.5.1/cupcake/editor/language/__init__.py
+-rw-r--r--   0        0        0      205 2022-05-21 11:11:55.093312 cupcake-editor-0.5.1/cupcake/editor/language/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1520 2022-05-21 11:11:55.116066 cupcake-editor-0.5.1/cupcake/editor/language/__pycache__/syntax.cpython-310.pyc
+-rw-r--r--   0        0        0      321 2022-05-21 11:11:16.733503 cupcake-editor-0.5.1/cupcake/editor/language/languages/__init__.py
+-rw-r--r--   0        0        0      105 2022-05-21 11:11:16.734501 cupcake-editor-0.5.1/cupcake/editor/language/languages/cpp.py
+-rw-r--r--   0        0        0      756 2022-05-21 11:11:16.735502 cupcake-editor-0.5.1/cupcake/editor/language/syntax.py
+-rw-r--r--   0        0        0     1107 2022-05-21 11:11:16.736500 cupcake-editor-0.5.1/cupcake/editor/language/test.py
+-rw-r--r--   0        0        0     2778 2022-06-15 20:20:04.777626 cupcake-editor-0.5.1/cupcake/editor/linenumbers/__init__.py
+-rw-r--r--   0        0        0     3619 2022-05-25 07:39:58.605409 cupcake-editor-0.5.1/cupcake/editor/linenumbers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1686 2022-05-21 11:11:55.068195 cupcake-editor-0.5.1/cupcake/editor/linenumbers/__pycache__/breakpoint.cpython-310.pyc
+-rw-r--r--   0        0        0     1209 2022-05-21 11:11:16.737500 cupcake-editor-0.5.1/cupcake/editor/linenumbers/breakpoint.py
+-rw-r--r--   0        0        0     2806 2022-06-15 20:20:04.778624 cupcake-editor-0.5.1/cupcake/editor/minimap.py
+-rw-r--r--   0        0        0     2505 2022-06-15 20:20:04.779623 cupcake-editor-0.5.1/cupcake/editor/scrollbar.py
+-rw-r--r--   0        0        0    10160 2022-06-15 20:20:04.780623 cupcake-editor-0.5.1/cupcake/editor/text.py
+-rw-r--r--   0        0        0     2969 2022-05-21 11:11:16.744508 cupcake-editor-0.5.1/cupcake/editor/textw.py
+-rw-r--r--   0        0        0     1093 2022-05-18 10:49:24.066411 cupcake-editor-0.5.1/LICENSE
+-rw-r--r--   0        0        0      424 2022-06-15 20:38:02.100379 cupcake-editor-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1835 2022-06-15 20:20:04.767630 cupcake-editor-0.5.1/README.md
+-rw-r--r--   0        0        0     2597 2022-06-15 20:38:20.182980 cupcake-editor-0.5.1/setup.py
+-rw-r--r--   0        0        0     2108 2022-06-15 20:38:20.182980 cupcake-editor-0.5.1/PKG-INFO
```

### Comparing `cupcake_editor-0.25.5/cupcake/breadcrumbs/pathview.py` & `cupcake-editor-0.5.1/cupcake/editor/find_replace/entrybox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-from ..utils import DirectoryTree, Toplevel
+import tkinter as tk
+from tkinter import font
 
 
-class PathView(Toplevel):
-    def __init__(self, master, width=150, *args, **kwargs):
+class EntryBox(tk.Frame):
+    def __init__(self, master, *args, **kwargs):
         super().__init__(master, *args, **kwargs)
-        self.width = round(width)
-        
-        self.tree = DirectoryTree(self, width=width)
-        self.tree.pack()
-
-        self.config(pady=1, padx=1, bg=self.base.theme.border)
-        self.overrideredirect(True)
-        self.withdraw()
+        self.master = master
 
+        self.config(bg="#3c3c3c", padx=1, pady=1)
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(0, weight=1)
-        self.configure_bindings()
 
-    def configure_bindings(self):
-        self.bind("<FocusOut>", self.hide)
-        self.bind("<Escape>", self.hide)
-    
-    def get_popup_x(self, width):
-        return self.winfo_rootx() + int(self.winfo_width() / 2) - int(width / 2)
+        self.term = tk.StringVar()
+
+        self.entry_frame = frame = tk.Frame(self, bg="#3c3c3c")
+        frame.grid(row=0, column=0, sticky=tk.NSEW)
 
-    def get_popup_y(self):
-        return self.winfo_rooty()
+        self.entry = tk.Entry(
+            frame, width=30, bg="#3c3c3c", fg="#ccccc7", font=("Helvetica", 11),
+            textvariable=self.term, relief=tk.FLAT, insertbackground="#aeafad")
+        self.entry.grid(sticky=tk.EW, padx=3, pady=3)
+
+        self.config_bindings()
     
-    def hide(self, *_):
-        self.withdraw()
-        
-    def show(self, e):
+    def get(self):
+        return self.term.get()
+
+    def config_bindings(self, *args): ...
+        # self.entry.bind("<FocusIn>", self.on_focus)
+        # self.entry.bind("<FocusOut>", self.off_focus)
+
+    def on_focus(self, *args):
+        self.update_idletasks()
+        self.config(bg="#007fd4")
+
+    def off_focus(self, *args):
         self.update_idletasks()
-        w = e.widget
-        x = w.winfo_rootx()
-        y = w.winfo_rooty() + w.winfo_height()
-        
-        if not w.path:
-            return
-        self.tree.change_path(w.path)
-
-        self.geometry(f"+{x}+{y}")
-        self.deiconify()
-        self.focus_set()
+        self.config(bg="#3c3c3c")
```

### Comparing `cupcake_editor-0.25.5/cupcake/texteditor/autocomplete/__init__.py` & `cupcake-editor-0.5.1/cupcake/editor/autocomplete/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,100 @@
 import tkinter as tk
-from itertools import chain
 
-from .kinds import Kinds
+from .itemkinds import Kinds
 from .item import AutoCompleteItem
 
-from ...utils import Toplevel
 
-
-class AutoComplete(Toplevel):
+class AutoComplete(tk.Toplevel):
     def __init__(self, master, items=None, active=False, *args, **kwargs):
         super().__init__(master, *args, **kwargs)
+        self.master = master
+
         self.autocomplete_kinds = Kinds(self)
-        self.config(padx=1, pady=1, bg=self.base.theme.border)
+        self.config(bg="#454545", padx=1, pady=1)
         
         self.active = active
+        self.font = self.master.font
+
         if not self.active:
             self.withdraw()
         
         self.overrideredirect(True)
         self.wm_attributes("-topmost", True)
+
         self.grid_columnconfigure(0, weight=1)
 
         self.menu_items = []
         self.active_items = []
+
         self.row = 0
         self.selected = 0
+
         if items:
-            # TODO this should be a dict
-            self.items = items # [(completion, type), ...]
+            self.items = items
+            # [(completion, type), ...]
+            
             self.add_all_items()
             self.refresh_selected()
+        
+        self.configure_bindings()
     
     def update_completions(self):
         self.refresh_geometry()
         self.update_idletasks()
         self.update_all_words()
 
         term = self.master.get_current_word()
 
-        exact, starts, includes = [], [], []
-        for i in self.menu_items:
-            if i.get_text() == term:
-                exact.append(i)
-            elif i.get_text().startswith(term):
-                starts.append(i)
-            elif term in i.get_text():
-                includes.append(i)
-        new = list(chain(exact, starts, includes))
+        new = [i for i in self.get_items() if i.get_text() == term]
+        new += [i for i in self.get_items() if i.get_text().startswith(term)]
+        new += [i for i in self.get_items() if term in i.get_text() and i.get_kind() != "word" and i not in new]
+        new += [i for i in self.get_items() if term in i.get_text() and i not in new]
 
         self.hide_all_items()
+        
         if any(new):
             self.show_items(new[:10] if len(new) > 10 else new, term)
         else:
             self.hide()
     
-    def move_up(self, *_):
+    def move_up(self, *args):
         if self.active:
             self.select(-1)
             return "break"
     
-    def move_down(self, *_):
+    def move_down(self, *args):
         if self.active:
             self.select(1)
             return "break"
 
     def add_all_items(self):
         for i in self.items:
             self.add_item(i[0], i[1] if len(i) > 1 else None) 
             
         self.active_items = self.menu_items
         self.refresh_selected()
     
     def update_all_words(self):
-        for word in self.master.words:
+        for word in self.master.get_all_words():
             if word not in self.get_items_text():
                 self.add_item(word, "word")
         
-        for word in self.menu_items:
-            if word.get_text() not in self.master.words and word.get_kind() == "word":
+        for word in self.get_items():
+            if word.get_text() not in self.master.get_all_words() and word.get_kind() == "word":
                 self.remove_item(word)
 
-    def add_item(self, text, kind=None):
-        new_item = AutoCompleteItem(self, text, kind=kind)
+    def configure_bindings(self):
+        # root.bind("<Button-1>" , self.hide)
+        # root.bind("<Configure>", self.refresh_geometry)
+        # root.bind("<FocusOut>", self.hide)
+        ...
+
+    def add_item(self, left, kind=None):
+        new_item = AutoCompleteItem(self, left, kind=kind)
         new_item.grid(row=self.row, sticky=tk.EW)
         
         self.menu_items.append(new_item)
 
         self.row += 1
     
     def remove_item(self, item):
@@ -107,14 +116,17 @@
         self.refresh_selected()
 
     def refresh_selected(self):
         for i in self.active_items:
             i.deselect()
         if self.selected < len(self.active_items):
             self.active_items[self.selected].select()
+
+    def get_items(self):
+        return self.menu_items
     
     def get_items_text(self):
         return [i.get_text() for i in self.menu_items]
     
     def hide_all_items(self):
         for i in self.menu_items:
             i.grid_forget()
@@ -128,35 +140,32 @@
             i.grid(row=self.row, sticky=tk.EW)
             self.row += 1
 
             i.mark_term(term)
 
         self.reset_selection()
     
-    def refresh_geometry(self, *_):
+    def refresh_geometry(self, *args):
         self.update_idletasks()
         self.geometry("+{}+{}".format(*self.master.cursor_screen_location()))
 
     def show(self, pos):
         self.active = True
         self.update_idletasks()
         self.geometry("+{}+{}".format(*pos))
         self.deiconify()
 
-    def hide(self, *_):
+    def hide(self, *args):
         self.active = False
         self.withdraw()
         self.reset()
     
     def reset(self):
         self.reset_selection()
     
-    def choose(self, this=None, *_):
-        if not self.active_items:
-            return
-        
+    def choose(self, this=None, *args):
+        self.hide()
         if not this:
             this = self.active_items[self.selected]
         
         self.master.confirm_autocomplete(this.get_text())
-        self.hide()
         return "break"
```

### Comparing `cupcake_editor-0.25.5/cupcake/texteditor/autocomplete/kinds.py` & `cupcake-editor-0.5.1/cupcake/editor/autocomplete/itemkinds.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,30 +48,30 @@
         0TuLE2EYxfH/eZLIikkweEFb2xQWostMOhUCUwha+BG0007wEwh22ilabmNpF1CbZCbeECzS2iqsMrmJu2bzvBa
         OQkJMfMr3nB8ceEVxnU7nSLVavQ9cb7VaJ1i6NE13gWfT6fROu93+DmB/wlqt9gC4FEK4uQwBJN0ALha9328Ag8
         Hg0HA4HJnZ5SiK0lUYoN/vt9z9xWg0Opokyb4B5Hl+HNiazWaf/gUBinyrXq8fW5gNYGZah5dzAyiVSqeAAzPLN
         +AcOAghnAZQmqbngYeSduM4vrIOA2RZ9hw4CdwqA2+Bubuf3QQB3P2upI/AG5O0Lem9md37H1z03gEXBNDtds+Z
         2WtJ9TiOf6yZfDiEMDaz7SiKPhiApM9A2d0bGyY3gPJ8Pv8CS1/l7mEDXsgNYDwefwP2KpXKmXW4yPcajcbXvzh
         Jkn1JO+7+JMuyq6tgr9e75u5PJe00m82fC7Mnk8lt4FUI4fEqLOkR8LLoAfALta2R2TiY6xMAAAAASUVORK5CYI
         I=""")
-        self.iproperties = tk.PhotoImage(data="""iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAA
-        AACXBIWXMAAA7DAAAOwwHHb6hkAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAdFJREFUK
-        JGN0r9rFEEUB/Dvd+8uxzUhoBCCEkhtEbTbHVdZIiQQfySKWmkjWtkIWtj4D1imsDQIRlCDoBbauOLNzR5aGrBV
-        EY0g2gQCtzfztTALinenrxt4n++8Nwwxorrd7ni/379O8gyAKQDvAdwyxqwAQDQCTnrvLcndJBcBnAewC0Be9Qz
-        F3vubJJ8aYy6GEGYkrZBcMMZsWGv3WWsvcxDM83xibGzsQ6/X29NoNPaTfExyPkmS1+12ezaKoucAfgy8udVqTZ
-        P8lGXZVlmW7yR9BLBYFMUBks9IXgEwM2zsr5Km8jyvZ1n2rSzLuRDCUgjhhaRLkt4C2ByIvfezANBsNicBoAqQt
-        Jym6RNJ1wCs/7VzURRHQgh3oyg6Gcdxx1o7XZbl5yzL+t1ud9x7fwPA0RBC/Ad2zs1JWvsNZiQfAQgANgHsBfCQ
-        5NUkSb7XK2itzSStSToVx3GnCgJwnOSG936iVqt9SZJkuzLcgQdJrocQzqZp+tI5d1jS/eo85FHBTqdzCMADAKe
-        NMa+cc/OS7lSjD4MAUAdwG8C5HbggaRXAUhzHxSgI/PqeLUnbzrllSashhBPGmH9CAKhLukDynqQtAMfSNH3zPx
-        AAfgL2/u9cQzl88QAAAABJRU5ErkJggg==""")
-        self.ikeywords = tk.PhotoImage(data="""iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAAAA
-        CXBIWXMAAA7DAAAOwwHHb6hkAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAPRJREFUKJG
-        lkrFKxEAURc8bHltbWqytYG0TYiC2VnZ+hK3iByhouX7HfkcmhAgigpXFgt02gpXETObZiEVMWI23PecOl+HBPy
-        Le+5cxaGaLLMsWY1yBHRE5NLO3Hrtwzm0BFEVxJCI3Q2XM7BIIPbYLPAOo6n2M8exHWUROxmaFEJ4AkiRZA+sxb
-        1KkLMvrTVKM8SHLsmVVVfMY4ynwnqbplZrZbFPZOacATdOIqs7MrP8/E2Z774+HQAjhMc/zFUBVVfOu6/b7jgLn
-        Q2VVvQVWXw/ticigNzlS1/X2b+UQwkeapq/f69q2Hb3tgdwBB39ZN5pP4uJac+7GJRAAAAAASUVORK5CYII=""")
-        self.iwords = tk.PhotoImage(data="""iVBORw0KGgoAAAANSUhEUgAAAA8AAAAICAYAAAAm06XyAAAACXB
-        IWXMAAA7DAAAOwwHHb6hkAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAATBJREFUGJWFjy
-        FLQ2EYhc95t31JEQYiGExaLBODYbvJaFBEGBqHGNW4n6BFBUGw2ZUJCoaxMGT3Xm+1LwkLgrILwzLZdwy7wTD0i
-        ec9z4EXmEAcx40wDPcn3X5j/xX+gmEYLgA4JLkE4KFSqdzEcdwA0Jc0A0CSzoMgSNrt9pRzrg5gRVLXSNZIfki6
-        AnDa6XRKGBsbku5IPpNsJkky55x7AjAv6ZLkV344HJ4VCoUdM9uUNMrlcsuZfBEEwS0ARFG0670/BrDY6/XWq9X
-        qCEAr75xrABgAeASwKilHElmGbIgkpwF8ZuL45yiKUgCBpG+SLwCOSG5LmvXebwEomdk9yTVJife+ViwWm/1+f9
-        tI1iW1ssIrgIGkd0lmZm9mdk1yr1wudwFUzewkTdOU5MEPhImOHsSTJnYAAAAASUVORK5CYII=""")
+        self.iproperties = tk.PhotoImage(data="""iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAAAACXB
+        IWXMAAA7DAAAOwwHHb6hkAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAdFJREFUKJGN0r
+        9rFEEUB/Dvd+8uxzUhoBCCEkhtEbTbHVdZIiQQfySKWmkjWtkIWtj4D1imsDQIRlCDoBbauOLNzR5aGrBVEY0g2
+        gQCtzfztTALinenrxt4n++8Nwwxorrd7ni/379O8gyAKQDvAdwyxqwAQDQCTnrvLcndJBcBnAewC0Be9QzF3vub
+        JJ8aYy6GEGYkrZBcMMZsWGv3WWsvcxDM83xibGzsQ6/X29NoNPaTfExyPkmS1+12ezaKoucAfgy8udVqTZP8lGX
+        ZVlmW7yR9BLBYFMUBks9IXgEwM2zsr5Km8jyvZ1n2rSzLuRDCUgjhhaRLkt4C2ByIvfezANBsNicBoAqQtJym6R
+        NJ1wCs/7VzURRHQgh3oyg6Gcdxx1o7XZbl5yzL+t1ud9x7fwPA0RBC/Ad2zs1JWvsNZiQfAQgANgHsBfCQ5NUkS
+        b7XK2itzSStSToVx3GnCgJwnOSG936iVqt9SZJkuzLcgQdJrocQzqZp+tI5d1jS/eo85FHBTqdzCMADAKeNMa+c
+        c/OS7lSjD4MAUAdwG8C5HbggaRXAUhzHxSgI/PqeLUnbzrllSashhBPGmH9CAKhLukDynqQtAMfSNH3zPxAAfgL
+        2/u9cQzl88QAAAABJRU5ErkJggg==""")
+        self.ikeywords = tk.PhotoImage(data="""iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAAAACXBIW
+        XMAAA7DAAAOwwHHb6hkAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAPRJREFUKJGlkrFK
+        xEAURc8bHltbWqytYG0TYiC2VnZ+hK3iByhouX7HfkcmhAgigpXFgt02gpXETObZiEVMWI23PecOl+HBPyLe+5c
+        xaGaLLMsWY1yBHRE5NLO3Hrtwzm0BFEVxJCI3Q2XM7BIIPbYLPAOo6n2M8exHWUROxmaFEJ4AkiRZA+sxb1KkLM
+        vrTVKM8SHLsmVVVfMY4ynwnqbplZrZbFPZOacATdOIqs7MrP8/E2Z774+HQAjhMc/zFUBVVfOu6/b7jgLnQ2VVv
+        QVWXw/ticigNzlS1/X2b+UQwkeapq/f69q2Hb3tgdwBB39ZN5pP4uJac+7GJRAAAAAASUVORK5CYII=""")
+        self.iwords = tk.PhotoImage(data="""iVBORw0KGgoAAAANSUhEUgAAAA8AAAAICAYAAAAm06XyAAAACXBIWXMAAA7DAAAOwwHHb6hkAAAA
+        GXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAATBJREFUGJWFjyFLQ2EYhc95t31JEQYiGExaLBO
+        DYbvJaFBEGBqHGNW4n6BFBUGw2ZUJCoaxMGT3Xm+1LwkLgrILwzLZdwy7wTD0iec9z4EXmEAcx40wDPcn3X5j/x
+        X+gmEYLgA4JLkE4KFSqdzEcdwA0Jc0A0CSzoMgSNrt9pRzrg5gRVLXSNZIfki6AnDa6XRKGBsbku5IPpNsJkky5
+        5x7AjAv6ZLkV344HJ4VCoUdM9uUNMrlcsuZfBEEwS0ARFG0670/BrDY6/XWq9XqCEAr75xrABgAeASwKilHElmG
+        bIgkpwF8ZuL45yiKUgCBpG+SLwCOSG5LmvXebwEomdk9yTVJife+ViwWm/1+f9tI1iW1ssIrgIGkd0lmZm9mdk1
+        yr1wudwFUzewkTdOU5MEPhImOHsSTJnYAAAAASUVORK5CYII=""")
```

### Comparing `cupcake_editor-0.25.5/cupcake/texteditor/highlighter.py` & `cupcake-editor-0.5.1/cupcake/editor/linenumbers/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,90 @@
-import os, tkinter as tk
+import tkinter as tk
 
-from pygments import lex
-from pygments.lexers import get_lexer_for_filename, get_lexer_by_name
+from .breakpoint import Breakpoint
 
 
-class Highlighter:
-    def __init__(self, master, language=None, *args, **kwargs):
-        self.text = master
-        self.base = master.base
-        self.language = language
+class LineNumbers(tk.Frame):
+    def __init__(self, master, text, *args, **kwargs):
+        super().__init__(master, *args, **kwargs)
+        self.master = master
+
+        self.config_appearance()
+
+        self.text = text
+
+        self.cw = tk.Canvas(self)
+        self.cw.config(width=68, bg="#1e1e1e", highlightthickness=0)
+        self.cw.pack(fill=tk.BOTH, expand=True)
+    
+    def set_bar_width(self, width):
+        self.configure(width=width)
+
+    def config_appearance(self):
+        self.font = self.master.font
+        self.fill = "#858585"
+        self.highlight_fill = "#c6c6c6"
+        self.config(bg="#1e1e1e")
+    
+    def attach(self, text):
+        self.text = text
+    
+    def clear(self):
+        self.cw.delete(tk.ALL)
+    
+    def mark_line(self, line):
+        dline = self.text.get_line_info(line)
         
-        if language:
-            try:
-                self.lexer = get_lexer_by_name(language)
-            except:
-                self.lexer = None
-                return
-        else:
-            try:
-                self.lexer = get_lexer_for_filename(os.path.basename(master.path), inencoding=master.encoding, encoding=master.encoding)
-            except:
-                self.lexer = None
-                return
-
-        self.setup_highlight_tags()
-
-    def setup_highlight_tags(self):
-        for token, color in self.base.settings.syntax.items():
-            self.text.tag_configure(f"Token.{token}", foreground=color)
-
-    def highlight(self):
-        if not self.lexer:
+        if not dline:
             return
         
-        for token, _ in self.base.settings.syntax.items():
-            self.text.tag_remove(f"Token.{token}", '1.0', tk.END)
+        y = dline[1]
+        btn =  tk.Menubutton(self.cw, 
+            text=">", font=("Consolas", 14), fg="#1e1e1e", bg="#1e1e1e", cursor="hand2", 
+            activeforeground="#c5c5c5", activebackground="#1e1e1e", borderwidth=0,
+            width=2, height=1, pady=0, padx=0, relief=tk.FLAT)
+        self.cw.create_window(70, y-2, anchor=tk.NE, window=btn)
+    
+    def highlight_current_line(self):
+        self.mark_line(tk.INSERT)
+    
+    def select_line(self, line):
+        self.text.select_line(line)
+
+    def redraw(self, *args):
+        self.clear()
+        self.highlight_current_line()
+        self.redraw_line_numbers()
+
+    def redraw_line_numbers(self):
+        i = self.text.get_origin()
+        while True:
+            dline = self.text.get_line_info(i)
+            if not dline:
+                break
+
+            y = dline[1]
+            ln = str(i).split(".")[0]
+
+            curline = self.text.get_line_info(tk.INSERT)
+            cur_y = None
+            if curline:
+                cur_y = curline[1]
+
+            if y == cur_y:
+                number = self.cw.create_text(46, y, anchor=tk.NE, text=ln, font=self.font, fill=self.highlight_fill, tag=i)
+            else:
+                number = self.cw.create_text(46, y, anchor=tk.NE, text=ln, font=self.font, fill=self.fill, tag=i)
             
-        text = self.text.get_all_text()
+            self.cw.tag_bind(i, "<Button-1>", lambda _, i=i: self.select_line(i))
 
-        # NOTE:  Highlighting only visible area
-        # total_lines = int(self.text.index('end-1c').split('.')[0])
-        # start_line = int(self.text.yview()[0] * total_lines)
-        # first_visible_index = f"{start_line}.0"
-        # last_visible_index =f"{self.text.winfo_height()}.end"
-        # for token, _ in self.tag_colors.items():
-        #     self.text.tag_remove(str(token), first_visible_index, last_visible_index)
-        # text = self.text.get(first_visible_index, last_visible_index)
-
-        self.text.mark_set("range_start", '1.0')
-        for token, content in lex(text, self.lexer):
-            self.text.mark_set("range_end", f"range_start + {len(content)}c")
-            self.text.tag_add(str(token), "range_start", "range_end")
-            self.text.mark_set("range_start", "range_end")
+            # drawing breakpoints - needs optimisations
+            # self.draw_breakpoint(y)
             
-            # DEBUG
-            # print(f"{content} is recognized as a <{str(token)}>")
-        # print("==================================")
+            i = self.text.index(f"{i}+1line")
+
+    def draw_breakpoint(self, y):
+        bp = Breakpoint(self.cw)
+        self.cw.create_window(21, y-2, anchor=tk.NE, window=bp)
+    
+    def toggle_breakpoint(self, y):
+        ...
```

### Comparing `cupcake_editor-0.25.5/cupcake/texteditor/linenumbers/breakpoint.py` & `cupcake-editor-0.5.1/cupcake/editor/find_replace/toggle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 import tkinter as tk
 
 
-class Breakpoint(tk.Label):
-    def __init__(self, master, *args, **kwargs):
+class ToggleButton(tk.Frame):
+    def __init__(self, master, bg, hbg, sbg, img=None, *args, **kwargs):
         super().__init__(master, *args, **kwargs)
         self.master = master
-        self.base = master.base
+        self.img = img
+        
+        self.hovered = False
+        self.state = False
 
-        self.config(text="●", font=("Consolas", 14), fg="#1e1e1e", cursor="hand2", 
-                    bg=self.base.theme.linenumbers["background"], borderwidth=0, 
-                    width=2, height=1, pady=0, padx=0, relief=tk.FLAT)
+        self.bg = bg
+        self.hbg = hbg
+        self.sbg = sbg
 
-        self.active = False
-        self.hovered = False
+        self.imagew = tk.Label(self, image=self.img)
+        self.imagew.config(bg=self.bg, relief=tk.FLAT)
+        self.imagew.grid(row=0, column=0, sticky=tk.NS)
+
+        self.config(bg=self.bg, pady=3, padx=3, cursor="hand2")
         self.config_bindings()
-    
-    def config_bindings(self):
-        self.bind("<Button-1>", self.on_click)
-        self.bind("<Enter>", self.on_enter)
-        self.bind("<Leave>", self.on_leave)
 
+    def config_bindings(self):
+        self.bind("<Enter>", self.on_hover)
+        self.bind("<Leave>", self.off_hover)
+        self.bind("<Button-1>", self.toggle)
+
+    def set_image(self, img):
+        self.img = img
+        self.imagew.config(image=self.img)
+    
     def redraw(self):
-        if self.active:
-            self.config(fg="#e51400")
+        if self.state:
+            self.config(bg=self.sbg)
             return 
         
         if self.hovered:
-            self.config(fg="#6e1911")
+            self.config(bg=self.hbg)
         else:
-            self.config(fg="#1e1e1e")
+            self.config(bg=self.bg)
         
-    def on_click(self, event):
-        self.active = not self.active
-        self.redraw()
+    def toggle(self, *args):
+        self.state = not self.state
     
-    def on_enter(self, event):
+    def on_hover(self, *args):
         self.hovered = True
         self.redraw()
 
-    def on_leave(self, event):
+    def off_hover(self, *args):
         self.hovered = False
         self.redraw()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cupcake_editor-0.25.5/cupcake/texteditor/minimap.py` & `cupcake-editor-0.5.1/cupcake/editor/scrollbar.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,67 @@
 import tkinter as tk
-from ..utils import Frame
 
 
-#TODO update minimap when scrollbar is used
-class Minimap(Frame):
+class Scrollbar(tk.Frame):
     def __init__(self, master, textw, *args, **kwargs):
         super().__init__(master, *args, **kwargs)
+        self.master = master
+        
         self.tw = textw
         self.font = ("Arial", 1, "bold")
-        self.config(highlightthickness=0, bg=self.base.theme.border)
-        
-        self.cw = tk.Canvas(self, width=100, highlightthickness=0, **self.base.theme.minimap)
-        self.cw.pack(fill=tk.BOTH, expand=True, side=tk.LEFT, padx=(1, 0))
+
+        self.config(bg="#252526", highlightthickness=0, padx=1)
+        self.cw = tk.Canvas(self, bg="#1e1e1e", width=15, highlightthickness=0)
+        self.cw.pack(fill=tk.BOTH, expand=True, side=tk.LEFT)
 
         self.slider_image = tk.PhotoImage(data="""iVBORw0KGgoAAAANSUhEUgAAAG4AAABFCAYAAACrMNMO
         AAAACXBIWXMAAABfAAAAXwEqnu0dAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAMBJRE
         FUeJzt0UENwCAAwMAxLajjhwOkz8M+pMmdgiYda5/5kPPeDuAf46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo
         46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46
         KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIuyrgo46KMizIu6gNeAwIJ
         26ERewAAAABJRU5ErkJggg==""")
 
         self.cw.create_image(0, 0, image=self.slider_image, anchor=tk.NW, tag="slider")
 
+        self.extra_y = 10
         self.y_top_lim = 0
-        self._drag_data = {"y": 0, "item": None}
+        self.drag_data = {"y": 0, "item": None}
         self.yvalue = 0
 
         self.cw.tag_bind("slider", "<ButtonPress-1>", self.drag_start)
         self.cw.tag_bind("slider", "<ButtonRelease-1>", self.drag_stop)
         self.cw.tag_bind("slider", "<B1-Motion>", self.drag)
 
         if textw:
             self.redraw()
 
     def attach(self, textw):
         self.tw = textw
 
     def redraw(self):
-        self.cw.delete("redrawn")
-        self.text = self.tw.get('1.0', tk.END)
-        self.cw.create_text(5, 0, text=self.text, anchor=tk.NW, font=self.font, fill="grey", tag="redrawn")
-
-        self.y_bottom_lim = int(self.tw.index(tk.END).split(".")[0]) * 2 + 10
-        # self.y_bottom_lim = self.tw.yview()[1] * self.cw.winfo_height()
+        self.y_bottom_lim = int(self.tw.index(tk.END).split(".")[0]) * 2 + self.extra_y
     
-    def redraw_cursor(self):
-        self.cw.delete("cursor")
-        y = int(self.tw.index(tk.INSERT).split(".")[0]) * 2
-        self.cw.create_line(0, y, 100, y, fill="#dc8c34", width=2, tag="cursor")
-
     def drag_start(self, event):
-        self._drag_data["item"] = self.cw.find_closest(event.x, event.y)[0]
-        self._drag_data["y"] = event.y
+        self.drag_data["item"] = self.cw.find_closest(event.x, event.y)[0]
+        self.drag_data["y"] = event.y
 
     def drag_stop(self, event):
-        self._drag_data["item"] = None
-        self._drag_data["y"] = 0
+        self.drag_data["item"] = None
+        self.drag_data["y"] = 0
 
     def drag(self, event):
-        item = self._drag_data["item"]
+        item = self.drag_data["item"]
         if item != 1:
             return
 
-        delta_y = event.y - self._drag_data["y"]
+        delta_y = event.y - self.drag_data["y"]
         self.cw.move(item, 0, delta_y)
-        self._drag_data["y"] = event.y
+        self.drag_data["y"] = event.y
 
         self.yvalue = y = self.cw.coords(item)[1]
         if y <= self.y_top_lim:
             self.cw.move("slider", 0, -(y - self.y_top_lim))
         elif y >= self.y_bottom_lim:
             self.cw.move("slider", 0, -(y - self.y_bottom_lim))
 
-        self.tw.yview(int(y / self.cw.winfo_height() * 350))
-        self.tw.master.on_scroll()
+        self.tw.yview(int(y / self.cw.winfo_height() * 100))
+        self.tw.master.redraw_ln()
```

### Comparing `cupcake_editor-0.25.5/LICENSE` & `cupcake-editor-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake_editor-0.25.5/README.md` & `cupcake-editor-0.5.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,18 @@
 # Cupcake: Embeddable Code Editor
-![](https://github.com/billyeatcookies/cupcake/blob/main/.github/res/screenshot.png)
-
-
-Cupcake is an **Embeddable** modern-looking code editor for **python tkinter** applications. It has rich **Autocompletions**, **Minimap** and **Semantic Syntax highlighting**. Cupcake is written in pure python with the tkinter library. It is the code editor which powers [Biscuit](https://github.com/billyeatcookies/Biscuit).
-```py
-import tkinter as tk
-from cupcake import Editor, Languages
-
-root = tk.Tk()
-root.minsize(800, 600)
-
-e = Editor(root, language=Languages.TYPESCRIPT)
-e.pack(expand=1, fill=tk.BOTH)
-
-e.content.insert("end", """
-// check this out
-import "./theme.scss";
-import "./global.css";
-import App from './App.svelte';
-
-const app = new App({
-	target: document.body
-});
-
-export default app;
-""")
-
-root.mainloop()
-
-```
-see [**examples**](./examples/) for instructions on **Diff viewer**, **Image viewer** and **Theming**
-
-## Syntax Highlighting & Minimap
-
-<img src=https://user-images.githubusercontent.com/70792552/162617464-65169951-fc20-44f3-9f24-a7d80cb6eb10.gif />
-
-## Auto completions 
-<img src=https://user-images.githubusercontent.com/70792552/162617435-a9145e3e-e380-4afd-8e78-cbeedeb1bd24.gif />
+Cupcake is an Embeddable Modern Code editor for python tkinter applications. It comes with features such as **Autocompletions**, **Minimap** and **Semantic Syntax highlighting**. Cupcake is written in pure python with the tkinter library. It is the the code editor which powers [Biscuit](https://github.com/billyeatcookies/Biscuit). See a good list of the code editor's [features](#features).
 
+<table>
+    <td>
+        <img src=https://user-images.githubusercontent.com/70792552/162617435-a9145e3e-e380-4afd-8e78-cbeedeb1bd24.gif />
+    </td>
+    <td>
+        <img src=https://user-images.githubusercontent.com/70792552/162617464-65169951-fc20-44f3-9f24-a7d80cb6eb10.gif />
+    </td>
+</table>
 
 <!-- ![something](.github/res/screenshot.png) -->
 
 ## Installation
 Cupcake can be installed by running:
 ```
 pip install cupcake-editor
@@ -64,20 +35,20 @@
 ```
 
 ## Examples!
 Examples demonstrating how to use cupcake are in the [examples](./examples) directory. You can learn how to integrate the editor to your app with these. You can run the examples like `python -m examples.hello`
 
 ## Features
 
-- [x] Syntax Highlighting (over 500+ languages supported)
-- [x] Auto=Completions (words + keywords)
-- [x] Auto-Indentation
-- [x] Diff Viewer
+- [x] Syntax Highlighting
+- [x] Auto completions
+- [x] Auto Indentation
 - [x] Minimap
-- [x] Breadcrumbs and Pathview tree
-- [x] Image Viewer
-- [x] Fully Customizable and Themable 
-- [x] Language Detection from File Extensions
+- [x] Find Replace
+- [ ] Extendable language support
+- [ ] Code Debugging
+- [ ] Language Detection
 - [ ] Code Folding
 
+
 ### Contributing
-Your contributions and support are greatly appreciated! 🧡 See [contributing](./CONTRIBUTING.md) for further details such as coding guidelines and tools used.
+Thank you if you are considering to contribute to Cupcake. See [contributing](./CONTRIBUTING.md) for further details such as coding guides and editing tools used.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cupcake_editor-0.25.5/PKG-INFO` & `cupcake-editor-0.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,29 @@
 Metadata-Version: 2.1
 Name: cupcake-editor
-Version: 0.25.5
-Summary: Embeddable code editor for python apps
-License: MIT
+Version: 0.5.1
+Summary: Embeddable code editor for tkinter
 Author: Billy
 Author-email: billydevbusiness@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # Cupcake: Embeddable Code Editor
-![](https://github.com/billyeatcookies/cupcake/blob/main/.github/res/screenshot.png)
-
-
-Cupcake is an **Embeddable** modern-looking code editor for **python tkinter** applications. It has rich **Autocompletions**, **Minimap** and **Semantic Syntax highlighting**. Cupcake is written in pure python with the tkinter library. It is the code editor which powers [Biscuit](https://github.com/billyeatcookies/Biscuit).
-```py
-import tkinter as tk
-from cupcake import Editor, Languages
-
-root = tk.Tk()
-root.minsize(800, 600)
-
-e = Editor(root, language=Languages.TYPESCRIPT)
-e.pack(expand=1, fill=tk.BOTH)
-
-e.content.insert("end", """
-// check this out
-import "./theme.scss";
-import "./global.css";
-import App from './App.svelte';
-
-const app = new App({
-	target: document.body
-});
-
-export default app;
-""")
-
-root.mainloop()
-
-```
-see [**examples**](./examples/) for instructions on **Diff viewer**, **Image viewer** and **Theming**
-
-## Syntax Highlighting & Minimap
-
-<img src=https://user-images.githubusercontent.com/70792552/162617464-65169951-fc20-44f3-9f24-a7d80cb6eb10.gif />
-
-## Auto completions 
-<img src=https://user-images.githubusercontent.com/70792552/162617435-a9145e3e-e380-4afd-8e78-cbeedeb1bd24.gif />
+Cupcake is an Embeddable Modern Code editor for python tkinter applications. It comes with features such as **Autocompletions**, **Minimap** and **Semantic Syntax highlighting**. Cupcake is written in pure python with the tkinter library. It is the the code editor which powers [Biscuit](https://github.com/billyeatcookies/Biscuit). See a good list of the code editor's [features](#features).
 
+<table>
+    <td>
+        <img src=https://user-images.githubusercontent.com/70792552/162617435-a9145e3e-e380-4afd-8e78-cbeedeb1bd24.gif />
+    </td>
+    <td>
+        <img src=https://user-images.githubusercontent.com/70792552/162617464-65169951-fc20-44f3-9f24-a7d80cb6eb10.gif />
+    </td>
+</table>
 
 <!-- ![something](.github/res/screenshot.png) -->
 
 ## Installation
 Cupcake can be installed by running:
 ```
 pip install cupcake-editor
@@ -80,21 +46,21 @@
 ```
 
 ## Examples!
 Examples demonstrating how to use cupcake are in the [examples](./examples) directory. You can learn how to integrate the editor to your app with these. You can run the examples like `python -m examples.hello`
 
 ## Features
 
-- [x] Syntax Highlighting (over 500+ languages supported)
-- [x] Auto=Completions (words + keywords)
-- [x] Auto-Indentation
-- [x] Diff Viewer
+- [x] Syntax Highlighting
+- [x] Auto completions
+- [x] Auto Indentation
 - [x] Minimap
-- [x] Breadcrumbs and Pathview tree
-- [x] Image Viewer
-- [x] Fully Customizable and Themable 
-- [x] Language Detection from File Extensions
+- [x] Find Replace
+- [ ] Extendable language support
+- [ ] Code Debugging
+- [ ] Language Detection
 - [ ] Code Folding
 
+
 ### Contributing
-Your contributions and support are greatly appreciated! 🧡 See [contributing](./CONTRIBUTING.md) for further details such as coding guidelines and tools used.
+Thank you if you are considering to contribute to Cupcake. See [contributing](./CONTRIBUTING.md) for further details such as coding guides and editing tools used.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

