# Comparing `tmp/hepfile-0.1.6.tar.gz` & `tmp/hepfile-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepfile-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hepfile-0.1.7.tar", last modified: Fri Jul 21 12:06:38 2023, max compression
```

## Comparing `hepfile-0.1.6.tar` & `hepfile-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,32 @@
--rw-r--r--   0        0        0    11389 2023-07-13 17:01:59.486751 hepfile-0.1.6/LICENSE
--rw-r--r--   0        0        0     8348 2023-07-13 17:01:59.486751 hepfile-0.1.6/README.md
--rw-r--r--   0        0        0     1939 2023-07-13 17:01:59.502752 hepfile-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1245 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/__init__.py
--rw-r--r--   0        0        0       76 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/_version.py
--rw-r--r--   0        0        0     8110 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/awkward_tools.py
--rw-r--r--   0        0        0      402 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/constants.py
--rw-r--r--   0        0        0     1962 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/csv_tools.py
--rw-r--r--   0        0        0     8841 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/df_tools.py
--rw-r--r--   0        0        0     7229 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/dict_tools.py
--rw-r--r--   0        0        0     1935 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/errors.py
--rw-r--r--   0        0        0        0 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/py.typed
--rw-r--r--   0        0        0    21714 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/read.py
--rw-r--r--   0        0        0    28920 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/write.py
--rw-r--r--   0        0        0    10302 1970-01-01 00:00:00.000000 hepfile-0.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:06:38.009739 hepfile-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-21 12:06:28.000000 hepfile-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22469 2023-07-21 12:06:38.009739 hepfile-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-07-21 12:06:28.000000 hepfile-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-21 12:06:28.000000 hepfile-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:06:38.009739 hepfile-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:06:38.005739 hepfile-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:06:38.005739 hepfile-0.1.7/src/hepfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/awkward_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/df_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/dict_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30022 2023-07-21 12:06:28.000000 hepfile-0.1.7/src/hepfile/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:06:38.009739 hepfile-0.1.7/src/hepfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22469 2023-07-21 12:06:37.000000 hepfile-0.1.7/src/hepfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-21 12:06:38.000000 hepfile-0.1.7/src/hepfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:06:37.000000 hepfile-0.1.7/src/hepfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 12:06:37.000000 hepfile-0.1.7/src/hepfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 12:06:37.000000 hepfile-0.1.7/src/hepfile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:06:38.009739 hepfile-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-21 12:06:28.000000 hepfile-0.1.7/tests/test_1_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-21 12:06:28.000000 hepfile-0.1.7/tests/test_2_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-21 12:06:28.000000 hepfile-0.1.7/tests/test_3_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-21 12:06:28.000000 hepfile-0.1.7/tests/test_4_awkward_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-21 12:06:28.000000 hepfile-0.1.7/tests/test_5_dict_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-21 12:06:28.000000 hepfile-0.1.7/tests/test_6_csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-21 12:06:28.000000 hepfile-0.1.7/tests/test_7_df_tools.py
```

### Comparing `hepfile-0.1.6/LICENSE` & `hepfile-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hepfile-0.1.6/README.md` & `hepfile-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,67 +31,67 @@
 [pypi-version]:             https://badge.fury.io/py/hepfile.svg
 [rtd-badge]:                https://readthedocs.org/projects/hepfile/badge/?version=latest
 [rtd-link]:                 https://hepfile.readthedocs.io/en/latest/?badge=latest
 [sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 
 # Heterogeneous Files in Parallel File (hepfile)
 
-In high energy physics, experiments require file formats that can accomodate 
+In high energy physics, experiments require file formats that can accomodate
 heterogeneity (each collection event can have differing amounts of data collected)
 and size (since HEP experiments can generate petabytes of data). Although the current
 file format of choice is ROOT, a file format developed by CERN, we believe that
 HDF5, which is a portable and more commonly used file format outside of HEP,
-has promise in being a new standard. 
+has promise in being a new standard.
 
 The only issue is that HDF5 works best with homogenous data formats, where each
 dataset occupies an n by m chunk of memory. This is not necessarily the case
 for HEP data, but we addressed this issue using an organizational method outlined
 in our schema.
 
 # Schema
 
-### Heterogenous Data ... 
+### Heterogenous Data ...
 
-We assume that data that we collect is composed of (insert some term for particle, 
-chair, etc.) each carrying a certain number of attributes. Each ___ is associated 
+We assume that data that we collect is composed of (insert some term for particle,
+chair, etc.) each carrying a certain number of attributes. Each ___ is associated
 with some increasing counter. In HEP, this counter is events. Each event can
-have an arbitrary number of particles of any type, making this data heterogenous. 
+have an arbitrary number of particles of any type, making this data heterogenous.
 
-### ... to Homogenous File 
+### ... to Homogenous File
 
-To make this data homogenous, we can create n by m chunks of data for each type 
-of particle, where n is the total number of this particle in all of the events, 
-and the specific row for each of the particles contains all of the attributes 
+To make this data homogenous, we can create n by m chunks of data for each type
+of particle, where n is the total number of this particle in all of the events,
+and the specific row for each of the particles contains all of the attributes
 for that particle in the original data.
 
 We also create a list for each type of particle whose length is the total number
 of events. At position *i*, we have the data for how many particles of said type
-appeared in event *i*. 
+appeared in event *i*.
 
 # Overview of use case
 
 `hepfile` is useful for datasets where there are n columns with different numbers
 of rows. In more "pythonic" language, you can imagine a dictionary where each key
 has a different number of values. For example:
 ```
    data = {x: [1],
            y: [1, 2],
 	   z: ['1', '2', '3']
    }
 ```
 This can not simply be converted to most common data structures, like a Pandas DataFrame,
 or written to a simple homogeneous file structure, like a CSV file. In a more complex case
-Let's have an image of a town, with cartoon people here. 
+Let's have an image of a town, with cartoon people here.
 
-To illustrate how to use hepfile with this example, we imagine a researcher conducting 
+To illustrate how to use hepfile with this example, we imagine a researcher conducting
 a census on a town. Each household in the town has some variable number of people
 in it, some variable number of vehicles, and only one residence. The people, vehicles,
-and residence all have different data associated with them. How would we record 
-these data? Well, to first order, we might decide to record them in multiple spreadsheets or 
-multiple .csv files. 
+and residence all have different data associated with them. How would we record
+these data? Well, to first order, we might decide to record them in multiple spreadsheets or
+multiple .csv files.
 
 ![](docs/images/household_example_spreadsheet_00_smaller.png)
 ![](docs/images/household_example_spreadsheet_01_smaller.png)
 ![](docs/images/household_example_spreadsheet_02_smaller.png)
 
 One could also imagine this data stored in a database with each of the csv files as tables.
 But the goal is to keep all of this data in one file, so that it is easier for someone to
@@ -149,13 +149,19 @@
 For local builds for testing follow these steps:
 1. Clone this repo
 2. Navigate to the top-level directory of this project (probably called hepfile)
 3. We then recommend installing with the developer dependencies. To do this run:
 ```
 python -m pip install -e .[dev]
 ```
-4. Then, run the following commands to setup the pre-commit git hook
-to automatically run our tests before committing!
+4. Then, run the following command to setup the pre-commit git hook
+to automatically run our code standard tests before committing!
 ```
-chmod a+x pre-commit-tests.sh
-ln -s ../../pre-commit-tests.sh .git/hooks/pre-commit
+pip install pre-commit
+pre-commit install
+```
+
+As a side note, to test developments to the code use the following command in the top-level directory of
+the project:
+```
+pytest
 ```
```

### Comparing `hepfile-0.1.6/pyproject.toml` & `hepfile-0.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
+requires = ['setuptools>=42']
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "hepfile"
 authors = [{name = "Matt Bellis", email = "mbellis@siena.edu"}]
 readme = "README.md"
 license = {file = "LICENSE"}
-dynamic = ["version", "description"]
+dynamic = ["version"] #, "description"]
 
 requires-python = ">=3.9"
 
 classifiers = [
   "License :: OSI Approved :: BSD License",
   "Topic :: Scientific/Engineering",
   "Intended Audience :: Science/Research",
@@ -33,41 +33,45 @@
 
 [project.urls]
 Documentation = "https://hepfile.github.io"
 Home = "https://github.com/mattbellis/hepfile"
 
 [project.optional-dependencies]
 pandas = ["pandas"]
-awkward = ["awkward"]
+awkward = ["awkward>2"]
 learn = [
       "hepfile[pandas,awkward]",
       "astropy"
       ]
 all = ["hepfile[pandas,awkward]"]
 
 # for developers
 dev = [
     "hepfile[all]",
     "pre-commit",
     "jupyter",
     "mistune",
-    "pytest"
+    "pytest",
+    "ruff"
     ]
 
 docs = [
   "hepfile[all]",
   "Sphinx>=3.0.0",
   "myst_parser>=0.13",
   "nbsphinx>=0.9.1",
   "sphinx-book-theme>=0.0.33",
   "sphinx_copybutton",
   "autodoc",
   "ipykernel"
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = 'hepfile._version.__version__'}
+
 [tool.pytest.ini_options]
 addopts = "-ra -Wd"
 testpaths = ["tests"]
 
 [tool.mypy]
 files = "src"
 python_version = "3.9"
@@ -81,8 +85,64 @@
 check_untyped_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 no_implicit_reexport = true
-strict_equality = true
+strict_equality = true
+
+[tool.ruff]
+# Enable the pycodestyle (`E`) and Pyflakes (`F`) rules by default.
+# Unlike Flake8, Ruff doesn't enable pycodestyle warnings (`W`) or
+# McCabe complexity (`C901`) by default.
+select = ["E", "F"]
+ignore = []
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["ALL"]
+unfixable = []
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".git-rewrite",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    ".github",
+    ".ipynb_checkpoints",
+    "docs",
+    "tests",
+    "paper",
+    "sandbox",
+    ".binder",
+]
+
+# set to the same as black
+line-length = 88
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.10.
+target-version = "py310"
+
+# Ignore `E402` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
+[tool.ruff.per-file-ignores]
+"src/hepfile/__init__.py" = ["E402", "F403", "F401"]
```

### Comparing `hepfile-0.1.6/src/hepfile/__init__.py` & `hepfile-0.1.7/src/hepfile/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A file description modeled after the ROOT analysis toolkit and common use-cases
 in High Energy Physics. Implemented in HDF5, hepfile stands for Heterogeneous
 Entries in Parallel-file.
 
 See hepfile.readthedocs.io for detailed documentation!
 """
 from __future__ import annotations
-import sys
+from importlib.util import find_spec
 
 from ._version import __version__
 from .errors import MissingOptionalDependency
 
 # explicitly set the package variable to ensure relative import work
 __package__ = "hepfile"
 
@@ -19,28 +19,24 @@
 _PANDAS = False
 
 # import modules
 from hepfile.read import *
 from hepfile.write import *
 import hepfile.dict_tools
 
-try:
+if find_spec("awkward") is not None:
     import hepfile.awkward_tools
 
     _AWKWARD = True
-except ImportError:
-    pass
 
-try:
+if find_spec("pandas") is not None:
     import hepfile.df_tools
     import hepfile.csv_tools
 
     _PANDAS = True
-except ImportError:
-    pass
 
 # put all these variables in __all__
 __all__ = ("__version__", "__package__", "_AWKWARD", "_PANDAS")
 
 
 # override getattr
 def __getattr__(name: str) -> bool:
```

### Comparing `hepfile-0.1.6/src/hepfile/awkward_tools.py` & `hepfile-0.1.7/src/hepfile/df_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,262 +1,270 @@
 """
-These are tools to make working with and translating between awkward arrays
-and hepfile data objects easier.
+Tools to work with Pandas DataFrames and Hepfile data
 
 Note: The base installation package does not contain these tools!
 You must have installed hepfile with either
-1) 'python -m pip install hepfile[awkward]', or
+1) 'python -m pip install hepfile[pandas]', or
 2) 'python -m pip install hepfile[all]'
 """
 from __future__ import annotations
 
-import warnings
-import awkward as ak
-import numpy as np
-from hepfile.write import (
-    initialize,
-    create_group,
-    create_dataset,
-    write_to_file,
-    create_single_bucket,
-    pack,
-)
-from hepfile.errors import AwkwardStructureError, InputError
-
-
-################################################################################
-def hepfile_to_awkward(
-    data: dict, groups: list = None, datasets: list = None
-) -> ak.Record:
+import pandas as pd
+import hepfile as hf
+from hepfile.errors import InputError, MissingOptionalDependency
+from hepfile.dict_tools import dictlike_to_hepfile
+
+
+def hepfile_to_df(
+    data: dict,
+    groups: list[str] = None,
+    events: list[int] = None,
+) -> dict[pd.DataFrame]:
     """
