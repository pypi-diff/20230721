# Comparing `tmp/ex4nicegui-0.2.1.tar.gz` & `tmp/ex4nicegui-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.2.1.tar", last modified: Wed Jul 19 08:12:51 2023, max compression
+gzip compressed data, was "ex4nicegui-0.2.2.tar", last modified: Thu Jul 20 18:25:30 2023, max compression
```

## Comparing `ex4nicegui-0.2.1.tar` & `ex4nicegui-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.528882 ex4nicegui-0.2.1/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-19 08:12:51.527884 ex4nicegui-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.401218 ex4nicegui-0.2.1/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-19 08:12:32.000000 ex4nicegui-0.2.1/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.417901 ex4nicegui-0.2.1/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.2.1/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.2.1/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.435106 ex4nicegui-0.2.1/ex4nicegui/reactive/
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.461398 ex4nicegui-0.2.1/ex4nicegui/reactive/ECharts/
--rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/ECharts/ECharts.js
--rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/ECharts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/ECharts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.467128 ex4nicegui-0.2.1/ex4nicegui/reactive/UseDraggable/
--rw-rw-rw-   0        0        0     4857 2023-07-17 16:36:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/UseDraggable/UseDraggable.js
--rw-rw-rw-   0        0        0     2888 2023-07-17 16:36:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/UseDraggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/UseDraggable/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-07-18 10:52:11.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/drawer.py
--rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0    41789 2023-07-19 08:10:43.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/officials.py
--rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/rxui.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.483484 ex4nicegui-0.2.1/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2468 2023-07-19 08:10:43.000000 ex4nicegui-0.2.1/ex4nicegui/reactive/usePagination.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.487335 ex4nicegui-0.2.1/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.2.1/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.2.1/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.525887 ex4nicegui-0.2.1/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.1/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.2.1/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.2.1/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:12:51.413912 ex4nicegui-0.2.1/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-19 08:12:51.000000 ex4nicegui-0.2.1/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1101 2023-07-19 08:12:51.000000 ex4nicegui-0.2.1/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 08:12:51.000000 ex4nicegui-0.2.1/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-19 08:12:51.000000 ex4nicegui-0.2.1/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-19 08:12:51.000000 ex4nicegui-0.2.1/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-19 08:12:51.000000 ex4nicegui-0.2.1/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 08:12:51.529817 ex4nicegui-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-07-18 10:52:21.000000 ex4nicegui-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.551543 ex4nicegui-0.2.2/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-20 18:25:30.550569 ex4nicegui-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.493533 ex4nicegui-0.2.2/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-20 18:25:11.000000 ex4nicegui-0.2.2/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.508113 ex4nicegui-0.2.2/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.2.2/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.2.2/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.522547 ex4nicegui-0.2.2/ex4nicegui/reactive/
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.530887 ex4nicegui-0.2.2/ex4nicegui/reactive/ECharts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/ECharts/ECharts.js
+-rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/ECharts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/ECharts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.535636 ex4nicegui-0.2.2/ex4nicegui/reactive/UseDraggable/
+-rw-rw-rw-   0        0        0     4857 2023-07-17 16:36:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     2888 2023-07-17 16:36:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-07-18 10:52:11.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/drawer.py
+-rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0    41993 2023-07-20 18:15:39.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/officials.py
+-rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/rxui.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.540020 ex4nicegui-0.2.2/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2468 2023-07-19 08:10:43.000000 ex4nicegui-0.2.2/ex4nicegui/reactive/usePagination.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.543015 ex4nicegui-0.2.2/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.2.2/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.2.2/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.548547 ex4nicegui-0.2.2/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.2/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.2.2/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.2.2/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:25:30.504983 ex4nicegui-0.2.2/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-20 18:25:30.000000 ex4nicegui-0.2.2/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1101 2023-07-20 18:25:30.000000 ex4nicegui-0.2.2/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:25:30.000000 ex4nicegui-0.2.2/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 18:25:30.000000 ex4nicegui-0.2.2/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-20 18:25:30.000000 ex4nicegui-0.2.2/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-20 18:25:30.000000 ex4nicegui-0.2.2/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 18:25:30.551543 ex4nicegui-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-07-18 10:52:21.000000 ex4nicegui-0.2.2/setup.py
```

### Comparing `ex4nicegui-0.2.1/LICENSE` & `ex4nicegui-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/README.md` & `ex4nicegui-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.2.2/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/ECharts/ECharts.js` & `ex4nicegui-0.2.2/ex4nicegui/reactive/ECharts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/ECharts/ECharts.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/ECharts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/UseDraggable/UseDraggable.js` & `ex4nicegui-0.2.2/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/UseDraggable/UseDraggable.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/__index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/officials.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/officials.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,23 +334,27 @@
         return self
 
 
 class SwitchBindableUi(SingleValueBindableUi[bool, ui.switch]):
     @staticmethod
     def _setup_(binder: "SwitchBindableUi"):
         def onValueChanged(e):
-            binder._ref.value = e.args  # type: ignore
+            ele._send_update_on_value_change = ele.LOOPBACK
+            cur_value = ele._event_args_to_value(e)
+            ele.set_value(cur_value)
+            ele._send_update_on_value_change = True
+            binder._ref.value = cur_value
 
         ele = cast(ValueElement, binder.element)
 
         @effect
         def _():
             ele.value = binder.value
 
-        ele.on("update:modelValue", handler=onValueChanged)
+        ele.on("update:modelValue", onValueChanged, [None], throttle=0)
 
     def __init__(
         self,
         text: TMaybeRef[str] = "",
         *,
         value: TMaybeRef[bool] = False,
         on_change: Optional[Callable[..., Any]] = None,
```

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/q_pagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.2.2/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.2.2/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/tools/debug.py` & `ex4nicegui-0.2.2/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui/utils/signals.py` & `ex4nicegui-0.2.2/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.2.2/ex4nicegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.1/setup.py` & `ex4nicegui-0.2.2/setup.py`

 * *Files identical despite different names*

