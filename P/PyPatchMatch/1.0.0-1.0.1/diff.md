# Comparing `tmp/PyPatchMatch-1.0.0.tar.gz` & `tmp/PyPatchMatch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPatchMatch-1.0.0.tar", last modified: Sun Mar  5 20:21:08 2023, max compression
+gzip compressed data, was "PyPatchMatch-1.0.1.tar", last modified: Thu Jul 20 23:49:28 2023, max compression
```

## Comparing `PyPatchMatch-1.0.0.tar` & `PyPatchMatch-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:08.620937 PyPatchMatch-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-05 20:21:08.620937 PyPatchMatch-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:08.612937 PyPatchMatch-1.0.0/PyPatchMatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-05 20:21:08.000000 PyPatchMatch-1.0.0/PyPatchMatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-05 20:21:08.000000 PyPatchMatch-1.0.0/PyPatchMatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 20:21:08.000000 PyPatchMatch-1.0.0/PyPatchMatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-05 20:21:08.000000 PyPatchMatch-1.0.0/PyPatchMatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-05 20:21:08.000000 PyPatchMatch-1.0.0/PyPatchMatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:08.620937 PyPatchMatch-1.0.0/patchmatch/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 20:21:08.620937 PyPatchMatch-1.0.0/patchmatch/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/inpaint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/inpaint.h
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/masked_image.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/masked_image.h
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/nnf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/nnf.h
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/pyinterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/csrc/pyinterface.h
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/patch_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/patchmatch/travis.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-05 20:20:48.000000 PyPatchMatch-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 20:21:08.620937 PyPatchMatch-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:49:28.794672 PyPatchMatch-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-20 23:49:28.794672 PyPatchMatch-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:49:28.794672 PyPatchMatch-1.0.1/PyPatchMatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-20 23:49:28.000000 PyPatchMatch-1.0.1/PyPatchMatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-20 23:49:28.000000 PyPatchMatch-1.0.1/PyPatchMatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:49:28.000000 PyPatchMatch-1.0.1/PyPatchMatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 23:49:28.000000 PyPatchMatch-1.0.1/PyPatchMatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 23:49:28.000000 PyPatchMatch-1.0.1/PyPatchMatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:49:28.794672 PyPatchMatch-1.0.1/patchmatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:49:28.794672 PyPatchMatch-1.0.1/patchmatch/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/inpaint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/inpaint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/masked_image.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/masked_image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/nnf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/nnf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/pyinterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/csrc/pyinterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/patch_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/patchmatch/travis.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-20 23:49:04.000000 PyPatchMatch-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:49:28.794672 PyPatchMatch-1.0.1/setup.cfg
```

### Comparing `PyPatchMatch-1.0.0/LICENSE` & `PyPatchMatch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/PKG-INFO` & `PyPatchMatch-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPatchMatch
-Version: 1.0.0
+Version: 1.0.1
 Summary: This library implements the PatchMatch based inpainting algorithm.
 Author-email: The InvokeAI Project <lincoln.stein@gmail.com>, Kyle Schouviller <kyle0654@hotmail.com>, Matthias Wild <mauwii@outlook.de>, Younesse ANDAM <younesse.andam@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Matthias Wild
         Copyright (c) 2020 Jiayuan Mao
         
@@ -23,15 +23,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Source Code, https://github.com/mauwii/PyPatchMatch
-Requires-Python: >=3.9
+Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: dist
 Provides-Extra: test
 License-File: LICENSE
 
 # PatchMatch based Inpainting
```

### Comparing `PyPatchMatch-1.0.0/PyPatchMatch.egg-info/PKG-INFO` & `PyPatchMatch-1.0.1/PyPatchMatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPatchMatch
-Version: 1.0.0
+Version: 1.0.1
 Summary: This library implements the PatchMatch based inpainting algorithm.
 Author-email: The InvokeAI Project <lincoln.stein@gmail.com>, Kyle Schouviller <kyle0654@hotmail.com>, Matthias Wild <mauwii@outlook.de>, Younesse ANDAM <younesse.andam@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Matthias Wild
         Copyright (c) 2020 Jiayuan Mao
         
@@ -23,15 +23,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Source Code, https://github.com/mauwii/PyPatchMatch
-Requires-Python: >=3.9
+Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: dist
 Provides-Extra: test
 License-File: LICENSE
 
 # PatchMatch based Inpainting
```

### Comparing `PyPatchMatch-1.0.0/PyPatchMatch.egg-info/SOURCES.txt` & `PyPatchMatch-1.0.1/PyPatchMatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/README.md` & `PyPatchMatch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/Makefile` & `PyPatchMatch-1.0.1/patchmatch/Makefile`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/inpaint.cpp` & `PyPatchMatch-1.0.1/patchmatch/csrc/inpaint.cpp`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/inpaint.h` & `PyPatchMatch-1.0.1/patchmatch/csrc/inpaint.h`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/masked_image.cpp` & `PyPatchMatch-1.0.1/patchmatch/csrc/masked_image.cpp`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/masked_image.h` & `PyPatchMatch-1.0.1/patchmatch/csrc/masked_image.h`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/nnf.cpp` & `PyPatchMatch-1.0.1/patchmatch/csrc/nnf.cpp`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/nnf.h` & `PyPatchMatch-1.0.1/patchmatch/csrc/nnf.h`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/pyinterface.cpp` & `PyPatchMatch-1.0.1/patchmatch/csrc/pyinterface.cpp`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/csrc/pyinterface.h` & `PyPatchMatch-1.0.1/patchmatch/csrc/pyinterface.h`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/patchmatch/patch_match.py` & `PyPatchMatch-1.0.1/patchmatch/patch_match.py`

 * *Files identical despite different names*

### Comparing `PyPatchMatch-1.0.0/pyproject.toml` & `PyPatchMatch-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 dependencies=["numpy", "pillow", "tqdm"]
 description='This library implements the PatchMatch based inpainting algorithm.'
 dynamic=["version"]
 license={file="LICENSE"}
 name='PyPatchMatch'
 readme={content-type="text/markdown", file="README.md"}
-requires-python=">=3.9"
+requires-python=">=3.9,<3.11"
 
 [project.urls]
 'Source Code'='https://github.com/mauwii/PyPatchMatch'
 
 [tool.setuptools.dynamic]
 version={attr="patchmatch.__version__"}
 
@@ -43,29 +43,28 @@
 ]
 "test"=["pytest", "pytest-coverage"]
 
 [tool.black]
 exclude='''
 /(
     .git
-    | .hg
-    | .mypy_cache
-    | .tox
     | .venv
-    | _build
-    | buck-out
     | build
+    | csrc
     | dist
 )/
 '''
 include='.pyi?$'
 line-length=88
 source=['examples', 'patchmatch']
 target-version=['py39']
 
+[tool.coverage.report]
+fail_under=75
+
 [tool.isort]
 profile="black"
 
 [tool.pytest.ini_options]
 addopts=["--cov-branch", "--cov-report=term:skip-covered", "--cov=patchmatch"]
 minversion="6.0"
 python_files=["test_*.py"]
```

