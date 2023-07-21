# Comparing `tmp/jsonlogic-rs-0.2.3.tar.gz` & `tmp/jsonlogic-rs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonlogic-rs-0.2.3.tar", last modified: Wed Jan  5 01:26:46 2022, max compression
+gzip compressed data, was "jsonlogic-rs-0.3.0.tar", last modified: Fri Jul 21 20:32:20 2023, max compression
```

## Comparing `jsonlogic-rs-0.2.3.tar` & `jsonlogic-rs-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 01:26:46.741228 jsonlogic-rs-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10456 2022-01-05 01:26:46.741228 jsonlogic-rs-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9365 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 01:26:46.741228 jsonlogic-rs-0.2.3/py/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 01:26:46.741228 jsonlogic-rs-0.2.3/py/jsonlogic_rs/
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/py/jsonlogic_rs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 01:26:46.741228 jsonlogic-rs-0.2.3/py/jsonlogic_rs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10456 2022-01-05 01:26:46.000000 jsonlogic-rs-0.2.3/py/jsonlogic_rs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-01-05 01:26:46.000000 jsonlogic-rs-0.2.3/py/jsonlogic_rs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 01:26:46.000000 jsonlogic-rs-0.2.3/py/jsonlogic_rs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 01:26:46.000000 jsonlogic-rs-0.2.3/py/jsonlogic_rs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-05 01:26:46.000000 jsonlogic-rs-0.2.3/py/jsonlogic_rs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-05 01:26:46.745228 jsonlogic-rs-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 01:26:46.741228 jsonlogic-rs-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/bin.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/func.rs
--rw-r--r--   0 runner    (1001) docker     (121)    41845 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/js_op.rs
--rw-r--r--   0 runner    (1001) docker     (121)    48168 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 01:26:46.741228 jsonlogic-rs-0.2.3/src/op/
--rw-r--r--   0 runner    (1001) docker     (121)    14230 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/op/array.rs
--rw-r--r--   0 runner    (1001) docker     (121)     8976 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/op/data.rs
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/op/impure.rs
--rw-r--r--   0 runner    (1001) docker     (121)     6828 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/op/logic.rs
--rw-r--r--   0 runner    (1001) docker     (121)    17078 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/op/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/op/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5685 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/op/string.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-01-05 01:25:34.000000 jsonlogic-rs-0.2.3/src/value.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/py/jsonlogic_rs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 20:32:20.000000 jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/bin.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/func.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    41847 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/js_op.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    48168 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:20.776376 jsonlogic-rs-0.3.0/src/op/
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/array.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/impure.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/logic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/op/string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-21 20:31:44.000000 jsonlogic-rs-0.3.0/src/value.rs
```

### Comparing `jsonlogic-rs-0.2.3/Cargo.toml` & `jsonlogic-rs-0.3.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 edition = "2018"
 homepage = "https://github.com/bestowinc/json-logic-rs"
 keywords = ["json", "jsonlogic", "s-expressions", "web", "logic"]
 license = "MIT"
 name = "jsonlogic-rs"
 readme = "README.md"
 repository = "https://github.com/bestowinc/json-logic-rs"
-version = "0.2.3"
+version = "0.3.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 # cdylib for CFFI and python integration
 # lib for regular rust stuff
 crate-type = ["cdylib", "lib"]
@@ -38,15 +38,15 @@
 features = ["serde-serialize"]
 optional = true
 version = "~0.2.62"
 
 [dependencies.cpython]
 features = ["extension-module"]
 optional = true
-version = "0.5"
+version = "0.7"
 
 [dependencies.anyhow]
 optional = true
 version = "~1.0.31"
 
 [dependencies.clap]
 optional = true
```

### Comparing `jsonlogic-rs-0.2.3/LICENSE` & `jsonlogic-rs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/PKG-INFO` & `jsonlogic-rs-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: jsonlogic-rs
-Version: 0.2.3
+Version: 0.3.0
 Summary: JsonLogic implemented with a Rust backend
 Home-page: https://www.github.com/bestowinc/json-logic-rs
 Author: Matthew Planchard
 Author-email: msplanchard@gmail.com
 Maintainer-email: msplanchard@gmail.com