-    Converts all (or a subset of) the output data from `hepfile.read.load` to
-    a dictionary of awkward arrays.
+    Converts hepfile data to dataframes where each group is in its own dataframe
+    and we add an extra column called 'event_num'. Singletons have its own df
 
     Args:
-        data (dict): Output data dictionary from the `hepfile.read.load` function.
-        groups (list): list of groups to pull from data and convert to awkward arrays.
-        datasets (list): list of full dataset paths (ex. 'jet/px' not 'px') to pull
-        from data and include in the awkward arrays.
+        data [dict]: data object either loaded from a hepfile or about to be
+                     written to a hepfile.
+        groups [list]: groups to include, None (default) means include all groups
+        events [list]: list of event indexes to include
 
     Returns:
-        ak_arrays (dict): dictionary of awkward arrays with the data.
+        Dictionary of requested groups as dataframes where the keys are the group names.
+        If only one group is requested then it just returns a dataframe of that group.
     """
 
+    dfs = {}  # list to of dataframes to return
+
+    # check inputs
+    if groups is not None and not isinstance(groups, (list, str)):
+        raise InputError("groups must be either a list or a string")
+
+    if events is not None and not isinstance(events, (list, int)):
+        raise InputError("events must be either a list or int")
+
     if isinstance(groups, str):
         groups = [groups]
 
-    if groups is None:
-        groups = list(data["_GROUPS_"].keys())
+    if isinstance(events, int):
+        events = [events]
 
-    ak_arrays = {}
+    if groups is None:
+        groups = data["_GROUPS_"].keys()
 
-    # turn a few things into sets for faster searching
-    list_of_counters = set(data["_LIST_OF_COUNTERS_"])
-    singletons_group = set(data["_GROUPS_"]["_SINGLETONS_GROUP_"])
+    if not all(group in data["_GROUPS_"] for group in groups):
+        raise InputError("Groups must be a subset of the group names in data!")
 
+    # 1) regular groups to a dataframe for each group
+    # 2) all singletons to a dataframe
+    counters = set(data["_MAP_DATASETS_TO_COUNTERS_"].values())
     for group in groups:
-        for dset in data["_GROUPS_"][group]:
-            if dset in singletons_group:
-                dataset = dset
-            else:
-                dataset = f"{group}/{dset}"
+        datasets = data["_GROUPS_"][group]
 
-            if dataset in list_of_counters:
+        # put the data for that group in a dictionary
+        for_df = {}
+        dataset = None
+        for dataset in datasets:
+            name = f"{group}/{dataset}"
+            if name in counters:
                 continue
+            if group == "_SINGLETONS_GROUP_" and dataset in data:
+                for_df[dataset] = data[dataset]
+            else:
+                if name in data:
+                    for_df[dataset] = data[name]
 
-            if dataset not in data.keys():
-                continue
+        # compute the event numbers
+        counter_name = data["_MAP_DATASETS_TO_COUNTERS_"][group]
+        counters_for_df = []
+        for i, counter in enumerate(data[counter_name]):
+            for _ in range(counter):
+                counters_for_df.append(i)
+        for_df["event_num"] = counters_for_df
+
+        group_df = pd.DataFrame(for_df)  # make for_df a df
+        # get rid of anything not in events
+        if events is None:
+            events = group_df.event_num.unique()
+
+        group_df = group_df[group_df.event_num.isin(events)]
+
+        dfs[group] = group_df
+
+    if len(dfs) == 1:
+        return dfs[list(dfs.keys())[0]]
+    return dfs
+
+
+def awkward_to_df(
+    ak_array: ak.Array,  # noqa: F821
+    groups: list[str] = None,
+    events: list[int] = None,
+) -> dict[pd.DataFrame]:
+    """
+    Converts an awkward array of hepfile data to a dataframe. Does the same thing
+    as hepfile_to_df but given an awkward array.
 
