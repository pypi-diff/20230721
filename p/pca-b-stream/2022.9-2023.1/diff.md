# Comparing `tmp/pca-b-stream-2022.9.tar.gz` & `tmp/pca-b-stream-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-b-stream-2022.9.tar", last modified: Fri Nov 18 14:50:19 2022, max compression
+gzip compressed data, was "pca-b-stream-2023.1.tar", last modified: Fri Jul 21 14:37:48 2023, max compression
```

## Comparing `pca-b-stream-2022.9.tar` & `pca-b-stream-2023.1.tar`

### file list

```diff
@@ -1,45 +1,37 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-11-10 08:42:16.000000 pca-b-stream-2022.9/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)    11743 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2022-11-10 08:44:16.000000 pca-b-stream-2022.9/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pca-b-stream-2022.9/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    10918 2022-11-10 08:40:30.000000 pca-b-stream-2022.9/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.902354 pca-b-stream-2022.9/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1907 2022-11-10 07:55:10.000000 pca-b-stream-2022.9/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/
--rw-r--r--   0 eric      (1000) users      (984)     1680 2022-11-14 15:09:17.000000 pca-b-stream-2022.9/pca_b_stream/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)     4372 2022-11-15 14:08:31.000000 pca-b-stream-2022.9/pca_b_stream/cli.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/flask/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/flask/html/
--rw-r--r--   0 eric      (1000) users      (984)     3078 2022-11-18 13:41:02.000000 pca-b-stream-2022.9/pca_b_stream/flask/html/constants.py
--rw-r--r--   0 eric      (1000) users      (984)     3857 2022-11-17 07:40:28.000000 pca-b-stream-2022.9/pca_b_stream/flask/html/main.html
--rw-r--r--   0 eric      (1000) users      (984)     4156 2022-11-18 14:09:48.000000 pca-b-stream-2022.9/pca_b_stream/flask/html/session.py
--rw-r--r--   0 eric      (1000) users      (984)     2476 2022-11-18 13:41:02.000000 pca-b-stream-2022.9/pca_b_stream/flask/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/flask/session/
--rw-r--r--   0 eric      (1000) users      (984)     1608 2022-11-14 15:45:05.000000 pca-b-stream-2022.9/pca_b_stream/flask/session/constants.py
--rw-r--r--   0 eric      (1000) users      (984)     2039 2022-11-17 08:06:33.000000 pca-b-stream-2022.9/pca_b_stream/flask/session/form.py
--rw-r--r--   0 eric      (1000) users      (984)     3411 2022-11-18 09:27:28.000000 pca-b-stream-2022.9/pca_b_stream/flask/session/processing.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/flask/static/
--rw-r--r--   0 eric      (1000) users      (984)     1964 2022-11-17 07:46:58.000000 pca-b-stream-2022.9/pca_b_stream/flask/static/main.css
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.902354 pca-b-stream-2022.9/pca_b_stream/flask/static/runtime/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/flask/static/runtime/input/
--rw-r--r--   0 eric      (1000) users      (984)       15 2022-10-28 08:01:48.000000 pca-b-stream-2022.9/pca_b_stream/flask/static/runtime/input/not-empty-folder.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/flask/static/runtime/output/
--rw-r--r--   0 eric      (1000) users      (984)       15 2022-10-28 08:01:48.000000 pca-b-stream-2022.9/pca_b_stream/flask/static/runtime/output/not-empty-folder.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/flask/static/runtime/session/
--rw-r--r--   0 eric      (1000) users      (984)       15 2022-10-28 08:01:48.000000 pca-b-stream-2022.9/pca_b_stream/flask/static/runtime/session/not-empty-folder.txt
--rw-r--r--   0 eric      (1000) users      (984)    11795 2022-11-17 12:54:43.000000 pca-b-stream-2022.9/pca_b_stream/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream/test/
--rw-r--r--   0 eric      (1000) users      (984)     5941 2022-11-17 12:24:03.000000 pca-b-stream-2022.9/pca_b_stream/test/test.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2022-11-18 14:49:50.000000 pca-b-stream-2022.9/pca_b_stream/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/pca_b_stream.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)    11743 2022-11-18 14:50:19.000000 pca-b-stream-2022.9/pca_b_stream.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      940 2022-11-18 14:50:19.000000 pca-b-stream-2022.9/pca_b_stream.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2022-11-18 14:50:19.000000 pca-b-stream-2022.9/pca_b_stream.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-11-18 14:50:19.000000 pca-b-stream-2022.9/pca_b_stream.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)      112 2022-11-18 14:50:19.000000 pca-b-stream-2022.9/pca_b_stream.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       13 2022-11-18 14:50:19.000000 pca-b-stream-2022.9/pca_b_stream.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-11-10 08:41:31.000000 pca-b-stream-2022.9/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2022-11-18 14:50:19.905688 pca-b-stream-2022.9/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     6340 2022-11-17 18:33:26.000000 pca-b-stream-2022.9/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2022-11-10 08:42:16.000000 pca-b-stream-2023.1/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)    11632 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2022-11-10 08:44:16.000000 pca-b-stream-2023.1/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pca-b-stream-2023.1/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    10807 2023-07-21 14:36:57.000000 pca-b-stream-2023.1/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1907 2022-11-10 07:55:10.000000 pca-b-stream-2023.1/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/
+-rw-r--r--   0 eric      (1000) users      (984)     1683 2023-07-21 09:16:55.000000 pca-b-stream-2023.1/pca_b_stream/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)     4459 2023-07-21 13:27:36.000000 pca-b-stream-2023.1/pca_b_stream/cli.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/html/
+-rw-r--r--   0 eric      (1000) users      (984)     3077 2023-07-21 09:16:13.000000 pca-b-stream-2023.1/pca_b_stream/flask/html/constants.py
+-rw-r--r--   0 eric      (1000) users      (984)     4144 2023-07-21 14:07:35.000000 pca-b-stream-2023.1/pca_b_stream/flask/html/main.html
+-rw-r--r--   0 eric      (1000) users      (984)     4490 2023-07-21 14:00:56.000000 pca-b-stream-2023.1/pca_b_stream/flask/html/session.py
+-rw-r--r--   0 eric      (1000) users      (984)     2549 2023-07-21 09:16:55.000000 pca-b-stream-2023.1/pca_b_stream/flask/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/session/
+-rw-r--r--   0 eric      (1000) users      (984)     1608 2022-11-14 15:45:05.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/constants.py
+-rw-r--r--   0 eric      (1000) users      (984)     2332 2023-07-21 09:16:13.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/form.py
+-rw-r--r--   0 eric      (1000) users      (984)     3838 2023-07-21 13:27:30.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/processing.py
+-rw-r--r--   0 eric      (1000) users      (984)     2663 2023-07-21 09:16:15.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/session.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/static/
+-rw-r--r--   0 eric      (1000) users      (984)     1964 2022-11-17 07:46:58.000000 pca-b-stream-2023.1/pca_b_stream/flask/static/main.css
+-rw-r--r--   0 eric      (1000) users      (984)    10500 2023-07-21 13:17:58.000000 pca-b-stream-2023.1/pca_b_stream/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-21 13:56:02.000000 pca-b-stream-2023.1/pca_b_stream/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)    11632 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      766 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      112 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       13 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-11-10 08:41:31.000000 pca-b-stream-2023.1/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     6080 2023-07-21 13:56:48.000000 pca-b-stream-2023.1/setup.py
```

### Comparing `pca-b-stream-2022.9/PKG-INFO` & `pca-b-stream-2023.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pca-b-stream
-Version: 2022.9
+Version: 2023.1
 Summary: Byte Stream Representation of Piecewise-constant Array
 Home-page: https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/pca-b-stream/
@@ -63,14 +63,16 @@
 ===================================
 
 
 
 Installation
 ============
 
+A Web app of |PROJECT_NAME| might be available on `PythonAnywhere <https://ericdbv.eu.pythonanywhere.com>`_.
+
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
 Otherwise, it can be installed from a command console:
 
 - For all users, after acquiring administrative rights:
@@ -84,15 +86,15 @@
 
 Brief Description
 =================
 
 In a Few Words
 --------------
 
-The ``PCA-B-Stream`` project allows to generate a printable `byte stream <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_ representation of a piecewise-constant `Numpy array <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_ and to re-create the array from the byte stream, similarly to what is available as part of the `COCO API <https://github.com/cocodataset/cocoapi>`_.
+The ``PCA-B-Stream`` project allows to generate a printable `byte stream <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_ representation of a piecewise-constant `Numpy array <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_, and to re-create the array from the byte stream, similarly to what is available as part of the `COCO API <https://github.com/cocodataset/cocoapi>`_.
 
 
 
 Illustration
 ------------
 
 In Python:
