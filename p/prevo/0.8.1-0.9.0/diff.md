# Comparing `tmp/prevo-0.8.1.tar.gz` & `tmp/prevo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\prevo-0.8.1.tar", last modified: Sun Mar  6 18:45:34 2022, max compression
+gzip compressed data, was "dist\prevo-0.9.0.tar", last modified: Sat Mar 26 10:02:56 2022, max compression
```

## Comparing `prevo-0.8.1.tar` & `prevo-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-03-06 18:45:34.267294 prevo-0.8.1/
--rw-rw-rw-   0        0        0       54 2022-02-16 19:29:36.000000 prevo-0.8.1/.gitignore
--rw-rw-rw-   0        0        0    35823 2022-02-16 20:16:06.000000 prevo-0.8.1/LICENSE
--rw-rw-rw-   0        0        0      108 2022-02-16 20:20:23.000000 prevo-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8278 2022-03-06 18:45:34.268292 prevo-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     5850 2022-03-06 17:30:45.000000 prevo-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2022-03-06 18:45:34.089770 prevo-0.8.1/data/
-drwxrwxrwx   0        0        0        0 2022-03-06 18:45:34.165565 prevo-0.8.1/data/manip/
--rw-rw-rw-   0        0        0      523 2021-04-06 09:26:27.000000 prevo-0.8.1/data/manip/Vacuum_Infos.json
--rw-rw-rw-   0        0        0   673514 2021-04-06 09:26:02.000000 prevo-0.8.1/data/manip/Vacuum_Pressure.tsv
--rw-rw-rw-   0        0        0   294104 2021-04-06 09:26:07.000000 prevo-0.8.1/data/manip/Vacuum_SourceBath.tsv
--rw-rw-rw-   0        0        0   428341 2021-10-09 13:35:31.000000 prevo-0.8.1/data/manip/Vacuum_Temperature.tsv
-drwxrwxrwx   0        0        0        0 2022-03-06 18:45:34.225406 prevo-0.8.1/prevo/
--rw-rw-rw-   0        0        0     1011 2022-02-22 15:38:55.000000 prevo-0.8.1/prevo/__init__.py
--rw-rw-rw-   0        0        0     6471 2022-02-28 18:26:21.000000 prevo-0.8.1/prevo/csv.py
--rw-rw-rw-   0        0        0     3396 2022-02-26 17:10:45.000000 prevo-0.8.1/prevo/measurements.py
--rw-rw-rw-   0        0        0     1588 2022-02-16 20:14:40.000000 prevo-0.8.1/prevo/misc.py
--rw-rw-rw-   0        0        0     3870 2022-03-06 18:38:29.000000 prevo-0.8.1/prevo/parser.py
--rw-rw-rw-   0        0        0    19601 2022-03-06 11:56:42.000000 prevo-0.8.1/prevo/plot.py
--rw-rw-rw-   0        0        0    23018 2022-03-06 11:22:37.000000 prevo-0.8.1/prevo/record.py
--rw-rw-rw-   0        0        0    30948 2022-02-25 21:46:04.000000 prevo-0.8.1/prevo/viewers.py
-drwxrwxrwx   0        0        0        0 2022-03-06 18:45:34.262308 prevo-0.8.1/prevo.egg-info/
--rw-rw-rw-   0        0        0     8278 2022-03-06 18:45:33.000000 prevo-0.8.1/prevo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2022-03-06 18:45:33.000000 prevo-0.8.1/prevo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-06 18:45:33.000000 prevo-0.8.1/prevo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2022-03-06 18:45:33.000000 prevo-0.8.1/prevo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-03-06 18:45:33.000000 prevo-0.8.1/prevo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1042 2022-03-06 18:45:34.279262 prevo-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      937 2022-02-16 20:15:24.000000 prevo-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-06 18:45:34.265300 prevo-0.8.1/tests/
--rw-rw-rw-   0        0        0     2027 2022-03-01 14:10:07.000000 prevo-0.8.1/tests/test_prevo.py
+drwxrwxrwx   0        0        0        0 2022-03-26 10:02:56.227555 prevo-0.9.0/
+-rw-rw-rw-   0        0        0       75 2022-03-26 10:02:29.000000 prevo-0.9.0/.gitignore
+-rw-rw-rw-   0        0        0     4866 2022-03-26 10:02:29.000000 prevo-0.9.0/GraphExamples.ipynb
+-rw-rw-rw-   0        0        0    35823 2022-02-16 20:16:06.000000 prevo-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      135 2022-03-26 10:02:29.000000 prevo-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8313 2022-03-26 10:02:56.230559 prevo-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5885 2022-03-26 10:02:29.000000 prevo-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-03-26 10:02:55.875702 prevo-0.9.0/data/
+drwxrwxrwx   0        0        0        0 2022-03-26 10:02:56.083936 prevo-0.9.0/data/manip/
+-rw-rw-rw-   0        0        0      523 2021-04-06 09:26:27.000000 prevo-0.9.0/data/manip/Vacuum_Infos.json
+-rw-rw-rw-   0        0        0   673514 2021-04-06 09:26:02.000000 prevo-0.9.0/data/manip/Vacuum_Pressure.tsv
+-rw-rw-rw-   0        0        0   294104 2021-04-06 09:26:07.000000 prevo-0.9.0/data/manip/Vacuum_SourceBath.tsv
+-rw-rw-rw-   0        0        0   428341 2021-10-09 13:35:31.000000 prevo-0.9.0/data/manip/Vacuum_Temperature.tsv
+drwxrwxrwx   0        0        0        0 2022-03-26 10:02:56.155758 prevo-0.9.0/prevo/
+-rw-rw-rw-   0        0        0     1011 2022-02-22 15:38:55.000000 prevo-0.9.0/prevo/__init__.py
+-rw-rw-rw-   0        0        0     6471 2022-02-28 18:26:21.000000 prevo-0.9.0/prevo/csv.py
+-rw-rw-rw-   0        0        0     3410 2022-03-21 10:09:54.000000 prevo-0.9.0/prevo/measurements.py
+-rw-rw-rw-   0        0        0     3470 2022-03-26 10:02:29.000000 prevo-0.9.0/prevo/misc.py
+-rw-rw-rw-   0        0        0     3870 2022-03-06 18:38:29.000000 prevo-0.9.0/prevo/parser.py
+drwxrwxrwx   0        0        0        0 2022-03-26 10:02:56.217579 prevo-0.9.0/prevo/plot/
+-rw-rw-rw-   0        0        0     1138 2022-03-16 15:28:57.000000 prevo-0.9.0/prevo/plot/__init__.py
+-rw-rw-rw-   0        0        0    12886 2022-03-26 10:02:29.000000 prevo-0.9.0/prevo/plot/general.py
+-rw-rw-rw-   0        0        0     9423 2022-03-26 10:02:29.000000 prevo-0.9.0/prevo/plot/oscillo.py
+-rw-rw-rw-   0        0        0    17915 2022-03-26 10:02:29.000000 prevo-0.9.0/prevo/plot/plot.py
+-rw-rw-rw-   0        0        0    23018 2022-03-26 10:02:29.000000 prevo-0.9.0/prevo/record.py
+-rw-rw-rw-   0        0        0    30948 2022-03-26 10:02:29.000000 prevo-0.9.0/prevo/viewers.py
+drwxrwxrwx   0        0        0        0 2022-03-26 10:02:56.186675 prevo-0.9.0/prevo.egg-info/
+-rw-rw-rw-   0        0        0     8313 2022-03-26 10:02:54.000000 prevo-0.9.0/prevo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2022-03-26 10:02:54.000000 prevo-0.9.0/prevo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-26 10:02:54.000000 prevo-0.9.0/prevo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2022-03-26 10:02:54.000000 prevo-0.9.0/prevo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-03-26 10:02:54.000000 prevo-0.9.0/prevo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1042 2022-03-26 10:02:56.239528 prevo-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      937 2022-02-16 20:15:24.000000 prevo-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-26 10:02:56.220571 prevo-0.9.0/tests/
+-rw-rw-rw-   0        0        0     2027 2022-03-01 14:10:07.000000 prevo-0.9.0/tests/test_prevo.py
```

### Comparing `prevo-0.8.1/LICENSE` & `prevo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/PKG-INFO` & `prevo-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: prevo
-Version: 0.8.1
+Version: 0.9.0
 Summary: Record arbitrary sensors periodically in an asynchronous manner. Control their properties in real time from CLI. Graph/view tools to visualize live data/images are also provided.
 Home-page: https://github.com/ovinc/prevo
 Author: Olivier Vincent
 Author-email: ovinc.py@gmail.com
 License: UNKNOWN
 Description: About
         =====
         