-            if datasets is not None and dataset not in datasets:
-                continue
+    Note: You must have installed with 'python -m pip install hepfile[all]'
+          to use this tool!
 
-            if (
-                len(data[dataset]) != 0
-                and isinstance(data[dataset], (np.ndarray, list))
-                and isinstance(data[dataset][0], bytes)
-            ):
-                data[dataset] = np.array([val.decode() for val in data[dataset]])
-
-            if dataset in singletons_group:
-                if dataset in data.keys():  # skip if it isn't in data
-                    ak_arrays[dataset] = ak.Array(data[dataset])
-                continue
+    Args:
+        ak_array [ak.Array]: awkward array in the format of a hepfile
+        groups [list]: groups to include, None (default) means include all groups
+        events [list]: list of event indexes to include
 
-            nkey = data["_MAP_DATASETS_TO_COUNTERS_"][dataset]
+    Returns:
+        Dictionary of requested groups as dataframes where the keys are the group names.
+        If only one group is requested then it just returns a dataframe of that group.
+    """
 
-            num = data[nkey]
-            vals = data[dataset]
+    if not hf._AWKWARD:
+        raise MissingOptionalDependency("awkward")
 
-            ak_array = ak.unflatten(list(vals), list(num))
+    import awkward as ak
 
-            if group not in ak_arrays:
-                ak_arrays[group] = {}
-            ak_arrays[group][dset] = ak_array
-
-    try:
-        awk = ak.Array(ak_arrays)
-    except ValueError:
-        warnings.warn(
-            "Cannot convert to an Awkward Array because dict arrays have"
-            + " different lengths! Returning an Awkward Record instead."
-        )
-        awk = ak.Record(ak_arrays)
-
-    try:
-        _is_valid_awkward(awk)
-    except AwkwardStructureError as err:
-        print(err)
-        raise AwkwardStructureError(
-            "Cannot convert to proper awkward array because of the above \
-            error! Check your input hepfile format"
-        ) from err
-
-    return awk
-
-
-################################################################################
-def awkward_to_hepfile(
-    ak_array: ak.Record,
-    outfile: str = None,
-    write_hepfile: bool = True,
-    verbose: bool = False,
-    **kwargs,
-) -> dict:
-    """
-    Converts a dictionary of awkward arrays to a hepfile
+    dfs = {}  # list to of dataframes to return
 
-    Args:
-        ak_array (Awkward Array): dictionary of Awkward Arrays to write to a hepfile
-        outfile (str): path to write output hdf5 file to
-        write_hepfile (bool): if True, writes data to outfile.
-                              If False, just converts to hepfile format and returns
-        verbose (bool): if true print some stuff
-        **kwargs (None): Passed to `hepfile.write.write_to_file`
+    # check inputs
+    if groups is not None and not isinstance(groups, (list, str)):
+        raise InputError("groups must be either a list or a string")
 
