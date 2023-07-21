# Comparing `tmp/cmu-graphics-1.1.8.tar.gz` & `tmp/cmu-graphics-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmu-graphics-1.1.8.tar", last modified: Fri Nov  5 17:32:54 2021, max compression
+gzip compressed data, was "cmu-graphics-1.1.9.tar", last modified: Thu Dec  2 15:26:15 2021, max compression
```

## Comparing `cmu-graphics-1.1.8.tar` & `cmu-graphics-1.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     1534 2021-11-05 17:32:00.000000 cmu-graphics-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4403 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3811 2021-11-05 17:32:00.000000 cmu-graphics-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/cmu_graphics/
--rw-r--r--   0 root         (0) root         (0)     1565 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23847 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/cmu_graphics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/cmu_graphics/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      706 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/libs/loader_util.py
--rw-r--r--   0 root         (0) root         (0)      670 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/libs/webrequest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/cmu_graphics/meta/
--rw-r--r--   0 root         (0) root         (0)        6 2021-11-05 17:32:11.000000 cmu-graphics-1.1.8/cmu_graphics/meta/version.txt
--rw-r--r--   0 root         (0) root         (0)    17870 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/modal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/cmu_graphics/samples/
--rw-r--r--   0 root         (0) root         (0)     3806 2021-11-05 17:32:11.000000 cmu-graphics-1.1.8/cmu_graphics/samples/highscore.py
--rw-r--r--   0 root         (0) root         (0)     4454 2021-11-05 17:32:11.000000 cmu-graphics-1.1.8/cmu_graphics/samples/pointillism.py
--rw-r--r--   0 root         (0) root         (0)     1350 2021-11-05 17:32:11.000000 cmu-graphics-1.1.8/cmu_graphics/samples/puffy.py
--rw-r--r--   0 root         (0) root         (0)     4848 2021-11-05 17:32:11.000000 cmu-graphics-1.1.8/cmu_graphics/samples/weather.py
--rw-r--r--   0 root         (0) root         (0)   157617 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/shape_logic.py
--rw-r--r--   0 root         (0) root         (0)     1717 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/sound.py
--rw-r--r--   0 root         (0) root         (0)     5875 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/updater.py
--rw-r--r--   0 root         (0) root         (0)     9026 2021-11-05 17:32:35.000000 cmu-graphics-1.1.8/cmu_graphics/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/cmu_graphics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4403 2021-11-05 17:32:54.000000 cmu-graphics-1.1.8/cmu_graphics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      649 2021-11-05 17:32:54.000000 cmu-graphics-1.1.8/cmu_graphics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-05 17:32:54.000000 cmu-graphics-1.1.8/cmu_graphics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2021-11-05 17:32:54.000000 cmu-graphics-1.1.8/cmu_graphics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-11-05 17:32:54.000000 cmu-graphics-1.1.8/cmu_graphics.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2021-11-05 17:32:11.000000 cmu-graphics-1.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-05 17:32:54.098753 cmu-graphics-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2021-11-05 17:32:11.000000 cmu-graphics-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1534 2021-12-02 15:25:20.000000 cmu-graphics-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4403 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3811 2021-12-02 15:25:20.000000 cmu-graphics-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/cmu_graphics/
+-rw-r--r--   0 root         (0) root         (0)     1565 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26133 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/cmu_graphics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/cmu_graphics/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      706 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/libs/loader_util.py
+-rw-r--r--   0 root         (0) root         (0)      670 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/libs/webrequest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/cmu_graphics/meta/
+-rw-r--r--   0 root         (0) root         (0)        6 2021-12-02 15:25:31.000000 cmu-graphics-1.1.9/cmu_graphics/meta/version.txt
+-rw-r--r--   0 root         (0) root         (0)    17870 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/modal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/cmu_graphics/samples/
+-rw-r--r--   0 root         (0) root         (0)     3806 2021-12-02 15:25:31.000000 cmu-graphics-1.1.9/cmu_graphics/samples/highscore.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2021-12-02 15:25:31.000000 cmu-graphics-1.1.9/cmu_graphics/samples/pointillism.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2021-12-02 15:25:31.000000 cmu-graphics-1.1.9/cmu_graphics/samples/puffy.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2021-12-02 15:25:31.000000 cmu-graphics-1.1.9/cmu_graphics/samples/weather.py
+-rw-r--r--   0 root         (0) root         (0)   157719 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/shape_logic.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/sound.py
+-rw-r--r--   0 root         (0) root         (0)     5875 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/updater.py
+-rw-r--r--   0 root         (0) root         (0)     9026 2021-12-02 15:25:56.000000 cmu-graphics-1.1.9/cmu_graphics/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/cmu_graphics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4403 2021-12-02 15:26:15.000000 cmu-graphics-1.1.9/cmu_graphics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      649 2021-12-02 15:26:15.000000 cmu-graphics-1.1.9/cmu_graphics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-02 15:26:15.000000 cmu-graphics-1.1.9/cmu_graphics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2021-12-02 15:26:15.000000 cmu-graphics-1.1.9/cmu_graphics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-12-02 15:26:15.000000 cmu-graphics-1.1.9/cmu_graphics.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2021-12-02 15:25:31.000000 cmu-graphics-1.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-12-02 15:26:15.948324 cmu-graphics-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2021-12-02 15:25:31.000000 cmu-graphics-1.1.9/setup.py
```

### Comparing `cmu-graphics-1.1.8/LICENSE` & `cmu-graphics-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/PKG-INFO` & `cmu-graphics-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmu-graphics
-Version: 1.1.8
+Version: 1.1.9
 Summary: The graphics framework used by CMU CS Academy, geared toward beginner CS students.
 Home-page: https://academy.cs.cmu.edu/
 Author: Austin Schick
 Author-email: aschick@andrew.cmu.edu
 License: BSD 3-Clause License
 Project-URL: Documentation, https://academy.cs.cmu.edu/docs
 Platform: UNKNOWN