-        **P**eriodic **RE**cording and **V**isualization of sensor **O**bjects
+        **P**eriodic **RE**cording and **V**isualization of (sensor) **O**bjects
         
         This package provides base classes to rapidly create interactive data recording for various applications (e.g. recording of temperature, time-lapses with cameras etc.). Sensors are read in a asynchronous fashion and can have different time intervals for data reading (or be continuous, i.e. as fast as possible). Tools for graphical visualizations of data during recording are also provided.
         
         Install
         -------
         
         ```bash
@@ -152,15 +152,15 @@
         
         
         Additional tools
         ================
         
         Some elements are also provided to simplify and/or extend the classes above:
         
-        - plot numerical data in real time (see `prevo.plot`)
+        - plot numerical data in real time (see `prevo.plot` module and `GraphExamples.ipynb`)
         - live view images from camera-like sensors (see `prevo.viewers`)
         - read / save with CSV files (see `prevo.csv`)
         - parse command line arguments to trigger functions or class methods (see `prevo.parser`)
         - some tools to format measurements for `Record`-like classes (see `prevo.measurements`)
         
         See docstrings for more help.
```

### Comparing `prevo-0.8.1/README.md` & `prevo-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 About
 =====
 
-**P**eriodic **RE**cording and **V**isualization of sensor **O**bjects
+**P**eriodic **RE**cording and **V**isualization of (sensor) **O**bjects
 
 This package provides base classes to rapidly create interactive data recording for various applications (e.g. recording of temperature, time-lapses with cameras etc.). Sensors are read in a asynchronous fashion and can have different time intervals for data reading (or be continuous, i.e. as fast as possible). Tools for graphical visualizations of data during recording are also provided.
 
 Install
 -------
 
 ```bash
@@ -144,15 +144,15 @@
 
 
 Additional tools
 ================
 
 Some elements are also provided to simplify and/or extend the classes above:
 
-- plot numerical data in real time (see `prevo.plot`)
+- plot numerical data in real time (see `prevo.plot` module and `GraphExamples.ipynb`)
 - live view images from camera-like sensors (see `prevo.viewers`)
 - read / save with CSV files (see `prevo.csv`)
 - parse command line arguments to trigger functions or class methods (see `prevo.parser`)
 - some tools to format measurements for `Record`-like classes (see `prevo.measurements`)
 
 See docstrings for more help.
```

