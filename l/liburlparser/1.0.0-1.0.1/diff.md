# Comparing `tmp/liburlparser-1.0.0.tar.gz` & `tmp/liburlparser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liburlparser-1.0.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "liburlparser-1.0.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `liburlparser-1.0.0.tar` & `liburlparser-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 liburlparser-1.0.0/.clang-format
--rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 liburlparser-1.0.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 liburlparser-1.0.0/.gitignore
--rw-r--r--   0        0        0     4786 2022-11-09 12:37:21.000000 liburlparser-1.0.0/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 liburlparser-1.0.0/LICENSE
--rw-r--r--   0        0        0     6779 2022-11-09 12:37:21.000000 liburlparser-1.0.0/README.md
--rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 liburlparser-1.0.0/conda.recipe/meta.yaml
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 liburlparser-1.0.0/docs/Doxyfile.in
--rw-r--r--   0        0        0     4529 2022-11-09 12:37:21.000000 liburlparser-1.0.0/docs/images/logo/liburlparser-logo-1.svg
--rw-r--r--   0        0        0     4515 2022-11-09 12:37:21.000000 liburlparser-1.0.0/docs/images/logo/liburlparser-logo-2.svg
--rw-r--r--   0        0        0     2517 2022-11-09 12:37:21.000000 liburlparser-1.0.0/examples/common.h
--rw-r--r--   0        0        0     2652 2022-11-09 12:37:21.000000 liburlparser-1.0.0/examples/main.cpp
--rw-r--r--   0        0        0     2303 2022-11-09 12:37:21.000000 liburlparser-1.0.0/include/urlparser.h
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 liburlparser-1.0.0/noxfile.py
--rw-r--r--   0        0        0     3198 2022-11-09 12:37:21.000000 liburlparser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5520 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/binding/main.cpp
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/liburlparser/__init__.py
--rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/liburlparser/__main__.py
--rw-r--r--   0        0        0      887 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/liburlparser/core.py
--rw-r--r--   0        0        0     4994 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/psl.cpp
--rw-r--r--   0        0        0     3372 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/psl.h
--rw-r--r--   0        0        0    26613 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/url.cpp
--rw-r--r--   0        0        0     8937 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/url.h
--rw-r--r--   0        0        0     8388 2022-11-09 12:37:21.000000 liburlparser-1.0.0/src/urlparser.cpp
--rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 liburlparser-1.0.0/tests/data/host_data.csv
--rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 liburlparser-1.0.0/tests/data/url_data.csv
--rw-r--r--   0        0        0        9 2022-11-09 12:37:21.000000 liburlparser-1.0.0/tests/pytest.ini
--rw-r--r--   0        0        0     1473 2022-11-09 12:37:21.000000 liburlparser-1.0.0/tests/test.cpp
--rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 liburlparser-1.0.0/tests/test_extra.py
--rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 liburlparser-1.0.0/tests/test_host.py
--rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 liburlparser-1.0.0/tests/test_url.py
--rw-r--r--   0        0        0     7825 2022-11-09 12:37:21.000000 liburlparser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 liburlparser-1.0.1/.clang-format
+-rw-r--r--   0        0        0     1838 2022-11-09 12:37:21.000000 liburlparser-1.0.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 liburlparser-1.0.1/.gitignore
+-rw-r--r--   0        0        0     4786 2022-11-09 12:37:21.000000 liburlparser-1.0.1/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 liburlparser-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6779 2022-11-09 12:37:21.000000 liburlparser-1.0.1/README.md
+-rw-r--r--   0        0        0      527 2022-11-09 12:37:21.000000 liburlparser-1.0.1/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 liburlparser-1.0.1/docs/Doxyfile.in
+-rw-r--r--   0        0        0     4529 2022-11-09 12:37:21.000000 liburlparser-1.0.1/docs/images/logo/liburlparser-logo-1.svg
+-rw-r--r--   0        0        0     4515 2022-11-09 12:37:21.000000 liburlparser-1.0.1/docs/images/logo/liburlparser-logo-2.svg
+-rw-r--r--   0        0        0     2517 2022-11-09 12:37:21.000000 liburlparser-1.0.1/examples/common.h
+-rw-r--r--   0        0        0     2652 2022-11-09 12:37:21.000000 liburlparser-1.0.1/examples/main.cpp
+-rw-r--r--   0        0        0     2303 2022-11-09 12:37:21.000000 liburlparser-1.0.1/include/urlparser.h
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 liburlparser-1.0.1/noxfile.py
+-rw-r--r--   0        0        0     3198 2022-11-09 12:37:21.000000 liburlparser-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5520 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/binding/main.cpp
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/liburlparser/__init__.py
+-rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/liburlparser/__main__.py
+-rw-r--r--   0        0        0      887 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/liburlparser/core.py
+-rw-r--r--   0        0        0     4994 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/psl.cpp
+-rw-r--r--   0        0        0     3372 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/psl.h
+-rw-r--r--   0        0        0    26613 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/url.cpp
+-rw-r--r--   0        0        0     8937 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/url.h
+-rw-r--r--   0        0        0     8388 2022-11-09 12:37:21.000000 liburlparser-1.0.1/src/urlparser.cpp
+-rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 liburlparser-1.0.1/tests/data/host_data.csv
+-rw-r--r--   0        0        0      401 2022-11-09 12:37:21.000000 liburlparser-1.0.1/tests/data/url_data.csv
+-rw-r--r--   0        0        0        9 2022-11-09 12:37:21.000000 liburlparser-1.0.1/tests/pytest.ini
+-rw-r--r--   0        0        0     1473 2022-11-09 12:37:21.000000 liburlparser-1.0.1/tests/test.cpp
+-rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 liburlparser-1.0.1/tests/test_extra.py
+-rw-r--r--   0        0        0      585 2022-11-09 12:37:21.000000 liburlparser-1.0.1/tests/test_host.py
+-rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 liburlparser-1.0.1/tests/test_url.py
+-rw-r--r--   0        0        0     7825 2022-11-09 12:37:21.000000 liburlparser-1.0.1/PKG-INFO
```

### Comparing `liburlparser-1.0.0/.github/workflows/wheels.yml` & `liburlparser-1.0.1/.github/workflows/wheels.yml`

 * *Files 6% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     - uses: actions/checkout@v3
       with:
         submodules: true
 
     - name: Build wheels
       uses: pypa/cibuildwheel@v2.13.1
       env:
-         CIBW_ARCHS_MACOS: universal2
-         CIBW_ARCHS_WINDOWS: auto ARM64
+#          CIBW_ARCHS_MACOS: universal2
+#          CIBW_ARCHS_WINDOWS: auto ARM64
          # Disable building PyPy wheels on all platforms
          CIBW_SKIP: pp*
 #         CIBW_PRERELEASE_PYTHONS: true
 
     - name: Verify clean directory
       run: git diff --exit-code
       shell: bash
```