@@ -124,19 +126,19 @@
 .. _sct_motivations:
 
 Motivations
 ===========
 
 The motivations for developing an alternative to existing solutions are:
 
-- Arrays can be of any dimension (i.e., not just 2-dimensional)
-- Their `dtype <https://numpy.org/devdocs/reference/generated/numpy.dtype.html>`_ can be of boolean, integer, or float
-- They can contain more than 2 distinct values (i.e., non-binary arrays) as long as the values are integers (potentially stored in a floating-point format though)
-- The byte stream representation is self-contained; In particular, there is no need to keep track of the array shape externally
-- The byte stream representation contains everything needed to re-create the array *exactly* as it was instantiated (``dtype``, endianness, C or Fortran ordering); See `note <note_on_exact_>`_ though
+- Arrays can be of any dimension (i.e., not just 2-dimensional),
+- Their `dtype <https://numpy.org/devdocs/reference/generated/numpy.dtype.html>`_ can be of boolean, integer, or float types,
+- They can contain more than 2 distinct values (i.e., non-binary arrays) as long as the values are integers (potentially stored in a floating-point format though),
+- The byte stream representation is self-contained; In particular, there is no need to keep track of the array shape externally,
+- The byte stream representation contains everything needed to re-create the array *exactly* as it was instantiated (``dtype``, endianness, C or Fortran ordering); See `note <note_on_exact_>`_ though.
 
 
 .. _note_on_exact:
 
 .. note::
     The statement "re-create the array *exactly* as it was instantiated" is over-confident. First this has not been fully tested by, for example, re-creating an array on a another machine with a native endianness different from the one it was originally instantiated on. Second, more work might be required to ensure that enumeration ordering is correctly dealt with.
 
@@ -147,41 +149,39 @@
 
 Functions
 ---------
 
 The ``pca_b_stream`` module defines the following functions:
 
 - ``PCA2BStream``
-    - Generates the byte stream representation of an array; Does not check the array validity (see ``PCAIsValid``)
+    - Generates the byte stream representation of an array; Does not check the array validity (see ``PCArrayIssues``)
     - Input: a `Numpy ndarray <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_
     - Output: an object of type `bytes <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_
 - ``BStream2PCA``
     - Re-creates the array from its bytes stream representation; Does not check the stream format validity
     - Input/Output: input and output of ``PCA2BStream`` swapped
-- ``PCAIsValid``
+- ``PCArrayIssues``
     - Checks whether an array is a valid input for stream representation generation; It is meant to be used before calling ``PCA2BStream``
     - Input: a `Numpy ndarray <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_
-    - Output: a tuple ``(validity, issue)`` where ``validity`` is a boolean and ``issue`` is None if ``validity`` is True, or a string describing why the array is considered invalid otherwise.
+    - Output: a tuple issues in ``str`` format. The tuple is empty if the array is valid.
     - Additional information about what are valid piecewise-constant arrays here is provided in the section `"Motivations" <sct_motivations_>`_.
 - ``BStreamDetails``
     - Extract details from a byte stream representation; See section `"Byte Stream Format" <byte_stream_format_>`_
     - Inputs:
         - a byte stream generated by ``PCA2BStream``
         - details: a string where each character corresponds to a detail to extract, or "+" to extract all of the available details; Default: "+"; Available details are:
-            - m=maximum value in array (also number of sub-streams)
-            - c=compression indicators (string of zeros and ones, one per sub-stream)
-            - e=endianness
-            - t=dtype type code
-            - T=dtype name
-            - o=enumeration order
-            - v=first value (0 for 0 or False, 1 for non-zero or True)
-            - d=array dimension
-            - l=array lengths per dimension
-        - should_print: a boolean to instruct whether the extracted details should be printed to console; Defaults: True
-        - should_return: a boolean to instruct whether the extracted details should be returned (see Outputs); Defaults: False
+            - c: compression indicator
+            - d: array dimension
+            - l: array lengths per dimension
+            - t: dtype type code; See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.char.html
+            - T: dtype name; Translated from "t" by Numpy.sctypeDict
+            - o: enumeration order; See: https://numpy.org/doc/stable/reference/generated/numpy.ndarray.flags.html, ?_CONTIGUOUS
+            - e: endianness (or byte order); See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.byteorder.html
+        - should_print: a boolean to instruct whether the extracted details should be printed to console; Defaults: False
+        - should_return: a boolean to instruct whether the extracted details should be returned (see Outputs); Defaults: True
     - Output: either one of:
         - None if should_return is False
         - a dictionary of all of the available details if the ``details`` parameter is "+"
         - a tuple of the requested details in the same order as in the ``details`` parameter
 
 
 
@@ -193,30 +193,36 @@
 
 
 .. _byte_stream_format:
 
 Byte Stream Format
 ------------------
 
-A byte stream is a sequence of `base85-encoded (sub-)streams <https://docs.python.org/3/library/base64.html#base64.b85encode>`_ joined with newlines characters b'\n'.
-
-For a boolean array or an array containing only 0's (zeros) and 1's (ones), there is only one such encoded stream. Once decoded, it has the following format (in lexicographical order; all characters are in ``bytes`` format):
+A byte stream is a `base85-encoded <https://docs.python.org/3/library/base64.html#base64.b85encode>`_ stream. Once decoded, it has the following format (in lexicographical order; all characters are in ``bytes`` format):
 
-- 0 or 1: indicates whether the remaining of the stream is in uncompressed or `ZLIB compressed <https://docs.python.org/3/library/zlib.html#zlib.compress>`_ format; See `note on compression <note_on_compression_>`_; The remaining of the description applies to the stream in uncompressed format
+- one character "0" or "1": indicates whether the remaining of the stream is in uncompressed or `ZLIB compressed <https://docs.python.org/3/library/zlib.html#zlib.compress>`_ format; See `note on compression <note_on_compression_>`_; The remaining of the description applies to the stream in uncompressed format
 - 3 characters "{E}{T}{O}":
     - E: endianness among "|", "<" and ">"
     - T: ``dtype`` character code among: "?" + numpy.typecodes["AllInteger"] + numpy.typecodes["Float"]
     - O: enumeration order among "C" (C-ordering) and "F" (Fortran-ordering)
-- 0 or 1: whether the first value in the array is zero (or False) or one (or True)
-- characters resulting from the `unsingned LEB128 encoding <https://en.wikipedia.org/wiki/LEB128#Unsigned_LEB128>`_ of some integers using the `leb128 project <https://github.com/mohanson/leb128>`_; These integers are:
-    - one integer for the dimension of the array (1 for vectors, 2 for matrices, 3 for volumes...)
-    - one integer per dimension giving the length of the array in that dimension
+- one integer for the dimension of the array (1 for vectors, 2 for matrices, 3 for volumes...)
+- one integer per dimension giving the length of the array in that dimension
+
+The remaining of the stream is the actual array content.
+
+- If the array is not all False's or zeros:
+    - one character "0" or "1": whether the first value in the array is zero (or False) or one (or True)
+    - one integer for the length of the run-length representation
     - integers of the `run-length representation <https://en.wikipedia.org/wiki/Run-length_encoding>`_ of the array read in its proper enumeration order
+- If the array is all False's or zeros:
+    - one character "2"
+
+All the integers are encoded by the `unsigned LEB128 encoding <https://en.wikipedia.org/wiki/LEB128#Unsigned_LEB128>`_ using the `leb128 project <https://github.com/mohanson/leb128>`_.
 
-For arrays containing 3 distinct integer values or more (or if the maximum value is higher than 1 regardless of the number of distinct values), there is one encoded stream per value between 1 and the maximum value in the array. The first encoded stream format is identical to the binary case above. The format of the remaining streams is a version of the above format where information already known has been removed: the 3 characters "{E}{T}{O}", the integers of the array dimension, and the length per dimension.
+For non-boolean arrays with a maximum value of 2 or more, the content part is the concatenation of the sub-contents corresponding to each value between 1 and the maximum value in the array.
 
 
 .. _note_on_compression:
 
 .. note::
     For small arrays, compressing the byte stream actually produces a longer stream.
```

### Comparing `pca-b-stream-2022.9/README-COPYRIGHT-utf8.txt` & `pca-b-stream-2023.1/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2022.9/README-LICENCE-utf8.txt` & `pca-b-stream-2023.1/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2022.9/README.rst` & `pca-b-stream-2023.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 ===================================
 
 
 
 Installation
 ============
 
+A Web app of |PROJECT_NAME| might be available on `PythonAnywhere <https://ericdbv.eu.pythonanywhere.com>`_.
+
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
 Otherwise, it can be installed from a command console:
 
 - For all users, after acquiring administrative rights:
@@ -65,15 +67,15 @@
 
 Brief Description
 =================
 
 In a Few Words
 --------------
 
