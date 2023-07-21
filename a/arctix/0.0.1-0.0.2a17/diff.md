# Comparing `tmp/arctix-0.0.1.tar.gz` & `tmp/arctix-0.0.2a17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.1.tar", max compression
+gzip compressed data, was "arctix-0.0.2a17.tar", max compression
```

## Comparing `arctix-0.0.1.tar` & `arctix-0.0.2a17.tar`

### file list

```diff
@@ -1,13 +1,29 @@
--rw-r--r--   0        0        0     1501 2023-07-17 04:19:03.663776 arctix-0.0.1/LICENSE
--rw-r--r--   0        0        0     5537 2023-07-17 04:19:03.663776 arctix-0.0.1/README.md
--rw-r--r--   0        0        0     4075 2023-07-17 04:19:03.663776 arctix-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      689 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/__init__.py
--rw-r--r--   0        0        0     3301 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/_numpy.py
--rw-r--r--   0        0        0     3338 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/_torch.py
--rw-r--r--   0        0        0    13603 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/formatter.py
--rw-r--r--   0        0        0    14735 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/summarizer.py
--rw-r--r--   0        0        0      348 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/testing.py
--rw-r--r--   0        0        0        0 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0     3399 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/utils/format.py
--rw-r--r--   0        0        0     1250 2023-07-17 04:19:03.663776 arctix-0.0.1/src/arctix/utils/imports.py
--rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 arctix-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-21 06:43:48.913849 arctix-0.0.2a17/LICENSE
+-rw-r--r--   0        0        0     5494 2023-07-21 06:43:48.913849 arctix-0.0.2a17/README.md
+-rw-r--r--   0        0        0     4115 2023-07-21 06:43:48.913849 arctix-0.0.2a17/pyproject.toml
+-rw-r--r--   0        0        0      346 2023-07-21 06:43:48.913849 arctix-0.0.2a17/src/arctix/__init__.py
+-rw-r--r--   0        0        0      459 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/__init__.py
+-rw-r--r--   0        0        0     3404 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/base.py
+-rw-r--r--   0        0        0    10448 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/default.py
+-rw-r--r--   0        0        0     3174 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/numpy_.py
+-rw-r--r--   0        0        0     3182 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/formatters/torch_.py
+-rw-r--r--   0        0        0      446 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/__init__.py
+-rw-r--r--   0        0        0     8728 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/base.py
+-rw-r--r--   0        0        0     1253 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/basic.py
+-rw-r--r--   0        0        0     1842 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/numpy_.py
+-rw-r--r--   0        0        0     2904 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/registry.py
+-rw-r--r--   0        0        0     1929 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reducers/torch_.py
+-rw-r--r--   0        0        0     1893 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/reduction.py
+-rw-r--r--   0        0        0      333 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/__init__.py
+-rw-r--r--   0        0        0     1170 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/base.py
+-rw-r--r--   0        0        0    11055 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/continuous.py
+-rw-r--r--   0        0        0     4087 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/discrete.py
+-rw-r--r--   0        0        0      459 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/stats/noop.py
+-rw-r--r--   0        0        0     1647 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarization.py
+-rw-r--r--   0        0        0      276 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarizers/__init__.py
+-rw-r--r--   0        0        0     1794 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarizers/base.py
+-rw-r--r--   0        0        0    12075 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/summarizers/summarizer.py
+-rw-r--r--   0        0        0      507 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/testing.py
+-rw-r--r--   0        0        0        0 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-21 06:43:48.917849 arctix-0.0.2a17/src/arctix/utils/format.py
+-rw-r--r--   0        0        0     6555 1970-01-01 00:00:00.000000 arctix-0.0.2a17/PKG-INFO
```

### Comparing `arctix-0.0.1/LICENSE` & `arctix-0.0.2a17/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.1/README.md` & `arctix-0.0.2a17/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/arctix/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-`arctix` is a Python library that provides simple functions to check in a single line if two
-complex/nested objects are equal or not.
+`arctix` is a Python library to compute a string representation of complex/nested objects.
 `arctix` was initially designed to work
 with [PyTorch `Tensor`s](https://pytorch.org/docs/stable/tensors.html)
 and [NumPy `ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
 is possible to extend it
 to [support other data structures](https://durandtibo.github.io/arctix/customization).
 
 - [Motivation](#motivation)
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
 # arctix
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  61b8574ea18ecf106dce/maintainability] [https://api.codeclimate.com/v1/badges/
                      61b8574ea18ecf106dce/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
-## Overview `arctix` is a Python library that provides simple functions to
-check in a single line if two complex/nested objects are equal or not. `arctix`
-was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
-docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
-reference/generated/numpy.ndarray.html), but it is possible to extend it to
-[support other data structures](https://durandtibo.github.io/arctix/
-customization). - [Motivation](#motivation) - [Documentation](https://
-durandtibo.github.io/arctix/) - [Installation](#installation) - [Contributing]
-(#contributing) - [API stability](#api-stability) - [License](#license) ##
-Motivation Let's imagine you have the following dictionaries that contain both
-a PyTorch `Tensor` and a NumPy `ndarray`. You want to compute a string
-representation of it. By default, Python tries to show the values of all the
-tensor/array. The `arctix` library was developed to easily compute structured
-string representation of nested objects. `arctix` provides a function `summary`
-that can indicate if two complex/nested objects are equal or not. ```pycon >>>
-import numpy >>> import torch >>> from arctix import summary >>> print(summary(
-{"torch": torch.ones(2, 3), "numpy": numpy.zeros((2, 3))}))
+## Overview `arctix` is a Python library to compute a string representation of
+complex/nested objects. `arctix` was initially designed to work with [PyTorch
+`Tensor`s](https://pytorch.org/docs/stable/tensors.html) and [NumPy `ndarray`]
+(https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
+is possible to extend it to [support other data structures](https://
+durandtibo.github.io/arctix/customization). - [Motivation](#motivation) -
+[Documentation](https://durandtibo.github.io/arctix/) - [Installation]
+(#installation) - [Contributing](#contributing) - [API stability](#api-
+stability) - [License](#license) ## Motivation Let's imagine you have the
+following dictionaries that contain both a PyTorch `Tensor` and a NumPy
+`ndarray`. You want to compute a string representation of it. By default,
+Python tries to show the values of all the tensor/array. The `arctix` library
+was developed to easily compute structured string representation of nested
+objects. `arctix` provides a function `summary` that can indicate if two
+complex/nested objects are equal or not. ```pycon >>> import numpy >>> import
+torch >>> from arctix import summary >>> print(summary({"torch": torch.ones(2,
+3), "numpy": numpy.zeros((2, 3))}))
 dict'> (length=2) (torch):
 torch.Tensor'> | shape=torch.Size([2, 3]) | dtype=torch.float32 | device=cpu
 (numpy):
 numpy.ndarray'> | shape=(2, 3) | dtype=float64 >>> print( ... summary( ...
 { ... "torch": [torch.ones(2, 3), torch.zeros(6)], ... "numpy": numpy.zeros((2,
 3)), ... "other": [42, 4.2, "abc"], ... }, ... max_depth=3, ... ) ... )
 dict'> (length=3) (torch):
```

### Comparing `arctix-0.0.1/pyproject.toml` & `arctix-0.0.2a17/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.1"
-description = "A library to get a text summary of nested objects"
+version = "0.0.2a17"
+description = "A library to compute a string representation of nested objects"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
 keywords = []
 license = "BSD-3-Clause"
 
@@ -23,14 +23,15 @@
 
 packages = [
     { include = "arctix", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
+coola = ">=0.0.13,<1.0"
 python = "^3.9"
 
 # Optional dependencies
 numpy = { version = ">=1.20,<2.0", optional = true }
 torch = { version = ">=1.10,<3.0", optional = true}
 
 [tool.poetry.extras]
```

### Comparing `arctix-0.0.1/src/arctix/_numpy.py` & `arctix-0.0.2a17/src/arctix/formatters/numpy_.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
+__all__ = ["NDArrayFormatter"]
+
 from typing import Any
 from unittest.mock import Mock
 
-from arctix.formatter import BaseFormatter
-from arctix.summarizer import BaseSummarizer, Summarizer
-from arctix.utils.imports import check_numpy, is_numpy_available
+from coola.utils.imports import check_numpy, is_numpy_available
+
+from arctix.formatters.base import BaseFormatter
+from arctix.summarizers.base import BaseSummarizer
 
 if is_numpy_available():
     import numpy
 else:
     numpy = Mock()  # pragma: no cover
 
 
@@ -66,15 +69,15 @@
             bool: ``True`` if the array data are shown,
                 ``False`` if the array metadata are shown.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix._numpy import NDArrayFormatter
+            >>> from arctix.formatters import NDArrayFormatter
             >>> formatter = NDArrayFormatter()
             >>> formatter.get_show_data()
             False
         """
         return self._show_data
 
     def set_show_data(self, show_data: bool) -> None:
@@ -89,23 +92,18 @@
         ------
             TypeError if ``show_data`` is not an boolean.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix._numpy import NDArrayFormatter
+            >>> from arctix.formatters import NDArrayFormatter
             >>> formatter = NDArrayFormatter()
             >>> formatter.set_show_data(True)
             >>> formatter.get_show_data()
             True
         """
         if not isinstance(show_data, bool):
             raise TypeError(
                 "Incorrect type for show_data. Expected bool value but received {show_data}"
             )
         self._show_data = show_data
-
-
-if is_numpy_available():  # pragma: no cover
-    if not Summarizer.has_formatter(numpy.ndarray):
-        Summarizer.add_formatter(numpy.ndarray, NDArrayFormatter())
```

### Comparing `arctix-0.0.1/src/arctix/_torch.py` & `arctix-0.0.2a17/src/arctix/formatters/torch_.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from typing import Any
 from unittest.mock import Mock
 
-from arctix.formatter import BaseFormatter
-from arctix.summarizer import BaseSummarizer, Summarizer
-from arctix.utils.imports import check_torch, is_torch_available
+from coola.utils.imports import check_torch, is_torch_available
+
+from arctix.formatters.base import BaseFormatter
+from arctix.summarizers.base import BaseSummarizer
 
 if is_torch_available():
     import torch
 else:
     torch = Mock()  # pragma: no cover
 
 
@@ -67,15 +68,15 @@
             bool: ``True`` if the tensor data are shown,
                 ``False`` if the tensor metadata are shown.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix._torch import TensorFormatter
+            >>> from arctix.formatters import TensorFormatter
             >>> formatter = TensorFormatter()
             >>> formatter.get_show_data()
             False
         """
         return self._show_data
 
     def set_show_data(self, show_data: bool) -> None:
@@ -90,23 +91,18 @@
         ------
             TypeError if ``show_data`` is not an boolean.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix._torch import TensorFormatter
+            >>> from arctix.formatters import TensorFormatter
             >>> formatter = TensorFormatter()
             >>> formatter.set_show_data(True)
             >>> formatter.get_show_data()
             True
         """
         if not isinstance(show_data, bool):
             raise TypeError(
                 "Incorrect type for show_data. Expected bool value but received {show_data}"
             )
         self._show_data = show_data
-
-
-if is_torch_available():  # pragma: no cover
-    if not Summarizer.has_formatter(torch.Tensor):
-        Summarizer.add_formatter(torch.Tensor, TensorFormatter())
```

### Comparing `arctix-0.0.1/src/arctix/formatter.py` & `arctix-0.0.2a17/src/arctix/formatters/default.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,143 +1,29 @@
 from __future__ import annotations
 
 __all__ = [
-    "BaseFormatter",
     "DefaultFormatter",
     "MappingFormatter",
     "SequenceFormatter",
     "SetFormatter",
 ]
 
-from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
 from itertools import islice
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from typing import TYPE_CHECKING, Any, TypeVar
 
+from arctix.formatters.base import BaseFormatter
 from arctix.utils.format import str_indent, str_mapping, str_sequence
 
 if TYPE_CHECKING:
-    from arctix.summarizer import BaseSummarizer
+    from arctix.summarizers.base import BaseSummarizer
 
 T = TypeVar("T")
 
 
-class BaseFormatter(ABC, Generic[T]):
-    r"""Define the base class to implement a formatter."""
-
-    @abstractmethod
-    def clone(self) -> BaseFormatter:
-        r"""Return a copy of the formatter.
-
-        Returns:
-        -------
-            ``BaseFormatter``: A copy of the formatter.
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix.formatter import DefaultFormatter
-            >>> formatter = DefaultFormatter()
-            >>> formatter2 = formatter.clone()
-            >>> formatter.set_max_characters(10)
-            >>> formatter
-            DefaultFormatter(max_characters=10)
-            >>> formatter2
-            DefaultFormatter(max_characters=-1)
-        """
-
-    @abstractmethod
-    def equal(self, other: Any) -> bool:
-        r"""Indicate if the other object is equal to the self object.
-
-        Args:
-        ----
-            other: Specifies the other object to compare.
-
-        Returns:
-        -------
-            bool: ``True`` if the objects are equal,
-                otherwise ``False``.
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix.formatter import DefaultFormatter
-            >>> formatter = DefaultFormatter()
-            >>> formatter.equal(DefaultFormatter())
-            True
-            >>> formatter.equal(DefaultFormatter(max_characters=10))
-            False
-        """
-
-    @abstractmethod
-    def format(self, summarizer: BaseSummarizer, value: T, depth: int, max_depth: int) -> str:
-        r"""Format a value.
-
-        Args:
-        ----
-            summarizer (``BaseSummarizer``): Specifies the summarizer.
-            value: Specifies the value to summarize.
-
-        Returns:
-        -------
-            str: The formatted value.
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix import Summarizer
-            >>> from arctix.formatter import DefaultFormatter
-            >>> formatter = DefaultFormatter()
-            >>> formatter.format(Summarizer(), 1)
-            <class 'int'> 1
-        """
-
-    @abstractmethod
-    def load_state_dict(self, state_dict: dict) -> None:
-        r"""Load the state values from a dict.
-
-        Args:
-        ----
-            state_dict (dict): a dict with parameters
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix.formatter import DefaultFormatter
-            >>> formatter = DefaultFormatter()
-            >>> # Please take a look to the implementation of the state_dict
-            >>> # function to know the expected structure
-            >>> formatter.load_state_dict({"max_characters": 10})
-            >>> formatter
-            DefaultFormatter(max_characters=10)
-        """
-
-    @abstractmethod
-    def state_dict(self) -> dict:
-        r"""Return a dictionary containing state values.
-
-        Example usage:
-            dict: the state values in a dict.
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix.formatter import DefaultFormatter
-            >>> formatter = DefaultFormatter()
-            >>> formatter.state_dict()
-            {'max_characters': -1}
-        """
-
-
 class DefaultFormatter(BaseFormatter[Any]):
     r"""Implements the default formatter.
 
     Args:
     ----
         max_characters (int, optional): Specifies the maximum number
             of characters to show. If a negative value is provided,
@@ -183,15 +69,15 @@
         -------
             int: The maximum number of characters to show.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix.formatter import DefaultFormatter
+            >>> from arctix.formatters import DefaultFormatter
             >>> formatter = DefaultFormatter()
             >>> formatter.get_max_characters()
             -1
         """
         return self._max_characters
 
     def set_max_characters(self, max_characters: int) -> None:
@@ -206,15 +92,15 @@
         ------
             TypeError if ``max_characters`` is not an integer.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix.formatter import DefaultFormatter
+            >>> from arctix.formatters import DefaultFormatter
             >>> formatter = DefaultFormatter()
             >>> formatter.set_max_characters(10)
             >>> formatter.get_max_characters()
             10
         """
         if not isinstance(max_characters, int):
             raise TypeError(
@@ -269,15 +155,15 @@
         -------
             int: The maximum number of items to show.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix.formatter import MappingFormatter
+            >>> from arctix.formatters import MappingFormatter
             >>> formatter = MappingFormatter()
             >>> formatter.get_max_items()
             5
         """
         return self._max_items
 
     def set_max_items(self, max_items: int) -> None:
@@ -292,15 +178,15 @@
         ------
             TypeError if ``max_items`` is not an integer.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix.formatter import MappingFormatter
+            >>> from arctix.formatters import MappingFormatter
             >>> formatter = MappingFormatter()
             >>> formatter.set_max_items(10)
             >>> formatter.get_max_items()
             10
         """
         if not isinstance(max_items, int):
             raise TypeError(
@@ -315,15 +201,15 @@
         -------
             int: The number of spaces for indentation.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix.formatter import MappingFormatter
+            >>> from arctix.formatters import MappingFormatter
             >>> formatter = MappingFormatter()
             >>> formatter.get_num_spaces()
             2
         """
         return self._num_spaces
 
     def set_num_spaces(self, num_spaces: int) -> None:
@@ -339,15 +225,15 @@
             TypeError if ``num_spaces`` is not an integer.
             TValueError if ``num_spaces`` is not a positive integer.
 
         Example usage:
 
         .. code-block:: pycon
 
-            >>> from arctix.formatter import MappingFormatter
+            >>> from arctix.formatters import MappingFormatter
             >>> formatter = MappingFormatter()
             >>> formatter.set_num_spaces(4)
             >>> formatter.get_num_spaces()
             4
         """
         if not isinstance(num_spaces, int):
             raise TypeError(
```

### Comparing `arctix-0.0.1/src/arctix/summarizer.py` & `arctix-0.0.2a17/src/arctix/summarizers/summarizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,30 @@
 from __future__ import annotations
 
-__all__ = [
-    "BaseSummarizer",
-    "Summarizer",
-    "summarizer_options",
-    "summary",
-]
+__all__ = ["BaseSummarizer", "Summarizer", "summarizer_options"]
 
-
-from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
 from contextlib import contextmanager
 from typing import Any
 
-from arctix.formatter import (
+from coola.utils.imports import is_numpy_available, is_torch_available
+
+from arctix.formatters import (
     BaseFormatter,
     DefaultFormatter,
     MappingFormatter,
+    NDArrayFormatter,
     SequenceFormatter,
     SetFormatter,
+    TensorFormatter,
 )
+from arctix.summarizers.base import BaseSummarizer
 from arctix.utils.format import str_indent, str_mapping
 
 
-def summary(value: Any, max_depth: int = 1, summarizer: BaseSummarizer | None = None) -> str:
-    r"""Summarize the input value in a string.
-
-    Args:
-    ----
-        value: Specifies the value to summarize.
-        max_depth (int, optional): Specifies the maximum depth to
-            summarize if the input is nested. Default: ``1``
-        summarizer (``BaseSummarizer`` or ``None``): Specifies the
-            summarization strategy. If ``None``, the default
-            ``Summarizer`` is used. Default: ``None``
-
-    Returns:
-    -------
-        str: The summary as a string.
-
-    Example usage:
-
-    .. code-block:: pycon
-
-        >>> from arctix import summary
-        >>> print(summary(1))
-        <class 'int'> 1
-        >>> print(summary(["abc", "def"]))
-        <class 'list'> (length=2)
-          (0): abc
-          (1): def
-        >>> print(summary([[0, 1, 2], {"key1": "abc", "key2": "def"}]))
-        <class 'list'> (length=2)
-          (0): [0, 1, 2]
-          (1): {'key1': 'abc', 'key2': 'def'}
-        >>> print(summary([[0, 1, 2], {"key1": "abc", "key2": "def"}], max_depth=2))
-        <class 'list'> (length=2)
-          (0): <class 'list'> (length=3)
-              (0): 0
-              (1): 1
-              (2): 2
-          (1): <class 'dict'> (length=2)
-              (key1): abc
-              (key2): def
-    """
-    summarizer = summarizer or Summarizer()
-    return summarizer.summary(value=value, depth=0, max_depth=max_depth)
-
-
-class BaseSummarizer(ABC):
-    r"""Define the base class to implement a summarizer."""
-
-    @abstractmethod
-    def summary(
-        self,
-        value: Any,
-        depth: int = 0,
-        max_depth: int = 1,
-    ) -> str:
-        r"""Summarize the input value in a string.
-
-        Args:
-        ----
-            value: Specifies the value to summarize.
-            max_depth (int, optional): Specifies the maximum depth to
-                summarize if the input is nested. Default: ``1``
-            summarizer (``BaseSummarizer`` or ``None``): Specifies the
-                summarization strategy. If ``None``, the default
-                ``Summarizer`` is used. Default: ``None``
-
-        Returns:
-        -------
-            str: The summary as a string.
-
-        Example usage:
-
-        .. code-block:: pycon
-
-            >>> from arctix import Summarizer
-            >>> print(Summarizer().summary(1))
-            <class 'int'> 1
-            >>> print(Summarizer().summary(["abc", "def"]))
-            <class 'list'> (length=2)
-              (0): abc
-              (1): def
-            >>> print(Summarizer().summary([[0, 1, 2], {"key1": "abc", "key2": "def"}]))
-            <class 'list'> (length=2)
-              (0): [0, 1, 2]
-              (1): {'key1': 'abc', 'key2': 'def'}
-            >>> print(Summarizer().summary([[0, 1, 2], {"key1": "abc", "key2": "def"}], max_depth=2))
-            <class 'list'> (length=2)
-              (0): <class 'list'> (length=3)
-                  (0): 0
-                  (1): 1
-                  (2): 2
-              (1): <class 'dict'> (length=2)
-                  (key1): abc
-                  (key2): def
-        """
-
-
 class Summarizer(BaseSummarizer):
     """Implement the default summarizer.
 
     The registry is a class variable, so it is shared with all the
     instances of this class.
     """
 
@@ -175,15 +76,15 @@
                 data type and ``exist_ok=False``.
 
         Example usage:
 
         .. code-block:: pycon
 
             >>> from arctix import Summarizer
-            >>> from arctix.formatter import MappingFormatter
+            >>> from arctix.formatters import MappingFormatter
             >>> Summarizer.add_formatter(dict, MappingFormatter(), exist_ok=True)
         """
         if data_type in cls.registry and not exist_ok:
             raise RuntimeError(
                 f"A formatter ({cls.registry[data_type]}) is already registered for the data "
                 f"type {data_type}. Please use `exist_ok=True` if you want to overwrite the "
                 "formatter for this type"
@@ -455,7 +356,20 @@
     """
     state = Summarizer.state_dict()
     set_summarizer_options(**kwargs)
     try:
         yield
     finally:
         Summarizer.load_state_dict(state)
+
+
+if is_numpy_available():  # pragma: no cover
+    import numpy
+
+    if not Summarizer.has_formatter(numpy.ndarray):
+        Summarizer.add_formatter(numpy.ndarray, NDArrayFormatter())
+
+if is_torch_available():  # pragma: no cover
+    import torch
+
+    if not Summarizer.has_formatter(torch.Tensor):
+        Summarizer.add_formatter(torch.Tensor, TensorFormatter())
```

### Comparing `arctix-0.0.1/src/arctix/utils/format.py` & `arctix-0.0.2a17/src/arctix/utils/format.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.1/PKG-INFO` & `arctix-0.0.2a17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: arctix
-Version: 0.0.1
-Summary: A library to get a text summary of nested objects
+Version: 0.0.2a17
+Summary: A library to compute a string representation of nested objects
 Home-page: https://github.com/durandtibo/arctix
 License: BSD-3-Clause
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: all
+Requires-Dist: coola (>=0.0.13,<1.0)
 Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
 Requires-Dist: torch (>=1.10,<3.0) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/arctix
 Description-Content-Type: text/markdown
 
 # arctix
 
@@ -65,16 +66,15 @@
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/arctix/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-`arctix` is a Python library that provides simple functions to check in a single line if two
-complex/nested objects are equal or not.
+`arctix` is a Python library to compute a string representation of complex/nested objects.
 `arctix` was initially designed to work
 with [PyTorch `Tensor`s](https://pytorch.org/docs/stable/tensors.html)
 and [NumPy `ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
 is possible to extend it
 to [support other data structures](https://durandtibo.github.io/arctix/customization).
 
 - [Motivation](#motivation)
```

#### html2text {}

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.1 Summary: A library to get a
-text summary of nested objects Home-page: https://github.com/durandtibo/arctix
-License: BSD-3-Clause Author: Thibaut Durand Author-email:
-durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-BSD License Classifier: Operating System :: POSIX :: Linux Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Provides-Extra: all Requires-Dist: numpy
-(>=1.20,<2.0) ; extra == "all" Requires-Dist: torch (>=1.10,<3.0) ; extra ==
-"all" Project-URL: Repository, https://github.com/durandtibo/arctix
-Description-Content-Type: text/markdown # arctix
+Metadata-Version: 2.1 Name: arctix Version: 0.0.2a17 Summary: A library to
+compute a string representation of nested objects Home-page: https://
+github.com/durandtibo/arctix License: BSD-3-Clause Author: Thibaut Durand
+Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Provides-Extra: all Requires-
+Dist: coola (>=0.0.13,<1.0) Requires-Dist: numpy (>=1.20,<2.0) ; extra == "all"
+Requires-Dist: torch (>=1.10,<3.0) ; extra == "all" Project-URL: Repository,
+https://github.com/durandtibo/arctix Description-Content-Type: text/markdown #
+arctix
           [CI] [CI] [Codecov] [https://api.codeclimate.com/v1/badges/
  61b8574ea18ecf106dce/maintainability] [https://api.codeclimate.com/v1/badges/
                      61b8574ea18ecf106dce/test_coverage]
 [PYPI_version] [Python] [BSD-3-Clause] [Code_style:_black] [Doc_style:_google]
                        [Downloads] [Monthly_downloads]
-## Overview `arctix` is a Python library that provides simple functions to
-check in a single line if two complex/nested objects are equal or not. `arctix`
-was initially designed to work with [PyTorch `Tensor`s](https://pytorch.org/
-docs/stable/tensors.html) and [NumPy `ndarray`](https://numpy.org/doc/stable/
-reference/generated/numpy.ndarray.html), but it is possible to extend it to
-[support other data structures](https://durandtibo.github.io/arctix/
-customization). - [Motivation](#motivation) - [Documentation](https://
-durandtibo.github.io/arctix/) - [Installation](#installation) - [Contributing]
-(#contributing) - [API stability](#api-stability) - [License](#license) ##
-Motivation Let's imagine you have the following dictionaries that contain both
-a PyTorch `Tensor` and a NumPy `ndarray`. You want to compute a string
-representation of it. By default, Python tries to show the values of all the
-tensor/array. The `arctix` library was developed to easily compute structured
-string representation of nested objects. `arctix` provides a function `summary`
-that can indicate if two complex/nested objects are equal or not. ```pycon >>>
-import numpy >>> import torch >>> from arctix import summary >>> print(summary(
-{"torch": torch.ones(2, 3), "numpy": numpy.zeros((2, 3))}))
+## Overview `arctix` is a Python library to compute a string representation of
+complex/nested objects. `arctix` was initially designed to work with [PyTorch
+`Tensor`s](https://pytorch.org/docs/stable/tensors.html) and [NumPy `ndarray`]
+(https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html), but it
+is possible to extend it to [support other data structures](https://
+durandtibo.github.io/arctix/customization). - [Motivation](#motivation) -
+[Documentation](https://durandtibo.github.io/arctix/) - [Installation]
+(#installation) - [Contributing](#contributing) - [API stability](#api-
+stability) - [License](#license) ## Motivation Let's imagine you have the
+following dictionaries that contain both a PyTorch `Tensor` and a NumPy
+`ndarray`. You want to compute a string representation of it. By default,
+Python tries to show the values of all the tensor/array. The `arctix` library
+was developed to easily compute structured string representation of nested
+objects. `arctix` provides a function `summary` that can indicate if two
+complex/nested objects are equal or not. ```pycon >>> import numpy >>> import
+torch >>> from arctix import summary >>> print(summary({"torch": torch.ones(2,
+3), "numpy": numpy.zeros((2, 3))}))
 dict'> (length=2) (torch):
 torch.Tensor'> | shape=torch.Size([2, 3]) | dtype=torch.float32 | device=cpu
 (numpy):
 numpy.ndarray'> | shape=(2, 3) | dtype=float64 >>> print( ... summary( ...
 { ... "torch": [torch.ones(2, 3), torch.zeros(6)], ... "numpy": numpy.zeros((2,
 3)), ... "other": [42, 4.2, "abc"], ... }, ... max_depth=3, ... ) ... )
 dict'> (length=3) (torch):
```

