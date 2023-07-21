# Comparing `tmp/crutil-0.1.1.tar.gz` & `tmp/crutil-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crutil-0.1.1.tar", last modified: Sat Mar 25 19:34:47 2023, max compression
+gzip compressed data, was "crutil-1.0.0.tar", last modified: Fri Jul 21 02:55:18 2023, max compression
```

## Comparing `crutil-0.1.1.tar` & `crutil-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 19:34:47.661620 crutil-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-02-13 00:43:47.000000 crutil-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2061 2023-03-25 19:34:47.661620 crutil-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1692 2023-03-25 19:33:54.000000 crutil-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-25 19:34:47.644515 crutil-0.1.1/crutil/
--rw-rw-rw-   0        0        0      247 2023-02-13 01:46:40.000000 crutil-0.1.1/crutil/__init__.py
--rw-rw-rw-   0        0        0     7238 2023-03-25 19:30:01.000000 crutil-0.1.1/crutil/crutil.py
--rw-rw-rw-   0        0        0      149 2023-03-25 19:34:17.000000 crutil-0.1.1/crutil/metadata.py
-drwxrwxrwx   0        0        0        0 2023-03-25 19:34:47.659622 crutil-0.1.1/crutil.egg-info/
--rw-rw-rw-   0        0        0     2061 2023-03-25 19:34:47.000000 crutil-0.1.1/crutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-03-25 19:34:47.000000 crutil-0.1.1/crutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 19:34:47.000000 crutil-0.1.1/crutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-03-25 19:34:47.000000 crutil-0.1.1/crutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-25 19:34:47.000000 crutil-0.1.1/crutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 19:34:47.662619 crutil-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-02-17 02:29:05.000000 crutil-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:55:18.273695 crutil-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-02-13 00:43:47.000000 crutil-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2528 2023-07-21 02:55:18.272697 crutil-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2159 2023-07-19 22:55:16.000000 crutil-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 02:55:18.226724 crutil-1.0.0/crutil/
+-rw-rw-rw-   0        0        0      247 2023-02-13 01:46:40.000000 crutil-1.0.0/crutil/__init__.py
+-rw-rw-rw-   0        0        0     8763 2023-07-20 22:13:21.000000 crutil-1.0.0/crutil/crutil.py
+-rw-rw-rw-   0        0        0      149 2023-07-20 23:53:58.000000 crutil-1.0.0/crutil/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:55:18.267698 crutil-1.0.0/crutil.egg-info/
+-rw-rw-rw-   0        0        0     2528 2023-07-21 02:55:17.000000 crutil-1.0.0/crutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-21 02:55:18.000000 crutil-1.0.0/crutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 02:55:17.000000 crutil-1.0.0/crutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-21 02:55:17.000000 crutil-1.0.0/crutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 02:55:17.000000 crutil-1.0.0/crutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 02:55:18.273695 crutil-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-07-19 19:54:36.000000 crutil-1.0.0/setup.py
```

### Comparing `crutil-0.1.1/LICENSE` & `crutil-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crutil-0.1.1/PKG-INFO` & `crutil-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crutil
-Version: 0.1.1
+Version: 1.0.0
 Summary: Cuboid Raptor's Utilities, A Garbage Collection Of Garbage For Your Garbage Needs™
 Home-page: https://github.com/CuboidRaptor/crutil
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: GNU GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -24,15 +24,15 @@
 
     with crutil.recursion(<some recursion limit here>):
         <do something here>
 	  
   Your recursion limit will be reset after.
   
 - crutil.suppress() ; A suppression context manager, use it with the "with" keyword like crutil.recursion(). This will
-  temporarily suppres stdout and stderr, preventing anything from being printed to console, even with sys.stderr.write.
+  temporarily suppress stdout and stderr, preventing anything from being printed to console, even with sys.stderr.write.
   This will, however, not silence error messages, although that's probably a good thing.
   
 - crutil.pubsub() ; Class that lets you use a publish subscribe model. You can create an instance, then publish/subscribe to that instance.::
 	
     ps = crutil.pubsub()
 	
 	def foo(bar):
@@ -48,7 +48,12 @@
   
 - crutil.find_args(func) ; Tries, *tries*, to return a list of all arguments of function.
 
 - crutil.blob(in, out) ; Takes a binary input file and converts it into a python script so that when said script is imported and the .unblob(out) method is run, it unblobs it's data to out.
   Can be used for easy pyinstallering.
 
 - crutil.test() ; idfk figure it out
+
+- crutil.gc() ; Nuclear bomb every variable in namespace, absolutely the most performant GC out there.
+
+- crutil.ll_import() ; Lazy import, you can do it in bulk with lists, and use semicolons as :code:`import as` and slashes are :code:`try: import except; import`
+  For example, :code:`"numpy;np"` imports numpy as np, and :code:`ujson;json/json` tries to import ujson as json, and if ujson doesn't exist on your python installation, it imports json instead.
```

### Comparing `crutil-0.1.1/README.rst` & `crutil-1.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     with crutil.recursion(<some recursion limit here>):
         <do something here>
 	  
   Your recursion limit will be reset after.
   
 - crutil.suppress() ; A suppression context manager, use it with the "with" keyword like crutil.recursion(). This will