```

### Comparing `cmu-graphics-1.1.8/README.md` & `cmu-graphics-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/__init__.py` & `cmu-graphics-1.1.9/cmu_graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/cmu_graphics.py` & `cmu-graphics-1.1.9/cmu_graphics/cmu_graphics.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         'toBack', 'toFront', 'contains', 'hits', 'containsShape', 'hitsShape'
     }
 
     # This represents the valid keyword arguments passed to the constructor
     _init_attrs = {'fill', 'border', 'borderWidth', 'opacity', 'rotateAngle', 'dashes', 'align', 'visible', 'db'}
 
     def __init__(self, clsName, argNames, args, kwargs):
+        global SHAPES_CREATED
+        SHAPES_CREATED += 1
+
         for attr in list(kwargs.keys()):
             en_attr = toEnglish(attr, 'shape-attr')
             if attr != en_attr and en_attr is not None:
                 kwargs[en_attr] = kwargs[attr]
                 del kwargs[attr]
 
             if not en_attr in self._init_attrs:
@@ -507,15 +510,27 @@
         callUserFn('onKeyHold', keys)
 
 def onKeyPresses(key, n):
     for _ in range(n):
         callUserFn('onKeyPress', key)
 
 def loop():
-    app._app.run()
+    run()
+
+def run():
+    global MAINLOOP_RUN
+    MAINLOOP_RUN = True
+
+    if not os.environ.get('CI', False):
+        t = threading.Thread(target=CSAcademyConsole().interact).start()
+
+    try:
+        app._app.run()
+    except KeyboardInterrupt:
+        os._exit(0)
 
 from code import InteractiveConsole
 class CSAcademyConsole(InteractiveConsole):
     def __init__(self):
         self.__class__.__name__ = "CS Academy Console"
         __main__.__dict__['exit'] = lambda: os._exit(0)
         super().__init__(locals=__main__.__dict__, filename = '<%s>' % self.__class__.__name__)
@@ -552,21 +567,14 @@
             last_tb = ei = None
 
     # Override interact so we can os._exit on EOF
     def interact(self):
         super().interact()
         os._exit(0)
 
-def run():
-    t = threading.Thread(target=CSAcademyConsole().interact).start()
-    try:
-        app._app.run()
-    except KeyboardInterrupt:
-        os._exit(0)
-
 import os
 import sys
 from datetime import datetime
 from datetime import timedelta
 import json
 import subprocess
 from cmu_graphics.libs import webrequest
@@ -669,9 +677,45 @@
 rgb = sli.rgb
 gradient = sli.gradient
 slNewSound = sli.newSound
 toEnglish = sli.toEnglish
 accentCombinations = sli.accentCombinations
 t = sli.t
 