### Comparing `prevo-0.8.1/data/manip/Vacuum_Infos.json` & `prevo-0.9.0/data/manip/Vacuum_Infos.json`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/data/manip/Vacuum_Pressure.tsv` & `prevo-0.9.0/data/manip/Vacuum_Pressure.tsv`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/data/manip/Vacuum_SourceBath.tsv` & `prevo-0.9.0/data/manip/Vacuum_SourceBath.tsv`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/data/manip/Vacuum_Temperature.tsv` & `prevo-0.9.0/data/manip/Vacuum_Temperature.tsv`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/prevo/__init__.py` & `prevo-0.9.0/prevo/__init__.py`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/prevo/csv.py` & `prevo-0.9.0/prevo/csv.py`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/prevo/measurements.py` & `prevo-0.9.0/prevo/measurements.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,11 +91,11 @@
         Here we assume that the first two columns in the csv represent
         - time (unix)
         - dt (s)
         and are considered as time columns, not value columns
         """
         measurement = {}
         measurement['name'] = self.name
-        measurement['time (unix)'] = self.data['time (unix)']
+        measurement['time (unix)'] = self.data['time (unix)'].values
         # remove time columns
-        measurement['values'] = [column for _, column in self.data.iloc[:, 2:].items()]
+        measurement['values'] = [column.values for _, column in self.data.iloc[:, 2:].items()]
         return measurement
```

### Comparing `prevo-0.8.1/prevo/parser.py` & `prevo-0.9.0/prevo/parser.py`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/prevo/plot.py` & `prevo-0.9.0/prevo/plot/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,33 +17,29 @@
 
 # You should have received a copy of the GNU General Public License
 # along with the prevo python package.
 # If not, see <https://www.gnu.org/licenses/>
 
 
 # Standard library imports
-from abc import ABC, abstractmethod
 from datetime import datetime
 from threading import Event, Thread
 from queue import Queue
 from pathlib import Path
 
 # Non standard imports
 import tzlocal
 import numpy as np
-import matplotlib
-
-matplotlib.use('Qt5Agg')
 
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
-from matplotlib.animation import FuncAnimation
 import oclock
 
-from .record import SensorError
+from .general import NumericalGraphBase, UpdateGraphBase
+from ..record import SensorError
 
 # The two lines below have been added following a console FutureWarning:
 # "Using an implicitly registered datetime converter for a matplotlib plotting
 # method. The converter was registered by pandas on import. Future versions of
 # pandas will require you to explicitly register matplotlib converters."
 try:
     import pandas as pd
@@ -57,193 +53,70 @@
 
 # Misc =======================================================================
 
 
 local_timezone = tzlocal.get_localzone()
 
 
-# ----------------------------------------------------------------------------
-
-
-class GraphBase(ABC):
-    """Base class for managing plotting of arbitrary measurement data"""
-
-    @abstractmethod
-    def format_measurement(self, measurement):
-        """Transform measurement from the queue into something usable by plot()
-
-        must return a dict with keys (at least):
-        - 'name' (identifier of sensor)
-        - 'values' (iterable of numerical values read by sensor)
-        - 'time' (time)
-
-        Subclass to adapt to your application.
-        """
-        pass
-
-    @abstractmethod
-    def plot(self, measurement):
-        """Plot individual measurement on existing graph.
-
-        Uses output of self.format_measurement()
-        """
-        pass
-
-
-class NumericalGraphBase(GraphBase):
-
-    def __init__(self, names, data_types, colors=None):
-        """Initiate figures and axes for data plot as a function of asked types.
-
-        Input
-        -----
-        - names: iterable of names of recordings/sensors that will be plotted.
-        - 'data types': dict with the recording names as keys, and the
-                        corresponding data types as values.
-        - 'colors': optional dict of colors with keys 'fig', 'ax', and the
-                    names of the recordings.
-        """
-        self.names = names
-        self.data_types = data_types
-        self.colors = colors
-
-        self.fig, self.axs = self.create_axes()
-
-        self.format_graph()
-        self.set_colors()
-        self.fig.tight_layout()
-
-        # Create onclick callback to activate / deactivate autoscaling
-        self.cid = self.fig.canvas.mpl_connect('button_press_event',
-                                               self.onclick)
-
-    @property
-    def all_data_types(self):
-        """Return a set of all datatypes corresponding to the active names."""
-        all_types = ()
-        for name in self.names:
-            data_types = self.data_types[name]
-            all_types += data_types
-        return set(all_types)
-
-    @staticmethod
-    def onclick(event):
-        """Activate/deactivate autoscale by clicking to allow for data inspection.
-
-        - Left click (e.g. when zooming, panning, etc.): deactivate autoscale
-        - Right click: reactivate autoscale.
-        """
-        ax = event.inaxes
-        if ax is None:
-            pass
-        elif event.button == 1:                        # left click
-            ax.axes.autoscale(False, axis='both')
-        elif event.button == 3:                        # right click
-            ax.axes.autoscale(True, axis='both')
-        else:
-            pass
-
-    def set_colors(self):
-        """"Define fig/ax colors if supplied"""
-        if self.colors is not None:
-            self.fig.set_facecolor(self.colors['fig'])
-
-            for ax in self.axs.values():
-                ax.set_facecolor(self.colors['ax'])
-                ax.grid()
-        else:
-            self.colors = {name: None for name in self.names}
+# =============================== Main classes ===============================
 