-  temporarily suppres stdout and stderr, preventing anything from being printed to console, even with sys.stderr.write.
+  temporarily suppress stdout and stderr, preventing anything from being printed to console, even with sys.stderr.write.
   This will, however, not silence error messages, although that's probably a good thing.
   
 - crutil.pubsub() ; Class that lets you use a publish subscribe model. You can create an instance, then publish/subscribe to that instance.::
 	
     ps = crutil.pubsub()
 	
 	def foo(bar):
@@ -35,8 +35,13 @@
   This will print [8]. There is also crutil.pubsub().clear(), which clears all subscribers and crutil.pubsub().view(), which will pretty print the cache.
   
 - crutil.find_args(func) ; Tries, *tries*, to return a list of all arguments of function.
 
 - crutil.blob(in, out) ; Takes a binary input file and converts it into a python script so that when said script is imported and the .unblob(out) method is run, it unblobs it's data to out.
   Can be used for easy pyinstallering.
 
-- crutil.test() ; idfk figure it out
+- crutil.test() ; idfk figure it out
+
+- crutil.gc() ; Nuclear bomb every variable in namespace, absolutely the most performant GC out there.
+
+- crutil.ll_import() ; Lazy import, you can do it in bulk with lists, and use semicolons as :code:`import as` and slashes are :code:`try: import except; import`
+  For example, :code:`"numpy;np"` imports numpy as np, and :code:`ujson;json/json` tries to import ujson as json, and if ujson doesn't exist on your python installation, it imports json instead.
```

### Comparing `crutil-0.1.1/crutil/crutil.py` & `crutil-1.0.0/crutil/crutil.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,78 @@
+"""
+Crutil is a pile of steamy lukewarm garbage that gives you
+random functions.
+"""
+
+from .metadata import * # get dem numbers
+__all__ = [
+    "ll_import",
+    "subscriber",
+    "pubsub",
+    "find_args",
+    "recursion",
+    "defer",
+    "suppress",
+    "blob",
+    "gc"
+]
+
 # imports?
+import lazy_import
+import importlib
 import inspect
-import hashlib
-import pprint
-import sys
-import traceback
-import os
-import lzma
-import base64
-
-try:
-    import dill as pickle
-
-except ModuleNotFoundError:
-    import pickle
-
-def test():
-    """just needed to test that the program is running"""
-    print("Hello... World?")
+
+def ll_import(imports, level="leaf"):
+    """Lazy import off a list. Semi-colon allows importing as, and slash allows try excepts. At sign is for from importing (e.g ["numpy;np", "ujson;json/json", "random@randint;r_int"])"""
+
+    frame = inspect.currentframe().f_back
+
+    if isinstance(imports, str):
+        imports = [imports]
+
+    for mod in imports:
+        for i, attempt in enumerate(pmod := mod.split("/")):
+            smod = attempt.split(";")
+
+            if importlib.util.find_spec(
+                (
+                    atsplit := smod[0].split("@")
+                )[0]
+            ):
+                if len(atsplit) > 1:
+                    if len(smod) > 1:
+                        mname = smod[~0]
+
+                    else:
+                        mname = atsplit[~0]
+
+                    frame.f_globals[mname] = lazy_import.lazy_callable(smod[0].replace("@", "."))
+
+                else:
+                    frame.f_globals[smod[~0]] = lazy_import.lazy_module(smod[0], level=level)
+
+                break
+
+            elif i >= (len(pmod) - 1):
+                raise ImportError(f"Could not import any of {pmod}")
+
+            else:
+                continue
+
+ll_import([
+    "hashlib",
+    "pprint",
+    "traceback",
+    "os",
+    "lzma",
+    "base64",
+    "pkgutil",
+    "sys",
+    "dill;pickle/pickle"
+])
 
 class subscriber:
     """Subscriber object for pubsub"""
     def __init__(self, topic, callback):
         self.topic = topic
         self.callback = callback
         self.sid = topic + chr(0) + hashlib.md5(pickle.dumps(callback)).hexdigest()
@@ -124,15 +176,15 @@
     def __enter__(self):
         self.old_limit = sys.getrecursionlimit()
         sys.setrecursionlimit(self.limit)
 
     def __exit__(self, type, value, tb):
         sys.setrecursionlimit(self.old_limit)
 
-class Defer(object):
+class defer(object):
     """Defers functions to the end of a function/context manager."""
     def __init__(self, f=None):
         self.tb = traceback
 
         if f == None:
             self.exits, self.args, self.kwargs = [], [], []
 
@@ -146,17 +198,17 @@
 
         import sys
 
         exits, aargs, akwargs = [], [], []
 
         def ddefer(f, *args, **kwargs):
             if callable(f):
