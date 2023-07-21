# Comparing `tmp/yautil-0.0.8.tar.gz` & `tmp/yautil-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yautil-0.0.8.tar", last modified: Wed Oct 21 15:03:09 2020, max compression
+gzip compressed data, was "dist/yautil-0.0.9.tar", last modified: Thu Oct 22 10:52:33 2020, max compression
```

## Comparing `yautil-0.0.8.tar` & `yautil-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-21 15:03:09.055253 yautil-0.0.8/
--rw-r--r--   0 dhkim      (501) staff       (20)      303 2020-10-21 15:03:09.054953 yautil-0.0.8/PKG-INFO
--rw-r--r--   0 dhkim      (501) staff       (20)        0 2020-10-17 12:10:25.000000 yautil-0.0.8/README.md
--rw-r--r--   0 dhkim      (501) staff       (20)       38 2020-10-21 15:03:09.055373 yautil-0.0.8/setup.cfg
--rw-r--r--   0 dhkim      (501) staff       (20)      795 2020-10-21 15:02:44.000000 yautil-0.0.8/setup.py
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-21 15:03:09.050268 yautil-0.0.8/yautil/
--rw-r--r--   0 dhkim      (501) staff       (20)      342 2020-10-21 13:40:24.000000 yautil-0.0.8/yautil/__init__.py
--rw-r--r--   0 dhkim      (501) staff       (20)      202 2020-10-07 08:33:40.000000 yautil-0.0.8/yautil/decorators.py
--rw-r--r--   0 dhkim      (501) staff       (20)      886 2020-10-07 08:33:40.000000 yautil-0.0.8/yautil/eventutil.py
--rw-r--r--   0 dhkim      (501) staff       (20)     2308 2020-10-07 08:33:40.000000 yautil-0.0.8/yautil/fcache.py
--rw-r--r--   0 dhkim      (501) staff       (20)     3543 2020-10-07 08:33:40.000000 yautil-0.0.8/yautil/fileutil.py
--rw-r--r--   0 dhkim      (501) staff       (20)     5198 2020-10-07 08:33:40.000000 yautil-0.0.8/yautil/mputil.py
--rw-r--r--   0 dhkim      (501) staff       (20)     6773 2020-10-21 12:16:33.000000 yautil-0.0.8/yautil/plotutil.py
--rw-r--r--   0 dhkim      (501) staff       (20)      641 2020-10-07 08:33:40.000000 yautil-0.0.8/yautil/shutil.py
--rw-r--r--   0 dhkim      (501) staff       (20)     2443 2020-10-07 08:33:40.000000 yautil-0.0.8/yautil/strutil.py
--rw-r--r--   0 dhkim      (501) staff       (20)     2238 2020-10-21 15:02:32.000000 yautil-0.0.8/yautil/subcommand.py
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-21 15:03:09.054538 yautil-0.0.8/yautil/tests/
--rw-r--r--   0 dhkim      (501) staff       (20)        0 2020-10-18 10:16:40.000000 yautil-0.0.8/yautil/tests/__init__.py
--rw-r--r--   0 dhkim      (501) staff       (20)     1294 2020-10-21 12:24:16.000000 yautil-0.0.8/yautil/tests/test_plotutil.py
--rw-r--r--   0 dhkim      (501) staff       (20)     2995 2020-10-21 14:52:11.000000 yautil-0.0.8/yautil/tests/test_subcommand.py
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-21 15:03:09.053450 yautil-0.0.8/yautil.egg-info/
--rw-r--r--   0 dhkim      (501) staff       (20)      303 2020-10-21 15:03:08.000000 yautil-0.0.8/yautil.egg-info/PKG-INFO
--rw-r--r--   0 dhkim      (501) staff       (20)      442 2020-10-21 15:03:08.000000 yautil-0.0.8/yautil.egg-info/SOURCES.txt
--rw-r--r--   0 dhkim      (501) staff       (20)        1 2020-10-21 15:03:08.000000 yautil-0.0.8/yautil.egg-info/dependency_links.txt
--rw-r--r--   0 dhkim      (501) staff       (20)        8 2020-10-21 15:03:08.000000 yautil-0.0.8/yautil.egg-info/requires.txt
--rw-r--r--   0 dhkim      (501) staff       (20)        7 2020-10-21 15:03:08.000000 yautil-0.0.8/yautil.egg-info/top_level.txt
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-22 10:52:33.480282 yautil-0.0.9/
+-rw-r--r--   0 dhkim      (501) staff       (20)      303 2020-10-22 10:52:33.479697 yautil-0.0.9/PKG-INFO
+-rw-r--r--   0 dhkim      (501) staff       (20)        0 2020-10-17 12:10:25.000000 yautil-0.0.9/README.md
+-rw-r--r--   0 dhkim      (501) staff       (20)       38 2020-10-22 10:52:33.480454 yautil-0.0.9/setup.cfg
+-rw-r--r--   0 dhkim      (501) staff       (20)      795 2020-10-22 10:52:21.000000 yautil-0.0.9/setup.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-22 10:52:33.473822 yautil-0.0.9/yautil/
+-rw-r--r--   0 dhkim      (501) staff       (20)      342 2020-10-21 13:40:24.000000 yautil-0.0.9/yautil/__init__.py
+-rw-r--r--   0 dhkim      (501) staff       (20)      202 2020-10-07 08:33:40.000000 yautil-0.0.9/yautil/decorators.py
+-rw-r--r--   0 dhkim      (501) staff       (20)      886 2020-10-07 08:33:40.000000 yautil-0.0.9/yautil/eventutil.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     2308 2020-10-07 08:33:40.000000 yautil-0.0.9/yautil/fcache.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     3543 2020-10-07 08:33:40.000000 yautil-0.0.9/yautil/fileutil.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     5198 2020-10-07 08:33:40.000000 yautil-0.0.9/yautil/mputil.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     7209 2020-10-22 10:51:05.000000 yautil-0.0.9/yautil/plotutil.py
+-rw-r--r--   0 dhkim      (501) staff       (20)      641 2020-10-07 08:33:40.000000 yautil-0.0.9/yautil/shutil.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     2443 2020-10-07 08:33:40.000000 yautil-0.0.9/yautil/strutil.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     2118 2020-10-22 10:47:01.000000 yautil-0.0.9/yautil/subcommand.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-22 10:52:33.478543 yautil-0.0.9/yautil/tests/
+-rw-r--r--   0 dhkim      (501) staff       (20)        0 2020-10-18 10:16:40.000000 yautil-0.0.9/yautil/tests/__init__.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     1294 2020-10-21 12:24:16.000000 yautil-0.0.9/yautil/tests/test_plotutil.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     2995 2020-10-21 14:52:11.000000 yautil-0.0.9/yautil/tests/test_subcommand.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2020-10-22 10:52:33.476711 yautil-0.0.9/yautil.egg-info/
+-rw-r--r--   0 dhkim      (501) staff       (20)      303 2020-10-22 10:52:33.000000 yautil-0.0.9/yautil.egg-info/PKG-INFO
+-rw-r--r--   0 dhkim      (501) staff       (20)      442 2020-10-22 10:52:33.000000 yautil-0.0.9/yautil.egg-info/SOURCES.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)        1 2020-10-22 10:52:33.000000 yautil-0.0.9/yautil.egg-info/dependency_links.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)        8 2020-10-22 10:52:33.000000 yautil-0.0.9/yautil.egg-info/requires.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)        7 2020-10-22 10:52:33.000000 yautil-0.0.9/yautil.egg-info/top_level.txt
```

### Comparing `yautil-0.0.8/setup.py` & `yautil-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yautil", # Replace with your own username
-    version="0.0.8",
+    version="0.0.9",
     author="Donghwi Kim",
     author_email="dhkim09@kaist.ac.kr",
     description="Yet Another Python util.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dhkim09a/pyutil",
     packages=setuptools.find_packages(),