-    def create_axes(self):
-        """To be defined in subclasses. Returns fig, axs"""
-        pass
 
-    def format_graph(self):
-        """To be defined in subclasses."""
-        pass
+class UpdateGraph(UpdateGraphBase):
 
+    def _manage_data(self, data):
+        self.graph.update_current_data(data)
 
-class UpdateGraph:
-
-    def __init__(self, graph, q_plot, e_stop,
-                 e_close=None, e_graph=None, dt_graph=1):
-        """Update plot with data received from a queue.
-
-        INPUTS
-        ------
-        - graph: object of GraphBase class and subclasses
-        - q_plot: dict {name: queue} with sensor names and data queues
-        - e_stop is set when there is an external stop request.
-        - e_close (optional) is set when the figure has been closed
-        - e_graph (optional) is set when the graph is activated
-        - 'dt graph': time interval to update the graph
-
-        Attention, if the figure is closed, the e_close event is triggered so
-        do not put in e_close a threading event that is supposed to stay alive
-        even if the figure gets closed. Rather, use the e_stop event.
-        """
-        self.graph = graph
-        self.q_plot = q_plot
-        self.e_stop = e_stop
-        self.e_close = e_close
-        self.e_graph = e_graph
-        self.dt_graph = dt_graph
-
-        self.graph.fig.canvas.mpl_connect('close_event', self.on_fig_close)
-
-    def on_fig_close(self, event):
-        """When figure is closed, set threading events accordingly."""
-        if self.e_close is not None:
-            self.e_close.set()
-        if self.e_graph is not None:
-            self.e_graph.clear()
-
-    def plot_new_data(self, i):
-        """define what to do at each loop of the matplotlib animation."""
-
-        for queue in self.q_plot.values():
-            while queue.qsize() > 0:
-                measurement = queue.get()
-                self.graph.plot(measurement)
-
-        if self.e_stop.is_set():
-            plt.close(self.graph.fig)
-            # since figure is closed, e_close and e_graph are taken care of
-            # by the on_fig_close() function
-
-    def run(self):
-
-        # Below, it does not work if there is no value = before the FuncAnimation
-        ani = FuncAnimation(fig=self.graph.fig,
-                            func=self.plot_new_data,
-                            interval=self.dt_graph * 1000,
-                            cache_frame_data=False)
-
-        plt.show(block=True)  # block=True allow the animation to work even
-        # when matplotlib is in interactive mode (plt.ion()).
-
-        return ani
+    def after_getting_measurements(self):
+        self.graph.update_lines()
+        self.graph.update_time_formatting()
 
 
 class NumericalGraph(NumericalGraphBase):
 