-                exits.append(f)
-                aargs.append(args)
-                akwargs.append(kwargs)
+                exits.insert(0, f)
+                aargs.insert(0, args)
+                akwargs.insert(0, kwargs)
 
             else:
                 raise TypeError(f"Object {f} cannot be deferred.")
 
         err = False
         try:
             out = self.function(defer=ddefer, *args, **kwargs)
@@ -172,47 +224,34 @@
             sys.exit()
 
     def __enter__(self):
         return self.fdefer
 
     def fdefer(self, f, *args, **kwargs):
         if callable(f):
-            self.exits.append(f)
-            self.args.append(args)
-            self.kwargs.append(kwargs)
+            self.exits.insert(0, f)
+            self.args.insert(0, args)
+            self.kwargs.insert(0, kwargs)
 
         else:
             raise TypeError(f"Object {f} cannot be deferred.")
 
     def __exit__(self, type, value, traceback):
         trace = self.tb.format_exc()
         err = False
 
         if not trace.startswith("None"):
             sys.stderr.write(self.tb.format_exc())
             err = True
 
-        temp = self.exits[::-1]
-        for i in range(0, len(temp)):
+        for i in range(0, len(self.exits)):
             try:
-                args, kwargs, curf = self.args[i], self.kwargs[i], temp[i]
+                args, kwargs, curf = self.args[i], self.kwargs[i], self.exits[i]
 
-                if args:
-                    if kwargs:
-                        curf(*args, **kwargs)
-
-                    else:
-                        curf(*args)
-
-                else:
-                    if kwargs:
-                        curf(**kwargs)
-
-                    else:
-                        curf()
+                curf(*args, **kwargs)
 
             except:
                 sys.stderr.write(self.tb.format_exc())
                 err = True
 
         if err:
             sys.exit()
@@ -258,7 +297,22 @@
                 )
                 + "\".replace(\"{\", \"\\\\\").replace(\"}\", \"\\\"\").encode(\"utf\")))\n"
                 + """def unblob(outf):
 \tglobal data
 \twith open(outf, "wb") as f:
 \t\tf.write(data)"""
             )
+
+def gc():
+    """Nukes every variable in scope excluding ones beginning with underscores."""
+
+    frame = inspect.currentframe().f_back
+
+    garbage = []
+    for var in frame.f_globals:
+        if (not var.startswith("_")) and (not var in ["crutil", "gc"]):
+            garbage.append(var)
+
+    for var in garbage:
+        del frame.f_globals[var]
+
+    __import__("gc").collect()
```

### Comparing `crutil-0.1.1/crutil.egg-info/PKG-INFO` & `crutil-1.0.0/crutil.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crutil
-Version: 0.1.1
+Version: 1.0.0
 Summary: Cuboid Raptor's Utilities, A Garbage Collection Of Garbage For Your Garbage Needs™
 Home-page: https://github.com/CuboidRaptor/crutil
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: GNU GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -24,15 +24,15 @@
 
     with crutil.recursion(<some recursion limit here>):
         <do something here>
 	  
   Your recursion limit will be reset after.
   
 - crutil.suppress() ; A suppression context manager, use it with the "with" keyword like crutil.recursion(). This will
-  temporarily suppres stdout and stderr, preventing anything from being printed to console, even with sys.stderr.write.
+  temporarily suppress stdout and stderr, preventing anything from being printed to console, even with sys.stderr.write.
   This will, however, not silence error messages, although that's probably a good thing.
   
 - crutil.pubsub() ; Class that lets you use a publish subscribe model. You can create an instance, then publish/subscribe to that instance.::
 	
     ps = crutil.pubsub()
 	
 	def foo(bar):
@@ -48,7 +48,12 @@
   
 - crutil.find_args(func) ; Tries, *tries*, to return a list of all arguments of function.
 
 - crutil.blob(in, out) ; Takes a binary input file and converts it into a python script so that when said script is imported and the .unblob(out) method is run, it unblobs it's data to out.
   Can be used for easy pyinstallering.
 
 - crutil.test() ; idfk figure it out
+
+- crutil.gc() ; Nuclear bomb every variable in namespace, absolutely the most performant GC out there.
+
+- crutil.ll_import() ; Lazy import, you can do it in bulk with lists, and use semicolons as :code:`import as` and slashes are :code:`try: import except; import`
+  For example, :code:`"numpy;np"` imports numpy as np, and :code:`ujson;json/json` tries to import ujson as json, and if ujson doesn't exist on your python installation, it imports json instead.
```

### Comparing `crutil-0.1.1/setup.py` & `crutil-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,13 +16,14 @@
     description="Cuboid Raptor's Utilities, A Garbage Collection Of Garbage For Your Garbage Needs™",
     url=mdata["__url__"],
     author=mdata["__author__"],
     author_email=mdata["__authoremail__"],
     license="GNU GPLv3",
     packages=["crutil"],
     install_requires=[
-        "dill>=0.3.0"
+        "dill>=0.3.0",
+        "lazy_import>=0.2.0"
     ],
     python_requires=">=3.6",
     long_description=readme,
     long_description_content_type="text/x-rst",
 )
```

