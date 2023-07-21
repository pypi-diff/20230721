# Comparing `tmp/pca-b-stream-2023.1.tar.gz` & `tmp/pca-b-stream-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-b-stream-2023.1.tar", last modified: Fri Jul 21 14:37:48 2023, max compression
+gzip compressed data, was "pca-b-stream-2023.2.tar", last modified: Fri Jul 21 14:51:41 2023, max compression
```

## Comparing `pca-b-stream-2023.1.tar` & `pca-b-stream-2023.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-11-10 08:42:16.000000 pca-b-stream-2023.1/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)    11632 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2022-11-10 08:44:16.000000 pca-b-stream-2023.1/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pca-b-stream-2023.1/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    10807 2023-07-21 14:36:57.000000 pca-b-stream-2023.1/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1907 2022-11-10 07:55:10.000000 pca-b-stream-2023.1/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/
--rw-r--r--   0 eric      (1000) users      (984)     1683 2023-07-21 09:16:55.000000 pca-b-stream-2023.1/pca_b_stream/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)     4459 2023-07-21 13:27:36.000000 pca-b-stream-2023.1/pca_b_stream/cli.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/html/
--rw-r--r--   0 eric      (1000) users      (984)     3077 2023-07-21 09:16:13.000000 pca-b-stream-2023.1/pca_b_stream/flask/html/constants.py
--rw-r--r--   0 eric      (1000) users      (984)     4144 2023-07-21 14:07:35.000000 pca-b-stream-2023.1/pca_b_stream/flask/html/main.html
--rw-r--r--   0 eric      (1000) users      (984)     4490 2023-07-21 14:00:56.000000 pca-b-stream-2023.1/pca_b_stream/flask/html/session.py
--rw-r--r--   0 eric      (1000) users      (984)     2549 2023-07-21 09:16:55.000000 pca-b-stream-2023.1/pca_b_stream/flask/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/session/
--rw-r--r--   0 eric      (1000) users      (984)     1608 2022-11-14 15:45:05.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/constants.py
--rw-r--r--   0 eric      (1000) users      (984)     2332 2023-07-21 09:16:13.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/form.py
--rw-r--r--   0 eric      (1000) users      (984)     3838 2023-07-21 13:27:30.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/processing.py
--rw-r--r--   0 eric      (1000) users      (984)     2663 2023-07-21 09:16:15.000000 pca-b-stream-2023.1/pca_b_stream/flask/session/session.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream/flask/static/
--rw-r--r--   0 eric      (1000) users      (984)     1964 2022-11-17 07:46:58.000000 pca-b-stream-2023.1/pca_b_stream/flask/static/main.css
--rw-r--r--   0 eric      (1000) users      (984)    10500 2023-07-21 13:17:58.000000 pca-b-stream-2023.1/pca_b_stream/main.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-21 13:56:02.000000 pca-b-stream-2023.1/pca_b_stream/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/pca_b_stream.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)    11632 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      766 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)      112 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       13 2023-07-21 14:37:48.000000 pca-b-stream-2023.1/pca_b_stream.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-11-10 08:41:31.000000 pca-b-stream-2023.1/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-21 14:37:48.410191 pca-b-stream-2023.1/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     6080 2023-07-21 13:56:48.000000 pca-b-stream-2023.1/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.440188 pca-b-stream-2023.2/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2022-11-10 08:42:16.000000 pca-b-stream-2023.2/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)    11632 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2022-11-10 08:44:16.000000 pca-b-stream-2023.2/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pca-b-stream-2023.2/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    10807 2023-07-21 14:36:57.000000 pca-b-stream-2023.2/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1907 2022-11-10 07:55:10.000000 pca-b-stream-2023.2/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/pca_b_stream/
+-rw-r--r--   0 eric      (1000) users      (984)     1683 2023-07-21 09:16:55.000000 pca-b-stream-2023.2/pca_b_stream/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)     4466 2023-07-21 14:49:20.000000 pca-b-stream-2023.2/pca_b_stream/cli.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/pca_b_stream/flask/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/pca_b_stream/flask/html/
+-rw-r--r--   0 eric      (1000) users      (984)     3077 2023-07-21 09:16:13.000000 pca-b-stream-2023.2/pca_b_stream/flask/html/constants.py
+-rw-r--r--   0 eric      (1000) users      (984)     4144 2023-07-21 14:07:35.000000 pca-b-stream-2023.2/pca_b_stream/flask/html/main.html
+-rw-r--r--   0 eric      (1000) users      (984)     4490 2023-07-21 14:00:56.000000 pca-b-stream-2023.2/pca_b_stream/flask/html/session.py
+-rw-r--r--   0 eric      (1000) users      (984)     2549 2023-07-21 09:16:55.000000 pca-b-stream-2023.2/pca_b_stream/flask/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/pca_b_stream/flask/session/
+-rw-r--r--   0 eric      (1000) users      (984)     1608 2022-11-14 15:45:05.000000 pca-b-stream-2023.2/pca_b_stream/flask/session/constants.py
+-rw-r--r--   0 eric      (1000) users      (984)     2332 2023-07-21 09:16:13.000000 pca-b-stream-2023.2/pca_b_stream/flask/session/form.py
+-rw-r--r--   0 eric      (1000) users      (984)     3838 2023-07-21 13:27:30.000000 pca-b-stream-2023.2/pca_b_stream/flask/session/processing.py
+-rw-r--r--   0 eric      (1000) users      (984)     2663 2023-07-21 09:16:15.000000 pca-b-stream-2023.2/pca_b_stream/flask/session/session.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/pca_b_stream/flask/static/
+-rw-r--r--   0 eric      (1000) users      (984)     1964 2022-11-17 07:46:58.000000 pca-b-stream-2023.2/pca_b_stream/flask/static/main.css
+-rw-r--r--   0 eric      (1000) users      (984)    10500 2023-07-21 13:17:58.000000 pca-b-stream-2023.2/pca_b_stream/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-21 14:49:45.000000 pca-b-stream-2023.2/pca_b_stream/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-21 14:51:41.436854 pca-b-stream-2023.2/pca_b_stream.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)    11632 2023-07-21 14:51:41.000000 pca-b-stream-2023.2/pca_b_stream.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      766 2023-07-21 14:51:41.000000 pca-b-stream-2023.2/pca_b_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-21 14:51:41.000000 pca-b-stream-2023.2/pca_b_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2023-07-21 14:51:41.000000 pca-b-stream-2023.2/pca_b_stream.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      112 2023-07-21 14:51:41.000000 pca-b-stream-2023.2/pca_b_stream.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       13 2023-07-21 14:51:41.000000 pca-b-stream-2023.2/pca_b_stream.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-11-10 08:41:31.000000 pca-b-stream-2023.2/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-21 14:51:41.440188 pca-b-stream-2023.2/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     6080 2023-07-21 13:56:48.000000 pca-b-stream-2023.2/setup.py
```

### Comparing `pca-b-stream-2023.1/PKG-INFO` & `pca-b-stream-2023.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pca-b-stream
-Version: 2023.1
+Version: 2023.2
 Summary: Byte Stream Representation of Piecewise-constant Array
 Home-page: https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/pca-b-stream/
