# Comparing `tmp/tubex2-1.0.0.tar.gz` & `tmp/tubex2-1.0.1.tar.gz`

## Comparing `tubex2-1.0.0.tar` & `tubex2-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tubex2-1.0.0/src/tubex2/__init__.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 tubex2-1.0.0/src/tubex2/__main__.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 tubex2-1.0.0/src/tubex2/exceptions.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 tubex2-1.0.0/src/tubex2/extract.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tubex2-1.0.0/src/tubex2/query.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tubex2-1.0.0/src/tubex2/stream.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tubex2-1.0.0/src/tubex2/version.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 tubex2-1.0.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 tubex2-1.0.0/LICENSE
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tubex2-1.0.0/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tubex2-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 tubex2-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tubex2-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tubex2-1.0.1/src/tubex2/__init__.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 tubex2-1.0.1/src/tubex2/__main__.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 tubex2-1.0.1/src/tubex2/exceptions.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 tubex2-1.0.1/src/tubex2/extract.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tubex2-1.0.1/src/tubex2/query.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tubex2-1.0.1/src/tubex2/stream.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tubex2-1.0.1/src/tubex2/version.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 tubex2-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 tubex2-1.0.1/LICENSE
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tubex2-1.0.1/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 tubex2-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 tubex2-1.0.1/PKG-INFO
```

### Comparing `tubex2-1.0.0/src/tubex2/__main__.py` & `tubex2-1.0.1/src/tubex2/__main__.py`

 * *Files identical despite different names*

### Comparing `tubex2-1.0.0/src/tubex2/exceptions.py` & `tubex2-1.0.1/src/tubex2/exceptions.py`

 * *Files identical despite different names*

### Comparing `tubex2-1.0.0/src/tubex2/extract.py` & `tubex2-1.0.1/src/tubex2/extract.py`

 * *Files identical despite different names*

### Comparing `tubex2-1.0.0/src/tubex2/query.py` & `tubex2-1.0.1/src/tubex2/query.py`

 * *Files identical despite different names*

### Comparing `tubex2-1.0.0/src/tubex2/stream.py` & `tubex2-1.0.1/src/tubex2/stream.py`

 * *Files identical despite different names*

### Comparing `tubex2-1.0.0/.gitignore` & `tubex2-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tubex2-1.0.0/README.md` & `tubex2-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 many new features are under development
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install tubex2.
 
 ```bash
-py -m pip install tubex_dl
+py -m pip install tubex2
 ```
 
 ## Usage
 
 ```python
-from tubex_dl import YouTube
+from tubex2 import YouTube
 import asyncio
 
 async def get_video():
      url = "youtube-video-url"
 
      #create YouTube object
      yt = YouTube(url)
@@ -37,11 +37,7 @@
      stream = yt.streams.all().first()
 
      #download video
      await stream.download(num_chunks=10)
 
 asyncio.run(get_video())
 ```
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
```