-    def __init__(self, names, data_types, colors=None):
+    def __init__(self,
+                 names,
+                 data_types,
+                 colors=None,
+                 linestyle='.',
+                 data_as_array=False,
+                 time_conversion='datetime'):
         """Initiate figures and axes for data plot as a function of asked types.
 
         Input
         -----
         - names: iterable of names of recordings/sensors that will be plotted.
-        - 'data types': dict with the recording names as keys, and the
-                        corresponding data types as values.
-        - 'colors': optional dict of colors with keys 'fig', 'ax', and the
-                    names of the recordings.
+        - data types: dict with the recording names as keys, and the
+                      corresponding data types as values.
+                      (dict can have more keys than those in 'names')
+        - colors: optional dict of colors with keys 'fig', 'ax', and the
+                  names of the recordings.
+        - linestyle: Matplotlib linestyle (e.g. '.', '-', '.-' etc.)
+        - data_as_array: if sensors return arrays of values for different times
+                         instead of values for a single time, put this
+                         bool as True (default False)
+        - time_conversion: how to convert from unix time to datetime;
+                           possible values: 'datetime', 'numpy', 'pandas'
+                           ('datetime' and 'pandas' are timezone aware
+                            'numpy is not)
         """
         self.timezone = local_timezone
 
-        super().__init__(names=names, data_types=data_types, colors=colors)
+        time_converters = {'datetime': self._to_datetime_datetime,
+                           'numpy': self._to_datetime_numpy,
+                           'pandas': self._to_datetime_pandas}
+
+        self.time_converter = time_converters[time_conversion]
+
+        super().__init__(names=names,
+                         data_types=data_types,
+                         colors=colors,
+                         linestyle=linestyle,
+                         data_as_array=data_as_array)
+
+        self.current_data = self.create_empty_data()  # For live updates
 
     def create_axes(self):
         """Generate figure/axes as a function of input data types"""
 
         if len(self.all_data_types) == 4:
             fig, axes = plt.subplots(2, 2, figsize=(10, 9))
         if len(self.all_data_types) == 3:
@@ -258,106 +131,167 @@
             raise Exception(msg)
 
         axs = {}
         for ax, datatype in zip(axes, self.all_data_types):
             ax.set_ylabel(datatype)
             axs[datatype] = ax
 
-        return fig, axs
+        self.fig = fig
+        self.axs = axs
 
     def format_graph(self):
         """Set colors, time formatting, etc."""
 
         # Concise formatting of time -----------------------------------------
 
         self.locator = {}
         self.formatter = {}
 
         for ax in self.axs.values():
             self.locator[ax] = mdates.AutoDateLocator(tz=self.timezone)
             self.formatter[ax] = mdates.ConciseDateFormatter(self.locator,
                                                              tz=self.timezone)
 