```

### Comparing `pca-b-stream-2023.1/README-COPYRIGHT-utf8.txt` & `pca-b-stream-2023.2/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/README-LICENCE-utf8.txt` & `pca-b-stream-2023.2/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/README.rst` & `pca-b-stream-2023.2/README.rst`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/documentation/wiki/description.asciidoc` & `pca-b-stream-2023.2/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/__init__.py` & `pca-b-stream-2023.2/pca_b_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/cli.py` & `pca-b-stream-2023.2/pca_b_stream/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,29 +35,28 @@
 
 >>> import pathlib
 >>> import sys
 >>> from unittest.mock import patch
 >>> path = pathlib.Path(".") / "resource" / "pca-0.png"
 >>> with patch("sys.argv", new=["fake_cmd_name", path]):
 ...     PCA2BStream()
-FnmHoFain+3jtU
-
+FnmHo0tyN+0}BCI
 >>> import imageio
 >>> import numpy
 >>> import pathlib
 >>> import sys
 >>> import tempfile
 >>> from unittest.mock import patch
 >>> folder = tempfile.mkdtemp()
 >>> path = pathlib.Path(folder) / "a.png"
->>> with patch("sys.argv", new=["fake_cmd_name", "FnmHoFain+3jtU", path]):
+>>> with patch("sys.argv", new=["fake_cmd_name", "FnmHo0tyN+0}BCI", path]):
 ...     BStream2PCA()
 >>> original_path = pathlib.Path(".") / "resource" / "pca-0.png"
->>> original = imageio.imread(original_path)
->>> image = imageio.imread(path)
+>>> original = imageio.v3.imread(original_path)
+>>> image = imageio.v3.imread(path)
 >>> print(numpy.array_equal(image, original))
 True
 """
 
 import sys as sstm
 from pathlib import Path as path_t
```

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/html/constants.py` & `pca-b-stream-2023.2/pca_b_stream/flask/html/constants.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/html/main.html` & `pca-b-stream-2023.2/pca_b_stream/flask/html/main.html`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/html/session.py` & `pca-b-stream-2023.2/pca_b_stream/flask/html/session.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/main.py` & `pca-b-stream-2023.2/pca_b_stream/flask/main.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/session/constants.py` & `pca-b-stream-2023.2/pca_b_stream/flask/session/constants.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/session/form.py` & `pca-b-stream-2023.2/pca_b_stream/flask/session/form.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/session/processing.py` & `pca-b-stream-2023.2/pca_b_stream/flask/session/processing.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/session/session.py` & `pca-b-stream-2023.2/pca_b_stream/flask/session/session.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/flask/static/main.css` & `pca-b-stream-2023.2/pca_b_stream/flask/static/main.css`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/main.py` & `pca-b-stream-2023.2/pca_b_stream/main.py`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/pca_b_stream/version.py` & `pca-b-stream-2023.2/pca_b_stream/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.1"
+__version__ = "2023.2"
```

### Comparing `pca-b-stream-2023.1/pca_b_stream.egg-info/PKG-INFO` & `pca-b-stream-2023.2/pca_b_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pca-b-stream
-Version: 2023.1
+Version: 2023.2
 Summary: Byte Stream Representation of Piecewise-constant Array
 Home-page: https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/pca-b-stream/
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/pca-b-stream/
```

### Comparing `pca-b-stream-2023.1/pca_b_stream.egg-info/SOURCES.txt` & `pca-b-stream-2023.2/pca_b_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pca-b-stream-2023.1/setup.py` & `pca-b-stream-2023.2/setup.py`

 * *Files identical despite different names*