-    Returns:
-        Dictionary of hepfile data
-    """
+    if events is not None and not isinstance(events, (list, int)):
+        raise InputError("events must be either a list or int")
 
-    # perform IO checks
+    if isinstance(groups, str):
+        groups = [groups]
 
-    _is_valid_awkward(ak_array)
+    if isinstance(events, int):
+        events = [events]
 
-    if write_hepfile is True and outfile is None:
-        raise InputError("Please provide an outfile path if write_hepfile=True!")
+    if groups is None:
+        groups = ak_array.fields
 
-    if write_hepfile is False and outfile is not None:
-        warnings.warn(
-            "You set write_hepfile to False but provided an output file path. \
-            This output file path will not be used!"
-        )
-
-    data = initialize()
-    # first create the named groups and datasets
-    for group in ak_array.fields:
-        counter = f"n{group}"
-
-        # check for singletons
-        if len(ak_array[group].fields) == 0:
-            dtype = _get_awkward_type(ak_array[group])
-            create_dataset(data, group, dtype=dtype)
-            continue
-
-        create_group(data, group, counter=counter)
-        for dataset in ak_array[group].fields:
-            if len(ak_array[group][dataset][0]) == 0:
-                dtype = None
-            else:
-                dtype = _get_awkward_type(ak_array[group][dataset])
-            create_dataset(data, dataset, group=group, dtype=dtype)
+    if not all(group in ak_array.fields for group in groups):
+        raise InputError("Groups must be a subset of the group names in data!")
 
-    # then pack data from the awkward array
-    for data_dict in ak_array:
-        bucket = create_single_bucket(data)
-        for group in data_dict.fields:
-            if group in bucket["_GROUPS_"]["_SINGLETONS_GROUP_"]:
-                bucket[group] = data_dict[group]
-                continue
+    for group in groups:
+        # convert the record
+        group_df = ak.to_dataframe(ak_array[group])
 
-            for dataset in data_dict[group].fields:
-                name = f"{group}/{dataset}"
-                bucket[name] = data_dict[group][dataset].to_list()
-        pack(data, bucket)
+        # caluclate the indexes
+        num = []
+        for i, awk in enumerate(ak_array[group]):
+            if isinstance(awk, (ak.Array, ak.Record)):
+                record_len = len(awk.to_list()[awk.fields[0]])
+                for _ in range(record_len):
+                    num.append(i)
+            else:
+                num.append(i)
 
-    # then write it out to a file
-    if write_hepfile:
-        if verbose:
-            print("Writing the hdf5 file from the awkward array...")
+        # put event number in the dataframe
+        group_df["event_num"] = num
 
-        write_to_file(outfile, data)
+        # only take events with event numbers in events
+        if events is None:
+            events = group_df.event_num.unique()
+        group_df = group_df[group_df.event_num.isin(events)]
 
-    return data
+        dfs[group] = group_df
 
+    if len(dfs) == 1:
+        return dfs[list(dfs.keys())[0]]
+    return dfs
 
-def _awkward_depth(ak_array: ak.Record) -> int:
-    max_depth = 0
-    for item in ak_array.to_list():
-        item_depth = 0
-        for string in str(item):
-            if string == "{":
-                item_depth += 1
 
-            if item_depth > max_depth:
-                max_depth = item_depth
+def df_to_hepfile(
+    df_dict: dict[pd.DataFrame],
+    outfile: str = None,
+    event_num_col="event_num",
+    write_hepfile: bool = True,
+) -> dict:
+    """
+    Converts a list of dataframes of group data to a hepfile. The opposite of
+    hepfile_to_df. Must have an event_num column!
 
-            if string == "}":
-                item_depth -= 1
+    Args:
+        df_dict [dict]: dictionary of pandas DataFrame groups to write to a hepfile
+        outfile [str]: output file name, required if write_hepfile is True
+        event_num_col [str]: name of a column in the pd.DataFrame to group by
+        write_hepfile [bool]: should we write the hepfile data to a hepfile?
+
+    Returns:
+        hepfile data dictionary
+    """
 
-    return max_depth
+    out = groupDF_to_eventDF(df_dict, event_num_col)
+    return dictlike_to_hepfile(
+        out,
+        outfile=outfile,
+        how_to_pack="classic",
+        write_hepfile=write_hepfile,
+        ignore_protected=True,
+    )
 
 
-def _is_valid_awkward(ak_array: ak.Record):
+def groupDF_to_eventDF(
+    df_dict: dict[pd.DataFrame], event_num_col: str = "event_num"
+) -> dict:
     """
-    Checks if the input awkward array is valid and raises an exception if not
+    Converts a dictionary of group dataframes to a dictionary of event dataframes
 
     Args:
-        ak_array (ak.Array): awkward array to check
+        df_dict [dict] : dictionary of groups to convert to a dictionary of events
+        event_num_col [str] : column to group each group by
     """
 
-    # validate input array
-    if not isinstance(ak_array, (ak.Array, ak.Record)):
-        raise AwkwardStructureError("Please input an Awkward Array or Awkward Record")
-
-    if len(ak_array.fields) == 0:
-        raise AwkwardStructureError(
-            "Your input Awkward Array must be a Record. \
-            This means it needs to have fields in it."
-        )
-
-    # check input array only has a "depth" of 2
-    # this can be removed once hepfiles support unlimited depth of groups!
-    if _awkward_depth(ak_array) > 2:
-        raise AwkwardStructureError(
-            "Hepfile only supports awkward arrays with a depth <= 2! \
-            Please ensure your input follows this guideline."
-        )
-
-
-def _get_awkward_type(ak_array: ak.Record) -> type:
-    ndim = ak_array.ndim
-    try:
-        if isinstance(ak_array[0], (ak.Record, ak.Array)):
-            arr = ak_array
-            type_str = ak_array.type.content
-            if isinstance(type_str, ak.types.NumpyType):
-                dtype = type_str.primitive
-            else:
-                dtype = str(type_str).rsplit("*", maxsplit=1)[-1].strip()
-        else:
-            arr = np.array(ak_array)
-            dtype = arr.dtype
-
-        if dtype == "string":
-            dtype = np.dtype("<U1")
-
-        np_dtype = np.dtype(dtype)
-        if np_dtype.char == "U":
-            np_dtype = str
+    out = {}
+    all_subkeys = {}
+    for group_name, data in df_dict.items():
+        if group_name != "_SINGLETONS_GROUP_":
+            all_subkeys[group_name] = set(data.columns)
+
+        if event_num_col not in data.columns:
+            raise InputError(
+                f"{event_num_col} not in group {group_name} in the input dictionary"
+            )
+
+        groups = data.groupby(event_num_col)
+        split_groups = [groups.get_group(item) for item in groups.groups]
+
+        for grouping in split_groups:
+            key = grouping[event_num_col].values[0]
+            if key not in out:
+                out[key] = {}
+
+            if group_name != "_SINGLETONS_GROUP_" and group_name not in out[key]:
+                out[key][group_name] = {}
+
+            for colname in grouping.columns:
+                if colname == event_num_col:
+                    to_write = key
+                    out[key][colname] = to_write
+                elif group_name == "_SINGLETONS_GROUP_":
+                    vals = grouping[colname].values
+                    if len(vals) == 1:
+                        to_write = vals[0]
+                    else:
+                        to_write = vals
+                    out[key][colname] = to_write
+                else:
+                    to_write = list(grouping[colname].values)
+                    out[key][group_name][colname] = to_write
+
+    out = list(out.values())
+
+    # check that the keys of each event are the same
+    for event in out:
+        missing1 = list(all_subkeys.keys() - event.keys())
+        for key1 in missing1:
+            if key1 != event_num_col:
+                event[key1] = {}
 
-    except Exception as exc:
-        raise InputError("Cannot convert input value to a numpy data type!") from exc
-
-    return np_dtype
+        for group_name in event:
+            if group_name == event_num_col or not isinstance(event[group_name], dict):
+                continue
+            missing = list(all_subkeys[group_name] - event[group_name].keys())
+            for key in missing:
+                if key != event_num_col:
+                    event[group_name][key] = []
+    return out
```

### Comparing `hepfile-0.1.6/src/hepfile/csv_tools.py` & `hepfile-0.1.7/src/hepfile/csv_tools.py`

 * *Files identical despite different names*

### Comparing `hepfile-0.1.6/src/hepfile/dict_tools.py` & `hepfile-0.1.7/src/hepfile/dict_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Functions to help convert dictionaries into hepfiles
 """
 from __future__ import annotations
 