+        # Create line objects for every sensor channel -----------------------
+        self.create_lines()
+
+    @property
+    def animated_artists(self):
+        return self.lines_list
+
     # ============================= Main methods =============================
 
+    def _to_datetime_datetime(self, unix_time):
+        """Transform single value of unix time into timezone-aware datetime."""
+        return datetime.fromtimestamp(unix_time, self.timezone)
+
     @staticmethod
     def _to_datetime_numpy(unix_times):
         """Transform iterable / array of unix times into datetimes.
 
         Note: this is the fastest method, but the datetimes are in UTC format
               (not local time)
         """
         return (np.array(unix_times) * 1e9).astype('datetime64[ns]')
 
-    @staticmethod
-    def _to_datetime_pandas(unix_times):
+    def _to_datetime_pandas(self, unix_times):
         """Transform iterable / array of datetimes into pandas Series.
 
         Note: here, the datetimes are in local timezone format, but this is
               slower than the numpy approach.
         """
         # For some reason, it's faster (and more precise) to convert to numpy first
         np_times = (np.array(unix_times) * 1e9).astype('datetime64[ns]')
         pd_times = pd.Series(np_times)
-        return pd.to_datetime(pd_times, utc=True).dt.tz_convert(local_timezone)
+        return pd.to_datetime(pd_times, utc=True).dt.tz_convert(self.timezone)
 
     def format_measurement(self, measurement):
         """Transform measurement from the queue into something usable by plot()
 
         must return a dict with keys (at least):
         - 'name' (identifier of sensor)
         - 'values' (iterable of numerical values read by sensor)
         - 'time' (time)
 
         Subclass to adapt to your application.
         """
         data = {key: measurement[key] for key in ('name', 'values')}
         t_unix = measurement['time (unix)']
-        try:
-            # works if time is a single value (int or float)
-            data['time'] = datetime.fromtimestamp(t_unix, local_timezone)
-        except TypeError:
-            # works if time is an array
-            if pandas_available:
-                data['time'] = self._to_datetime_pandas(t_unix)
-            else:
-                data['time'] = self._to_datetime_numpy(t_unix)
-
+        data['time'] = self.time_converter(t_unix)
         return data
 
-    def plot(self, measurement):
-        """Generic plot method that chooses axes depending on data type.
+    # For static plots -------------------------------------------------------
 
-        measurement is an object from the data queue.
-        """
-        # The line below allows some sensors to avoid being plotted by reading
-        # None when called.
-        if measurement is None:
-            return
-
-        data = self.format_measurement(measurement)
+    def _plot(self, data):
+        """Generic plot method for static data.
 
+        data is a dict obtained from format_measurement(measurement)
+        where measurement is an object from the data queue.
+        """
         name = data['name']
         values = data['values']
         time = data['time']
 
         dtypes = self.data_types[name]  # all data types for this specific signal
         clrs = self.colors[name]
 
         for value, dtype, clr in zip(values, dtypes, clrs):
             ax = self.axs[dtype]  # plot data in correct axis depending on type
-            ax.plot(time, value, '.', color=clr)
+            ax.plot(time, value, self.linestyle, color=clr)
 
         # Use Concise Date Formatting for minimal space used on screen by time
         different_types = set(dtypes)
         for dtype in different_types:
             ax = self.axs[dtype]
             ax.xaxis.set_major_locator(self.locator[ax])
             ax.xaxis.set_major_formatter(self.formatter[ax])
 