### Comparing `liburlparser-1.0.0/CMakeLists.txt` & `liburlparser-1.0.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/LICENSE` & `liburlparser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/README.md` & `liburlparser-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/conda.recipe/meta.yaml` & `liburlparser-1.0.1/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/docs/images/logo/liburlparser-logo-1.svg` & `liburlparser-1.0.1/docs/images/logo/liburlparser-logo-1.svg`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/docs/images/logo/liburlparser-logo-2.svg` & `liburlparser-1.0.1/docs/images/logo/liburlparser-logo-2.svg`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/examples/common.h` & `liburlparser-1.0.1/examples/common.h`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/examples/main.cpp` & `liburlparser-1.0.1/examples/main.cpp`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/include/urlparser.h` & `liburlparser-1.0.1/include/urlparser.h`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/pyproject.toml` & `liburlparser-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #requires = ["scikit-build-core>=0.3.3", "nanobind==1.4.0"]
 requires = ["scikit-build-core==0.4.6", "nanobind==1.4.0"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "liburlparser"
-version = "1.0.0"
+version = "1.0.1"
 description="Fastest Url parser in the world"
 readme = "README.md"
 authors = [
   { name = "Mohammad Raziei", email = "mohammadraziei1375@gmail.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `liburlparser-1.0.0/src/binding/main.cpp` & `liburlparser-1.0.1/src/binding/main.cpp`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/src/liburlparser/__main__.py` & `liburlparser-1.0.1/src/liburlparser/__main__.py`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/src/liburlparser/core.py` & `liburlparser-1.0.1/src/liburlparser/core.py`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/src/psl.cpp` & `liburlparser-1.0.1/src/psl.cpp`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/src/psl.h` & `liburlparser-1.0.1/src/psl.h`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/src/url.cpp` & `liburlparser-1.0.1/src/url.cpp`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/src/url.h` & `liburlparser-1.0.1/src/url.h`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/src/urlparser.cpp` & `liburlparser-1.0.1/src/urlparser.cpp`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/tests/test.cpp` & `liburlparser-1.0.1/tests/test.cpp`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/tests/test_extra.py` & `liburlparser-1.0.1/tests/test_extra.py`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/tests/test_host.py` & `liburlparser-1.0.1/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/tests/test_url.py` & `liburlparser-1.0.1/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `liburlparser-1.0.0/PKG-INFO` & `liburlparser-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liburlparser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fastest Url parser in the world
 Author-Email: Mohammad Raziei <mohammadraziei1375@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: liburlparser Version: 1.0.0 Summary: Fastest Url
+Metadata-Version: 2.1 Name: liburlparser Version: 1.0.1 Summary: Fastest Url
 parser in the world Author-Email: Mohammad Raziei
 gmail.com> Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

