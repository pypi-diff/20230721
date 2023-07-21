# Comparing `tmp/pycompile-0.1.7.tar.gz` & `tmp/pycompile-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompile-0.1.7.tar", max compression
+gzip compressed data, was "pycompile-0.1.9.tar", max compression
```

## Comparing `pycompile-0.1.7.tar` & `pycompile-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1074 2023-07-07 16:50:17.956671 pycompile-0.1.7/LICENSE
--rw-r--r--   0        0        0    10555 2023-07-07 16:50:17.956671 pycompile-0.1.7/README.md
--rw-r--r--   0        0        0     1581 2023-07-07 16:50:17.968671 pycompile-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      515 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/__init__.py
--rw-r--r--   0        0        0     7161 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/benchmark.py
--rw-r--r--   0        0        0        0 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/__init__.py
--rw-r--r--   0        0        0     2583 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/benchmark_cmd.py
--rw-r--r--   0        0        0     2365 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/compile_cmd.py
--rw-r--r--   0        0        0     1721 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/dry_run_cmd.py
--rw-r--r--   0        0        0      701 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/cli/entrypoint.py
--rw-r--r--   0        0        0     2886 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/compiler_handler.py
--rw-r--r--   0        0        0        0 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/__init__.py
--rw-r--r--   0        0        0      243 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/examples_benchmark.py
--rw-r--r--   0        0        0      145 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/fib.py
--rw-r--r--   0        0        0      128 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/harmonic.py
--rw-r--r--   0        0        0      441 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/sum.py
--rw-r--r--   0        0        0       97 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/examples/test_examples.py
--rw-r--r--   0        0        0     4692 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/file_handler.py
--rw-r--r--   0        0        0     2888 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/helpers.py
--rw-r--r--   0        0        0     1341 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/logging_setup.py
--rw-r--r--   0        0        0     3284 2023-07-07 16:50:17.972671 pycompile-0.1.7/src/wrappers.py
--rw-r--r--   0        0        0    11242 1970-01-01 00:00:00.000000 pycompile-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-07 17:25:50.606086 pycompile-0.1.9/LICENSE
+-rw-r--r--   0        0        0    10555 2023-07-07 17:25:50.606086 pycompile-0.1.9/README.md
+-rw-r--r--   0        0        0     1581 2023-07-07 17:25:50.618086 pycompile-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      515 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/__init__.py
+-rw-r--r--   0        0        0     7161 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/benchmark.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/cli/__init__.py
+-rw-r--r--   0        0        0     2609 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/cli/benchmark_cmd.py
+-rw-r--r--   0        0        0     2391 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/cli/compile_cmd.py
+-rw-r--r--   0        0        0     1747 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/cli/dry_run_cmd.py
+-rw-r--r--   0        0        0      791 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/cli/entrypoint.py
+-rw-r--r--   0        0        0     2886 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/compiler_handler.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/examples/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/examples/examples_benchmark.py
+-rw-r--r--   0        0        0      145 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/examples/fib.py
+-rw-r--r--   0        0        0      128 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/examples/harmonic.py
+-rw-r--r--   0        0        0      441 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/examples/sum.py
+-rw-r--r--   0        0        0       97 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/examples/test_examples.py
+-rw-r--r--   0        0        0     4692 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/file_handler.py
+-rw-r--r--   0        0        0     2888 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/helpers.py
+-rw-r--r--   0        0        0     1341 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/logging_setup.py
+-rw-r--r--   0        0        0     3284 2023-07-07 17:25:50.618086 pycompile-0.1.9/src/wrappers.py
+-rw-r--r--   0        0        0    11242 1970-01-01 00:00:00.000000 pycompile-0.1.9/PKG-INFO
```

### Comparing `pycompile-0.1.7/LICENSE` & `pycompile-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/README.md` & `pycompile-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/pyproject.toml` & `pycompile-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycompile"
-version = "0.1.7"
+version = "0.1.9"
 description = "A CLI tool for compiling python"
 authors = ["iplitharas <johnplitharas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src" }
 ]
```

### Comparing `pycompile-0.1.7/src/__init__.py` & `pycompile-0.1.9/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/src/benchmark.py` & `pycompile-0.1.9/src/benchmark.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/src/cli/benchmark_cmd.py` & `pycompile-0.1.9/src/cli/benchmark_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from src.benchmark import Benchmark
 from src.helpers import Colors
 
 logger = logging.getLogger(__name__)
 
 
-@click.command(name="benchmark")
+@click.command(name="benchmark")  # type: ignore[arg-type]
 @click.option(
     "-i",
     "--input-path",
     required=True,
     type=click.Path(exists=True),
     help="Specify the file/folder input path",
 )
```

### Comparing `pycompile-0.1.7/src/cli/compile_cmd.py` & `pycompile-0.1.9/src/cli/compile_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     NuitkaWrapper,
     setup_logging,
 )
 
 logger = logging.getLogger(__name__)
 
 
-@click.command(name="compile")
+@click.command(name="compile")  # type: ignore[arg-type]
 @click.option(
     "-i",
     "--input-path",
     required=True,
     type=click.Path(exists=True),
     help="Specify the file/folder input path, "
     "by default it will exclude any `test` and `__init__.py` files",
```

### Comparing `pycompile-0.1.7/src/cli/dry_run_cmd.py` & `pycompile-0.1.9/src/cli/dry_run_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from src import FileHandler, setup_logging
 from src.helpers import Colors
 
 logger = logging.getLogger(__name__)
 
 
-@click.command(name="dry_run")
+@click.command(name="dry_run")  # type: ignore[arg-type]
 @click.option(
     "-i",
     "--input-path",
     required=True,
     type=click.Path(exists=True),
     help="Specify the file/folder input path",
 )
```

### Comparing `pycompile-0.1.7/src/compiler_handler.py` & `pycompile-0.1.9/src/compiler_handler.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/src/file_handler.py` & `pycompile-0.1.9/src/file_handler.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/src/helpers.py` & `pycompile-0.1.9/src/helpers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/src/logging_setup.py` & `pycompile-0.1.9/src/logging_setup.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/src/wrappers.py` & `pycompile-0.1.9/src/wrappers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.7/PKG-INFO` & `pycompile-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompile
-Version: 0.1.7
+Version: 0.1.9
 Summary: A CLI tool for compiling python
 License: MIT
 Author: iplitharas
 Author-email: johnplitharas@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