+    # For updated plots ------------------------------------------------------
+
+    def update_current_data(self, data):
+        """Store measurement time and values in active data lists."""
+
+        name = data['name']
+        values = data['values']
+        time = data['time']
+
+        self.current_data[name]['times'].append(time)
+        for i, value in enumerate(values):
+            self.current_data[name]['values'][i].append(value)
+
+    def update_lines(self):
+        """Update line positions with current data."""
+
+        for lines, current_data in zip(self.lines.values(),
+                                       self.current_data.values()):
+
+            if not current_data['times']:  # No data yet
+                return
+
+            times = self.timelist_to_array(current_data['times'])
+
+            for line, curr_values in zip(lines,
+                                         current_data['values']):
+
+                values = self.datalist_to_array(curr_values)
+                line.set_data(times, values)
+
+    def update_time_formatting(self):
+        """Use Concise Date Formatting for minimal space used on screen by time"""
+        for ax in self.axs.values():
+            ax.xaxis.set_major_locator(self.locator[ax])
+            ax.xaxis.set_major_formatter(self.formatter[ax])
+            # Lines below are needed for autoscaling to work
+            ax.relim()
+            ax.autoscale_view(tight=True, scalex=True, scaley=True)
+
+    def run(self, q_plot, e_stop=None, e_close=None, e_graph=None,
+            dt_graph=0.1, blit=False):
+        """Run live view of plot with data from queues.
+
+        (Convenience method to instantiate a UpdateGraph object)
+
+        Parameters
+        ----------
+        - q_plot: dict {name: queue} with sensor names and data queues
+        - e_stop (optional): external stop request, closes the figure if set
+        - e_close (optional) is set when the figure has been closed
+        - e_graph (optional) is set when the graph is activated
+        - dt graph: time interval to update the graph
+        - blit: if True, use blitting to speed up the matplotlib animation
+        """
+        update_plot = UpdateGraph(graph=self,
+                                  q_plot=q_plot,
+                                  e_stop=e_stop,
+                                  e_close=e_close,
+                                  e_graph=e_graph,
+                                  dt_graph=dt_graph,
+                                  blit=blit)
+        update_plot.run()
+
 
 # ============== Classes using Graph-like objects to plot data ===============
 
 
 # ------------------------------- Static graph -------------------------------
 
 
@@ -435,21 +369,19 @@
             Thread(target=self.get_data, args=(name,)).start()
 
         self.e_graph.set()  # This is supposed to be set when graph is active.
 
         # e_stop two times, because we want a figure closure event to also
         # trigger stopping of the recording process here.
 
-        update_graph = UpdateGraph(self.graph,
-                                   q_plot=self.queues,
-                                   e_stop=self.e_stop,
-                                   e_close=self.e_stop,
-                                   e_graph=self.e_graph,
-                                   dt_graph=self.dt_graph)
-        update_graph.run()
+        self.graph.run(q_plot=self.queues,
+                       e_stop=self.e_stop,
+                       e_close=self.e_stop,
+                       e_graph=self.e_graph,
+                       dt_graph=self.dt_graph)
 
 
 class PlotLiveSensors(PlotUpdatedData):
     """Create live graph by reading the sensors directly."""
 
     def __init__(self, graph, recordings, dt_data=1, dt_graph=1):
         """Parameters:
```

### Comparing `prevo-0.8.1/prevo/record.py` & `prevo-0.9.0/prevo/record.py`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/prevo/viewers.py` & `prevo-0.9.0/prevo/viewers.py`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/prevo.egg-info/PKG-INFO` & `prevo-0.9.0/prevo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: prevo
-Version: 0.8.1
+Version: 0.9.0
 Summary: Record arbitrary sensors periodically in an asynchronous manner. Control their properties in real time from CLI. Graph/view tools to visualize live data/images are also provided.
 Home-page: https://github.com/ovinc/prevo
 Author: Olivier Vincent
 Author-email: ovinc.py@gmail.com
 License: UNKNOWN
 Description: About
         =====
         
-        **P**eriodic **RE**cording and **V**isualization of sensor **O**bjects
+        **P**eriodic **RE**cording and **V**isualization of (sensor) **O**bjects
         
         This package provides base classes to rapidly create interactive data recording for various applications (e.g. recording of temperature, time-lapses with cameras etc.). Sensors are read in a asynchronous fashion and can have different time intervals for data reading (or be continuous, i.e. as fast as possible). Tools for graphical visualizations of data during recording are also provided.
         
         Install
         -------
         
         ```bash
@@ -152,15 +152,15 @@
         
         
         Additional tools
         ================
         
         Some elements are also provided to simplify and/or extend the classes above:
         
-        - plot numerical data in real time (see `prevo.plot`)
+        - plot numerical data in real time (see `prevo.plot` module and `GraphExamples.ipynb`)
         - live view images from camera-like sensors (see `prevo.viewers`)
         - read / save with CSV files (see `prevo.csv`)
         - parse command line arguments to trigger functions or class methods (see `prevo.parser`)
         - some tools to format measurements for `Record`-like classes (see `prevo.measurements`)
         
         See docstrings for more help.
```

### Comparing `prevo-0.8.1/setup.cfg` & `prevo-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/setup.py` & `prevo-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `prevo-0.8.1/tests/test_prevo.py` & `prevo-0.9.0/tests/test_prevo.py`

 * *Files identical despite different names*