```

### Comparing `yautil-0.0.8/yautil/eventutil.py` & `yautil-0.0.9/yautil/eventutil.py`

 * *Files identical despite different names*

### Comparing `yautil-0.0.8/yautil/fcache.py` & `yautil-0.0.9/yautil/fcache.py`

 * *Files identical despite different names*

### Comparing `yautil-0.0.8/yautil/fileutil.py` & `yautil-0.0.9/yautil/fileutil.py`

 * *Files identical despite different names*

### Comparing `yautil-0.0.8/yautil/mputil.py` & `yautil-0.0.9/yautil/mputil.py`

 * *Files identical despite different names*

### Comparing `yautil-0.0.8/yautil/plotutil.py` & `yautil-0.0.9/yautil/plotutil.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,17 @@
            maxcol: int = 4,
            xlabel: str = None,
            ylabel: str = None,
            xlim: List = None,
            ylim: List = None,
            padding: float = 0.2,
            block: bool = True,
-           legend_loc: str = 'best'):
+           legend_loc: str = 'best',
+           font_family: str = None,
+           ):
     """
     Usage examples:
 
     * Data should be a list of integers
 
       plot_cdf( [0, 1, 2, 3, 4] )
 
@@ -41,22 +43,26 @@
     import matplotlib.pyplot as plt
 
     if not titles:
         titles = []
 
     fig = plt.figure()
     plt.clf()
-    plt.rc('font', family='NanumGothicOTF')
+    if font_family:
+        # 'NanumGothicOTF'
+        plt.rc('font', family=font_family)
 
     for i, subplot_data in enumerate(data):
         if not isinstance(subplot_data, tuple):
             assert isinstance(subplot_data, list)
             subplot_data = (subplot_data,)
 
-        subplot = fig.add_subplot((len(data) - 1) / maxcol + 1, min(len(data), maxcol), i + 1)
+        subplot = fig.add_subplot(int((len(data) - 1) / maxcol + 1),
+                                  int(min(len(data), maxcol)),
+                                  int(i + 1))
         if i < len(titles):
             subplot.title.set_text(titles[i])
         if xlabel:
             subplot.set_xlabel(xlabel)
         if ylabel:
             subplot.set_ylabel(ylabel)
         if xlim:
@@ -117,15 +123,17 @@
 
 def plot_cdf(*data,
              titles: Union[str, List[str]] = None,
              maxcol: int = 4,
              xlabel: str = None,
              padding: float = 0.2,
              block: bool = True,
-             legend_loc: str = 'best'):
+             legend_loc: str = 'best',
+             font_family: str = None,
+             ):
     """
     Usage examples:
 
     * Data should be a list of integers
 
       plot_cdf( [0, 1, 2, 3, 4] )
 