-import warnings
 import numpy as np
 
 import hepfile as hf
 from hepfile.errors import (
     AwkwardStructureError,
     DictStructureError,
     InputError,
@@ -30,25 +29,26 @@
     This wraps on `hepfile.awkward_tools.awkward_to_hepfile`
     and writes a list of dictionaries to a hepfile.
 
     Writes a list of dictlike object to a hepfile. Must have a specific format:
     - each dictlike object is a "event"
     - first level of dict keys are the groups
     - second level of dict keys are the datasets
-    - entries in second level of dict object is the data and can be either awkward arrays or lists
+    - entries in second level of dict object is the data (awkward array or list)
     - data entries in the first level of the dict are singleton objects
 
     Args:
         dict_list (list): list of dictionaries or dataframes where each dictionary/df
                           holds information on an event
         outfile (str): path to write output hepfile to
-        how_to_pack (str): how to pack the input dataset. Options are 'awkward' or 'classic'.
-                      'awkward' called awkward_to_hepfile, 'classic' does it more traditional.
-                      default is 'classic'. To use how_to_pack='awkward', make sure you
-                      installed hepfile with the 'awkward' or 'all' optional dependency!
+        how_to_pack (str): how to pack the input dataset. Options are 'awkward'
+                           or 'classic'. 'awkward' called awkward_to_hepfile,
+                           'classic' does it more traditional. default is 'classic'.
+                           To use how_to_pack='awkward', make sure you installed
+                           hepfile with the 'awkward' or 'all' optional dependency!
         **kwargs: passed to `hepfile.write.write_to_file` if 'awkward'. Can only be
                   'write_to_hepfile' and 'ignore_protected' if 'classic'.
     Returns:
         Dictionary of Awkward Arrays with the data stored in outfile
     """
 
     # check if it is a list of dictionaries or dataframe
@@ -80,15 +80,15 @@
 
     raise InputError("how_to_pack should either be 'awkward' or 'classic'")
 
 
 def _classic(
     dict_list: dict, outfile: str = None, write_hepfile=True, ignore_protected=False
 ) -> dict:
-    """Private method to convert a list of events to a hepfile using the traditional method"""
+    """Private method to convert a list of events to a hepfile using loop+pack method"""
 
     if outfile is None and write_hepfile:
         raise InputError("if write_hepfile is True, and outfile name must be provided")
 
     # first create the group names and dataset names
     data = initialize()
     for group_name in dict_list[0]:
@@ -117,27 +117,27 @@
 
             test_list = temp_dict[group_name][dataset_name]
 
             dtype = _get_dtype(test_list)
             create_dataset(data, dataset_name, group=group_name, dtype=dtype)
 
     # now pack the data from each data dictionary
+    bucket = create_single_bucket(data)
     for data_dict in dict_list:
-        bucket = create_single_bucket(data)
         for group in data_dict:
             group_name = group.replace("/", "-")
             if group in bucket["_GROUPS_"]["_SINGLETONS_GROUP_"]:
                 bucket[group_name] = data_dict[group]
                 continue
 
             if isinstance(data_dict, dict):  # make sure this isn't a singleton
                 for dataset in data_dict[group]:
                     dataset_name = dataset.replace("/", "-")
                     name = f"{group}/{dataset_name}"
-                    bucket[name] = data_dict[group][dataset]
+                    bucket[name] = list(data_dict[group][dataset])
         pack(data, bucket)
 
     # finally write the data out to a file
     if write_hepfile:
         write_to_file(outfile, data)
     return data
 
@@ -145,48 +145,49 @@
 def _awkward(dict_list: list[dict], outfile: str = None, **kwargs):
     """Private method to convert a list of events to a hepfile using awkward arrays"""
 
     if not hf._AWKWARD:
         raise MissingOptionalDependency("awkward")
 
     import awkward as ak
-    from hepfile.awkward_tools import awkward_to_hepfile, _is_valid_awkward
+    from hepfile.awkward_tools import awkward_to_hepfile
 
     # convert dictionary list to  an awkward array and write to hepfile
     out_ak = ak.Array(dict_list)
 
     # catch an awkward structure error and instead return a dictionary structure error
     try:
         awkward_to_hepfile(out_ak, outfile, **kwargs)
     except AwkwardStructureError as err:
         raise DictStructureError(err) from err
 
     return out_ak
 
 
-def append(ak_dict: ak.Record, new_dict: dict) -> ak.Record:
+def append(ak_dict: ak.Record, new_dict: dict) -> ak.Record:  # noqa: F821
     """
     Append a new event to an existing awkward dictionary with events
 
     Note: This tool requires awkward to be installed. Make sure you installed with
     either
     1) 'python -m pip install hepfile[awkward]' or,
     2) 'python -m pip install hepfile[all]'
 
     Args:
         ak_dict (ak.Record): awkward Record of data
