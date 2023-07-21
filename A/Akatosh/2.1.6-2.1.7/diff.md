# Comparing `tmp/Akatosh-2.1.6.tar.gz` & `tmp/Akatosh-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.6.tar", last modified: Wed Jul 19 04:57:01 2023, max compression
+gzip compressed data, was "Akatosh-2.1.7.tar", last modified: Fri Jul 21 05:28:57 2023, max compression
```

## Comparing `Akatosh-2.1.6.tar` & `Akatosh-2.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 04:57:01.648851 Akatosh-2.1.6/
-drwxrwxrwx   0        0        0        0 2023-07-19 04:57:01.634853 Akatosh-2.1.6/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-07-13 05:05:39.000000 Akatosh-2.1.6/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    14879 2023-07-19 04:52:07.000000 Akatosh-2.1.6/Akatosh/entity.py
--rw-rw-rw-   0        0        0    13327 2023-07-17 05:10:45.000000 Akatosh-2.1.6/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-11 12:42:40.000000 Akatosh-2.1.6/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-11 12:42:40.000000 Akatosh-2.1.6/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-11 12:42:40.000000 Akatosh-2.1.6/Akatosh/states.py
--rw-rw-rw-   0        0        0     6365 2023-07-19 04:55:41.000000 Akatosh-2.1.6/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-19 04:57:01.644852 Akatosh-2.1.6/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-19 04:57:01.646852 Akatosh-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-11 12:42:40.000000 Akatosh-2.1.6/README.md
--rw-rw-rw-   0        0        0      635 2023-07-19 04:56:29.000000 Akatosh-2.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-19 04:57:01.649852 Akatosh-2.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 05:28:57.560065 Akatosh-2.1.7/
+drwxrwxrwx   0        0        0        0 2023-07-21 05:28:57.502698 Akatosh-2.1.7/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.7/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    14879 2023-07-20 01:56:56.000000 Akatosh-2.1.7/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    13484 2023-07-21 05:26:19.000000 Akatosh-2.1.7/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.7/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-20 06:14:59.000000 Akatosh-2.1.7/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.7/Akatosh/states.py
+-rw-rw-rw-   0        0        0     6365 2023-07-20 01:43:52.000000 Akatosh-2.1.7/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:28:57.547165 Akatosh-2.1.7/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-21 05:28:57.551339 Akatosh-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.7/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-21 05:27:30.000000 Akatosh-2.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 05:28:57.561031 Akatosh-2.1.7/setup.cfg
```

### Comparing `Akatosh-2.1.6/Akatosh/entity.py` & `Akatosh-2.1.7/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.6/Akatosh/event.py` & `Akatosh-2.1.7/Akatosh/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,19 +64,25 @@
             raise RuntimeError(f"Event {self.label} tries to later the past.")
         else:
             Mundus.current_events.append(self)
 
     def end(self):
         """End the event and activate the follower events if there is any."""
         self.state = State.ENDED
+        if self in Mundus.future_events:
+            Mundus.future_events.remove(self)
+        if self in Mundus.current_events:
+            Mundus.current_events.remove(self)
+        Mundus.past_events.append(self)
         for event in self.follower:
             try:
                 event.activate()
             except RuntimeError:
                 logger.debug(f"Event {event.label} passed due time.")
+        logger.debug(f"Event {self.label} is ended.")
 
     def activate(self, force: bool = False):
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
 
         if force:
             self.state = State.ACTIVE
@@ -97,15 +103,15 @@
             RuntimeError: raise if the event has already ended.
         """
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
         self.state = State.INACTIVE
 
     def cancel(self):
-        """Cancel the event.
+        """Cancel the event. Will not set the follower events to active.
 
         Raises:
             RuntimeError: raise if the event has already ended.
         """
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
         self.state = State.CANCELED
@@ -221,15 +227,14 @@
                 if inspect.iscoroutinefunction(self.action):
                     await self.action()
                 else:
                     self.action()
             Mundus.current_events.remove(self)
             Mundus.past_events.append(self)
             self.end()
-            logger.debug(f"Event {self.label} is ended.")
 
 
 def instant_event(
     at: int | float | Callable,
     precursor: Event | List[Event] | None = None,
     priority: int | float | Callable = 0,
     label: str | None = None,
@@ -304,19 +309,17 @@
             if callable(self.interval):
                 self._at = round(self.interval() + Mundus.now, Mundus.resolution)
             else:
                 self._at = round(self.interval + Mundus.now, Mundus.resolution)
             if self.at <= self.till:
                 logger.debug(f"Event {self.label} next step is at {self.at}.")
                 Mundus.future_events.append(self)
+                Mundus.current_events.remove(self)
             else:
                 self.end()
-                logger.debug(f"Event {self.label} is ended.")
-            Mundus.current_events.remove(self)
-            Mundus.past_events.append(self)
 
     @property
     def interval(self) -> int | float | Callable[..., Any]:
         """Return the interval between each action repeat."""
         return self._interval
 
     @property
```

### Comparing `Akatosh-2.1.6/Akatosh/resource.py` & `Akatosh-2.1.7/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.6/Akatosh/universe.py` & `Akatosh-2.1.7/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.6/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.7/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.6
+Version: 2.1.7
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.6/PKG-INFO` & `Akatosh-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.6
+Version: 2.1.7
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.6/README.md` & `Akatosh-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.6/pyproject.toml` & `Akatosh-2.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.6"
+version = "2.1.7"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