-License: UNKNOWN
 Keywords: json,jsonlogic,s-expressions,rust
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json-logic-rs
 
 ![Continuous Integration](https://github.com/Bestowinc/json-logic-rs/workflows/Continuous%20Integration/badge.svg?branch=master)
@@ -295,9 +294,7 @@
 importable by your local venv. When building wheels, the wrapper and the C
 extension are all packaged together into the resultant wheel, which will
 be found in `dist/`. When building an sdist, the Rust extension is not compiled.
 The Rust and Python source are distributed together in a `.tar.gz` file, again
 found in `dist/`.
 
 [jsonlogic]: http://jsonlogic.com/
-
-
```

### Comparing `jsonlogic-rs-0.2.3/README.md` & `jsonlogic-rs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/py/jsonlogic_rs/__init__.py` & `jsonlogic-rs-0.3.0/py/jsonlogic_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/py/jsonlogic_rs.egg-info/PKG-INFO` & `jsonlogic-rs-0.3.0/py/jsonlogic_rs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: jsonlogic-rs
-Version: 0.2.3
+Version: 0.3.0
 Summary: JsonLogic implemented with a Rust backend
 Home-page: https://www.github.com/bestowinc/json-logic-rs
 Author: Matthew Planchard
 Author-email: msplanchard@gmail.com
 Maintainer-email: msplanchard@gmail.com
-License: UNKNOWN
 Keywords: json,jsonlogic,s-expressions,rust
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json-logic-rs
 
 ![Continuous Integration](https://github.com/Bestowinc/json-logic-rs/workflows/Continuous%20Integration/badge.svg?branch=master)
@@ -295,9 +294,7 @@
 importable by your local venv. When building wheels, the wrapper and the C
 extension are all packaged together into the resultant wheel, which will
 be found in `dist/`. When building an sdist, the Rust extension is not compiled.
 The Rust and Python source are distributed together in a `.tar.gz` file, again
 found in `dist/`.
 
 [jsonlogic]: http://jsonlogic.com/
-
-
```

### Comparing `jsonlogic-rs-0.2.3/setup.py` & `jsonlogic-rs-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def get_version():
     generate_lockfile()
     proc = Popen(("cargo", "pkgid"), stdout=PIPE, stderr=PIPE)
     out, err = tuple(map(bytes.decode, proc.communicate()))
     if proc.returncode != 0:
         raise RuntimeError(f"Could not get Cargo package info: {err}")
-    version = out.split(":")[-1]
+    version = out.split("@")[-1]
     return version.strip()
 
 
 with open(PKG_ROOT / "README.md") as readme_f:
     LONG_DESCRIPTION = readme_f.read()
 
 VERSION = get_version()
@@ -47,42 +47,28 @@
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords=["json", "jsonlogic", "s-expressions", "rust"],
     classifiers=[
         # See https://pypi.python.org/pypi?%3Aaction=list_classifiers for all
         # available setup classifiers
-        # "Development Status :: 1 - Planning",
-        # 'Development Status :: 2 - Pre-Alpha',
-        # "Development Status :: 3 - Alpha",
-        # "Development Status :: 4 - Beta",
         'Development Status :: 5 - Production/Stable',
-        # 'Development Status :: 6 - Mature',
-        # 'Framework :: AsyncIO',
-        # 'Framework :: Flask',
-        # 'Framework :: Sphinx',
-        # 'Environment :: Web Environment',
         "Intended Audience :: Developers",
-        # 'Intended Audience :: End Users/Desktop',
-        # 'Intended Audience :: Science/Research',
-        # 'Intended Audience :: System Administrators',
-        # 'License :: Other/Proprietary License',
-        # 'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         "License :: OSI Approved :: MIT License",
-        # "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Rust",
         # 'Programming Language :: Python :: Implementation :: PyPy',
     ],
     rust_extensions=[
         RustExtension(
             # Python package name before the dot, name of C extension to
             # stick inside of it after the dot.
```

### Comparing `jsonlogic-rs-0.2.3/src/bin.rs` & `jsonlogic-rs-0.3.0/src/bin.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/error.rs` & `jsonlogic-rs-0.3.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/func.rs` & `jsonlogic-rs-0.3.0/src/func.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/js_op.rs` & `jsonlogic-rs-0.3.0/src/js_op.rs`

 * *Files 0% similar despite different names*

```diff
@@ -896,15 +896,15 @@
     fn test_to_string_bool() {
         assert_eq!(&to_string(&json!(true)), "true");
         assert_eq!(&to_string(&json!(false)), "false");
     }
 
     #[test]
     fn test_to_string_number() {
-        assert_eq!(&to_string(&json!(1.0)), "1");
+        assert_eq!(&to_string(&json!(1.0)), "1.0");
         assert_eq!(&to_string(&json!(1)), "1");
     }
 
     #[test]
     fn test_abstract_eq() {
         equal_values().iter().for_each(|(first, second)| {
             println!("{:?}-{:?}", &first, &second);
```

### Comparing `jsonlogic-rs-0.2.3/src/lib.rs` & `jsonlogic-rs-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/op/array.rs` & `jsonlogic-rs-0.3.0/src/op/array.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/op/data.rs` & `jsonlogic-rs-0.3.0/src/op/data.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/op/logic.rs` & `jsonlogic-rs-0.3.0/src/op/logic.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/op/mod.rs` & `jsonlogic-rs-0.3.0/src/op/mod.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/op/numeric.rs` & `jsonlogic-rs-0.3.0/src/op/numeric.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/op/string.rs` & `jsonlogic-rs-0.3.0/src/op/string.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.2.3/src/value.rs` & `jsonlogic-rs-0.3.0/src/value.rs`

 * *Files identical despite different names*