-        new_dict (dict): Dictionary of value to append to ak_dict. All keys must match ak_dict!
+        new_dict (dict): Dictionary of value to append to ak_dict.
+                         All keys must match ak_dict!
     Return:
         Awkward Record of awkward arrays with the new_dict appended
     """
     if not hf._AWKWARD:
         raise MissingOptionalDependency("awkward")
 
     import awkward as ak
-    from hepfile.awkward_tools import awkward_to_hepfile, _is_valid_awkward
+    from hepfile.awkward_tools import _is_valid_awkward
 
     _is_valid_awkward(ak_dict)
 
     if sorted(list(new_dict.keys())) != sorted(ak_dict.fields):
         raise InputError(
             f"Keys of new array do not match keys of existing array!\nExisting \
             Array Keys: {ak_dict.fields}\nNew Dictionary Keys: {new_dict.keys()}"
```

### Comparing `hepfile-0.1.6/src/hepfile/errors.py` & `hepfile-0.1.7/src/hepfile/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,13 +78,14 @@
 class MissingOptionalDependency(ImportError):
     """
     Thrown when the user tries to use an optional part of the package that was
     not installed when they installed.
     """
 
     def __init__(self, module):
-        self.err = f"{module} is not supported with this distribution of hepfile. Please reinstall with one of the following options \n\
+        self.err = f"{module} is not supported with this distribution of hepfile. \
+        Please reinstall with one of the following options \n \
         1) pip install hepfile[{module}]  \n\
         2) pip install hepfile[all]"
 
     def __str__(self):
         return self.err
```

### Comparing `hepfile-0.1.6/src/hepfile/read.py` & `hepfile-0.1.7/src/hepfile/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,24 +36,25 @@
 
         verbose (boolean): True if debug output is required
 
         desired_groups (list): Groups to be read from input file,
 
         subset (int): Number of buckets to be read from input file
 
-        return_type (str): Type to return. Options are 'dictionary', 'awkward', and 'pandas'.
-                           Default is 'dictionary'. Note: the 'awkward' option requires
-                           hepfile to be installed with the awkward or all option and the
-                           'pandas' option requires hepfile to be installed with the pandas
-                           or all option!
+        return_type (str): Type to return. Options are 'dictionary', 'awkward', and '
+                           'pandas'. Default is 'dictionary'. Note: the 'awkward' option
+                           requires hepfile to be installed with the awkward or all
+                           option and the 'pandas' option requires hepfile to be
+                           installed with the pandas or all option!
 
     Returns:
         data (dict): Selected data from HDF5 file
 
-        bucket (dict): An empty bucket dictionary to be filled by data from select buckets
+        bucket (dict): An empty bucket dictionary to be filled by data from
+                       select buckets
 
     """
 
     if return_type not in {"dictionary", "awkward", "pandas"}:
         raise InputError("return_type must be dictionary, awkward, or pandas")
 
     if return_type == "awkward" and not hf._AWKWARD:
@@ -84,15 +85,15 @@
             if isinstance(subset, tuple):
                 subset = list(subset)
 
             if isinstance(subset, int):
                 if verbose:
                     warning = "\n".join(
                         (
-                            "Single subset value of {subset} being interpreted as a high range",
+                            f"Single subset value ({subset}) being used as high range",
                             f"subset being set to a range of (0,{subset})\n",
                         )
                     )
                     warnings.warn(warning)
 
                 subset = [0, subset]
 
@@ -123,15 +124,16 @@
 
             data["_NUMBER_OF_BUCKETS_"] = subset[1] - subset[0]
             nbuckets = data["_NUMBER_OF_BUCKETS_"]
 
             if verbose:
                 print("Will read in a subset of the file!")
                 print(
-                    f"From bucket {subset[0]} (inclusive) through bucket {subset[1]-1} (inclusive)"
+                    f"From bucket {subset[0]} (inclusive) through bucket"
+                    + f"{subset[1]-1} (inclusive)"
                 )
                 print(f"Bucket {subset[1]} is not read in")
                 print(f"Reading in {nbuckets} buckets\n")
 
         ############################################################################
         # Get the datasets and counters
         ############################################################################
@@ -246,16 +248,16 @@
             full_file_index = calculate_index_from_counters(full_file_counters)
 
             if verbose:
                 print(f"full file counters: {full_file_counters}\n")
                 print(f"full file index: {full_file_index}\n")
 
             if subset is not None:
-                # We tack on +1 to the high range of subset when we pull out the counters
-                # and index because we want to get all of the entries for the last entry.
+                # We tack on +1 to the high range of subset when we get the counters
+                # and index because we want all of the entries for the last entry.
                 data[counter_name] = infile[counter_name][subset[0] : subset[1] + 1]
                 index = full_file_index[subset[0] : subset[1] + 1]
             else:
                 data[counter_name] = infile[counter_name][:]
                 index = full_file_index
 
             subset_index = index
@@ -304,26 +306,30 @@
                         lo = subset[0]
                         hi = subset[1]
                     else:
                         lo = full_file_indices[index_name][0]
                         hi = full_file_indices[index_name][-1]
                     if verbose:
                         print(f"dataset name/lo/hi: {dataset_name},{lo},{hi}\n")
-                    data[dataset_name] = dataset[lo:hi]
+                    data[dataset_name] = dataset[int(lo) : int(hi)]
                 else:
                     data[dataset_name] = dataset[:]
 
                 bucket[dataset_name] = None  # This will be filled for individual bucket
                 if verbose:
                     print(dataset)
 
             # write the metadata for that group to data if it exists
             if name not in constants.protected_names and "meta" in dataset.attrs.keys():
                 data["_META_"][name] = dataset.attrs["meta"]
 
+        # Add the GROUPS field to the bucket. It's a bit of extra data
+        # that most of the time is not needed, but can be helpful for
+        # if we want to convert the bucket to a dataframe.
+
     if verbose:
         print("Data is read in and input file is closed.")
 
     # edit data so it matches the format of the data dict that was saved to the file
     # this makes it so that data can be directly passed to write_to_file
     # 1) add back in _GROUP_
     datasets = np.array(data["_LIST_OF_DATASETS_"])