+SHAPES_CREATED = 0
+MAINLOOP_RUN = False
+
+# Checks to see if a user created shapes but did not call
+# cmu_graphics.run()
+def check_for_exit_without_run():
+    global SHAPES_CREATED, MAINLOOP_RUN
+
+    # The app's top level group is created even if the user creates no
+    # shapes on their own
+    if SHAPES_CREATED > 1 and not MAINLOOP_RUN:
+        print("""                                           
+                         (                                              
+                    (    (                                              
+                    ((  (*(                                             
+                    (*( (*/                                             
+                    (**.***,                                            
+                    (***************((((((((((((((((                    
+                    (********************************                   
+                    (*******************************(                   
+                    (*******************************(                   
+                    (*******************************(                   
+                    /*******************************(                   
+                    (/******************(((((((     ((                   
+                (*****(****************,                                
+                /**********(************(                                 
+            ((***************(*********                                  
+                (*****(/*********(*****(                                  
+                    (**********/(/***(*/                                   
+                    (****************(                                  
+                        (/***********(                                    
+                            (*******(                                      
+                            (**(                                                                                                          
+""")
+        print(" ** To run your animation, add cmu_graphics.run() to the bottom of your file **\n")
+
 app = AppWrapper(App())
-atexit.register(run)
+atexit.register(check_for_exit_without_run)
```

### Comparing `cmu-graphics-1.1.8/cmu_graphics/libs/loader_util.py` & `cmu-graphics-1.1.9/cmu_graphics/libs/loader_util.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/libs/webrequest.py` & `cmu-graphics-1.1.9/cmu_graphics/libs/webrequest.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/modal.py` & `cmu-graphics-1.1.9/cmu_graphics/modal.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/samples/highscore.py` & `cmu-graphics-1.1.9/cmu_graphics/samples/highscore.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/samples/pointillism.py` & `cmu-graphics-1.1.9/cmu_graphics/samples/pointillism.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/samples/puffy.py` & `cmu-graphics-1.1.9/cmu_graphics/samples/puffy.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/samples/weather.py` & `cmu-graphics-1.1.9/cmu_graphics/samples/weather.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/shape_logic.py` & `cmu-graphics-1.1.9/cmu_graphics/shape_logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 import copy
 import os
+from cmu_graphics import cmu_graphics
 from cmu_graphics import utils
 
 ### PYPI VERSION ###
 import cairo
 from PIL import Image
 ### END PYPI VERSION ###
 from cmu_graphics.libs import webrequest
@@ -152,14 +153,16 @@
         return translation
 
 supportedLanguages = ['en', 'es', 'de']
 
 class CMUException(Exception): pass
 
 def printTraceback(exceptionType, exception, tb):
+    atexit.unregister(cmu_graphics.check_for_exit_without_run)
+
     stack = traceback.extract_tb(tb)
     lines = (''.join(traceback.format_list(stack))).splitlines()
 
     print('An error occurred. Here is the stack trace:')
     hasSourceLines = False
 
     while (lines):
```

### Comparing `cmu-graphics-1.1.8/cmu_graphics/sound.py` & `cmu-graphics-1.1.9/cmu_graphics/sound.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/updater.py` & `cmu-graphics-1.1.9/cmu_graphics/updater.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics/utils.py` & `cmu-graphics-1.1.9/cmu_graphics/utils.py`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/cmu_graphics.egg-info/PKG-INFO` & `cmu-graphics-1.1.9/cmu_graphics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmu-graphics
-Version: 1.1.8
+Version: 1.1.9
 Summary: The graphics framework used by CMU CS Academy, geared toward beginner CS students.
 Home-page: https://academy.cs.cmu.edu/
 Author: Austin Schick
 Author-email: aschick@andrew.cmu.edu
 License: BSD 3-Clause License
 Project-URL: Documentation, https://academy.cs.cmu.edu/docs
 Platform: UNKNOWN
```

### Comparing `cmu-graphics-1.1.8/cmu_graphics.egg-info/SOURCES.txt` & `cmu-graphics-1.1.9/cmu_graphics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmu-graphics-1.1.8/setup.py` & `cmu-graphics-1.1.9/setup.py`

 * *Files identical despite different names*

