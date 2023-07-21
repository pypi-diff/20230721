# Comparing `tmp/streams_py-0.3.tar.gz` & `tmp/streams_py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_py-0.3.tar", max compression
+gzip compressed data, was "streams_py-0.3.1.tar", max compression
```

## Comparing `streams_py-0.3.tar` & `streams_py-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35149 2023-07-20 18:17:11.485866 streams_py-0.3/LICENSE
--rw-r--r--   0        0        0    10867 2023-07-20 18:17:11.485866 streams_py-0.3/README.md
--rw-r--r--   0        0        0      731 2023-07-20 18:17:11.489866 streams_py-0.3/pyproject.toml
--rw-r--r--   0        0        0      155 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__init__.py
--rw-r--r--   0        0        0      336 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__iterate.py
--rw-r--r--   0        0        0     3910 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__optional.py
--rw-r--r--   0        0        0     3483 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/__stream.py
--rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_itertools/__init__.py
--rw-r--r--   0        0        0     1713 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_itertools/tools.py
--rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_lazy/__init__.py
--rw-r--r--   0        0        0      626 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_lazy/process.py
--rw-r--r--   0        0        0      593 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_lazy/queue.py
--rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_parallel/__init__.py
--rw-r--r--   0        0        0     3885 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_parallel/fork_and_join.py
--rw-r--r--   0        0        0      787 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_parallel/parallelizer.py
--rw-r--r--   0        0        0    13872 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__base_stream.py
--rw-r--r--   0        0        0        0 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__init__.py
--rw-r--r--   0        0        0     3629 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__parallel_stream.py
--rw-r--r--   0        0        0     2482 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/__sequential_stream.py
--rw-r--r--   0        0        0     3271 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/error/__error.py
--rw-r--r--   0        0        0      258 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/error/__levels.py
--rw-r--r--   0        0        0      307 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/error/__sentinel.py
--rw-r--r--   0        0        0     3595 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/numeric/__numeric_base_stream.py
--rw-r--r--   0        0        0      861 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
--rw-r--r--   0        0        0      686 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
--rw-r--r--   0        0        0      221 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/conditions/__init__.py
--rw-r--r--   0        0        0      307 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/conditions/combiners.py
--rw-r--r--   0        0        0    10878 2023-07-20 18:17:11.489866 streams_py-0.3/pystreamapi/conditions/date.py
--rw-r--r--   0        0        0     4937 2023-07-20 18:17:11.493867 streams_py-0.3/pystreamapi/conditions/numeric.py
--rw-r--r--   0        0        0     1385 2023-07-20 18:17:11.493867 streams_py-0.3/pystreamapi/conditions/string.py
--rw-r--r--   0        0        0      735 2023-07-20 18:17:11.493867 streams_py-0.3/pystreamapi/conditions/types.py
--rw-r--r--   0        0        0    11720 1970-01-01 00:00:00.000000 streams_py-0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 14:03:59.216597 streams_py-0.3.1/LICENSE
+-rw-r--r--   0        0        0    10867 2023-07-21 14:03:59.216597 streams_py-0.3.1/README.md
+-rw-r--r--   0        0        0      733 2023-07-21 14:03:59.220598 streams_py-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3910 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__optional.py
+-rw-r--r--   0        0        0     3483 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/__stream.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_itertools/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_itertools/tools.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     3885 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0      787 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_parallel/parallelizer.py
+-rw-r--r--   0        0        0    14521 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:03:59.220598 streams_py-0.3.1/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3629 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2482 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3062 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/error/__error.py
+-rw-r--r--   0        0        0      258 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/error/__levels.py
+-rw-r--r--   0        0        0      307 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/error/__sentinel.py
+-rw-r--r--   0        0        0     3595 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      861 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      686 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0    10878 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2023-07-21 14:03:59.224598 streams_py-0.3.1/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0    11722 1970-01-01 00:00:00.000000 streams_py-0.3.1/PKG-INFO
```

### Comparing `streams_py-0.3/LICENSE` & `streams_py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/README.md` & `streams_py-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pyproject.toml` & `streams_py-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streams.py"
-version = "0.3"
+version = "0.3.1"
 authors = ["Stefan Garlonta <stefan@pickwicksoft.org>"]
 description = "A stream library for Python inspired by Java Stream API"
 keywords = ["streams", "parallel", "data"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/PickwickSoft/pystreamapi"
 repository = "https://github.com/PickwickSoft/pystreamapi"
 readme = "README.md"
```

### Comparing `streams_py-0.3/pystreamapi/__optional.py` & `streams_py-0.3.1/pystreamapi/__optional.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/__stream.py` & `streams_py-0.3.1/pystreamapi/__stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_itertools/tools.py` & `streams_py-0.3.1/pystreamapi/_itertools/tools.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_lazy/process.py` & `streams_py-0.3.1/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_lazy/queue.py` & `streams_py-0.3.1/pystreamapi/_lazy/queue.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_parallel/fork_and_join.py` & `streams_py-0.3.1/pystreamapi/_parallel/fork_and_join.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_parallel/parallelizer.py` & `streams_py-0.3.1/pystreamapi/_parallel/parallelizer.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_streams/__base_stream.py` & `streams_py-0.3.1/pystreamapi/_streams/__base_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # pylint: disable=protected-access
 from __future__ import annotations
 import functools
 import itertools
 from abc import abstractmethod
 from builtins import reversed
 from functools import cmp_to_key
-from typing import Iterable, Callable, Any, TypeVar, Iterator, TYPE_CHECKING
+from typing import Iterable, Callable, Any, TypeVar, Iterator, TYPE_CHECKING, Union
 
 from pystreamapi.__optional import Optional
 from pystreamapi._itertools.tools import dropwhile
 from pystreamapi._lazy.process import Process
 from pystreamapi._lazy.queue import ProcessQueue
 from pystreamapi._streams.error.__error import ErrorHandler
+from pystreamapi._streams.error.__levels import ErrorLevel
+
 if TYPE_CHECKING:
     from pystreamapi._streams.numeric.__numeric_base_stream import NumericBaseStream
 
 K = TypeVar('K')
 _V = TypeVar('_V')
 _identity_missing = object()
 
@@ -89,38 +91,50 @@
 
         :param streams: The streams to concatenate
         :return: The concatenated stream
         """
         return cls(itertools.chain(*list(streams)))
 
     @_operation
-    def distinct(self) -> 'BaseStream[_V]':
+    def distinct(self) -> 'BaseStream[K]':
         """Returns a stream consisting of the distinct elements of this stream."""
         self._queue.append(Process(self.__distinct))
         return self
 
     def __distinct(self):
         """Removes duplicate elements from the stream."""
         self._source = list(set(self._source))
 
     @_operation
-    def drop_while(self, predicate: Callable[[K], bool]) -> 'BaseStream[_V]':
+    def drop_while(self, predicate: Callable[[K], bool]) -> 'BaseStream[K]':
         """
         Returns, if this stream is ordered, a stream consisting of the remaining elements of this
         stream after dropping the longest prefix of elements that match the given predicate.
 
         :param predicate:
         """
         self._queue.append(Process(self.__drop_while, predicate))
         return self
 
     def __drop_while(self, predicate: Callable[[Any], bool]):
         """Drops elements from the stream while the predicate is true."""
         self._source = list(dropwhile(predicate, self._source, self))
 
+    def error_level(self, level: ErrorLevel, *exceptions)\
+            -> Union["BaseStream[K]", NumericBaseStream]:
+        """
+        Sets the error level of the stream. If an exception is raised during the execution of the
+        stream, the error level determines what to do with the exception.
+        :param level: Error level from ErrorLevel
+        :param exceptions: Exceptions to ignore. If not provided, all exceptions will be ignored
+        :return: The stream itself
+        """
+        self._queue.append(Process(lambda: self._error_level(level, *exceptions)))
+        return self
+
     @_operation
     def filter(self, predicate: Callable[[K], bool]) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the elements of this stream that match the given predicate.
 
         :param predicate:
         """
@@ -164,15 +178,15 @@
         self._source = groups.items()
 
     @abstractmethod
     def _group_to_dict(self, key_mapper: Callable[[K], Any]) -> dict[K, list]:
         """Groups the stream into a dictionary. Should be implemented by subclasses."""
 
     @_operation
-    def limit(self, max_size: int) -> 'BaseStream[_V]':
+    def limit(self, max_size: int) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the elements of this stream, truncated to be no longer
         than maxSize in length.
 
         :param max_size:
         """
         self._queue.append(Process(self.__limit, max_size))
@@ -194,41 +208,41 @@
         return self
 
     @abstractmethod
     def _map(self, mapper: Callable[[K], _V]):
         """Implementation of map. Should be implemented by subclasses."""
 
     @_operation
-    def map_to_int(self) -> NumericBaseStream[_V]:
+    def map_to_int(self) -> NumericBaseStream:
         """
         Returns a stream consisting of the results of converting the elements of this stream to
         integers.
         """
         self._queue.append(Process(self.__map_to_int))
         return self._to_numeric_stream()
 
     def __map_to_int(self):
         """Converts the stream to integers."""
         self._map(int)
 
     @_operation
-    def map_to_str(self) -> 'BaseStream[_V]':
+    def map_to_str(self) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the results of converting the elements of this stream to
         strings.
         """
         self._queue.append(Process(self.__map_to_str))
         return self
 
     def __map_to_str(self):
         """Converts the stream to strings."""
         self._map(str)
 
     @_operation
-    def peek(self, action: Callable) -> 'BaseStream[_V]':
+    def peek(self, action: Callable) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the elements of this stream, additionally performing the
         provided action on each element as elements are consumed from the resulting stream.
 
         :param action:
         """
         self._queue.append(Process(self._peek, action))
@@ -236,15 +250,15 @@
 
     @abstractmethod
     @_operation
     def _peek(self, action: Callable):
         """Implementation of peek. Should be implemented by subclasses."""
 
     @_operation
-    def reversed(self) -> 'BaseStream[_V]':
+    def reversed(self) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the elements of this stream, with their order being
         reversed.
         """
         self._queue.append(Process(self.__reversed))
         return self
 
@@ -252,30 +266,30 @@
         """Reverses the stream."""
         try:
             self._source = reversed(self._source)
         except TypeError:
             self._source = reversed(list(self._source))
 
     @_operation
-    def skip(self, n: int) -> 'BaseStream[_V]':
+    def skip(self, n: int) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the remaining elements of this stream after discarding the
         first n elements of the stream.
 
         :param n:
         """
         self._queue.append(Process(self.__skip, n))
         return self
 
     def __skip(self, n: int):
         """Skips the first n elements of the stream."""
         self._source = self._source[n:]
 
     @_operation
-    def sorted(self, comparator: Callable[[K], int] = None) -> 'BaseStream[_V]':
+    def sorted(self, comparator: Callable[[K], int] = None) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the elements of this stream, sorted according to natural
         order.
         """
         self._queue.append(Process(self.__sorted, comparator))
         return self
 
@@ -283,15 +297,15 @@
         """Sorts the stream."""
         if comparator is None:
             self._source = sorted(self._source)
         else:
             self._source = sorted(self._source, key=cmp_to_key(comparator))
 
     @_operation
-    def take_while(self, predicate: Callable[[K], bool]) -> 'BaseStream[_V]':
+    def take_while(self, predicate: Callable[[K], bool]) -> 'BaseStream[K]':
         """
         Returns, if this stream is ordered, a stream consisting of the longest prefix of elements
         taken from this stream that match the given predicate.
 
         :param predicate:
         """
         self._queue.append(Process(self.__take_while, predicate))
@@ -413,9 +427,9 @@
         Returns a dictionary consisting of the results of grouping the elements of this stream
         by the given classifier.
 
         :param key_mapper:
         """
 
     @abstractmethod
-    def _to_numeric_stream(self) -> NumericBaseStream[_V]:
+    def _to_numeric_stream(self) -> NumericBaseStream:
         """Converts a stream to a numeric stream. To be implemented by subclasses."""
```

### Comparing `streams_py-0.3/pystreamapi/_streams/__parallel_stream.py` & `streams_py-0.3.1/pystreamapi/_streams/__parallel_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_streams/__sequential_stream.py` & `streams_py-0.3.1/pystreamapi/_streams/__sequential_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_streams/error/__error.py` & `streams_py-0.3.1/pystreamapi/_streams/error/__error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING
+
 from pystreamapi._streams.error.__levels import ErrorLevel
 from pystreamapi._streams.error.__sentinel import Sentinel
 
-if TYPE_CHECKING:
-    # Avoid circular import
-    from pystreamapi._streams.__base_stream import BaseStream
-
 _sentinel = Sentinel()
 
 
 def nothing(sth):
     """Do not modify the input"""
     return sth
 
@@ -24,24 +20,22 @@
 
 class ErrorHandler:
     """Handle errors in stream operations"""
 
     __error_level = ErrorLevel.RAISE
     __exceptions_to_ignore = (Exception,)
 
-    def error_level(self, level: ErrorLevel, *exceptions) -> BaseStream:
+    def _error_level(self, level: ErrorLevel, *exceptions):
         """
         Set the error level
         :param level: Error level from ErrorLevel
         :param exceptions: Exceptions to ignore. If not provided, all exceptions will be ignored
-        :return: The stream itself
         """
         self.__exceptions_to_ignore = exceptions or (Exception,)
         self.__error_level = level
-        return self
 
     def _get_error_level(self):
         """Get the error level"""
         return self.__error_level
 
     def _itr(self, src, mapper=nothing, condition=true_condition) -> list:
         """Iterate over the source and apply the mapper and condition"""
```

### Comparing `streams_py-0.3/pystreamapi/_streams/numeric/__numeric_base_stream.py` & `streams_py-0.3.1/pystreamapi/_streams/numeric/__numeric_base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py` & `streams_py-0.3.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/_streams/numeric/__sequential_numeric_stream.py` & `streams_py-0.3.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/conditions/date.py` & `streams_py-0.3.1/pystreamapi/conditions/date.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/conditions/numeric.py` & `streams_py-0.3.1/pystreamapi/conditions/numeric.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/conditions/string.py` & `streams_py-0.3.1/pystreamapi/conditions/string.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/pystreamapi/conditions/types.py` & `streams_py-0.3.1/pystreamapi/conditions/types.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3/PKG-INFO` & `streams_py-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streams-py
-Version: 0.3
+Version: 0.3.1
 Summary: A stream library for Python inspired by Java Stream API
 Home-page: https://github.com/PickwickSoft/pystreamapi
 License: GPL-3.0-or-later
 Keywords: streams,parallel,data
 Author: Stefan Garlonta
 Author-email: stefan@pickwicksoft.org
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streams-py Version: 0.3 Summary: A stream library
+Metadata-Version: 2.1 Name: streams-py Version: 0.3.1 Summary: A stream library
 for Python inspired by Java Stream API Home-page: https://github.com/
 PickwickSoft/pystreamapi License: GPL-3.0-or-later Keywords:
 streams,parallel,data Author: Stefan Garlonta Author-email:
 stefan@pickwicksoft.org Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