@@ -404,21 +410,27 @@
                      dictionary and inserted into the bucket dictionary.
 
     """
 
     keys = bucket.keys()
 
     for key in keys:
-        # if "num" in key:
+
+        # BELLIS EDITS TRYING SOMETHING OUT
+        if key == '_GROUPS_' or key == '_MAP_DATASETS_TO_COUNTERS_':
+            continue
+
         # IS THERE A WAY THAT THIS COULD BE FASTER?
         # print(data['_LIST_OF_COUNTERS_'],key)
+        # unpack the singletons and the counters (which are themselves 
+        # singletons, effectively)
         if key in data["_LIST_OF_COUNTERS_"] or key in data["_SINGLETONS_GROUP_"]:
             bucket[key] = data[key][n]
 
-        elif "INDEX" not in key:  # and 'Jets' in key:
+        elif "INDEX" not in key:
             indexkey = data["_MAP_DATASETS_TO_INDEX_"][key]
             numkey = data["_MAP_DATASETS_TO_COUNTERS_"][key]
 
             if len(data[indexkey]) > 0:
                 index = data[indexkey][n]
 
             if len(data[numkey]) > 0:
```

### Comparing `hepfile-0.1.6/src/hepfile/write.py` & `hepfile-0.1.7/src/hepfile/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,21 @@
     data["_META_"] = {}
 
     return data
 
 
 ################################################################################
 def clear_bucket(bucket: dict) -> None:
-    """Clears the data from the bucket dictionary - should the name of the function change?
+    """
+    Clears the data from the bucket dictionary - should the name of the function change?
 
     Args:
-        bucket (dict): The dictionary to be cleared. This is designed to clear the data from
-                      the lists in the bucket dictionary, but theoretically, it would
-                      clear out the lists from any dictionary.
+        bucket (dict): The dictionary to be cleared. This is designed to clear the
+                      data from the lists in the bucket dictionary, but theoretically,
+                      it would clear out the lists from any dictionary.
 
     """
 
     for key in bucket.keys():
         if key == "_LIST_OF_COUNTERS_":
             continue
 
@@ -168,19 +169,23 @@
                 "The new name will be {new_counter_name}",
                 "----------------------------------------------------",
             )
         )
         warnings.warn(warning)
         counter_name = new_counter_name
 
-    keys = data.keys()
+    data.keys()
 
     # Then put the group and any datasets in there next.
     if group_name in data["_GROUPS_"]:
-        raise ValueError(f"\033[1m{group_name}\033[0m is already in the dictionary!")
+        warning = (
+            f"\033[1m{group_name}\033[0m is already in the dictionary! Not Adding!"
+        )
+        warnings.warn(warning)
+        return
 
     data["_GROUPS_"][group_name] = []
     if verbose:
         print(f"Adding group \033[1m{group_name}\033[0m")
 
     data["_GROUPS_"][group_name].append(counter_name)
     full_counter_name = f"{group_name}/{counter_name}"
@@ -190,56 +195,60 @@
 
     if full_counter_name not in data["_LIST_OF_COUNTERS_"]:
         data["_LIST_OF_COUNTERS_"].append(full_counter_name)
 
     data[full_counter_name] = []
     if verbose:
         print(
-            f"Adding a counter for \033[1m{group_name}\033[0m as \033[1m{counter_name}\033[0m"
+            f"Adding a counter for \033[1m{group_name}\033[0m "
+            + "as \033[1m{counter_name}\033[0m"
         )
 
 
 ################################################################################
 
 
 ################################################################################
 # This adds a dataset to the dictionary, similar to
 # a la CreateBranch in ROOT
 #
 # This can also add a dataset that is not associate with a group
 ################################################################################
 def create_dataset(
     data: dict,
-    datasets: list,
+    dset_name: list,
     group: str = None,
     dtype: type = float,
     verbose=False,
     ignore_protected=False,
 ):
-    """Adds a dataset to a group in a dictionary. If the group does not exist, it will be created.
+    """
+    Adds a dataset to a group in a dictionary.
+    If the group does not exist, it will be created.
 
     Args:
         data (dict): Dictionary that contains the group
 