-The ``PCA-B-Stream`` project allows to generate a printable `byte stream <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_ representation of a piecewise-constant `Numpy array <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_ and to re-create the array from the byte stream, similarly to what is available as part of the `COCO API <https://github.com/cocodataset/cocoapi>`_.
+The ``PCA-B-Stream`` project allows to generate a printable `byte stream <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_ representation of a piecewise-constant `Numpy array <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_, and to re-create the array from the byte stream, similarly to what is available as part of the `COCO API <https://github.com/cocodataset/cocoapi>`_.
 
 
 
 Illustration
 ------------
 
 In Python:
@@ -105,19 +107,19 @@
 .. _sct_motivations:
 
 Motivations
 ===========
 
 The motivations for developing an alternative to existing solutions are:
 
-- Arrays can be of any dimension (i.e., not just 2-dimensional)
-- Their `dtype <https://numpy.org/devdocs/reference/generated/numpy.dtype.html>`_ can be of boolean, integer, or float
-- They can contain more than 2 distinct values (i.e., non-binary arrays) as long as the values are integers (potentially stored in a floating-point format though)
-- The byte stream representation is self-contained; In particular, there is no need to keep track of the array shape externally
-- The byte stream representation contains everything needed to re-create the array *exactly* as it was instantiated (``dtype``, endianness, C or Fortran ordering); See `note <note_on_exact_>`_ though
+- Arrays can be of any dimension (i.e., not just 2-dimensional),
+- Their `dtype <https://numpy.org/devdocs/reference/generated/numpy.dtype.html>`_ can be of boolean, integer, or float types,
+- They can contain more than 2 distinct values (i.e., non-binary arrays) as long as the values are integers (potentially stored in a floating-point format though),
+- The byte stream representation is self-contained; In particular, there is no need to keep track of the array shape externally,
+- The byte stream representation contains everything needed to re-create the array *exactly* as it was instantiated (``dtype``, endianness, C or Fortran ordering); See `note <note_on_exact_>`_ though.
 
 
 .. _note_on_exact:
 
 .. note::
     The statement "re-create the array *exactly* as it was instantiated" is over-confident. First this has not been fully tested by, for example, re-creating an array on a another machine with a native endianness different from the one it was originally instantiated on. Second, more work might be required to ensure that enumeration ordering is correctly dealt with.
 
@@ -128,41 +130,39 @@
 
 Functions
 ---------
 
 The ``pca_b_stream`` module defines the following functions:
 
 - ``PCA2BStream``
-    - Generates the byte stream representation of an array; Does not check the array validity (see ``PCAIsValid``)
+    - Generates the byte stream representation of an array; Does not check the array validity (see ``PCArrayIssues``)
     - Input: a `Numpy ndarray <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_
     - Output: an object of type `bytes <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_
 - ``BStream2PCA``
     - Re-creates the array from its bytes stream representation; Does not check the stream format validity
     - Input/Output: input and output of ``PCA2BStream`` swapped
-- ``PCAIsValid``
+- ``PCArrayIssues``
     - Checks whether an array is a valid input for stream representation generation; It is meant to be used before calling ``PCA2BStream``
     - Input: a `Numpy ndarray <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_
-    - Output: a tuple ``(validity, issue)`` where ``validity`` is a boolean and ``issue`` is None if ``validity`` is True, or a string describing why the array is considered invalid otherwise.
+    - Output: a tuple issues in ``str`` format. The tuple is empty if the array is valid.
     - Additional information about what are valid piecewise-constant arrays here is provided in the section `"Motivations" <sct_motivations_>`_.
 - ``BStreamDetails``
     - Extract details from a byte stream representation; See section `"Byte Stream Format" <byte_stream_format_>`_
     - Inputs:
         - a byte stream generated by ``PCA2BStream``
         - details: a string where each character corresponds to a detail to extract, or "+" to extract all of the available details; Default: "+"; Available details are:
-            - m=maximum value in array (also number of sub-streams)
-            - c=compression indicators (string of zeros and ones, one per sub-stream)
-            - e=endianness
-            - t=dtype type code
-            - T=dtype name
-            - o=enumeration order
-            - v=first value (0 for 0 or False, 1 for non-zero or True)
-            - d=array dimension
-            - l=array lengths per dimension
-        - should_print: a boolean to instruct whether the extracted details should be printed to console; Defaults: True
-        - should_return: a boolean to instruct whether the extracted details should be returned (see Outputs); Defaults: False
+            - c: compression indicator
+            - d: array dimension
+            - l: array lengths per dimension
+            - t: dtype type code; See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.char.html
+            - T: dtype name; Translated from "t" by Numpy.sctypeDict
+            - o: enumeration order; See: https://numpy.org/doc/stable/reference/generated/numpy.ndarray.flags.html, ?_CONTIGUOUS
+            - e: endianness (or byte order); See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.byteorder.html
+        - should_print: a boolean to instruct whether the extracted details should be printed to console; Defaults: False
+        - should_return: a boolean to instruct whether the extracted details should be returned (see Outputs); Defaults: True
     - Output: either one of:
         - None if should_return is False
         - a dictionary of all of the available details if the ``details`` parameter is "+"
         - a tuple of the requested details in the same order as in the ``details`` parameter
 
 
 
@@ -174,30 +174,36 @@
 
 
 .. _byte_stream_format:
 
 Byte Stream Format
 ------------------
 
-A byte stream is a sequence of `base85-encoded (sub-)streams <https://docs.python.org/3/library/base64.html#base64.b85encode>`_ joined with newlines characters b'\n'.
-
-For a boolean array or an array containing only 0's (zeros) and 1's (ones), there is only one such encoded stream. Once decoded, it has the following format (in lexicographical order; all characters are in ``bytes`` format):
+A byte stream is a `base85-encoded <https://docs.python.org/3/library/base64.html#base64.b85encode>`_ stream. Once decoded, it has the following format (in lexicographical order; all characters are in ``bytes`` format):
 
-- 0 or 1: indicates whether the remaining of the stream is in uncompressed or `ZLIB compressed <https://docs.python.org/3/library/zlib.html#zlib.compress>`_ format; See `note on compression <note_on_compression_>`_; The remaining of the description applies to the stream in uncompressed format
+- one character "0" or "1": indicates whether the remaining of the stream is in uncompressed or `ZLIB compressed <https://docs.python.org/3/library/zlib.html#zlib.compress>`_ format; See `note on compression <note_on_compression_>`_; The remaining of the description applies to the stream in uncompressed format
 - 3 characters "{E}{T}{O}":
     - E: endianness among "|", "<" and ">"
     - T: ``dtype`` character code among: "?" + numpy.typecodes["AllInteger"] + numpy.typecodes["Float"]
     - O: enumeration order among "C" (C-ordering) and "F" (Fortran-ordering)
-- 0 or 1: whether the first value in the array is zero (or False) or one (or True)
-- characters resulting from the `unsingned LEB128 encoding <https://en.wikipedia.org/wiki/LEB128#Unsigned_LEB128>`_ of some integers using the `leb128 project <https://github.com/mohanson/leb128>`_; These integers are:
-    - one integer for the dimension of the array (1 for vectors, 2 for matrices, 3 for volumes...)
-    - one integer per dimension giving the length of the array in that dimension
+- one integer for the dimension of the array (1 for vectors, 2 for matrices, 3 for volumes...)
+- one integer per dimension giving the length of the array in that dimension
+
+The remaining of the stream is the actual array content.
+
+- If the array is not all False's or zeros:
+    - one character "0" or "1": whether the first value in the array is zero (or False) or one (or True)
+    - one integer for the length of the run-length representation
     - integers of the `run-length representation <https://en.wikipedia.org/wiki/Run-length_encoding>`_ of the array read in its proper enumeration order
+- If the array is all False's or zeros:
+    - one character "2"
+
+All the integers are encoded by the `unsigned LEB128 encoding <https://en.wikipedia.org/wiki/LEB128#Unsigned_LEB128>`_ using the `leb128 project <https://github.com/mohanson/leb128>`_.
 
-For arrays containing 3 distinct integer values or more (or if the maximum value is higher than 1 regardless of the number of distinct values), there is one encoded stream per value between 1 and the maximum value in the array. The first encoded stream format is identical to the binary case above. The format of the remaining streams is a version of the above format where information already known has been removed: the 3 characters "{E}{T}{O}", the integers of the array dimension, and the length per dimension.
+For non-boolean arrays with a maximum value of 2 or more, the content part is the concatenation of the sub-contents corresponding to each value between 1 and the maximum value in the array.
 
 
 .. _note_on_compression:
 
 .. note::
     For small arrays, compressing the byte stream actually produces a longer stream.
