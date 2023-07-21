# Comparing `tmp/python2verilog-0.0.2.tar.gz` & `tmp/python2verilog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python2verilog-0.0.2.tar", last modified: Sun Jul 16 07:08:58 2023, max compression
+gzip compressed data, was "python2verilog-0.0.3.tar", last modified: Fri Jul 21 15:27:40 2023, max compression
```

## Comparing `python2verilog-0.0.2.tar` & `python2verilog-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-16 07:08:58.059761 python2verilog-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-16 07:08:41.000000 python2verilog-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-16 07:08:41.000000 python2verilog-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.055761 python2verilog-0.0.2/python2verilog/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/statements.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/backend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15689 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/generator2ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/frontend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.059761 python2verilog-0.0.2/python2verilog/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-16 07:08:41.000000 python2verilog-0.0.2/python2verilog/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 07:08:58.055761 python2verilog-0.0.2/python2verilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-16 07:08:58.000000 python2verilog-0.0.2/python2verilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 07:08:58.059761 python2verilog-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.532267 python2verilog-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-21 15:27:40.532267 python2verilog-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-21 15:27:26.000000 python2verilog-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-21 15:27:26.000000 python2verilog-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.524267 python2verilog-0.0.3/python2verilog/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/backend/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19875 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/frontend/generator_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.532267 python2verilog-0.0.3/python2verilog/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:27:40.532267 python2verilog-0.0.3/setup.cfg
```

### Comparing `python2verilog-0.0.2/PKG-INFO` & `python2verilog-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,126 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
+![Python Package](https://github.com/worldofkerry/python2verilog/actions/workflows/python-package.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/python2verilog/badge/?version=latest)](https://python2verilog.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/python2verilog)
+
 # Python 2 Verilog
 
 Converts a subset of python generator functions into synthesizable sequential SystemVerilog.
 
 A use case is for drawing shapes on grids (for VGA output), where the user may prototype the algorithm in python and then convert it to verilog for use in an FPGA.
 
-A testbench is also generated and asserted against the Python outputs.
+A testbench can also be generated and asserted against the Python outputs.
 
 Supports Python [Generator functions](https://wiki.python.org/moin/Generators) as well as the following block types:
 
 - `if`
 - `while`
-- `for ... in range(...)` with 1 or 2 args in `range` (quite inefficient)
-
-**Warning**: Variables must be unique, i.e. variables do not have block scope, e.g. the following modifies global `i`:
 
-```python
-for i in range(10):
-    pass
-```
+**Warning**: Variables are treated as global and therefore no variable shadowing.
 
 ## Sample Usage
 `pip install python2verilog`
 
-### Basic usage
-`python3 -m python2verilog.convert generator.py`
-`python3 -m python2verilog.convert generator.py -c "(1, 2, 3, 4)"`
+### Basic Usage
+Create a python file containing a generator function with output type hints, named `<name>.py`.
+
+A sample can be found [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/integration/circle_lines/python.py)
 
-### More Complex Usage
+`python3 -m python2verilog.convert <name>.py`. Use `--help` for additional options, including outputting a testbench.
 
 ## Testing
 
 ### Requirements
 
 Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
 
 Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
 
-Python: `python3 -m pip install -r tests/requirements.txt`
+Python Libraries: `python3 -m pip install -r tests/requirements.txt`
 
 ### Creating New Test
 
-To create a new test case and set up configs, run `python3 tests/frontend/new_generator.py <name>`.
+To create a new test case and set up configs, run `python3 tests/integration/new_test_case.py <test-name>`.
 
 ### Running Tests
 
 To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
-Those files will be stored in `tests/frontend/data/generator/<name>/`.
+Those files will be stored in `tests/integration/data/integration/<test-name>/`.
 
 ## Tested Generations
 
-The outputs of the Python script tests can be found [as a github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
-
-Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md), more up-to-date ones can be found in the artifact.
+Outputs of tests in repo can be found as a [github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/tests-data.zip)
 
 ## For Developers
 
 Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
 
 Architecture is based on [LLVM](https://llvm.org/).
 
 To setup pre-commit, run `pre-commit install`.
 
 ### Epics
 
 - Support arrays
+- Mimic combinational logic with "regular" Python functions
+- Division approximations
 
 ## Docs
 
-- Generate `.html` docs: `bash docs/generate.sh`
-- Live docs: `python3 -m pydoc -b`
+- cd to `docs/`
+- `sphinx-apidoc -o . ../python2verilog/`
+- `make html`
 
 ## Random Planning, Design, and Notes
 
+## What needs to be duplicated in testbenches?
+declare I/O and other signals
+declare DUT
+start clock
+
+loop for each test case
+- start signal
+- while wait for done signal
+  - clock
+  - set start zero
+  - display output
+endloop
+
+
 ### Potential API
 
 ```python
 import python2verilog as p2v
 import ast
 
 func = ast.parse(code).body[0]
 
-ir = p2v.from_python_get_ir(func.body) # returns an ir node for the root of the body
+ir = p2v.from_python_get_ir(func.body)
 
 # Optimization passes
 ir = p2v.optimizations.replace_single_item_cases(ir)
 ir = p2v.optimizations.remove_nesting(ir)
 ir = p2v.optimizations.combine_statements(ir)
-for i in dir(p2v.optimizations): # Do one pass of every optimization
-  item = getattr(pv2.optimizations, i)
-    if callable(item):
-      ir = item(ir)
 
 verilog = p2v.Verilog()
-verilog.from_python_do_setup(func) # module I/O is dependent on Python
-verilog.from_ir_fill_body(ir) # fills the body
+verilog.from_python_do_setup(ir.get_context()) # module I/O is dependent on Python
+verilog.from_ir_fill_body(ir.get_root()) # fills the body
 
 # whether has valid or done signal,
 # whether initialization is always happening or only on start,
 # verilog sim name
 verilog.config(has_valid=True, has_done=True, lazy_start=True, verilog_sim="iverilog")
 
 with open(f"{verilog.get_module_name()}.sv", mode="w") as module:
```

### Comparing `python2verilog-0.0.2/README.md` & `python2verilog-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,114 @@
+![Python Package](https://github.com/worldofkerry/python2verilog/actions/workflows/python-package.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/python2verilog/badge/?version=latest)](https://python2verilog.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/python2verilog)
+
 # Python 2 Verilog
 
 Converts a subset of python generator functions into synthesizable sequential SystemVerilog.
 
 A use case is for drawing shapes on grids (for VGA output), where the user may prototype the algorithm in python and then convert it to verilog for use in an FPGA.
 
-A testbench is also generated and asserted against the Python outputs.
+A testbench can also be generated and asserted against the Python outputs.
 
 Supports Python [Generator functions](https://wiki.python.org/moin/Generators) as well as the following block types:
 
 - `if`
 - `while`
-- `for ... in range(...)` with 1 or 2 args in `range` (quite inefficient)
-
-**Warning**: Variables must be unique, i.e. variables do not have block scope, e.g. the following modifies global `i`:
 
-```python
-for i in range(10):
-    pass
-```
+**Warning**: Variables are treated as global and therefore no variable shadowing.
 
 ## Sample Usage
 `pip install python2verilog`
 
-### Basic usage
-`python3 -m python2verilog.convert generator.py`
-`python3 -m python2verilog.convert generator.py -c "(1, 2, 3, 4)"`
+### Basic Usage
+Create a python file containing a generator function with output type hints, named `<name>.py`.
+
+A sample can be found [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/integration/circle_lines/python.py)
 
-### More Complex Usage
+`python3 -m python2verilog.convert <name>.py`. Use `--help` for additional options, including outputting a testbench.
 
 ## Testing
 
 ### Requirements
 
 Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
 
 Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
 
-Python: `python3 -m pip install -r tests/requirements.txt`
+Python Libraries: `python3 -m pip install -r tests/requirements.txt`
 
 ### Creating New Test
 
-To create a new test case and set up configs, run `python3 tests/frontend/new_generator.py <name>`.
+To create a new test case and set up configs, run `python3 tests/integration/new_test_case.py <test-name>`.
 
 ### Running Tests
 
 To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
-Those files will be stored in `tests/frontend/data/generator/<name>/`.
+Those files will be stored in `tests/integration/data/integration/<test-name>/`.
 
 ## Tested Generations
 
-The outputs of the Python script tests can be found [as a github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
-
-Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md), more up-to-date ones can be found in the artifact.
+Outputs of tests in repo can be found as a [github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/tests-data.zip)
 
 ## For Developers
 
 Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
 
 Architecture is based on [LLVM](https://llvm.org/).
 
 To setup pre-commit, run `pre-commit install`.
 
 ### Epics
 
 - Support arrays
+- Mimic combinational logic with "regular" Python functions
+- Division approximations
 
 ## Docs
 
-- Generate `.html` docs: `bash docs/generate.sh`
-- Live docs: `python3 -m pydoc -b`
+- cd to `docs/`
+- `sphinx-apidoc -o . ../python2verilog/`
+- `make html`
 
 ## Random Planning, Design, and Notes
 
+## What needs to be duplicated in testbenches?
+declare I/O and other signals
+declare DUT
+start clock
+
+loop for each test case
+- start signal
+- while wait for done signal
+  - clock
+  - set start zero
+  - display output
+endloop
+
+
 ### Potential API
 
 ```python
 import python2verilog as p2v
 import ast
 
 func = ast.parse(code).body[0]
 
-ir = p2v.from_python_get_ir(func.body) # returns an ir node for the root of the body
+ir = p2v.from_python_get_ir(func.body)
 
 # Optimization passes
 ir = p2v.optimizations.replace_single_item_cases(ir)
 ir = p2v.optimizations.remove_nesting(ir)
 ir = p2v.optimizations.combine_statements(ir)
-for i in dir(p2v.optimizations): # Do one pass of every optimization
-  item = getattr(pv2.optimizations, i)
-    if callable(item):
-      ir = item(ir)
 
 verilog = p2v.Verilog()
-verilog.from_python_do_setup(func) # module I/O is dependent on Python
-verilog.from_ir_fill_body(ir) # fills the body
+verilog.from_python_do_setup(ir.get_context()) # module I/O is dependent on Python
+verilog.from_ir_fill_body(ir.get_root()) # fills the body
 
 # whether has valid or done signal,
 # whether initialization is always happening or only on start,
 # verilog sim name
 verilog.config(has_valid=True, has_done=True, lazy_start=True, verilog_sim="iverilog")
 
 with open(f"{verilog.get_module_name()}.sv", mode="w") as module:
```

### Comparing `python2verilog-0.0.2/python2verilog/backend/codegen.py` & `python2verilog-0.0.3/python2verilog/backend/verilog.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,385 +1,573 @@
 """Verilog Abstract Syntax Tree Components"""
 
+from __future__ import annotations
 import warnings
 import ast
+from typing import Optional
 
-from ..frontend.utils import Lines, Indent
-from .utils import assert_list_elements
-from .. import backend as irast
-
-
-def create_module_from_python(func: ast.FunctionDef):
-    """
-    Creates a module wrapper from python AST,
-    e.g. the I/O (from Python), clock, valid and done signals
-    """
-    inputs = []
-    for var in func.args.args:
-        inputs.append(var.arg)
-    outputs = []
-    assert isinstance(func.returns, ast.Subscript)
-    assert isinstance(func.returns.slice, ast.Tuple)
-    for i in range(len((func.returns.slice.elts))):
-        outputs.append(f"_out{str(i)}")
-    # TODO: make these extras optional
-    return Module(func.name, inputs, outputs)
+from ..utils.string import Lines, Indent
+from ..utils.assertions import assert_list_elements
+from .. import ir
 
 
-class Verilog:
+class Expression:
     """
-    Code Generation for Verilog
+    Verilog expression, e.g.
+    a + b
+    Currently just a string
     """
 
-    def __init__(self):
-        # TODO: throw errors if user tries to generate verilog beforeconfig
-        self.root = None
-        self.global_vars = None
-        self.module = None
-        self.always = None
-        self.python_func = None
+    def __init__(self, expr: str):
+        assert isinstance(expr, str)
+        self.expr = expr
 
-    def build_tree(self, node: irast.Statement):
+    def to_string(self):
         """
-        Builds the Verilog AST
+        To Verilog
         """
-        if not node:
-            return Statement("")
-        if isinstance(node, irast.Case):
-            case_items = []
-            for item in node.case_items:
-                case_items.append(self.build_tree(item))
-            return Case(self.build_tree(node.condition), case_items)
-        if isinstance(node, irast.CaseItem):
-            case_items = []
-            for item in node.statements:
-                case_items.append(self.build_tree(item))
-            return CaseItem(self.build_tree(node.condition), case_items)
-        if isinstance(node, irast.Expression):
-            return Expression(node.to_string())
-        return Statement(node.to_string().replace("\n", " "))
+        return self.expr
+
+
+class AtPosedge(Expression):
+    """
+    @(posedge <condition>)
+    """
+
+    def __init__(self, condition: Expression):
+        assert isinstance(condition, Expression)
+        self.condition = condition
+        super().__init__(f"@(posedge {condition.to_string()})")
+
+
+class AtNegedge(Expression):
+    """
+    @(negedge <condition>)
+    """
+
+    def __init__(self, condition: Expression):
+        assert isinstance(condition, Expression)
+        self.condition = condition
+        super().__init__(f"@(negedge {condition.to_string()})")
+
 
-    def from_ir(self, root: irast.Statement, global_vars: dict[str, str]):
+class Statement:
+    """
+    Represents a statement in verilog (i.e. a line or a block)
+    If used directly, it is treated as a string literal
+    """
+
+    def __init__(self, literal: str = "", comment: str = ""):
+        self.literal = literal
+        self.comment = comment
+
+    def to_lines(self):
         """
-        Builds tree from IR
+        To Verilog
         """
-        root.append_end_statements([irast.NonBlockingSubsitution("_done", "1")])
-        self.root = self.build_tree(root)
-        self.global_vars = global_vars
-        return self
+        if self.literal:
+            return Lines(
+                self.literal + self.get_inline_comment()[1:]
+            )  # Removes leading space
+        return Lines(self.get_inline_comment()[1:])
 
-    def get_module(self):
+    def to_string(self):
         """
-        Get Verilog module
+        To Verilog
         """
+        return self.to_lines().to_string()
 
-        def get_init_lines(global_vars: dict[str, str]):
-            """
-            if (_start) begin
-                <var> = <value>;
-                ...
-            end else begin
-            ...
-            end
-            """
-            start_lines, end_lines = Lines(), Lines()
-            start_lines += "if (_start) begin"
-            start_lines += Indent(1) + "_done <= 0;"
-            for var in global_vars:
-                start_lines += Indent(1) + f"{var} <= {global_vars[var]};"
-            start_lines += "end else begin"
-            end_lines += "end"
-            return (start_lines, end_lines)
-
-        module_lines = self.module.to_lines()
-        always_blk_lines = self.always.to_lines()
-        decl_lines = (
-            Lines([f"reg signed [31:0] {v};" for v in self.global_vars]),
-            Lines(),
-        )
-        init_lines = get_init_lines(self.global_vars)
-        stmt_lines = (self.root.to_lines(), Lines())
-
-        decl_and_always_blk_lines = (
-            decl_lines[0].concat(always_blk_lines[0]),
-            decl_lines[1].concat(always_blk_lines[1]),
-        )
-
-        return Lines.nestify(
-            [
-                module_lines,
-                decl_and_always_blk_lines,
-                init_lines,
-                stmt_lines,
-            ]
-        )
+    def get_inline_comment(self):
+        """
+        // <comment>
+        """
+        if self.comment != "":
+            return f" // {self.comment}"
+        return ""
 
-    def setup_from_python(self, func: ast.FunctionDef):
+    def get_blocked_comment(self):
         """
-        Setups up module, always block, declarations, etc from Python AST
+        // <comment>
+        ...
+        // <comment>
+        Separated by newlines
         """
-        assert isinstance(func, ast.FunctionDef)
-        self.module = create_module_from_python(func)
-        self.always = Always("_clock", "_valid")
-        self.python_func = func
-        return self
+        actual_lines = self.comment.split("\n")
+        lines = Lines()
+        for line in actual_lines:
+            lines += f"// {line}"
+        return lines
 
-    def get_testbench(self, test_case: tuple):
+    def append_end_statements(self, _: list[Statement]):
         """
-        Creates a test bench for a test case
-        TODO: convert output to lines
+        Append end statements
         """
-        func = self.python_func
-        func_name = func.name
+        raise NotImplementedError("Statements cannot be appended to")
 
-        text = f"module {func_name}"
-
-        text += """_tb;
-    // Inputs
-    reg _clock;
-    reg _start;
-    """  # TODO: use the NAMED_FUNCTION constant instead of generator
-        for idx, val in enumerate(func.args.args):
-            text += f"  reg signed [31:0] {val.arg};\n"
-        text += "\n  // Outputs\n"
-        for idx in range(len(func.returns.slice.elts)):
-            text += f"  wire signed [31:0] _out{idx};\n"
-
-        text += """
-    wire _done;
-    wire _valid;
-
-    // Instantiate the module under test
-    """
-        text += func_name
-
-        text += """ dut (
-    ._clock(_clock),
-    ._start(_start),
-    """
-        for idx, val in enumerate(func.args.args):
-            text += f"    .{val.arg}({val.arg}),\n"
-        for idx in range(len(func.returns.slice.elts)):
-            text += f"    ._out{idx}(_out{idx}),\n"
-        text += """
-    ._done(_done),
-    ._valid(_valid)
-    );
 
-    // Clock generation
-    always #5 _clock = !_clock;
+class AtPosedgeStatement(Statement):
+    """
+    @(posedge <condition>);
+    """
 
-    // Stimulus
-    initial begin
-    // Initialize inputs
-    _start = 0;
+    def __init__(self, condition: Expression, *args, **kwargs):
+        assert isinstance(condition, Expression)
+        super().__init__(f"{AtPosedge(condition).to_string()};", *args, **kwargs)
+
+
+class AtNegedgeStatement(Statement):
+    """
+    @(negedge <condition>);
     """
 
-        for idx, val in enumerate(func.args.args):
-            text += f"    {val.arg} = {test_case[idx]};\n"
-        text += """
-    _clock = 0;
+    def __init__(self, condition: Expression, *args, **kwargs):
+        assert isinstance(condition, Expression)
+        super().__init__(f"{AtNegedge(condition).to_string()};", *args, **kwargs)
+
 
-    // Wait for a few clock cycles
-    #10;
+class Verilog:
+    """
+    Code Generation for Verilog
+    """
 
-    // Start the drawing process
-    @(posedge _clock);
-    _start = 1;
-    @(posedge _clock);
+    @staticmethod
+    def __create_module_from_python(root: Statement, context: ir.Context):
+        """
+        Creates a module wrapper from the context
+        e.g. the I/O (from Python), clock, valid and done signals
+        """
+        assert isinstance(root, Statement)
+        assert isinstance(context, ir.Context)
+        inputs = []
+        for var in context.input_vars:
+            inputs.append(var)
+        outputs = []
+        for i in range(len((context.output_vars))):
+            outputs.append(f"_out{str(i)}")
+        # TODO: make these extras optional
+        always = PosedgeSyncAlways(
+            Expression("_clock"),
+            valid="_valid",
+            body=[Verilog.__get_init(root, context.global_vars)],
+        )
+        return Module(context.name, inputs, outputs, body=[always])
+
+    def __init__(
+        self,
+        root: Optional[ir.Statement] = None,
+        context: Optional[ir.Context] = None,
+    ):
+        # TODO: throw errors if user tries to generate verilog beforeconfig
+        self.module: Optional[Module] = None
+        self.context: Optional[ir.Context] = None
+        if root is not None and context is not None:
+            self.from_ir(root, context)
 
-    // Wait for the drawing to complete
-    while (!_done) begin
-    @(posedge _clock);
-    _start = 0;
-    // Display the outputs for every cycle after start
-    $display(\"%0d, """  # TODO: use NAMED_FUNCTION instead of "generator dut"
+    @staticmethod
+    def build_tree_stmt(node: ir.Statement) -> Statement:
+        """
+        Builds the Verilog AST
+        """
+        assert isinstance(node, (ir.Statement, ir.CaseItem))
+        if not node:
+            return Statement("")
+        if isinstance(node, ir.Case):
+            return Verilog.build_tree_case(node)
+        if isinstance(node, ir.IfElse):
+            then_body = []
+            for stmt in node.then_body:
+                then_body.append(Verilog.build_tree_stmt(stmt))
+            else_body = []
+            for stmt in node.else_body:
+                else_body.append(Verilog.build_tree_stmt(stmt))
+            return IfElse(Verilog.build_tree_expr(node.condition), then_body, else_body)
+        if isinstance(node, ir.Statement):
+            return Statement(node.to_string().replace("\n", " "))
+        raise NotImplementedError(f"Unexpected type {type(node)}")
+
+    @staticmethod
+    def build_tree_expr(node: ir.Expression) -> Expression:
+        """
+        Handles expressions
+        """
+        assert isinstance(node, ir.Expression)
+        return Expression(node.to_string())
+
+    @staticmethod
+    def build_tree_case(node: ir.Case) -> Case:
+        """
+        Handles case statements
+        """
+        assert isinstance(node, ir.Case)
+        case_items = []
+        for item in node.case_items:
+            case_items.append(Verilog.build_tree_caseitem(item))
+        return Case(Verilog.build_tree_expr(node.condition), case_items)
+
+    @staticmethod
+    def build_tree_caseitem(node: ir.CaseItem) -> CaseItem:
+        """
+        Handles case item
+        """
+        case_items = []
+        for item in node.statements:
+            case_items.append(Verilog.build_tree_stmt(item))
+        return CaseItem(Verilog.build_tree_expr(node.condition), case_items)
 
-        text += "%0d, " * (len(func.returns.slice.elts) - 1)
-        text += """%0d\", _valid"""
+    def from_ir(self, root: ir.Statement, context: ir.Context):
+        """
+        Builds tree from IR
+        """
+        assert isinstance(root, ir.Statement)
+        assert isinstance(context, ir.Context)
+        root.append_end_statements(
+            [ir.NonBlockingSubsitution(ir.Var("_done"), ir.Int(1))]
+        )
+        self.context = context
+        self.module = Verilog.__create_module_from_python(
+            Verilog.build_tree_stmt(root), context
+        )
+        return self
 
-        for idx in range(len(func.returns.slice.elts)):
-            text += f", _out{idx}"
+    @staticmethod
+    def __get_init(root: Statement, global_vars: dict[str, str]):
+        """
+        if (_start) begin
+            <var> = <value>;
+            ...
+        end else begin
+        ...
+        end
+        """
+        then_body: list[Statement] = [NonBlockingSubsitution("_done", "0")]
+        then_body += [
+            NonBlockingSubsitution(key, str(val)) for key, val in global_vars.items()
+        ]
+        block = IfElse(
+            Expression("_start"),
+            then_body,
+            [root],
+        )
+        return block
 
-        text += ");\n"
+    def get_module(self):
+        """
+        Get Verilog module
+        """
+        decls = [
+            Declaration(v, is_reg=True, is_signed=True)
+            for v in self.context.global_vars
+        ]
+        self.module.body = decls + self.module.body
+        return self.module.to_lines()
 
-        text += """
-    end
+    def get_testbench(self, test_cases: list[tuple[str]]):
+        """
+        Creates testbench with multiple test cases using the _done signal
+        """
 
-    // Finish simulation
-    $finish;
-    end
+        def make_display_stmt():
+            """
+            Creates a display statement for valid + outputs
 
-    endmodule
+            $display("%0d, ...", _valid, ...);
+            """
+            string = '$display("%0d, '
+            string += "%0d, " * (len(self.context.output_vars) - 1)
+            string += '%0d", _valid'
+            for var in self.context.output_vars:
+                string += f", {var}"
+            string += ");"
+            return Statement(literal=string)
+
+        assert self.context is not None
+        decl: list[Declaration] = []
+        decl.append(Declaration("_clock", size=1, is_reg=True))
+        decl.append(Declaration("_start", size=1, is_reg=True))
+        decl += [
+            Declaration(var, is_signed=True, is_reg=True)
+            for var in self.context.input_vars
+        ]
+        decl += [Declaration(var, is_signed=True) for var in self.context.output_vars]
+
+        decl.append(Declaration("_done", size=1))
+        decl.append(Declaration("_valid", size=1))
+
+        ports = {
+            decl.name: decl.name for decl in decl
+        }  # Caution: expects decl to only contain declarations
+
+        setups: list[Statement] = list(decl)
+        setups.append(Instantiation(self.context.name, "DUT", ports))
+
+        setups.append(Statement(literal="always #5 _clock = !_clock;"))
+
+        initial_body: list[Statement | While] = []  # TODO: replace with Sequence
+        initial_body.append(BlockingSubsitution("_clock", "0"))
+        initial_body.append(BlockingSubsitution("_start", "0"))
+        initial_body.append(AtNegedgeStatement(Expression("_clock")))
+        initial_body.append(Statement())
+
+        for i, test_case in enumerate(test_cases):
+            # setup for new test case
+            initial_body.append(Statement(comment=f"Test case {i}: {str(test_case)}"))
+            for i, var in enumerate(self.context.input_vars):
+                initial_body.append(BlockingSubsitution(var, str(test_case[i])))
+            initial_body.append(BlockingSubsitution("_start", "1"))
+
+            initial_body.append(AtNegedgeStatement(Expression("_clock")))
+
+            # wait for done signal
+            while_body: list[Statement] = []
+            while_body.append(BlockingSubsitution("_start", "0"))
+            while_body.append(make_display_stmt())
+            while_body.append(AtNegedgeStatement(Expression("_clock")))
+
+            initial_body.append(While(condition=Expression("!_done"), body=while_body))
+            initial_body.append(make_display_stmt())
+            initial_body.append(Statement())
+
+        initial_body.append(Statement(literal="$finish;"))
+
+        initial_loop = Initial(body=initial_body)
+
+        if self.context:
+            module = Module(
+                f"{self.context.name}_tb",
+                [],
+                [],
+                body=setups + [initial_loop],
+                add_default_ports=False,
+            )
+            return module
+        raise RuntimeError("Needs the context")
+
+
+class Instantiation(Statement):
     """
-        return text
+    Instantiationo f Verilog module.
+    <module-name> <given-name> (...);
+    """
+
+    def __init__(
+        self,
+        module_name: str,
+        given_name: str,
+        port_connections: dict[str, str],
+        *args,
+        **kwargs,
+    ):
+        """
+        port_connections[port_name] = signal_name, i.e. `.port_name(signal_name)`
+        """
+        assert isinstance(given_name, str)
+        assert isinstance(module_name, str)
+        for key, val in port_connections.items():
+            assert isinstance(key, str)
+            assert isinstance(val, str)
+        self.given_name = given_name
+        self.module_name = module_name
+        self.port_connections = port_connections
+        super().__init__(*args, **kwargs)
+
+    def to_lines(self):
+        """
+        To Verilog
+        """
+        lines = Lines()
+        lines += f"{self.module_name} {self.given_name} ("
+        for key, val in self.port_connections.items():
+            lines += Indent(1) + f".{key}({val}),"
+        lines[-1] = lines[-1][:-1]  # Remove last comma
+        lines += Indent(1) + ");"
+        return lines
 
 
 class Module:
     """
     module name(...); endmodule
     """
 
-    def __init__(self, name: str, inputs: list[str], outputs: list[str]):
+    def __init__(
+        self,
+        name: str,
+        inputs: list[str],
+        outputs: list[str],
+        body: Optional[list[Statement]] = None,
+        add_default_ports=True,
+    ):
         self.name = name  # TODO: assert invalid names
 
         input_lines = Lines()
         for inputt in inputs:
             assert isinstance(inputt, str)
             input_lines += f"input wire [31:0] {inputt}"
-        input_lines += "input wire _start"
-        input_lines += "input wire _clock"
+        if add_default_ports:
+            input_lines += "input wire _start"
+            input_lines += "input wire _clock"
         self.input = input_lines
 
         output_lines = Lines()
         for output in outputs:
             assert isinstance(output, str)
             output_lines += f"output reg [31:0] {output}"
-        output_lines += "output reg _done"
-        output_lines += "output reg _valid"
+        if add_default_ports:
+            output_lines += "output reg _done"
+            output_lines += "output reg _valid"
         self.output = output_lines
 
+        if body:
+            for stmt in body:
+                assert isinstance(stmt, Statement), f"got {type(stmt)} instead"
+            self.body = body
+        else:
+            self.body = []
+
     def to_lines(self):
         """
         To Verilog
         """
         lines = Lines()
-        lines += f"module {self.name}("
+        lines += f"module {self.name} ("
         for line in self.input:
             lines += Indent(1) + line + ","
         for line in self.output:
             lines += Indent(1) + line + ","
-        lines[-1] = lines[-1][0:-1]  # removes last comma
+        if len(lines) > 1:  # This means there are ports
+            lines[-1] = lines[-1][0:-1]  # removes last comma
         lines += ");"
-        return (lines, Lines("endmodule"))
+        for stmt in self.body:
+            if stmt.to_lines() is None:
+                warnings.warn(type(stmt))
+            lines.concat(stmt.to_lines(), 1)
+        lines += "endmodule"
+        return lines
 
 
-class Always:
+class Initial(Statement):
     """
-    always @(posedge <clock>) begin
-        <valid> = 0;
+    initial begin
+        ...
     end
     """
 
-    def __init__(self, clock: str, valid: str = ""):
-        assert isinstance(clock, str)
-        if valid != "":
-            valid = NonBlockingSubsitution(valid, "0")
-        self.clock = clock
-        self.valid = valid
+    def __init__(self, *args, body: Optional[list[Statement]] = None, **kwargs):
+        if body:
+            assert_list_elements(body, Statement)
+        self.body = body
+        super().__init__(*args, **kwargs)
 
     def to_lines(self):
-        """
-        To Verilog
-        """
-        lines = Lines(f"always @(posedge {self.clock}) begin")
-        if self.valid != "":
-            lines.concat(self.valid.to_lines())
-        return (
-            lines,
-            Lines(["end"]),
-        )
+        lines = Lines("initial begin")
+        for stmt in self.body:
+            lines.concat(stmt.to_lines(), 1)
+        lines += "end"
+        return lines
 
 
-class Expression:
+class Always(Statement):
     """
-    Verilog expression, e.g.
-    a + b
-    Currently just a string
+    always () begin
+        ...
+    end
     """
 
-    def __init__(self, string: str):
-        self.string = string
+    def __init__(
+        self,
+        trigger: Expression,
+        *args,
+        body: Optional[list[Statement]] = None,
+        valid: Optional[str] = None,
+        **kwargs,
+    ):
+        assert isinstance(trigger, Expression)
+        self.trigger = trigger
+        if valid:
+            self.valid: Optional[NonBlockingSubsitution] = NonBlockingSubsitution(
+                valid, "0"
+            )
+        else:
+            self.valid = None
+        if body:
+            for stmt in body:
+                assert isinstance(stmt, Statement)
+            self.body = body
+        else:
+            self.body = []
+        super().__init__(*args, **kwargs)
 
-    def to_string(self):
+    def to_lines(self):
         """
         To Verilog
         """
-        return self.string
+        lines = Lines(f"always {self.trigger.to_string()} begin")
+        if self.valid:
+            lines.concat(self.valid.to_lines(), 1)
+        lines.concat(NonBlockingSubsitution("_done", "0").to_lines(), 1)
+        for stmt in self.body:
+            lines.concat(stmt.to_lines(), 1)
+        lines += "end"
+        return lines
 
 
-class Statement:
+class PosedgeSyncAlways(Always):
     """
-    Represents a statement in verilog (i.e. a line or a block)
-    If used directly, it is treated as a string literal
+    always @(posedge <clock>) begin
+        <valid> = 0;
+    end
     """
 
-    def __init__(self, literal: str = None):
-        self.literal = literal
-
-    def to_lines(self):
-        """
-        To Verilog
-        """
-        return Lines(self.literal)
-
-    def to_string(self):
-        """
-        To Verilog
-        """
-        return self.to_lines().to_string()
-
-    # def append_end_statements(self, statements: list):
-    #     warnings.warn("append_end_statements on base class")
-    #     self.literal += str(statements)
+    def __init__(self, clock: Expression, *args, **kwargs):
+        assert isinstance(clock, Expression)
+        self.clock = clock
+        super().__init__(AtPosedge(clock), *args, **kwargs)
 
 
 class Subsitution(Statement):
     """
     Interface for
     <lvalue> <blocking or nonblocking> <rvalue>
     """
 
-    def __init__(self, lvalue: str, rvalue: str, *args, **kwargs):
-        assert isinstance(rvalue, str)  # TODO: should eventually take an expression
+    def __init__(self, lvalue: str, rvalue: str, oper: str, *args, **kwargs):
+        assert isinstance(
+            rvalue, str
+        ), f"got {type(rvalue)} instead"  # TODO: should eventually take an expression
         assert isinstance(lvalue, str)
         self.lvalue = lvalue
         self.rvalue = rvalue
-        self.type = None
-        self.appended = []
+        self.oper = oper
         super().__init__(*args, **kwargs)
 
     def to_lines(self):
         """
         Converts to Verilog
         """
-        assert isinstance(self.type, str), "Subclasses need to set self.type"
-        itself = f"{self.lvalue} {self.type} {self.rvalue};"
+        assert isinstance(self.oper, str), "Subclasses need to set self.type"
+        itself = f"{self.lvalue} {self.oper} {self.rvalue};"
         lines = Lines(itself)
-        if self.appended:
-            for stmt in self.appended:
-                lines.concat(stmt.to_lines())
         return lines
 
-    def append_end_statements(self, statements: list[Statement]):
-        """
-        Appends to last block of code
-        """
-        self.appended = self.appended + assert_list_elements(statements, Statement)
-        return self
-
 
 class NonBlockingSubsitution(Subsitution):
     """
     <lvalue> <= <rvalue>
     """
 
     def __init__(self, lvalue: str, rvalue: str, *args, **kwargs):
-        super().__init__(lvalue, rvalue, *args, **kwargs)
-        self.type = "<="
+        super().__init__(lvalue, rvalue, "<=", *args, **kwargs)
 
 
 class BlockingSubsitution(Subsitution):
     """
     <lvalue> = <rvalue>
     """
 
     def __init__(self, lvalue: str, rvalue: str, *args, **kwargs):
-        super().__init__(lvalue, rvalue, *args, *kwargs)
-        self.type = "="
+        super().__init__(lvalue, rvalue, "=", *args, *kwargs)
 
 
 class Declaration(Statement):
     """
     <reg or wire> <modifiers> <[size-1:0]> <name>;
     """
 
@@ -405,15 +593,16 @@
         string = ""
         if self.is_reg:
             string += "reg"
         else:
             string += "wire"
         if self.is_signed:
             string += " signed"
-        string += f" [{self.size-1}:0]"
+        if self.size > 1:
+            string += f" [{self.size-1}:0]"
         string += f" {self.name}"
         string += ";"
         return Lines(string)
 
 
 class CaseItem:
     """
@@ -517,14 +706,15 @@
         condition: Expression,
         then_body: list[Statement],
         else_body: list[Statement],
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
+        assert isinstance(condition, Expression)
         self.condition = condition
         self.then_body = assert_list_elements(then_body, Statement)
         self.else_body = assert_list_elements(else_body, Statement)
 
     def to_lines(self):
         lines = Lines()
         lines += f"if ({self.condition.to_string()}) begin"
@@ -545,30 +735,35 @@
         # if len(statements) > 1:
         #     warnings.warn(statements[1].to_string())
         self.then_body[-1].append_end_statements(statements)
         self.else_body[-1].append_end_statements(statements)
         return self
 
 
-class While(Case):
+class While(Statement):
     """
-    Abstract While wrapper
-    Case (WHILE)
-        0: if (!<conditional>)
-                <continue>
-            else
-                <loop body / go state 1>
-        1: <loop body>
+    Unsynthesizable While
+    while (<condition>) begin
+        ...
+    end
     """
 
-    def append_end_statements(self, statements: list[Statement]):
-        """
-        While statements have a special case structure,
-        where their first case always contains an if statement
-        """
-        statements = assert_list_elements(statements, Statement)
-        assert isinstance(self.case_items[0], CaseItem)
-        assert isinstance(self.case_items[0].statements[0], IfElse)
-        self.case_items[0].statements[0].then_body = (
-            self.case_items[0].statements[0].then_body + statements
-        )
-        return self
+    def __init__(
+        self,
+        *args,
+        condition: Expression,
+        body: Optional[list[Statement]] = None,
+        **kwargs,
+    ):
+        assert isinstance(condition, Expression)
+        self.condition = condition
+        if body:
+            assert_list_elements(body, Statement)
+        self.body = body
+        super().__init__(*args, **kwargs)
+
+    def to_lines(self):
+        lines = Lines(f"while ({self.condition.to_string()}) begin")
+        for stmt in self.body:
+            lines.concat(stmt.to_lines(), 1)
+        lines += "end"
+        return lines
```

### Comparing `python2verilog-0.0.2/python2verilog/backend/statements.py` & `python2verilog-0.0.3/python2verilog/ir/statements.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-"""Verilog Abstract Syntax Tree Components"""
+"""An Intermediate Representation for HDL based on Verilog"""
 
+from __future__ import annotations
 import warnings
 import inspect
+from typing import Optional
 
-from ..frontend.utils import Lines
-from .utils import assert_list_elements
-from .expressions import Expression
+from python2verilog.ir.expressions import Expression
+
+from ..utils.string import Lines
+from ..utils.assertions import assert_list_elements
 
 
 class Statement:
     """
-    Represents a statement in verilog (i.e. a line or a block)
+    Represents a statements (i.e. a line or a block)
     If used directly, it is treated as a string literal
     """
 
-    def __init__(self, literal: str = None):
+    def __init__(self, literal: Optional[str] = None):
         self.literal = literal
 
     def to_lines(self):
         """
-        To Verilog
+        To Lines
         """
         return Lines(self.literal)
 
     def to_string(self):
         """
-        To Verilog
+        To String
         """
         return self.to_lines().to_string()
 
-    # def append_end_statements(self, statements: list):
-    #     warnings.warn("append_end_statements on base class")
-    #     self.literal += str(statements)
+    def __repr__(self):
+        return self.to_string()
+
+    def append_end_statements(self, _: list[Statement]):
+        """
+        Abstract
+        """
+        raise NotImplementedError("cannot append to statement")
 
 
 def is_valid_append_end_statements(stmt: Statement, statements: list[Statement]):
     """
     Checks if stmt encapsulates other Statements or not
     If it does, it handles the append, otherwise returns false
     # TODO: there should be a subclass/interface for ones that do encapsulate
@@ -48,66 +56,65 @@
 
 class Subsitution(Statement):
     """
     Interface for
     <lvalue> <blocking or nonblocking> <rvalue>
     """
 
-    def __init__(self, lvalue: str, rvalue: str, *args, **kwargs):
-        assert isinstance(rvalue, str)  # TODO: should eventually take an expression
-        assert isinstance(lvalue, str)
+    def __init__(
+        self, lvalue: Expression, rvalue: Expression, oper: str, *args, **kwargs
+    ):
+        assert isinstance(lvalue, Expression)
+        assert isinstance(rvalue, Expression)
         self.lvalue = lvalue
         self.rvalue = rvalue
-        self.type = None
-        self.appended = []
+        self.oper = oper
         super().__init__(*args, **kwargs)
 
     def to_lines(self):
         """
-        Converts to Verilog
+        To Lines
         """
-        assert isinstance(self.type, str), "Subclasses need to set self.type"
-        itself = f"{self.lvalue} {self.type} {self.rvalue};"
+        itself = f"{self.lvalue.to_string()} {self.oper} {self.rvalue.to_string()};"
         lines = Lines(itself)
-        if self.appended:
-            for stmt in self.appended:
-                lines.concat(stmt.to_lines())
         return lines
 
-    def append_end_statements(self, statements: list[Statement]):
-        """
-        Appends to last block of code
-        """
-        raise DeprecationWarning()
-        warnings.warn(
-            "want to remove "
-            + str(inspect.getouterframes(inspect.currentframe(), 2)[1][3])
-        )
-        self.appended = self.appended + assert_list_elements(statements, Statement)
-        return self
-
 
 class NonBlockingSubsitution(Subsitution):
     """
     <lvalue> <= <rvalue>
     """
 
-    def __init__(self, lvalue: str, rvalue: str, *args, **kwargs):
-        super().__init__(lvalue, rvalue, *args, **kwargs)
-        self.type = "<="
+    def __init__(self, lvalue: Expression, rvalue: Expression, *args, **kwargs):
+        super().__init__(lvalue, rvalue, "<=", *args, **kwargs)
 
 
 class BlockingSubsitution(Subsitution):
     """
     <lvalue> = <rvalue>
     """
 
-    def __init__(self, lvalue: str, rvalue: str, *args, **kwargs):
-        super().__init__(lvalue, rvalue, *args, *kwargs)
-        self.type = "="
+    def __init__(self, lvalue: Expression, rvalue: Expression, *args, **kwargs):
+        super().__init__(lvalue, rvalue, "=", *args, *kwargs)
+
+
+class ValidSubsitution(NonBlockingSubsitution):
+    """
+    Special type to indicate this modifies the valid signal
+
+    More than one of these cannot be in the same block / clock cycle,
+    otherwise output values may be overwriting each other
+    """
+
+
+class StateSubsitution(NonBlockingSubsitution):
+    """
+    Special type to indicate this modifies the local-to-case-statement
+    state varaible
+    """
 
 
 class Declaration(Statement):
     """
     <reg or wire> <modifiers> <[size-1:0]> <name>;
     """
 
@@ -141,15 +148,15 @@
         string += f" {self.name}"
         string += ";"
         return Lines(string)
 
 
 class CaseItem:
     """
-    Verilog case item, i.e.
+    case item, i.e.
     <condition>: begin
         <statements>
     end
     """
 
     def __init__(self, condition: Expression, statements: list[Statement]):
         assert isinstance(condition, Expression)
@@ -159,26 +166,26 @@
                 assert isinstance(stmt, Statement), f"unexpected {type(stmt)}"
             self.statements = statements
         else:
             self.statements = []
 
     def to_lines(self):
         """
-        To Verilog lines
+        To Lines
         """
         lines = Lines()
         lines += f"{self.condition.to_string()}: begin"
         for stmt in self.statements:
             lines.concat(stmt.to_lines(), indent=1)
         lines += "end"
         return lines
 
     def to_string(self):
         """
-        To Verilog
+        To String
         """
         return self.to_lines().to_string()
 
     def append_end_statements(self, statements: list[Statement]):
         """
         Append statements to case item
         """
@@ -187,15 +194,14 @@
                 statements, Statement
             )
         return self
 
 
 class Case(Statement):
     """
-    Verilog case statement with various cases
     case (<expression>)
         <items[0]>
         ...
         <items[n]>
     endcase
     """
 
@@ -210,15 +216,15 @@
             self.case_items = case_items
         else:
             self.case_items = []
         super().__init__(*args, **kwargs)
 
     def to_lines(self):
         """
-        To Verilog Lines
+        To Lines
         """
         lines = Lines()
         lines += f"case ({self.condition.to_string()})"
         for item in self.case_items:
             lines.concat(item.to_lines(), indent=1)
         lines += "endcase"
         return lines
@@ -231,26 +237,27 @@
             assert_list_elements(statements, Statement)
         )
         return self
 
 
 class IfElse(Statement):
     """
-    Verilog if else
+    If Else
     """
 
     def __init__(
         self,
         condition: Expression,
         then_body: list[Statement],
         else_body: list[Statement],
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
+        assert isinstance(condition, Expression)
         self.condition = condition
         self.then_body = assert_list_elements(then_body, Statement)
         self.else_body = assert_list_elements(else_body, Statement)
 
     def to_lines(self):
         lines = Lines()
         lines += f"if ({self.condition.to_string()}) begin"
@@ -273,17 +280,18 @@
         if not is_valid_append_end_statements(self.then_body[-1], statements):
             self.then_body = self.then_body + statements
         if not is_valid_append_end_statements(self.else_body[-1], statements):
             self.else_body = self.else_body + statements
         return self
 
 
-class While(Case):
+class WhileWrapper(Case):
     """
-    Abstract While wrapper
+    A while case statement
+
     Case (WHILE)
         0: if (!<conditional>)
                 <continue>
             else
                 <loop body / go state 1>
         1: <loop body>
     """
@@ -296,7 +304,31 @@
         statements = assert_list_elements(statements, Statement)
         assert isinstance(self.case_items[0], CaseItem)
         assert isinstance(self.case_items[0].statements[0], IfElse)
         self.case_items[0].statements[0].then_body = (
             self.case_items[0].statements[0].then_body + statements
         )
         return self
+
+
+class IfElseWrapper(Case):
+    """
+    A if-else case statement
+
+    case (<state_name>)
+
+        0: IfElse type (condition check)
+
+        1: <then body>
+
+        2: <else body>
+
+    endcase
+    """
+
+    def __init__(
+        self, expression: Expression, case_items: list[CaseItem], *args, **kwargs
+    ):
+        assert len(case_items) == 3
+        assert len(case_items[0].statements) == 1
+        assert isinstance(case_items[0].statements[0], IfElse)
+        super().__init__(expression, case_items, *args, **kwargs)
```

### Comparing `python2verilog-0.0.2/python2verilog/convert.py` & `python2verilog-0.0.3/python2verilog/convert.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,118 @@
 """
-To run the basic conversion as a script
+To run the basic conversion as a CLI script
 """
 
 import argparse
 import os
 import ast
-from .frontend import Generator2Ast
-from .backend.codegen import Verilog
+import warnings
+from .frontend import GeneratorParser
+from .backend.verilog import Verilog
+from .optimizer import optimizer
+
+
+def convert(func: ast.FunctionDef, optimization_level: int):
+    """
+    Wrapper for common Python to Verilog conversion
+    """
+    ir_root, context = GeneratorParser(func).get_results()
+    if optimization_level > 0:
+        ir_root = optimizer.replace_single_case(ir_root)
+        ir_root = optimizer.optimize_if(ir_root)
+        ir_root = optimizer.combine_cases(ir_root)
+    return Verilog(ir_root, context)
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(
+        description=__doc__, formatter_class=argparse.RawTextHelpFormatter
+    )
+
+    parser.add_argument(
+        "input_file",
+        type=str,
+        help="Input file containing a python generator function",
+    )
+
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=str,
+        help="Output file for System Verilog module",
+        default="",
+    )
+
+    TESTBENCH_ARG = parser.add_argument(
+        "-t",
+        "--testbench",
+        type=str,
+        help="Output file for System Verilog testbench",
+        default="",
+    )
+
+    parser.add_argument(
+        "-c",
+        "--test-cases",
+        type=str,
+        help='A list of test cases for testbench. \
+            Required to output testbench. E.g. `-c "[(1, 2, 3, 4)]"`',
+        default="",
+    )
+    parser.add_argument(
+        "-O",
+        "--optimization-level",
+        type=int,
+        help="Optimization level of output, between 0 and 3 inclusive, \
+            \nhigher means more optimized but may be more difficult to reason",
+        default=0,
+    )
+
+    def get_default_tb_filename(stem: str):
+        """
+        Gets default testbench filename
+        """
+        return stem + "_tb.sv"
+
+    args = parser.parse_args()
+    input_file_path = parser.parse_args().input_file
+    input_file_stem = os.path.splitext(input_file_path)[0]
+    if args.output == "":
+        args.output = input_file_stem + ".sv"
+
+    if args.testbench == "":
+        args.testbench = get_default_tb_filename(input_file_stem)
+
+    with open(
+        os.path.abspath(input_file_path), mode="r", encoding="utf8"
+    ) as python_file:
+        python = python_file.read()
+        _locals: dict[str, str] = {}
+        exec(python, None, _locals)  # grab's exec's populated scoped variables
+
+        tree = ast.parse(python)
+        function = tree.body[0]
+        assert isinstance(function, ast.FunctionDef)
+        verilog = convert(function, args.optimization_level)
 
-parser = argparse.ArgumentParser(
-    description=__doc__, formatter_class=argparse.RawTextHelpFormatter
-)
-
-parser.add_argument(
-    "input_file",
-    type=str,
-    help="Input file containing a python generator function",
-)
-
-
-parser.add_argument(
-    "-o",
-    "--output",
-    type=str,
-    help="Output file for System Verilog module",
-    default="",
-)
-
-parser.add_argument(
-    "-t",
-    "--testbench",
-    type=str,
-    help="Output file for System Verilog testbench",
-    default="",
-)
-
-parser.add_argument(
-    "-c",
-    "--test-case",
-    type=str,
-    help='Test case for testbench. Required to output testbench. E.g. `-c "(1, 2, 3, 4)"`',
-    default="",
-)
-
-args = parser.parse_args()
-input_file_path = parser.parse_args().input_file
-input_file_stem = os.path.splitext(input_file_path)[0]
-if args.output == "":
-    args.output = input_file_stem + ".sv"
-
-if args.testbench == "":
-    args.testbench = input_file_stem + "_tb.sv"
-
-with open(os.path.abspath(input_file_path), mode="r", encoding="utf8") as python_file:
-    python = python_file.read()
-    _locals = {}
-    exec(python, None, _locals)  # grab's exec's populated scoped variables
-
-    tree = ast.parse(python)
-    function = tree.body[0]
-    ir_generator = Generator2Ast(function)
-    output = ir_generator.parse_statements(function.body, "")
-    verilog = Verilog()
-    verilog.from_ir(output, ir_generator.global_vars)
-    verilog.setup_from_python(function)
-
-    with open(os.path.abspath(args.output), mode="w+", encoding="utf8") as module_file:
-        module_file.write(verilog.get_module().to_string())
-
-    if args.test_case != "":
         with open(
-            os.path.abspath(args.testbench), mode="w+", encoding="utf8"
-        ) as tb_file:
-            tb_file.write(verilog.get_testbench(ast.literal_eval(args.test_case)))
+            os.path.abspath(args.output), mode="w+", encoding="utf8"
+        ) as module_file:
+            module_file.write(verilog.get_module().to_string())
+
+        if args.test_cases != "":
+            with open(
+                os.path.abspath(args.testbench), mode="w+", encoding="utf8"
+            ) as tb_file:
+                tb_file.write(
+                    verilog.get_testbench(ast.literal_eval(args.test_cases))
+                    .to_lines()
+                    .to_string()
+                )
+        elif args.test_cases == "" and args.testbench != get_default_tb_filename(
+            input_file_stem
+        ):
+            raise argparse.ArgumentError(
+                TESTBENCH_ARG,
+                f"testbench path provided by no test cases provided \
+                    {args.test_cases}, {args.testbench}",
+            )
```

### Comparing `python2verilog-0.0.2/python2verilog/frontend/generator2ast.py` & `python2verilog-0.0.3/python2verilog/frontend/generator_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,200 @@
-"""Parser for Python Generator Functions"""
+"""Parses Python Generator Functions to Intermediate Representation"""
 
 from __future__ import annotations
+import copy
+import warnings
 import ast as pyast
-from .utils import Lines, Indent
-from .. import backend as vast
+from typing import Optional
 
+from .. import ir
+from ..utils.string import Lines, Indent
 
-class Generator2Ast:
+
+class GeneratorParser:
     """
     Parses python generator functions to Verilog AST
     """
 
-    @staticmethod
-    def generate_output_vars(node: pyast.AST, prefix: str):
-        """
-        Generates the yielded variables of the function
+    def __init__(self, python_func: pyast.FunctionDef):
         """
-        assert isinstance(node, pyast.Subscript)
-        assert isinstance(node.slice, pyast.Tuple)
-        return [f"{prefix}_out{str(i)}" for i in range(len(node.slice.elts))]
-
-    def create_unique_name(self):
-        """
-        Generates an id that is unique among all unique global variables
+        Initializes the parser, does quick setup work
         """
-        self.unique_name_counter += 1
-        return f"{self.unique_name_counter}"
+        assert isinstance(python_func, pyast.FunctionDef)
+        self._name = python_func.name
+        self._unique_name_counter = 0
+        self._global_vars: dict[str, str] = {}
+        self._python_func = python_func
+
+        assert python_func.returns is not None, "Write a return type-hint for function"
+        self._output_vars = self.__generate_output_vars(python_func.returns, "")
+        self._input_vars = [var.arg for var in self._python_func.args.args]
+        self._root = self.__parse_statements(list(python_func.body), "")
 
-    def add_global_var(self, initial_value: str, name: str):
-        """
-        Adds global variables
-        """
-        self.global_vars[name] = initial_value
-        return name
+    def __str__(self):
+        return self.generate_verilog().to_string()
 
-    @staticmethod
-    def stringify_always_block():
+    def get_root(self):
         """
-        always @(posedge _clock) begin
-        end
+        Gets the root of the IR tree
         """
-        return (
-            Lines(["always @(posedge _clock) begin", Indent(1) + "_valid <= 0;"]),
-            Lines(["end"]),
-        )
-
-    def __str__(self):
-        return self.generate_verilog().to_string()
+        return copy.deepcopy(self._root)
 
     def generate_verilog(self, indent: int = 0):
         """
         Generates the verilog (does the most work, calls other functions)
         """
         stmt_lines = (
-            self.parse_statements(
-                self.root.body,
+            self.__parse_statements(
+                list(self._python_func.body),
                 prefix="",
-                end_stmts=[vast.NonBlockingSubsitution("_done", "1")],
+                end_stmts=[ir.NonBlockingSubsitution(ir.Var("_done"), ir.Int(1))],
             ).to_lines(),
             Lines(),
         )
-        module_lines = self.stringify_module()
-        decl_lines = self.stringify_declarations(self.global_vars)
-        always_blk_lines = self.stringify_always_block()
+        module_lines = self.__stringify_module()
+        decl_lines = self.__stringify_declarations(self._global_vars)
+        always_blk_lines = self.__stringify_always_block()
         decl_and_always_blk_lines = (
             decl_lines[0].concat(always_blk_lines[0]),
             decl_lines[1].concat(always_blk_lines[1]),
         )  # TODO: there should be a function for this
-        init_lines = self.stringify_initialization(self.global_vars)
+        init_lines = self.__stringify_initialization(self._global_vars)
 
         return Lines.nestify(
             [
                 module_lines,
                 decl_and_always_blk_lines,
                 init_lines,
                 stmt_lines,
             ],
             indent,
         )
 
+    def parse_statements(
+        self,
+        stmts: list[pyast.AST],
+        prefix: str,
+        end_stmts: Optional[list[ir.Statement]] = None,
+        reset_to_zero: bool = False,
+    ):
+        """
+        Parses a list of python statements
+        """
+        return self.__parse_statements(stmts, prefix, end_stmts, reset_to_zero)
+
+    def __parse_statements(
+        self,
+        stmts: list[pyast.AST],
+        prefix: str,
+        end_stmts: Optional[list[ir.Statement]] = None,
+        reset_to_zero: bool = False,
+    ):
+        """
+        Warning: mutates global_vars
+
+        {
+            <statement0>
+            <statement1>
+            ...
+        }
+        """
+        if not end_stmts:
+            end_stmts = []
+        assert end_stmts is not None
+        state_var = self.__add_global_var(
+            str(0), f"{prefix}_STATE{self.__create_unique_name()}"
+        )
+        cases = []
+
+        index = 0
+        for stmt in stmts:
+            body = self.__parse_statement(stmt, prefix=state_var)
+            case_item = ir.CaseItem(ir.Expression(str(index)), body)
+            if (
+                not isinstance(stmt, pyast.For)
+                and not isinstance(stmt, pyast.While)
+                and not isinstance(stmt, pyast.If)
+            ):
+                case_item.append_end_statements(
+                    [
+                        ir.StateSubsitution(
+                            ir.Var(state_var), ir.Add(ir.Var(state_var), ir.Int(1))
+                        )
+                    ]
+                )
+            cases.append(case_item)  # TODO: cases can have multiple statements
+            index += 1
+        if reset_to_zero:
+            end_stmts.append(ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(0)))
+
+        the_case = ir.Case(ir.Expression(state_var), cases)
+        assert end_stmts is not None
+        the_case.append_end_statements(end_stmts)
+
+        return ir.Case(ir.Expression(state_var), cases)
+
+    @staticmethod
+    def __generate_output_vars(node: pyast.AST, prefix: str):
+        """
+        Generates the yielded variables of the function
+        """
+        assert isinstance(node, pyast.Subscript)
+        if isinstance(node.slice, pyast.Tuple):
+            return [f"{prefix}_out{str(i)}" for i in range(len(node.slice.elts))]
+        if isinstance(node.slice, pyast.Name):
+            return [f"{prefix}_out0"]
+        raise NotImplementedError(
+            f"Unexpected function return type hint {type(node.slice)}, {pyast.dump(node.slice)}"
+        )
+
+    def __create_unique_name(self):
+        """
+        Generates an id that is unique among all unique global variables
+        """
+        self._unique_name_counter += 1
+        return f"{self._unique_name_counter}"
+
+    def __add_global_var(self, initial_value: str, name: str):
+        """
+        Adds global variables
+        """
+        self._global_vars[name] = initial_value
+        return name
+
+    def get_context(self):
+        """
+        Gets the context of the Python function
+        """
+        return ir.Context(
+            name=self._name,
+            global_vars=copy.deepcopy(self._global_vars),
+            input_vars=copy.deepcopy(self._input_vars),
+            output_vars=copy.deepcopy(self._output_vars),
+        )
+
+    def get_results(self):
+        """
+        Gets root of IR and Context
+        """
+        return (self.get_root(), self.get_context())
+
+    @staticmethod
+    def __stringify_always_block():
+        """
+        always @(posedge _clock) begin
+        end
+        """
+        return (
+            Lines(["always @(posedge _clock) begin", Indent(1) + "_valid <= 0;"]),
+            Lines(["end"]),
+        )
+
     @staticmethod
-    def stringify_initialization(global_vars: dict[str, str]):
+    def __stringify_initialization(global_vars: dict[str, str]):
         """
         if (_start) begin
             <var> = <value>;
             ...
         end else begin
         ...
         end
@@ -95,311 +205,306 @@
         for var in global_vars:
             start_lines += Indent(1) + f"{var} <= {global_vars[var]};"
         start_lines += "end else begin"
         end_lines += "end"
         return (start_lines, end_lines)
 
     @staticmethod
-    def stringify_declarations(global_vars: dict[str, str]) -> tuple[Lines, Lines]:
+    def __stringify_declarations(global_vars: dict[str, str]) -> tuple[Lines, Lines]:
         """
         reg [31:0] <name>;
         ...
         """
         return (Lines([f"reg signed [31:0] {v};" for v in global_vars]), Lines())
 
-    def stringify_module(self) -> tuple[Lines, Lines]:
+    def __stringify_module(self) -> tuple[Lines, Lines]:
         """
         module <name>(...);
 
         endmodule
         """
         start_lines, end_lines = Lines(), Lines()
-        assert self.name not in {
+        assert self._name not in {
             "default",
             "module",
             "output",
             "function",
         }  # Verilog Reserved Keywords
-        start_lines += f"module {self.name}("
+        start_lines += f"module {self._name}("
         start_lines += Indent(1) + "input wire _clock,"
         start_lines += Indent(1) + "input wire _start,"
-        for var in self.root.args.args:
+        for var in self._python_func.args.args:
             start_lines += Indent(1) + f"input wire signed [31:0] {var.arg},"
-        for var in self.output_vars:
+        for var in self._output_vars:
             start_lines += Indent(1) + f"output reg signed [31:0] {var},"
         start_lines += Indent(1) + "output reg _done,"
         start_lines += Indent(1) + "output reg _valid"
         start_lines += ");"
         end_lines += "endmodule"
         return (start_lines, end_lines)
 
-    def __init__(self, root: pyast.FunctionDef):
-        """
-        Initializes the parser, does quick setup work
-        """
-        assert isinstance(root, pyast.FunctionDef)
-        self.name = root.name
-        self.output_vars = self.generate_output_vars(root.returns, "")
-        self.unique_name_counter = 0
-        self.global_vars: dict[str, str] = {}
-        self.root = root
-
-    def parse_for(self, node: pyast.For, prefix: str = ""):
+    def __parse_for(self, node: pyast.For, prefix: str):
         """
         Creates a conditional while loop from for loop
         """
-        raise NotImplementedError("for")
-
-        def parse_iter(iterator: pyast.AST, node: pyast.AST):
-            assert isinstance(iterator, pyast.Call)
-            assert iterator.func.id == "range"
-
-            # range(x, y) or range(x)
-            if len(iterator.args) == 2:
-                start, end = str(iterator.args[0].value), iterator.args[1].id
-            else:
-                start, end = "0", iterator.args[0].id
-
-            self.add_global_var(
-                start, node.target.id
-            )  # TODO: not require unique range iterator variables
-            return (
-                Lines(
-                    [
-                        f"if ({node.target.id} >= {end}) begin // FOR LOOP START",
-                        Indent(1) + f"{prefix}_STATE = {prefix}_STATE + 1;",
-                        Indent(1) + f"{node.target.id} <= 0;",
-                        "end else begin // FOR LOOP BODY",
-                    ]
-                ),
-                Lines(["end // FOR LOOP END"]),
-            )
+        raise NotImplementedError("for not implemented")
 
-        conditional_lines = parse_iter(node.iter, node)
-        stmt_lines = self.parse_statements(
-            node.body,
-            f"{prefix}_BODY_{self.create_unique_name()}",
-            end_stmts=Lines([f"{node.target.id} <= {node.target.id} + 1;"]),
-            reset_to_zero=True,
-        )
-        return Lines.nestify([conditional_lines, stmt_lines])
-
-    def parse_targets(self, nodes: list[pyast.AST]):
+    def __parse_targets(self, nodes: list[pyast.AST]):
         """
         Warning: only single target on left-hand-side supported
 
         <target0, target1, ...> =
         """
-        buffer = ""
         assert len(nodes) == 1
         node = nodes[0]
-        assert isinstance(node, pyast.Name)
-        if node.id not in self.global_vars:
-            self.add_global_var(0, node.id)
-        buffer += self.parse_expression(node).to_string()
-        return buffer
+        if isinstance(node, pyast.Subscript):
+            assert isinstance(node.value, pyast.Name)
+            if node.value.id not in set(
+                [*self._global_vars, *self._output_vars, *self._input_vars]
+            ):
+                warnings.warn(
+                    str(
+                        set([*self._global_vars, *self._output_vars, *self._input_vars])
+                    )
+                )
+                self.__add_global_var(str(0), node.value.id)
+        elif isinstance(node, pyast.Name):
+            if node.id not in self._global_vars:
+                self.__add_global_var(str(0), node.id)
+        else:
+            raise TypeError(f"Unsupported lvalue type {type(node)} {pyast.dump(node)}")
+        return self.__parse_expression(node)
 
-    def parse_assign(self, node: pyast.Assign):
+    def __parse_assign(self, node: pyast.Assign):
         """
         <target0, target1, ...> = <value>;
         """
-        assign = vast.NonBlockingSubsitution(
-            self.parse_targets(node.targets),
-            self.parse_expression(node.value).to_string(),
+        assign = ir.NonBlockingSubsitution(
+            self.__parse_targets(list(node.targets)),
+            self.__parse_expression(node.value),
         )
         return [assign]
 
-    def parse_statement(self, stmt: pyast.AST, prefix: str = ""):
+    def __parse_statement(self, stmt: pyast.AST, prefix: str):
         """
         <statement> (e.g. assign, for loop, etc., those that do not return a value)
         """
         if isinstance(stmt, pyast.Assign):
-            return self.parse_assign(stmt)
+            return self.__parse_assign(stmt)
         if isinstance(stmt, pyast.For):
-            return self.parse_for(stmt, prefix=prefix)
+            return self.__parse_for(stmt, prefix=prefix)
         if isinstance(stmt, pyast.Expr):
-            return self.parse_statement(stmt.value, prefix=prefix)
+            return self.__parse_statement(stmt.value, prefix=prefix)
         if isinstance(stmt, pyast.Yield):
-            return self.parse_yield(stmt)
+            return self.__parse_yield(stmt)
         if isinstance(stmt, pyast.While):
-            return self.parse_while(stmt, prefix=prefix)
+            return self.__parse_while(stmt, prefix=prefix)
         if isinstance(stmt, pyast.If):
-            return self.parse_if(stmt, prefix=prefix)
+            return self.__parse_ifelse(stmt, prefix=prefix)
+        if isinstance(stmt, pyast.AugAssign):
+            assert isinstance(
+                stmt.target, pyast.Name
+            ), "Error: only supports single target"
+            return [
+                ir.NonBlockingSubsitution(
+                    self.__parse_expression(stmt.target),
+                    self.__parse_expression(
+                        pyast.BinOp(stmt.target, stmt.op, stmt.value)
+                    ),
+                )
+            ]
         raise TypeError(
             "Error: unexpected statement type", type(stmt), pyast.dump(stmt)
         )
 
-    def parse_if(self, stmt: pyast.If, prefix: str = ""):
+    def __parse_ifelse(self, stmt: pyast.If, prefix: str):
         """
         If statement
         """
         assert isinstance(stmt, pyast.If)
-        state_var = self.add_global_var("0", f"{prefix}_IF")
-        conditional_item = vast.CaseItem(
-            vast.Expression("0"),
+        state_var = self.__add_global_var(
+            str(0), f"{prefix}_IFELSE{self.__create_unique_name()}"
+        )
+        conditional_item = ir.CaseItem(
+            ir.Int(0),
             [
-                vast.Statement(f"if ({self.parse_expression(stmt.test).to_string()})"),
-                vast.NonBlockingSubsitution(state_var, "1"),
-                vast.Statement(
-                    "else "
-                    + vast.NonBlockingSubsitution(state_var, "2").to_string().strip()
-                ),  # TODO: cleanup
+                ir.IfElse(
+                    self.__parse_expression(stmt.test),
+                    [ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(1))],
+                    [ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(2))],
+                )
             ],
         )
-        then_item = vast.CaseItem(
-            vast.Expression("1"),
+        then_item = ir.CaseItem(
+            ir.Expression("1"),
             [
-                self.parse_statements(
-                    stmt.body,
-                    f"{state_var}{self.create_unique_name()}",
+                self.__parse_statements(
+                    list(stmt.body),
+                    f"{state_var}",
                     end_stmts=[
-                        vast.NonBlockingSubsitution(
-                            f"{prefix}_STATE", f"{prefix}_STATE + 1"
+                        ir.StateSubsitution(
+                            ir.Var(prefix), ir.Add(ir.Var(prefix), ir.Int(1))
                         ),
-                        vast.NonBlockingSubsitution(state_var, "0"),
+                        ir.StateSubsitution(ir.Var(state_var), ir.Int(0)),
                     ],
                     reset_to_zero=True,
                 )
             ],
         )
-        else_item = vast.CaseItem(
-            vast.Expression("2"),
+        else_item = ir.CaseItem(
+            ir.Expression("2"),
             [
-                self.parse_statements(
-                    stmt.orelse,
-                    f"{state_var}{self.create_unique_name()}",
+                self.__parse_statements(
+                    list(stmt.orelse),
+                    f"{state_var}",
                     end_stmts=[
-                        vast.NonBlockingSubsitution(
-                            f"{prefix}_STATE", f"{prefix}_STATE + 1"
+                        ir.StateSubsitution(
+                            ir.Var(prefix), ir.Add(ir.Var(prefix), ir.Int(1))
                         ),
-                        vast.NonBlockingSubsitution(state_var, "0"),
+                        ir.StateSubsitution(ir.Var(state_var), ir.Int(0)),
                     ],
                     reset_to_zero=True,
                 )
             ],
         )
         return [
-            vast.Case(
-                vast.Expression(f"{state_var}"),
+            ir.IfElseWrapper(
+                ir.Expression(f"{state_var}"),
                 [conditional_item, then_item, else_item],
             )
         ]
 
-    def parse_statements(
-        self,
-        stmts: list[pyast.AST],
-        prefix: str,
-        end_stmts: list[vast.Statement] = None,
-        reset_to_zero: bool = False,
-    ):
-        """
-        Warning: mutates global_vars
-        {
-            <statement0>
-            <statement1>
-            ...
-        }
-        """
-        if not end_stmts:
-            end_stmts = Lines()
-        state_var = self.add_global_var("0", f"{prefix}_STATE")
-        cases = []
-
-        index = 0
-        for stmt in stmts:
-            a_output = self.parse_statement(stmt, prefix=prefix)
-            assert isinstance(a_output, list)
-            body = self.parse_statement(stmt, prefix=prefix)
-            case_item = vast.CaseItem(vast.Expression(str(index)), body)
-            if (
-                not isinstance(stmt, pyast.For)
-                and not isinstance(stmt, pyast.While)
-                and not isinstance(stmt, pyast.If)
-            ):
-                case_item.append_end_statements(
-                    [vast.NonBlockingSubsitution(state_var, f"{state_var} + 1")]
-                )
-            cases.append(case_item)  # TODO: cases can have multiple statements
-            index += 1
-        # end_stmts = [vast.Statement(stmt) for stmt in end_stmts]
-        for stmt in end_stmts:
-            assert isinstance(stmt, vast.Statement)
-        if reset_to_zero:
-            end_stmts.append(vast.NonBlockingSubsitution(state_var, "0"))
-
-        the_case = vast.Case(vast.Expression(state_var), cases)
-        the_case.append_end_statements(end_stmts)
-
-        return vast.Case(vast.Expression(state_var), cases)
-
-    def parse_yield(self, node: pyast.Yield):
+    def __parse_yield(self, node: pyast.Yield):
         """
         Warning: may not work for single output
 
         Warning: requires self.yieldVars to be complete
 
         yield <value>;
         """
-        assert isinstance(node.value, pyast.Tuple)
-        return [
-            vast.NonBlockingSubsitution(
-                self.output_vars[idx], self.parse_expression(elem).to_string()
+        if isinstance(node.value, pyast.Tuple):
+            output_vars = node.value.elts  # e.g. `yield (1, 2)`
+        elif isinstance(node.value, pyast.Constant):
+            output_vars = [node.value]  # e.g. `yield 1`
+        else:
+            raise NotImplementedError(
+                f"Unexpected yield {type(node.value)} {pyast.dump(node)}"
             )
-            for idx, elem in enumerate(node.value.elts)
-        ] + [vast.NonBlockingSubsitution("_valid", "1")]
+        try:
+            return [
+                ir.NonBlockingSubsitution(
+                    ir.Var(self._output_vars[idx]), self.__parse_expression(elem)
+                )
+                for idx, elem in enumerate(output_vars)
+            ] + [ir.ValidSubsitution(ir.Var("_valid"), ir.Int(1))]
+        except IndexError as e:
+            raise IndexError(
+                "yield return length differs from function return length type hint"
+            ) from e
 
-    @staticmethod
-    def parse_binop(node: pyast.BinOp):
+    def __parse_binop_improved(self, expr: pyast.BinOp):
         """
         <left> <op> <right>
         """
-        if isinstance(node.op, pyast.Add):
-            return " + "
-        if isinstance(node.op, pyast.Sub):
-            return " - "
-        if isinstance(node.op, pyast.Mult):
-            return " * "
-        if isinstance(node.op, pyast.Div):
-            return " / "
+        if isinstance(expr.op, pyast.Add):
+            return ir.Add(
+                self.__parse_expression(expr.left), self.__parse_expression(expr.right)
+            )
+        if isinstance(expr.op, pyast.Sub):
+            return ir.Sub(
+                self.__parse_expression(expr.left), self.__parse_expression(expr.right)
+            )
+
+        if isinstance(expr.op, pyast.Mult):
+            return ir.Mul(
+                self.__parse_expression(expr.left), self.__parse_expression(expr.right)
+            )
+
+        if isinstance(expr.op, (pyast.Div, pyast.FloorDiv)):
+            return ir.Div(
+                self.__parse_expression(expr.left), self.__parse_expression(expr.right)
+            )
         raise TypeError(
-            "Error: unexpected binop type", type(node.op), pyast.dump(node.op)
+            "Error: unexpected binop type", type(expr.op), pyast.dump(expr.op)
         )
 
-    def parse_expression(self, expr: pyast.AST):
+    def __parse_expression(self, expr: pyast.AST):
         """
         <expression> (e.g. constant, name, subscript, etc., those that return a value)
         """
         if isinstance(expr, pyast.Constant):
-            return vast.Expression(str(expr.value))
+            return ir.Int(expr.value)
         if isinstance(expr, pyast.Name):
-            return vast.Expression(expr.id)
+            return ir.Var(expr.id)
         if isinstance(expr, pyast.Subscript):
-            return self.parse_subscript(expr)
+            return self.__parse_subscript(expr)
         if isinstance(expr, pyast.BinOp):
-            return vast.Expression(
-                "("
-                + self.parse_expression(expr.left).to_string()
-                + self.parse_binop(expr)
-                + self.parse_expression(expr.right).to_string()
-                + ")"
+            # Special case for floor division with  2 on right-hand-side
+            # Due to Verilog handling negative division "rounding"
+            # differently than Python floor division
+            # e.g. Verilog: -5 / 2 == -2, Python: -5 // 2 == -3
+            if (
+                isinstance(expr.op, pyast.FloorDiv)
+                and isinstance(expr.right, pyast.Constant)
+                and expr.right.value > 0
+                and expr.right.value % 2 == 0
+            ):
+                # return vast.Expression(
+                #     f"({self.parse_expression(expr.left).to_string()}
+                # >> {int(expr.right.value / 2)})"
+                # )
+                a_var = self.__parse_expression(expr.left).to_string()
+                b_var = expr.right.value
+                # return vast.Expression(
+                #     f"({a} > 0) ? ({a} >> {int(b / 2)}) : -(-({a}) >> {int(b / 2)})"
+                # )
+                return ir.Expression(
+                    f"({a_var} > 0) ? ({a_var} / {b_var}) : ({a_var} / {b_var} - 1)"
+                )
+
+            # warnings.warn(pyast.dump(expr))
+            # return irast.Expression(
+            #     "("
+            #     + self.__parse_expression(expr.left).to_string()
+            #     + self.__parse_binop(expr)
+            #     + self.__parse_expression(expr.right).to_string()
+            #     + ")"
+            # )
+            return self.__parse_binop_improved(expr)
+        if isinstance(expr, pyast.UnaryOp):
+            if isinstance(expr.op, pyast.USub):
+                return ir.Expression(
+                    f"-({self.__parse_expression(expr.operand).to_string()})"
+                )
+            raise TypeError(
+                "Error: unexpected unaryop type", type(expr.op), pyast.dump(expr.op)
             )
         if isinstance(expr, pyast.Compare):
-            return self.parse_compare(expr)
-        raise TypeError("Error: unexpected expression type", type(expr))
+            return self.__parse_compare(expr)
+        if isinstance(expr, pyast.BoolOp):
+            if isinstance(expr.op, pyast.And):
+                return ir.Expression(
+                    f"({self.__parse_expression(expr.values[0]).to_string()}) \
+                    && ({self.__parse_expression(expr.values[1]).to_string()})"
+                )
+        raise TypeError(
+            "Error: unexpected expression type", type(expr), pyast.dump(expr)
+        )
 
-    def parse_subscript(self, node: pyast.Subscript):
+    def __parse_subscript(self, node: pyast.Subscript):
         """
         <value>[<slice>]
         Note: built from right to left, e.g. [z] -> [y][z] -> [x][y][z] -> matrix[x][y][z]
         """
-        return vast.Expression(
-            f"{self.parse_expression(node.value)}[{self.parse_expression(node.slice)}]"
+        return ir.Expression(
+            f"{self.__parse_expression(node.value).to_string()}\
+                [{self.__parse_expression(node.slice).to_string()}]"
         )
 
-    def parse_compare(self, node: pyast.Compare):
+    def __parse_compare(self, node: pyast.Compare):
         """
         <left> <op> <comparators>
         """
         assert len(node.ops) == 1
         assert len(node.comparators) == 1
 
         if isinstance(node.ops[0], pyast.Lt):
@@ -410,51 +515,54 @@
             operator = ">"
         elif isinstance(node.ops[0], pyast.GtE):
             operator = ">="
         else:
             raise TypeError(
                 "Error: unknown operator", type(node.ops[0]), pyast.dump(node.ops[0])
             )
-        return vast.Expression(
-            f"{self.parse_expression(node.left).to_string()} {operator}"
-            f" {self.parse_expression(node.comparators[0]).to_string()}"
+        return ir.Expression(
+            f"{self.__parse_expression(node.left).to_string()} {operator}"
+            f" {self.__parse_expression(node.comparators[0]).to_string()}"
         )
 
-    def parse_while(self, stmt: pyast.While, prefix: str = ""):
+    def __parse_while(self, stmt: pyast.While, prefix: str):
         """
         Converts while loop to a while-true-if-break loop
         """
         assert isinstance(stmt, pyast.While)
-        state_var = self.add_global_var("0", f"{prefix}_WHILE")
-        conditional_item = vast.CaseItem(
-            vast.Expression("0"),
+        assert prefix != ""
+        state_var = self.__add_global_var(
+            str(0), f"{prefix}_WHILE{self.__create_unique_name()}"
+        )
+        conditional_item = ir.CaseItem(
+            ir.Int(0),
             [
-                vast.IfElse(
-                    vast.Expression(
-                        f"!({self.parse_expression(stmt.test).to_string()})"
+                ir.IfElse(
+                    ir.Expression(
+                        f"!({self.__parse_expression(stmt.test).to_string()})"
                     ),
                     [
-                        vast.NonBlockingSubsitution(
-                            f"{prefix}_STATE", f"{prefix}_STATE + 1"
+                        ir.StateSubsitution(
+                            ir.Var(prefix), ir.Add(ir.Var(prefix), ir.Int(1))
                         )
                     ],
-                    [vast.NonBlockingSubsitution(state_var, "1")],
+                    [ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(1))],
                 )
             ],
         )
-        then_item = vast.CaseItem(
-            vast.Expression("1"),
+        then_item = ir.CaseItem(
+            ir.Expression("1"),
             [
-                self.parse_statements(
-                    stmt.body,
-                    f"{state_var}{self.create_unique_name()}",
-                    end_stmts=[vast.NonBlockingSubsitution(f"{state_var}", "0")],
+                self.__parse_statements(
+                    list(stmt.body),
+                    f"{state_var}",
+                    end_stmts=[ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(0))],
                     reset_to_zero=True,
                 )
             ],
         )
         return [
-            vast.While(
-                vast.Expression(f"{state_var}"),
+            ir.WhileWrapper(
+                ir.Expression(f"{state_var}"),
                 [conditional_item, then_item],
             )
         ]
```

### Comparing `python2verilog-0.0.2/python2verilog/frontend/utils.py` & `python2verilog-0.0.3/python2verilog/utils/string.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 class Lines:
     """
     A list of str that can be serialized to string with provided indents
     """
 
     @staticmethod
-    def assert_no_newline(stringable: any):
+    def assert_no_newline(string: str):
         """
-        Asserts no newline character in str(stringable)
+        Asserts no newline character in string
         """
-        assert str(stringable).find("\n") == -1, "Newline in Lines: " + str(stringable)
+        assert string.find("\n") == -1, "Newline in Lines: " + string
 
-    def __init__(self, data: list[str] | str = None):
+    def __init__(self, data: list[str] | str | None = None):
         if data is None:
             self.lines = []
         elif isinstance(data, str):
             self.assert_no_newline(data)
             self.lines = [data]
         elif isinstance(data, list):
             for line in data:
@@ -47,15 +47,15 @@
     def __setitem__(self, key: int, value: str):
         self.lines[key] = value
 
     def __delitem__(self, key: int):
         del self.lines[key]
 
     def __rshift__(self, indent: int):
-        indent(indent)
+        self.indent(indent)
 
     def indent(self, indent_amount: int):
         """
         Indent all lines by amount
         """
         self.lines = [Indent(indent_amount) + line for line in self.lines]
         return self
@@ -78,21 +78,21 @@
         self.lines.append(other)
         return self
 
     def concat(self, other: Lines, indent: int = 0):
         """
         Concats two Lines
         """
-        assert isinstance(other, Lines)
+        assert isinstance(other, Lines), f"got {type(other)} instead"
         for line in other.lines:
             self.lines.append(Indent(indent) + line)
         return self
 
     @staticmethod
-    def nestify(buffers: list[tuple[Lines][Lines]], indent: int = 0):
+    def nestify(buffers: list[tuple[Lines, Lines]], indent: int = 0):
         """
         pair[0][0]
             pair[1][0]
                 pair[2][0]
                 pair[2][1]
             pair[1][0]
         pair[0][1]
```

### Comparing `python2verilog-0.0.2/python2verilog/utils/visualization.py` & `python2verilog-0.0.3/python2verilog/utils/visualization.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 def make_visual(generator_inst, directory: str):
     """
     Any iterable of tuples where the tuples are of length > 0 will work.
     Visualizes the first 3 elements of each tuple as (x, y, colour)
     """
 
     # Generate the data using the generator function
-    data_triple = []
+    data_triple_list = []
 
     for yields in generator_inst:
         if len(yields) >= 3:
-            data_triple.append(yields[:3])
+            data_triple_list.append(yields[:3])
         elif len(yields) >= 2:
-            data_triple.append((*yields[:2], 1))
+            data_triple_list.append((*yields[:2], 1))
         else:
-            data_triple.append((yields[0], 1, 2))
+            data_triple_list.append((yields[0], 1, 2))
 
-    data_triple = np.array(data_triple)
+    data_triple = np.array(data_triple_list)
 
     height = max(data_triple[:, 0])
     width = max(data_triple[:, 1])
-    # warnings.warn(f"{height}, {width}, {data_triple}")
     grid = np.zeros((int(height) + 1, int(width) + 1))
     for x_coord, y_coord, colour in data_triple:
         grid[x_coord, y_coord] = colour
 
     # Create the pixel-like plot
     plt.imshow(grid)
 
@@ -43,7 +42,10 @@
     cbar.set_label("Z")
 
     plt.gca().invert_yaxis()
 
     # Show the plot
     # plt.show()
     plt.savefig(directory)
+
+    plt.clf()
+    plt.cla()
```

### Comparing `python2verilog-0.0.2/python2verilog.egg-info/PKG-INFO` & `python2verilog-0.0.3/python2verilog.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,126 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
+![Python Package](https://github.com/worldofkerry/python2verilog/actions/workflows/python-package.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/python2verilog/badge/?version=latest)](https://python2verilog.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/python2verilog)
+
 # Python 2 Verilog
 
 Converts a subset of python generator functions into synthesizable sequential SystemVerilog.
 
 A use case is for drawing shapes on grids (for VGA output), where the user may prototype the algorithm in python and then convert it to verilog for use in an FPGA.
 
-A testbench is also generated and asserted against the Python outputs.
+A testbench can also be generated and asserted against the Python outputs.
 
 Supports Python [Generator functions](https://wiki.python.org/moin/Generators) as well as the following block types:
 
 - `if`
 - `while`
-- `for ... in range(...)` with 1 or 2 args in `range` (quite inefficient)
-
-**Warning**: Variables must be unique, i.e. variables do not have block scope, e.g. the following modifies global `i`:
 
-```python
-for i in range(10):
-    pass
-```
+**Warning**: Variables are treated as global and therefore no variable shadowing.
 
 ## Sample Usage
 `pip install python2verilog`
 
-### Basic usage
-`python3 -m python2verilog.convert generator.py`
-`python3 -m python2verilog.convert generator.py -c "(1, 2, 3, 4)"`
+### Basic Usage
+Create a python file containing a generator function with output type hints, named `<name>.py`.
+
+A sample can be found [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/integration/circle_lines/python.py)
 
-### More Complex Usage
+`python3 -m python2verilog.convert <name>.py`. Use `--help` for additional options, including outputting a testbench.
 
 ## Testing
 
 ### Requirements
 
 Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
 
 Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
 
-Python: `python3 -m pip install -r tests/requirements.txt`
+Python Libraries: `python3 -m pip install -r tests/requirements.txt`
 
 ### Creating New Test
 
-To create a new test case and set up configs, run `python3 tests/frontend/new_generator.py <name>`.
+To create a new test case and set up configs, run `python3 tests/integration/new_test_case.py <test-name>`.
 
 ### Running Tests
 
 To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
-Those files will be stored in `tests/frontend/data/generator/<name>/`.
+Those files will be stored in `tests/integration/data/integration/<test-name>/`.
 
 ## Tested Generations
 
-The outputs of the Python script tests can be found [as a github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/data-generator.zip)
-
-Python vs Verilog stats on sample inputs (not up-to-date) can be found [here](tests/frontend/data/generator/stats.md), more up-to-date ones can be found in the artifact.
+Outputs of tests in repo can be found as a [github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/tests-data.zip)
 
 ## For Developers
 
 Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
 
 Architecture is based on [LLVM](https://llvm.org/).
 
 To setup pre-commit, run `pre-commit install`.
 
 ### Epics
 
 - Support arrays
+- Mimic combinational logic with "regular" Python functions
+- Division approximations
 
 ## Docs
 
-- Generate `.html` docs: `bash docs/generate.sh`
-- Live docs: `python3 -m pydoc -b`
+- cd to `docs/`
+- `sphinx-apidoc -o . ../python2verilog/`
+- `make html`
 
 ## Random Planning, Design, and Notes
 
+## What needs to be duplicated in testbenches?
+declare I/O and other signals
+declare DUT
+start clock
+
+loop for each test case
+- start signal
+- while wait for done signal
+  - clock
+  - set start zero
+  - display output
+endloop
+
+
 ### Potential API
 
 ```python
 import python2verilog as p2v
 import ast
 
 func = ast.parse(code).body[0]
 
-ir = p2v.from_python_get_ir(func.body) # returns an ir node for the root of the body
+ir = p2v.from_python_get_ir(func.body)
 
 # Optimization passes
 ir = p2v.optimizations.replace_single_item_cases(ir)
 ir = p2v.optimizations.remove_nesting(ir)
 ir = p2v.optimizations.combine_statements(ir)
-for i in dir(p2v.optimizations): # Do one pass of every optimization
-  item = getattr(pv2.optimizations, i)
-    if callable(item):
-      ir = item(ir)
 
 verilog = p2v.Verilog()
-verilog.from_python_do_setup(func) # module I/O is dependent on Python
-verilog.from_ir_fill_body(ir) # fills the body
+verilog.from_python_do_setup(ir.get_context()) # module I/O is dependent on Python
+verilog.from_ir_fill_body(ir.get_root()) # fills the body
 
 # whether has valid or done signal,
 # whether initialization is always happening or only on start,
 # verilog sim name
 verilog.config(has_valid=True, has_done=True, lazy_start=True, verilog_sim="iverilog")
 
 with open(f"{verilog.get_module_name()}.sv", mode="w") as module:
```

### Comparing `python2verilog-0.0.2/python2verilog.egg-info/SOURCES.txt` & `python2verilog-0.0.3/python2verilog.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 python2verilog/__init__.py
 python2verilog/convert.py
 python2verilog.egg-info/PKG-INFO
 python2verilog.egg-info/SOURCES.txt
 python2verilog.egg-info/dependency_links.txt
 python2verilog.egg-info/top_level.txt
 python2verilog/backend/__init__.py
-python2verilog/backend/codegen.py
-python2verilog/backend/expressions.py
-python2verilog/backend/statements.py
-python2verilog/backend/utils.py
+python2verilog/backend/verilog.py
 python2verilog/frontend/__init__.py
-python2verilog/frontend/generator.py
-python2verilog/frontend/generator2ast.py
-python2verilog/frontend/utils.py
+python2verilog/frontend/generator_parser.py
+python2verilog/ir/__init__.py
+python2verilog/ir/context.py
+python2verilog/ir/expressions.py
+python2verilog/ir/statements.py
 python2verilog/optimizer/__init__.py
+python2verilog/optimizer/optimizer.py
 python2verilog/utils/__init__.py
+python2verilog/utils/assertions.py
+python2verilog/utils/string.py
 python2verilog/utils/visualization.py
```