-        datasets (list): Dataset to be added to the group (This doesn't have to be a list)
+        dset_name (list/str): Dataset to be added to the group
+                              (This doesn't have to be a list)
 
         group (string): Name of group the dataset will be added to.  None by default
 
         dtype (type): The data type. None by default - I don't think this is every used
 
     Returns:
         -1: If the group is None
 
     """
 
-    if not isinstance(datasets, list):
-        datasets = [datasets]
+    if not isinstance(dset_name, list):
+        dset_name = [dset_name]
 
     # Check for slashes in the dataset name. We can't have them.
-    for i, tempname in enumerate(datasets):
+    for i, tempname in enumerate(dset_name):
         # check that tempname isn't in protected_names
         if not ignore_protected and tempname in constants.protected_names:
             raise InputError(
                 f"{tempname} is protected, please choose a different dataset name!"
             )
 
         if "/" in tempname:
@@ -250,30 +259,31 @@
                     "Slashes / are not allowed in dataset names",
                     f"Replacing / with - in dataset name {tempname}",
                     f"The new name will be {new_dataset_name}",
                     "----------------------------------------------------",
                 )
             )
             warnings.warn(warning)
-            datasets[i] = new_dataset_name
+            dset_name[i] = new_dataset_name
 
     keys = data.keys()
 
     # These will be entries for the SINGLETON_GROUP, if there is no group passed in
     if group is None:
-        for dataset in datasets:
+        for dataset in dset_name:
             if dataset in data["_GROUPS_"]["_SINGLETONS_GROUP_"]:
                 warnings.warn(
                     f"\033[1m{dataset}\033[0m is already in the dictionary! Skipping!"
                 )
                 continue
 
             if verbose:
                 print(
-                    f"Adding dataset \033[1m{dataset}\033[0m to the dictionary as a SINGLETON."
+                    f"Adding dataset \033[1m{dataset}\033[0m to the dictionary "
+                    + "as a SINGLETON."
                 )
             data["_GROUPS_"]["_SINGLETONS_GROUP_"].append(dataset)
             data[dataset] = []
             data["_MAP_DATASETS_TO_COUNTERS_"][dataset] = "_SINGLETONS_GROUP_/COUNTER"
 
             data["_MAP_DATASETS_TO_DATA_TYPES_"][dataset] = dtype
 
@@ -284,15 +294,15 @@
         counter = f"N_{group}"
         warnings.warn(
             f"Your group, \033[1m{group}\033[0m is not in the dictionary yet! \
             Adding it, along with a counter of \033[1m{counter}\033[0m"
         )
         create_group(data, group, counter=counter)
 
-    for dataset in datasets:
+    for dataset in dset_name:
         name = f"{group}/{dataset}"
 
         # check that tempname isn't in protected_names
         if not ignore_protected and name in constants.protected_names:
             raise InputError(
                 f"{name} is protected, please choose a different dataset or group name!"
             )
@@ -322,16 +332,17 @@
 ###############################################################################
 def add_meta(data: dict, name: str, meta_data: list):
     """
     Create metadata for a group (or singleton) and add it to data
 
     Args:
         data (dict): a data object returned by hf.initialize()
-        name (str): name of either a group, singleton, or dataset the metadata corresponds to.
-                    if passing a dataset name, make sure it is the full path (group/dataset)!
+        name (str): name of either a group, singleton, or dataset the metadata
+                    corresponds to. if passing a dataset name, make sure it is the full
+                    path (group/dataset)!
         meta_data (list): list of metadata to write to that group/dataset/singleton
     """
 
     if name in data["_META_"].keys():
         warnings.warn(
             f"This name {name} already has metadata in the hepfile data, skipping!"
         )
@@ -413,15 +424,16 @@
                         # Don't worry about the dataset
                         if counter == temp_full_dataset_name:
                             continue
                         err += f"{tempd}: {len(bucket[temp_full_dataset_name])}\n"
 
                     # Raise an exception for the external program to catch.
                     raise DatasetSizeDiscrepancy(
-                        f"Oh no!!!! Two datasets in group {group} have different sizes! {err}"
+                        f"Oh no!!!! Two datasets in group {group} "
+                        + f"have different sizes! {err}"
                     )
 
     # Then pack the bucket into the data
     keys = list(bucket.keys())
 
     for key in keys:
         if key in {
@@ -435,52 +447,67 @@
             "_LIST_OF_DATASETS",
             "_SINGLETONS_GROUP_",
             "_HEADER_",
             "_NUMBER_OF_BUCKETS_",
         }:
             continue
 
-        if isinstance(data[key], np.ndarray):
-            data[key] = data[key].tolist()
-
-        if isinstance(bucket[key], np.ndarray):
-            bucket[key] = bucket[key].tolist()
-
         # The singletons will only have 1 entry per bucket
         if key == "_SINGLETONS_GROUP_/COUNTER":
-            data[key].append(1)
+            # import pdb; pdb.set_trace()
+            data[key] = _append(data[key], 1)  # np.append(data[key], 1).astype(int)
             continue
 
-        if isinstance(bucket[key], list):
+        if isinstance(bucket[key], (list, np.ndarray)):
             value = bucket[key]
             if len(value) > 0:
-                data[key] += value
+                data[key] = _append(
+                    data[key], value
+                )  # np.append(data[key], value)  # += value
         else:
             # This is for counters and SINGLETONS
             if key in data["_GROUPS_"]["_SINGLETONS_GROUP_"]:
                 if bucket[key] is None:
                     raise MissingSingletonValue(
-                        f"\n\033[1m{key}\033[0m is part of the SINGLETON group \
-                        and is expected to have a value for each bucket. However it is None!"
+                        f"\n\033[1m{key}\033[0m is part of the SINGLETON group "
+                        + "and is expected to have a value for each bucket. "
+                        + "However it is None!"
                     )
 
                 # Append the single value from the singletons
-                data[key].append(bucket[key])
+                data[key] = _append(
+                    data[key], bucket[key]
+                )  # np.append(data[key], bucket[key])
             # Append the values to the counters
             else:
-                data[key].append(bucket[key])
+                data[key] = _append(data[key], bucket[key])  # .astype(int)
 
     # Clear out the bucket after it's been packed if that's what we want
     if EMPTY_OUT_BUCKET:
         clear_bucket(bucket)
 
 
 ################################################################################
 
 
+def _append(data, bucket):
+    if isinstance(data, np.ndarray):
+        return np.append(data, bucket)
+    elif isinstance(data, list):
+        if isinstance(bucket, np.ndarray):
+            return np.append(data, bucket)
+        elif isinstance(bucket, list):
+            return data + bucket
+        else:  # these are values like counters or singletons
+            data.append(bucket)
+            return data
+    else:
+        raise ValueError("data should be a list or numpy array!")
+
+
 def _convert_list_and_key_to_string_data(datalist: list[any], key: str) -> str:
     """Converts data dictionary to a string
 
     Args:
         datalist (list): A list to be saved as a string.
 
     Returns:
@@ -678,15 +705,16 @@
     Args:
         filename (string): Name of output file
 
         data (dictionary): Data to be written into output file
 
         comp_type (string): Type of compression
 
-        force_single_precision (boolean): True if data should be written in single precision
+        force_single_precision (boolean): True if data should be written in single
+                                          precision
 
     Returns:
         hdoutfile (HDF5): File to which the data has been written
 
     """
 
     # hdoutfile = h5.File(filename, "w")
@@ -755,17 +783,19 @@
                 # Do single precision only, unless specified
                 if force_single_precision:
                     # different type calls depending on input datastructure
                     if isinstance(x, np.ndarray):
                         dtype = x.dtype
                     else:
                         dtype = None
-                        warnings.warn(
-                            "Not a proper data type to convert to single precision, skipping!"
-                        )
+                        if verbose:
+                            warnings.warn(
+                                "Not a proper data type to convert to single precision,"
+                                + " skipping!"
+                            )
 
                     if dtype == np.float64:
                         if verbose:
                             print("\tConverting array to single precision...")
                         x = x.astype(np.float32)
                         dataset_dtype = np.float32
 
@@ -783,14 +813,17 @@
                     # For writing strings, we need to make sure our strings are ascii
                     # and not Unicode
                     #
                     # See my question on StackOverflow and the super-helpful response!
                     #
                     # https://stackoverflow.com/questions/68500454/can-i-use-h5py-to-write-strings-to-an-hdf5-file-in-one-line-rather-than-looping
                     dataset_dtype = h5.special_dtype(vlen=str)
+
+                    if not hasattr(x[0], "__len__"):
+                        x = x.astype(str)
                     longest_word = len(max(x, key=len))
                     arr = np.array(x, dtype="S" + str(longest_word))
                     hdoutfile.create_dataset(
                         name,
                         data=arr,
                         dtype=dataset_dtype,
                         compression=comp_type,
@@ -812,15 +845,15 @@
             ncounter = len(data[countername])
 
             if verbose:
                 print(f"{countername:<32s} has {ncounter:<12d} entries")
 
             if i > 0 and ncounter != num_buckets:
                 warnings.warn(
-                    f"{countername} and {prevcounter} have differing numbers of entries!"
+                    f"{countername} and {prevcounter} have differing number of entries!"
                 )
                 # SHOULD WE EXIT ON THIS?
 
             num_buckets = max(num_buckets, ncounter)
 
             prevcounter = countername
```