```

### Comparing `pca-b-stream-2022.9/documentation/wiki/description.asciidoc` & `pca-b-stream-2023.1/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2022.9/pca_b_stream/__init__.py` & `pca-b-stream-2023.1/pca_b_stream/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from pca_b_stream.main import BStream2PCA, BStreamDetails, PCA2BStream, PCAIsValid
+from pca_b_stream.main import BStream2PCA, BStreamDetails, PCA2BStream, PCArrayIssues
 from pca_b_stream.version import __version__
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/cli.py` & `pca-b-stream-2023.1/pca_b_stream/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,22 +80,24 @@
     path = path_t(sstm.argv[1])
     if not path.is_file():
         print(f"{path}: Specified path is not a(n existing) file")
         sstm.exit(error_code)
     error_code -= 1
 
     try:
-        image = mgio.imread(path)
+        image = mgio.v3.imread(path)
     except Exception as exception:
         print(exception)
         sstm.exit(error_code)
     error_code -= 1
 
-    if not pcas.PCAIsValid(image):
-        print(f"{path}: Not a valid Piecewise-Constant Array")
+    issues = pcas.PCArrayIssues(image)
+    if issues.__len__() > 0:
+        issues = "\n    ".join(issues)
+        print(f"{path}: Not a valid Piecewise-Constant Array:\n    {issues}")
         sstm.exit(error_code)
     error_code -= 1
 
     print(pcas.PCA2BStream(image).decode("ascii"))
 
 
 def BStream2PCA() -> None:
@@ -108,16 +110,16 @@
         )
         sstm.exit(error_code)
     error_code -= 1
 
     stream = sstm.argv[1]
     if ("'" in stream) or ('"' in stream):
         print(
-            f"{stream}: Stream contains \' or \"; "
-            f"Note that the stream must not be passed with the \"b\" string type prefix"
+            f"{stream}: Stream contains ' or \"; "
+            f'Note that the stream must not be passed with the "b" string type prefix'
         )
         sstm.exit(error_code)
     error_code -= 1
 
     stream = bytes(stream, "ascii")
 
     path = path_t(sstm.argv[2])
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/html/constants.py` & `pca-b-stream-2023.1/pca_b_stream/flask/html/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dominate.tags as html
 
 from pca_b_stream.flask.session.constants import PROJECT_NAME
 