@@ -138,14 +146,15 @@
       plot_cdf( [0, 1, 2, 3, 4], [2, 4, 8, 6, 0] )
 
     * Data in the same tuple are plotted on the same subfigure.
 
       plot_cdf( ([0, 1, 2, 3, 4], [2, 4, 8, 6, 0]) )
 
 
+    :param font_family:
     :param data: List(s) of integers
     :param titles: Title(s) of each subfigure
     :param maxcol: Maximum number of subfigures in the same row
     :param xlabel: Label (e.g., 'sec')
     :param padding:
     :param block:
     :param legend_loc: One of
@@ -171,27 +180,31 @@
            titles=titles,
            maxcol=maxcol,
            xlabel=xlabel,
            ylabel='CDF',
            ylim=[0,1],
            padding=padding,
            block=block,
-           legend_loc=legend_loc)
+           legend_loc=legend_loc,
+           font_family=font_family,
+           )
 
 
 def plot_linear(*data,
                 titles: Union[str, List[str]] = None,
                 maxcol: int = 4,
                 xlabel: str = None,
                 ylabel: str = None,
                 xlim: List = None,
                 ylim: List = None,
                 padding: float = 0.2,
                 block: bool = True,
-                legend_loc: str = 'best'):
+                legend_loc: str = 'best',
+                font_family: str = None,
+                ):
     """
     Usage examples:
 
     * Data should be a list of integers
 
       plot_cdf( [0, 1, 2, 3, 4] )
 
@@ -204,14 +217,15 @@
       plot_cdf( [0, 1, 2, 3, 4], [2, 4, 8, 6, 0] )
 
     * Data in the same tuple are plotted on the same subfigure.
 
       plot_cdf( ([0, 1, 2, 3, 4], [2, 4, 8, 6, 0]) )
 
 
+    :param font_family:
     :param data: List(s) of integers
     :param titles: Title(s) of each subfigure
     :param maxcol: Maximum number of subfigures in the same row
     :param xlabel: Label (e.g., 'sec')
     :param ylabel:
     :param xlim:
     :param ylim:
@@ -236,8 +250,10 @@
            maxcol=maxcol,
            xlabel=xlabel,
            ylabel=ylabel,
            xlim=xlim,
            ylim=ylim,
            padding=padding,
            block=block,
-           legend_loc=legend_loc)
+           legend_loc=legend_loc,
+           font_family=font_family,
+           )
```

### Comparing `yautil-0.0.8/yautil/shutil.py` & `yautil-0.0.9/yautil/shutil.py`

 * *Files identical despite different names*

### Comparing `yautil-0.0.8/yautil/strutil.py` & `yautil-0.0.9/yautil/strutil.py`

 * *Files identical despite different names*

### Comparing `yautil-0.0.8/yautil/subcommand.py` & `yautil-0.0.9/yautil/subcommand.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,18 +19,15 @@
     def on_command(self, args):
         raise NotImplementedError
 
     def _register(self, subparsers, _help=None):
         self.parser = subparsers.add_parser(self.name, help=_help)
         self.parser.set_defaults(func=self.on_command)
         self.on_parser_init(self.parser)
-        if subparsers.metavar:
-            subparsers.metavar = subparsers.metavar + ', ' + self.name
-        else:
-            subparsers.metavar = self.name
+        subparsers.metavar = 'command'
 
     def __init__(self, subparsers = None, name: str = None, help: str = '', dependency: Union[str, List[str]] = ''):
         self.name = name if name else type(self).__name__.lower()
         if subparsers:
             self._register(subparsers, _help=help)
```

### Comparing `yautil-0.0.8/yautil/tests/test_plotutil.py` & `yautil-0.0.9/yautil/tests/test_plotutil.py`

 * *Files identical despite different names*

### Comparing `yautil-0.0.8/yautil/tests/test_subcommand.py` & `yautil-0.0.9/yautil/tests/test_subcommand.py`

 * *Files identical despite different names*