-
 NAME_MEANING = "Byte Stream Representation of Piecewise-constant Array"
 SHORT_DESCRIPTION = (
     "Generation of a printable byte stream representation of a piecewise-constant Numpy array, "
     "and re-creation of the array from the byte stream."
 )
 
 ABOUT = html.div(
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/html/main.html` & `pca-b-stream-2023.1/pca_b_stream/flask/html/main.html`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,21 @@
     <h3>Inputs</h3>
 
     <p
         class="container"
         style="color:DarkGoldenRod">
         Note: Uploaded files are limited in size to {{ max_file_size }} MB each.
     </p>
+    <p
+        class="container"
+        style="color:DarkGoldenRod">
+        Byte Stream Example:<br/>
+        F?iamadKul!FYnvXe0x}2|Q8~!vmgRl!P!OhbaA&lt;aWn=-V_-A}Mq^+=X#oDN(G&<br/>
+        (Copy and paste into Byte Stream text area, then convert to piecewise-constant array)
+    </p>
 
     <!-- https://pythonhosted.org/Flask-Bootstrap/forms.html -->
     <form
         role="form"
         method="post"
         action=""
         enctype="multipart/form-data"
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/html/session.py` & `pca-b-stream-2023.1/pca_b_stream/flask/html/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dominate.tags as html
-from si_fi_o.generic import URLOfPath
-from si_fi_o.session.session import session_t
+from si_fi_o.path.html import URLOfPath
 
+from pca_b_stream.flask.session.session import session_t
 
 _LEGEND = {
     "m": "Max. value in array (= number of sub-streams)",
-    "c": "Compression indicator per sub-stream",
+    "c": "Compressed",
     "e": "Endianness (or byte order)",
     "t": "dtype code",
     "T": "dtype name",
     "o": "Enumeration order",
     "v": "First value per sub-stream (0: 0 or False, 1: non-zero or True)",
     "d": "Array dimension",
     "l": "Lengths per dimension",
@@ -55,40 +55,52 @@
 def SessionOutputsAsHTML(session: session_t, /) -> html.html_tag | None:
     """
     Needs to be kept in sync with processing.py since it assigns the outputs
     """
     if (outputs := session.outputs) is None:
         return None
 
-    stream, stream_size, details = outputs  # This is where syncing matters
+    (
+        stream,
+        stream_size,
+        details,
+        high_contrast_name,
+    ) = outputs  # This is where syncing matters
     if stream is None:
         stream = session["stream"]
         path = session.outputs_path
         name = "Decoded Stream"
     else:
-        path = session["array"].path
-        name = session["array"].name
+        path = session["array"].server_path
+        name = session["array"].client_name
+    if high_contrast_name is None:
+        high_contrast_path = path
+    else:
+        high_contrast_path = session.additional_paths[high_contrast_name]
 
     if path is None:
         figure = html.p("Decoding Error: Invalid Byte-Stream Representation")
         array_size = ""
     else:
         figure = html.figure(
-            html.img(src=URLOfPath(path)), html.figcaption(html.i(name))
+            html.img(src=URLOfPath(high_contrast_path)),
+            html.figcaption(
+                html.i(f"{name} (do not download; contrast-enhanced version)")
+            ),
         )
         array_size = path.stat().st_size
 
     output = html.div()
     with output:
         with html.table(style="margin-bottom:1em"):
             with html.tr():
                 html.td(
                     html.div(
                         html.pre(stream),
-                        style="margin-right:2em; height:10em; overflow:auto",
+                        style="margin-right:2em; width:50em; height:10em; overflow:auto",
                     )
                 )
                 html.td(figure)
             with html.tr():
                 html.td(f"Stream length: {stream_size}")
                 html.td(f"Filesize: {array_size}")
         with html.table(border="1px", style="margin-bottom:1em"):
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/main.py` & `pca-b-stream-2023.1/pca_b_stream/flask/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,36 +25,38 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from flask import Flask as flask_app_t
 from si_fi_o.app import ConfigureApp
 
+from flask import Flask as flask_app_t
 from pca_b_stream.flask.html.constants import ABOUT, MAX_IMAGE_SIZE, NAME_MEANING
 from pca_b_stream.flask.html.session import SessionInputsAsHTML, SessionOutputsAsHTML
 from pca_b_stream.flask.session.constants import APP_NAME, PROJECT_NAME
 from pca_b_stream.flask.session.form import form_t
 from pca_b_stream.flask.session.processing import ProcessSession
-
+from pca_b_stream.flask.session.session import session_t
 
 HTML_FOLDER = "html"
 HOME_PAGE_DETAILS = {
     "html_template": "main.html",
     "name": PROJECT_NAME,
     "name_meaning": NAME_MEANING,
     "about": ABOUT,
     "SessionInputsAsHTML": SessionInputsAsHTML,
     "max_file_size": MAX_IMAGE_SIZE,
     "SessionOutputsAsHTML": SessionOutputsAsHTML,
 }
 
 
 app = flask_app_t(__name__, template_folder=HTML_FOLDER)
-ConfigureApp(app, HOME_PAGE_DETAILS, form_t, MAX_IMAGE_SIZE, ProcessSession, APP_NAME)
+ConfigureApp(
+    app, HOME_PAGE_DETAILS, form_t, session_t, MAX_IMAGE_SIZE, ProcessSession, APP_NAME
+)
 
 
 if __name__ == "__main__":
     #
     app.run()
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/session/constants.py` & `pca-b-stream-2023.1/pca_b_stream/flask/session/constants.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/session/form.py` & `pca-b-stream-2023.1/pca_b_stream/flask/session/form.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,19 +28,30 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import wtforms as wtfm
 from si_fi_o.session.form import form_t as base_form_t
 
+from flask import request as flask_request
+
+_TO_BYTE_STREAM = "to byte stream"
+_TO_ARRAY = "to array"
+
 
 class form_t(base_form_t):
     """"""
 
     array = wtfm.FileField(label="Piecewise-constant Array")
     stream = wtfm.TextAreaField(label="Byte Stream", render_kw={"cols": 75, "rows": 3})
     submit_to_str = wtfm.SubmitField(
-        label="Convert to Byte Stream", name="to byte stream"
+        label="Convert to Byte Stream", name=_TO_BYTE_STREAM
     )
     submit_to_ary = wtfm.SubmitField(
-        label="Convert to Piecewise-constant Array", name="to array"
+        label="Convert to Piecewise-constant Array", name=_TO_ARRAY
     )
+
+    @staticmethod
+    def RequestedToByteStream() -> bool:
+        """"""
+        # FIXME: Find a better way to guess targeted conversion
+        return _TO_BYTE_STREAM in flask_request.form
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/session/processing.py` & `pca-b-stream-2023.1/pca_b_stream/flask/session/session.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,76 +25,35 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from pathlib import Path as path_t
-from typing import Any
+from si_fi_o.session.form import file_t
+from si_fi_o.session.session import session_t as base_session_t
 
-import flask as flsk
-import imageio as mgio
-from si_fi_o.session.session import session_t
-
-import pca_b_stream.main as pcas
-
-
-output_types_h = tuple[tuple[str | None, int, Any], path_t | None]
-
-
-def ProcessSession(
-    session: session_t, session_id: str, folder: path_t, /
-) -> output_types_h:
-    """"""
-    # FIXME: Find a better way to guess targeted conversion
-    if "to byte stream" in flsk.request.form:
-        return _ToSTR(session, session_id, folder)
-    else:
-        return _ToARY(session, session_id, folder)
-
-
-def _ToSTR(session: session_t, _: str, __: path_t, /) -> output_types_h:
-    """"""
-    image = mgio.imread(session["array"].path)
-    if pcas.PCAIsValid(image):
-        stream = pcas.PCA2BStream(image)
-        length = stream.__len__()
-        details = pcas.BStreamDetails(
-            stream,
-            should_print=False,
-            should_return=True,
-        )
-        stream = stream.decode("ascii")
-    else:
-        stream = "Invalid Piecewise-constant Array"
-        length = -1
-        details = None
-
-    return (stream, length, details), None
-
-
-def _ToARY(session: session_t, session_id: str, folder: path_t, /) -> output_types_h:
-    """"""
-    stream = bytes(session["stream"], "ascii")
-    stream = b"\n".join(stream.splitlines())  # To convert newlines to \n
-
-    try:
-        decoded = pcas.BStream2PCA(stream)
-    except:
-        decoded = None
-
-    length = stream.__len__()
-    if decoded is None:
-        details = None
-        path = None
-    else:
-        details = pcas.BStreamDetails(
-            stream,
-            should_print=False,
-            should_return=True,
-        )
-        path = folder / f"decoded-{session_id}.png"
-        folder.mkdir(exist_ok=True)
-        mgio.imwrite(path, decoded)
+from pca_b_stream.flask.session.form import form_t
 
-    return (None, length, details), path
+
+class session_t(base_session_t):
+    # additional_paths: list[path_t] | None = None
+    #
+    # def DeleteOutputsFile(self) -> None:
+    #     """"""
+    #     super().DeleteOutputsFile()
+    #
+    #     if self.additional_paths is not None:
+    #         for path in self.additional_paths:
+    #             if path.is_file():
+    #                 path.unlink()
+    #         self.additional_paths = None
+
+    def IsComplete(self, *, form: form_t = None) -> bool:
+        """"""
+        # Do not use self[_key] below since reference and/or detection files are missing if the form has been submitted
+        # without these files (they are not required fields since the session can supply them) and the session has not
+        # received these files yet, e.g. on the first run if not selecting these files.
+        if form_t.RequestedToByteStream():
+            return isinstance(self.get("array"), file_t)
+
+        return self["stream"].__len__() > 0
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/flask/static/main.css` & `pca-b-stream-2023.1/pca_b_stream/flask/static/main.css`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2022.9/pca_b_stream/main.py` & `pca-b-stream-2023.1/pca_b_stream/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,23 +25,21 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import leb128 as lenc
-
-import numpy as nmpy
-
 import base64 as bs64
 import sys as syst
-from typing import Any, Optional, Tuple
 import zlib as cmpr
+from typing import Any, Sequence
 
+import leb128 as lenc
+import numpy as nmpy
 
 array_t = nmpy.ndarray
 
 
 # See also: nmpy.sctypes and nmpy.sctypeDict
 # /!\ Some types have several codes (e.g., "l" = "p" = numpy.int64; see mpy.sctypeDict)
 VALID_NUMPY_TYPES = "?" + nmpy.typecodes["AllInteger"] + nmpy.typecodes["Float"]
@@ -62,241 +60,171 @@
     else:
         enumeration_order = "F"
     storage = byte_order + dtype.char + enumeration_order
 
     # --- Geometry
     geometry = [mask.ndim, *mask.shape]
 
-    # --- Contents
+    # --- Content
     raveled_mask = nmpy.ravel(mask, order="K")
-    n_elements = raveled_mask.size
-    values = range(max(1, int(nmpy.max(raveled_mask))) + 1)
-    streams = []
-    for v_idx, value in enumerate(values[1:]):
-        if values.__len__() > 2:
-            binary_mask = raveled_mask == value
-            first_value_is_one = binary_mask[0]
-        else:
-            # Avoid additional array allocation when already binary
-            binary_mask = raveled_mask
-            first_value = binary_mask[0]
-            first_value_is_one = (first_value == True) or (first_value > 0)
-
-        # --- First value indicator
-        if first_value_is_one:
-            first_value = b"1"
-        else:
-            first_value = b"0"
+    max_value = int(nmpy.amax(raveled_mask))
+    if max_value > 1:
+        content = []
+        for value in range(1, max_value + 1):
+            content.append(_EncodedMask(raveled_mask == value))
+        content = b"".join(content)
+    elif max_value > 0:
+        content = _EncodedMask(raveled_mask.astype(nmpy.bool_, copy=False))
+    else:
+        content = b""
 
-        # --- Run lengths
-        jumps = nmpy.diff(binary_mask)
-        jump_idc = nmpy.nonzero(jumps)[0]
-        if jump_idc.size > 1:
-            run_lengths = (
-                [jump_idc[0] + 1]
-                + nmpy.diff(jump_idc).tolist()
-                + [n_elements - jump_idc[-1] - 1]
-            )
-        elif jump_idc.size > 0:
-            run_lengths = [jump_idc[0] + 1, n_elements - jump_idc[0] - 1]
-        else:
-            run_lengths = [n_elements]
+    # --- Complete stream
+    stream = bytes(storage, "ascii") + _EncodedIntegers(geometry) + content
 
-        # --- Numeric encoding ([geometry + ]run lengths)
-        numeric_encoding = []
-        if v_idx > 0:
-            numbers = run_lengths
-        else:
-            numbers = geometry + run_lengths
-        for number in numbers:
-            numeric_encoding.append(lenc.u.encode(number))
-        numeric_encoding = b"".join(numeric_encoding)
-
-        # --- Compression
-        if v_idx > 0:
-            uncompressed = first_value + numeric_encoding
-        else:
-            uncompressed = bytes(storage, "ascii") + first_value + numeric_encoding
-        compressed = cmpr.compress(uncompressed, cmpr.Z_BEST_COMPRESSION)
-        if compressed.__len__() > uncompressed.__len__():
-            stream = b"0" + uncompressed
-        else:
-            stream = b"1" + compressed
-        streams.append(bs64.b85encode(stream))
+    # --- Compression and encoding
+    compressed = cmpr.compress(stream, cmpr.Z_BEST_COMPRESSION)
+    if compressed.__len__() < stream.__len__():
+        stream = b"1" + compressed
+    else:
+        stream = b"0" + stream
 
-    return b"\n".join(streams)
+    return bs64.b85encode(stream)
 
 
-def BStream2PCA(stream: bytes, /) -> array_t:
+def BStream2PCA(
+    stream: bytes, /, *, just_details: bool = False
+) -> array_t | tuple[bool, int, int, str, Sequence[int]]:
     """"""
     output = None
 
-    dtype_as_str = None
-    enumeration_order = None
-    shape = None
-
-    for s_idx, str_line in enumerate(stream.splitlines()):
-        # --- Decompression
-        decoded = bs64.b85decode(str_line)
-        if chr(decoded[0]) == "0":
-            decompressed = decoded[1:]
-        else:
-            decompressed = cmpr.decompress(decoded[1:])
+    # --- Decoding and decompression
+    decoded = bs64.b85decode(stream)
+    if decoded[0] == ord("0"):  # decoded[0] is an integer. Hence, the "ord".
+        uncompressed = decoded[1:]
+    else:
+        uncompressed = cmpr.decompress(decoded[1:])
 
-        # --- Storage
-        if s_idx > 0:
-            first_value_idx = 0
-        else:
-            *dtype_as_str, enumeration_order = decompressed[:3]
-            dtype_as_str = chr(dtype_as_str[0]) + chr(dtype_as_str[1])
-            if dtype_as_str[0] == "|":
-                dtype_as_str = dtype_as_str[1]
-            enumeration_order = chr(enumeration_order)
-            first_value_idx = 3
-
-        # --- Numbers ([geometry + ]run lengths)
-        numbers = []
-        c_idx = first_value_idx + 1
-        while c_idx < decompressed.__len__():
-            last_idx = c_idx
-            while decompressed[last_idx] & 0b10000000 > 0:
-                last_idx += 1
-            encoded_value = decompressed[c_idx : (last_idx + 1)]
-            decoded_value = lenc.u.decode(encoded_value)
-            numbers.append(decoded_value)
-            c_idx = last_idx + 1
-
-        # --- Geometry
-        if s_idx > 0:
-            run_lengths_idx = 0
-        else:
-            ndim = numbers[0]
-            shape = numbers[1 : (ndim + 1)]
-            run_lengths_idx = ndim + 1
-
-        # --- Contents
-        first_value = int(chr(decompressed[first_value_idx]))
-        run_lengths = numbers[run_lengths_idx:]
-        value_groups = (
-            _lgt * (2 ** ((_idx + first_value) % 2) - 1,)
-            for _idx, _lgt in enumerate(run_lengths)
+    # --- Storage
+    storage_length = 3
+    byte_order, dtype, enumeration_order = uncompressed[:storage_length]
+    if byte_order == ord("|"):
+        dtype_spec = chr(dtype)
+    else:
+        dtype_spec = chr(byte_order) + chr(dtype)
+    enumeration_order = chr(enumeration_order)
+    next_reading_idx = storage_length
+
+    # --- Geometry
+    ndim, next_reading_idx = _DecodedIntegers(
+        uncompressed, next_reading_idx=next_reading_idx, n_integers=1
+    )
+    shape, next_reading_idx = _DecodedIntegers(
+        uncompressed, next_reading_idx=next_reading_idx, n_integers=ndim
+    )
+    if isinstance(shape, int):  # One-dimensional array.
+        shape = (shape,)
+
+    if just_details:
+        return (
+            decoded[0] != ord("0"),
+            byte_order,
+            dtype,
+            enumeration_order,
+            shape,
         )
-        values = tuple(_elm for _grp in value_groups for _elm in _grp)
 
-        # --- Array creation
-        if output is None:
-            output = nmpy.array(values, dtype=dtype_as_str)
-            output = nmpy.reshape(output, shape, order=enumeration_order)
-        else:
-            value = s_idx + 1
-            mask = nmpy.array(values, dtype=dtype_as_str)
-            mask = nmpy.reshape(mask, shape, order=enumeration_order)
-            output[mask > 0] = value
+    if next_reading_idx == uncompressed.__len__():
+        return nmpy.zeros(shape, dtype=dtype_spec, order=enumeration_order)
+
+    value = 1
+    while next_reading_idx < uncompressed.__len__():
+        first_value = int(chr(uncompressed[next_reading_idx]))
+        next_reading_idx += 1
+
+        if first_value < 2:
+            substream_length, next_reading_idx = _DecodedIntegers(
+                uncompressed, next_reading_idx=next_reading_idx, n_integers=1
+            )
+            run_lengths = _DecodedIntegers(
+                uncompressed[next_reading_idx : (next_reading_idx + substream_length)]
+            )
+            value_groups = (
+                _lgt * (_idx % 2,)
+                for _idx, _lgt in enumerate(run_lengths, start=first_value)
+            )
+            values = tuple(_elm for _grp in value_groups for _elm in _grp)
+
+            if output is None:
+                output = nmpy.array(values, dtype=dtype_spec)
+                output = nmpy.reshape(output, shape, order=enumeration_order)
+            else:
+                mask = nmpy.array(values, dtype=nmpy.bool_)
+                mask = nmpy.reshape(mask, shape, order=enumeration_order)
+                output[mask] = value
+        else:
+            substream_length = 0
+            if output is None:
+                output = nmpy.zeros(shape, dtype=dtype_spec, order=enumeration_order)
+
+        next_reading_idx += substream_length
+        value += 1
 
     return output
 
 
 def BStreamDetails(
     stream: bytes,
     /,
     *,
     details: str = "+",
-    should_print: bool = True,
-    should_return: bool = False,
-) -> Optional[Any]:
+    should_print: bool = False,
+    should_return: bool = True,
+) -> dict[str, Any] | tuple[Any, ...] | Any | None:
     """
     Details: if "+", retrieve all details. Otherwise, pick among:
-    m: maximum value in array (also number of sub-streams)
-    c: compression indicator (string of zeros and ones, one per sub-stream)
-    e: endianness (or byte order); See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.byteorder.html
+    c: compression indicator
+    d: array dimension
+    l: array lengths per dimension
     t: dtype type code; See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.char.html
     T: dtype name; Translated from "t" by Numpy.sctypeDict
     o: enumeration order; See: https://numpy.org/doc/stable/reference/generated/numpy.ndarray.flags.html, ?_CONTIGUOUS
-    v: first value (0 for 0 or False, 1 for non-zero or True, one per sub-stream)
-    d: array dimension
-    l: array lengths per dimension
+    e: endianness (or byte order); See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.byteorder.html
     """
     if not (should_print or should_return):
         return None
 
     if details == "+":
         output = {}
     else:
         output = {_key: None for _key in details}
 
-    sub_streams = stream.splitlines()
-    if ("m" in details) or (details == "+"):
-        output["m"] = sub_streams.__len__()
-
-    for s_idx, str_line in enumerate(sub_streams):
-        # --- Decompression
-        decoded = bs64.b85decode(str_line)
-        compression_indicator = chr(decoded[0])
-        if ("c" in details) or (details == "+"):
-            if ("c" in output) and (output["c"] is not None):
-                output["c"] = output["c"] + compression_indicator
-            else:
-                output["c"] = compression_indicator
-        if compression_indicator == "0":
-            decompressed = decoded[1:]
-        else:
-            decompressed = cmpr.decompress(decoded[1:])
-
-        # --- Storage
-        if s_idx > 0:
-            first_value_idx = 0
-        else:
-            *dtype_as_str, enumeration_order = decompressed[:3]
-            dtype_as_str = chr(dtype_as_str[0]) + chr(dtype_as_str[1])
-            if ("e" in details) or (details == "+"):
-                output["e"] = dtype_as_str[0]
-            if ("t" in details) or (details == "+"):
-                output["t"] = dtype_as_str[1]
-            if ("T" in details) or (details == "+"):
-                output["T"] = nmpy.sctypeDict[dtype_as_str[1]].__name__
-            enumeration_order = chr(enumeration_order)
-            if ("o" in details) or (details == "+"):
-                output["o"] = enumeration_order
-            first_value_idx = 3
-
-        # --- Contents
-        if ("v" in details) or (details == "+"):
-            first_value = chr(decompressed[first_value_idx])
-            if ("v" in output) and (output["v"] is not None):
-                output["v"] = output["v"] + first_value
-            else:
-                output["v"] = first_value
-
-        if (s_idx > 0) or (
-            ("d" not in details) and ("l" not in details) and (details != "+")
-        ):
-            continue
-
-        # --- Numbers ([geometry + ]run lengths)
-        numbers = []
-        c_idx = first_value_idx + 1
-        expected_n_numbers = 1  # In fact, at least one
-        while (c_idx < decompressed.__len__()) and (
-            numbers.__len__() < expected_n_numbers
-        ):
-            last_idx = c_idx
-            while decompressed[last_idx] & 0b10000000 > 0:
-                last_idx += 1
-            encoded_value = decompressed[c_idx : (last_idx + 1)]
-            decoded_value = lenc.u.decode(encoded_value)
-            if (numbers.__len__() == 0) and (("l" in details) or (details == "+")):
-                expected_n_numbers = decoded_value + 1
-            numbers.append(decoded_value)
-            c_idx = last_idx + 1
-
-        # --- Geometry
-        if ("d" in details) or (details == "+"):
-            output["d"] = numbers[0]
-        if ("l" in details) or (details == "+"):
-            output["l"] = tuple(numbers[1 : (numbers[0] + 1)])
+    (
+        is_compressed,
+        byte_order,
+        dtype,
+        enumeration_order,
+        shape,
+    ) = BStream2PCA(stream, just_details=True)
+
+    if ("c" in details) or (details == "+"):
+        output["c"] = is_compressed
+
+    if ("d" in details) or (details == "+"):
+        output["d"] = shape.__len__()
+    if ("l" in details) or (details == "+"):
+        output["l"] = tuple(shape)
+
+    if ("t" in details) or (details == "+"):
+        output["t"] = chr(dtype)
+    if ("T" in details) or (details == "+"):
+        output["T"] = nmpy.sctypeDict[chr(dtype)].__name__
+    if ("o" in details) or (details == "+"):
+        output["o"] = enumeration_order
+    if ("e" in details) or (details == "+"):
+        output["e"] = chr(byte_order)
 
     if should_print:
         for key, value in output.items():
             print(f"{key} = {value}")
 
     if should_return:
         if details == "+":
@@ -309,25 +237,90 @@
                 return output[0]
             else:
                 return output  # Empty tuple
 
     return None
 
 
-def PCAIsValid(mask: array_t, /) -> Tuple[bool, Optional[str]]:
+def PCArrayIssues(mask: array_t, /) -> Sequence[str]:
     """"""
-    issue = None
+    output = []
 
-    if issue is None:
-        if mask.dtype.char not in VALID_NUMPY_TYPES:
-            issue = f"{mask.dtype.name}: Invalid type with code {mask.dtype.char}; Expected codes={VALID_NUMPY_TYPES}"
-
-    if issue is None:
-        unique_values = tuple(nmpy.unique(mask))
-        if (unique_values != (False, True)) and (
-            not set(unique_values).issubset(range(int(unique_values[-1]) + 1))
-        ):
-            issue = (
-                "Mask is neither a boolean mask nor a numeric mask with integer values"
+    if mask.dtype.char not in VALID_NUMPY_TYPES:
+        output.append(
+            f"{mask.dtype.name}: Invalid type with code {mask.dtype.char}; "
+            f"Expected={VALID_NUMPY_TYPES}."
+        )
+
+    unique_values = tuple(nmpy.unique(mask))
+    if (unique_values != (False, True)) and (
+        not set(unique_values).issubset(range(int(unique_values[-1]) + 1))
+    ):
+        output.append(
+            "Mask is neither a boolean mask nor a numeric mask with integer values."
+        )
+
+    return output
+
+
+def _EncodedMask(mask: array_t, /) -> bytes:
+    """
+    mask: boolean array
+    """
+    if any(mask):
+        # --- Run lengths
+        n_elements = mask.size
+        jumps = nmpy.diff(mask)
+        jump_idc = nmpy.nonzero(jumps)[0]
+        if jump_idc.size > 1:
+            run_lengths = (
+                [jump_idc[0] + 1]
+                + nmpy.diff(jump_idc).tolist()
+                + [n_elements - jump_idc[-1] - 1]
             )
+        elif jump_idc.size > 0:
+            run_lengths = (jump_idc[0] + 1, n_elements - jump_idc[0] - 1)
+        else:
+            run_lengths = (n_elements,)
+        encoded = _EncodedIntegers(run_lengths)
+
+        # --- First value indicator
+        if mask[0]:  # First value is "True"
+            first_value = b"1"
+        else:
+            first_value = b"0"
+
+        return first_value + lenc.u.encode(encoded.__len__()) + encoded
+    else:
+        return b"2"  # Fake first value.
+
+
+def _EncodedIntegers(integers: Sequence[int], /) -> bytes:
+    """"""
+    return b"".join(map(lenc.u.encode, integers))
+
+
+def _DecodedIntegers(
+    encoded: bytes, /, *, next_reading_idx: int = 0, n_integers: int = None
+) -> Sequence[int] | tuple[int | Sequence[int], int]:
+    """"""
+    integers = []
+
+    while next_reading_idx < encoded.__len__():
+        until_idx = next_reading_idx
+        # TODO: Document the loop below.
+        while encoded[until_idx] & 0b10000000 > 0:
+            until_idx += 1
+        past_until = until_idx + 1
+
+        piece = encoded[next_reading_idx:past_until]
+        integers.append(lenc.u.decode(piece))
+
+        next_reading_idx = past_until
+
+        if integers.__len__() == n_integers:
+            if n_integers > 1:
+                return integers, next_reading_idx
+            else:
+                return integers[0], next_reading_idx
 
-    return issue is None, issue
+    return integers
```

### Comparing `pca-b-stream-2022.9/pca_b_stream/version.py` & `pca-b-stream-2023.1/pca_b_stream/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2022.9"
+__version__ = "2023.1"
```

### Comparing `pca-b-stream-2022.9/pca_b_stream.egg-info/PKG-INFO` & `pca-b-stream-2023.1/pca_b_stream.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pca-b-stream
-Version: 2022.9
+Version: 2023.1
 Summary: Byte Stream Representation of Piecewise-constant Array
 Home-page: https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/pca-b-stream/
@@ -63,14 +63,16 @@
 ===================================
 
 
 
 Installation
 ============
 
+A Web app of |PROJECT_NAME| might be available on `PythonAnywhere <https://ericdbv.eu.pythonanywhere.com>`_.
+
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
 Otherwise, it can be installed from a command console:
 
 - For all users, after acquiring administrative rights:
@@ -84,15 +86,15 @@
 
 Brief Description
 =================
 
 In a Few Words
 --------------
 
-The ``PCA-B-Stream`` project allows to generate a printable `byte stream <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_ representation of a piecewise-constant `Numpy array <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_ and to re-create the array from the byte stream, similarly to what is available as part of the `COCO API <https://github.com/cocodataset/cocoapi>`_.
+The ``PCA-B-Stream`` project allows to generate a printable `byte stream <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_ representation of a piecewise-constant `Numpy array <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_, and to re-create the array from the byte stream, similarly to what is available as part of the `COCO API <https://github.com/cocodataset/cocoapi>`_.
 
 
 
 Illustration
 ------------
 
 In Python:
@@ -124,19 +126,19 @@
 .. _sct_motivations:
 
 Motivations
 ===========
 
 The motivations for developing an alternative to existing solutions are:
 
-- Arrays can be of any dimension (i.e., not just 2-dimensional)
-- Their `dtype <https://numpy.org/devdocs/reference/generated/numpy.dtype.html>`_ can be of boolean, integer, or float
-- They can contain more than 2 distinct values (i.e., non-binary arrays) as long as the values are integers (potentially stored in a floating-point format though)
-- The byte stream representation is self-contained; In particular, there is no need to keep track of the array shape externally
-- The byte stream representation contains everything needed to re-create the array *exactly* as it was instantiated (``dtype``, endianness, C or Fortran ordering); See `note <note_on_exact_>`_ though
+- Arrays can be of any dimension (i.e., not just 2-dimensional),
+- Their `dtype <https://numpy.org/devdocs/reference/generated/numpy.dtype.html>`_ can be of boolean, integer, or float types,
+- They can contain more than 2 distinct values (i.e., non-binary arrays) as long as the values are integers (potentially stored in a floating-point format though),
+- The byte stream representation is self-contained; In particular, there is no need to keep track of the array shape externally,
+- The byte stream representation contains everything needed to re-create the array *exactly* as it was instantiated (``dtype``, endianness, C or Fortran ordering); See `note <note_on_exact_>`_ though.
 
 
 .. _note_on_exact:
 
 .. note::
     The statement "re-create the array *exactly* as it was instantiated" is over-confident. First this has not been fully tested by, for example, re-creating an array on a another machine with a native endianness different from the one it was originally instantiated on. Second, more work might be required to ensure that enumeration ordering is correctly dealt with.
 
@@ -147,41 +149,39 @@
 
 Functions
 ---------
 
 The ``pca_b_stream`` module defines the following functions:
 
 - ``PCA2BStream``
-    - Generates the byte stream representation of an array; Does not check the array validity (see ``PCAIsValid``)
+    - Generates the byte stream representation of an array; Does not check the array validity (see ``PCArrayIssues``)
     - Input: a `Numpy ndarray <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_
     - Output: an object of type `bytes <https://docs.python.org/3/library/stdtypes.html#bytes-objects>`_
 - ``BStream2PCA``
     - Re-creates the array from its bytes stream representation; Does not check the stream format validity
     - Input/Output: input and output of ``PCA2BStream`` swapped
-- ``PCAIsValid``
+- ``PCArrayIssues``
     - Checks whether an array is a valid input for stream representation generation; It is meant to be used before calling ``PCA2BStream``
     - Input: a `Numpy ndarray <https://numpy.org/devdocs/reference/generated/numpy.ndarray.html>`_
-    - Output: a tuple ``(validity, issue)`` where ``validity`` is a boolean and ``issue`` is None if ``validity`` is True, or a string describing why the array is considered invalid otherwise.
+    - Output: a tuple issues in ``str`` format. The tuple is empty if the array is valid.
     - Additional information about what are valid piecewise-constant arrays here is provided in the section `"Motivations" <sct_motivations_>`_.
 - ``BStreamDetails``
     - Extract details from a byte stream representation; See section `"Byte Stream Format" <byte_stream_format_>`_
     - Inputs:
         - a byte stream generated by ``PCA2BStream``
         - details: a string where each character corresponds to a detail to extract, or "+" to extract all of the available details; Default: "+"; Available details are:
-            - m=maximum value in array (also number of sub-streams)
-            - c=compression indicators (string of zeros and ones, one per sub-stream)
-            - e=endianness
-            - t=dtype type code
-            - T=dtype name
-            - o=enumeration order
-            - v=first value (0 for 0 or False, 1 for non-zero or True)
-            - d=array dimension
-            - l=array lengths per dimension
-        - should_print: a boolean to instruct whether the extracted details should be printed to console; Defaults: True
-        - should_return: a boolean to instruct whether the extracted details should be returned (see Outputs); Defaults: False
+            - c: compression indicator
+            - d: array dimension
+            - l: array lengths per dimension
+            - t: dtype type code; See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.char.html
+            - T: dtype name; Translated from "t" by Numpy.sctypeDict
+            - o: enumeration order; See: https://numpy.org/doc/stable/reference/generated/numpy.ndarray.flags.html, ?_CONTIGUOUS
+            - e: endianness (or byte order); See: https://numpy.org/doc/stable/reference/generated/numpy.dtype.byteorder.html
+        - should_print: a boolean to instruct whether the extracted details should be printed to console; Defaults: False
+        - should_return: a boolean to instruct whether the extracted details should be returned (see Outputs); Defaults: True
     - Output: either one of:
         - None if should_return is False
         - a dictionary of all of the available details if the ``details`` parameter is "+"
         - a tuple of the requested details in the same order as in the ``details`` parameter
 
 
 
@@ -193,30 +193,36 @@
 
 
 .. _byte_stream_format:
 
 Byte Stream Format
 ------------------
 
-A byte stream is a sequence of `base85-encoded (sub-)streams <https://docs.python.org/3/library/base64.html#base64.b85encode>`_ joined with newlines characters b'\n'.
-
-For a boolean array or an array containing only 0's (zeros) and 1's (ones), there is only one such encoded stream. Once decoded, it has the following format (in lexicographical order; all characters are in ``bytes`` format):
+A byte stream is a `base85-encoded <https://docs.python.org/3/library/base64.html#base64.b85encode>`_ stream. Once decoded, it has the following format (in lexicographical order; all characters are in ``bytes`` format):
 
-- 0 or 1: indicates whether the remaining of the stream is in uncompressed or `ZLIB compressed <https://docs.python.org/3/library/zlib.html#zlib.compress>`_ format; See `note on compression <note_on_compression_>`_; The remaining of the description applies to the stream in uncompressed format
+- one character "0" or "1": indicates whether the remaining of the stream is in uncompressed or `ZLIB compressed <https://docs.python.org/3/library/zlib.html#zlib.compress>`_ format; See `note on compression <note_on_compression_>`_; The remaining of the description applies to the stream in uncompressed format
 - 3 characters "{E}{T}{O}":
     - E: endianness among "|", "<" and ">"
     - T: ``dtype`` character code among: "?" + numpy.typecodes["AllInteger"] + numpy.typecodes["Float"]
     - O: enumeration order among "C" (C-ordering) and "F" (Fortran-ordering)
-- 0 or 1: whether the first value in the array is zero (or False) or one (or True)
-- characters resulting from the `unsingned LEB128 encoding <https://en.wikipedia.org/wiki/LEB128#Unsigned_LEB128>`_ of some integers using the `leb128 project <https://github.com/mohanson/leb128>`_; These integers are:
-    - one integer for the dimension of the array (1 for vectors, 2 for matrices, 3 for volumes...)
-    - one integer per dimension giving the length of the array in that dimension
+- one integer for the dimension of the array (1 for vectors, 2 for matrices, 3 for volumes...)
+- one integer per dimension giving the length of the array in that dimension
+
+The remaining of the stream is the actual array content.
+
+- If the array is not all False's or zeros:
+    - one character "0" or "1": whether the first value in the array is zero (or False) or one (or True)
+    - one integer for the length of the run-length representation
     - integers of the `run-length representation <https://en.wikipedia.org/wiki/Run-length_encoding>`_ of the array read in its proper enumeration order
+- If the array is all False's or zeros:
+    - one character "2"
+
+All the integers are encoded by the `unsigned LEB128 encoding <https://en.wikipedia.org/wiki/LEB128#Unsigned_LEB128>`_ using the `leb128 project <https://github.com/mohanson/leb128>`_.
 
-For arrays containing 3 distinct integer values or more (or if the maximum value is higher than 1 regardless of the number of distinct values), there is one encoded stream per value between 1 and the maximum value in the array. The first encoded stream format is identical to the binary case above. The format of the remaining streams is a version of the above format where information already known has been removed: the 3 characters "{E}{T}{O}", the integers of the array dimension, and the length per dimension.
+For non-boolean arrays with a maximum value of 2 or more, the content part is the concatenation of the sub-contents corresponding to each value between 1 and the maximum value in the array.
 
 
 .. _note_on_compression:
 
 .. note::
     For small arrays, compressing the byte stream actually produces a longer stream.
```

### Comparing `pca-b-stream-2022.9/pca_b_stream.egg-info/SOURCES.txt` & `pca-b-stream-2023.1/pca_b_stream.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,12 +18,9 @@
 pca_b_stream/flask/main.py
 pca_b_stream/flask/html/constants.py
 pca_b_stream/flask/html/main.html
 pca_b_stream/flask/html/session.py
 pca_b_stream/flask/session/constants.py
 pca_b_stream/flask/session/form.py
 pca_b_stream/flask/session/processing.py
-pca_b_stream/flask/static/main.css
-pca_b_stream/flask/static/runtime/input/not-empty-folder.txt
-pca_b_stream/flask/static/runtime/output/not-empty-folder.txt
-pca_b_stream/flask/static/runtime/session/not-empty-folder.txt
-pca_b_stream/test/test.py
+pca_b_stream/flask/session/session.py
+pca_b_stream/flask/static/main.css
```

### Comparing `pca-b-stream-2022.9/setup.py` & `pca-b-stream-2023.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,24 +27,23 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import re as rgex
 from pathlib import Path as path_t
-from typing import Dict
 
 from setuptools import setup
 
 
 HERE = path_t(__file__).parent.resolve()
 DOCUMENTATION_HOME = HERE / "documentation" / "wiki" / "description.asciidoc"
 
 
-def DescriptionFromDocumentation(documentation: path_t, /) -> Dict[str, str]:
+def DescriptionFromDocumentation(documentation: path_t, /) -> dict[str, str]:
     """"""
     output = {}
 
     pattern = rgex.compile(r":([A-Z_]+): +(.+)\n?", flags=rgex.ASCII)
 
     with open(documentation) as accessor:
         for line in accessor.readlines():
@@ -72,15 +71,14 @@
 
 IMPORT_NAME = "pca_b_stream"
 PACKAGES = [
     IMPORT_NAME,
     f"{IMPORT_NAME}.flask",
     f"{IMPORT_NAME}.flask.html",
     f"{IMPORT_NAME}.flask.session",
-    f"{IMPORT_NAME}.test",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
     f"{IMPORT_NAME}.flask.static",
     f"{IMPORT_NAME}.resource",
 )
 ENTRY_POINTS = {
@@ -94,26 +92,26 @@
 long_description = (HERE / "README.rst").read_text(encoding="utf-8")
 repository_url = (
     f"https://"
     f"{DESCRIPTION['REPOSITORY_SITE']}/"
     f"{DESCRIPTION['REPOSITORY_USER']}/"
     f"{DESCRIPTION['REPOSITORY_NAME']}/"
 )
-#f"{DESCRIPTION['REPOSITORY_USER']}.gitlabpages.inria.fr"
-#f"{repository_url}/{DOCUMENTATION_SITE}"
+# f"{DESCRIPTION['REPOSITORY_USER']}.gitlabpages.inria.fr"
+# f"{repository_url}/{DOCUMENTATION_SITE}"
 documentation_url = repository_url
 
 
 def CheckCoherenceBetweenDeclarationAndReality() -> None:
     """"""
     folders = [IMPORT_NAME]
     for node in (HERE / IMPORT_NAME).rglob("*"):
         if node.is_dir() and not str(node).startswith("."):
             node = node.relative_to(HERE)
-            node = str(node).replace("/", ".")
+            node = ".".join(node.parts)
             if not (
                 (node in EXCLUDED_FOLDERS)
                 or any(node.startswith(_fld + ".") for _fld in EXCLUDED_FOLDERS)
             ):
                 folders.append(node)
     folders = sorted(folders)
 
@@ -170,17 +168,14 @@
         },
         #
         packages=PACKAGES,
         package_data = {
             IMPORT_NAME: [
                 "flask/html/main.html",
                 "flask/static/main.css",
-                "flask/static/runtime/input/not-empty-folder.txt",
-                "flask/static/runtime/output/not-empty-folder.txt",
-                "flask/static/runtime/session/not-empty-folder.txt",
             ],
         },
         entry_points=ENTRY_POINTS,
         python_requires=f">={PY_VERSION}",
         install_requires=[
             "dominate",
             "flask",
```

