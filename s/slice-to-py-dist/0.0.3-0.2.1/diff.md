# Comparing `tmp/slice_to_py_dist-0.0.3.tar.gz` & `tmp/slice_to_py_dist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slice_to_py_dist-0.0.3.tar", max compression
+gzip compressed data, was "slice_to_py_dist-0.2.1.tar", max compression
```

## Comparing `slice_to_py_dist-0.0.3.tar` & `slice_to_py_dist-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1099 2023-07-07 07:26:26.664954 slice_to_py_dist-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6376 2023-07-07 06:27:18.737532 slice_to_py_dist-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-07-04 04:30:11.675500 slice_to_py_dist-0.0.3/slice_to_py_dist/__init__.py
--rw-r--r--   0        0        0     3083 2023-07-06 04:56:29.003197 slice_to_py_dist-0.0.3/slice_to_py_dist/__main__.py
--rw-r--r--   0        0        0     4548 2023-07-07 06:10:58.974792 slice_to_py_dist-0.0.3/slice_to_py_dist/build_sdist.py
--rw-r--r--   0        0        0     2419 2023-07-07 06:10:58.971815 slice_to_py_dist-0.0.3/slice_to_py_dist/custom_build_backend/backend.py
--rw-r--r--   0        0        0      235 2023-07-05 05:00:12.037048 slice_to_py_dist-0.0.3/slice_to_py_dist/types.py
--rw-r--r--   0        0        0      852 2023-07-06 03:54:13.948132 slice_to_py_dist-0.0.3/slice_to_py_dist/utils.py
--rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 slice_to_py_dist-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6376 2023-07-12 09:02:11.606973 slice_to_py_dist-0.2.1/README.md
+-rw-r--r--   0        0        0     1318 2023-07-21 16:10:25.234064 slice_to_py_dist-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 16:09:15.461548 slice_to_py_dist-0.2.1/slice_to_py_dist/__init__.py
+-rw-r--r--   0        0        0     3113 2023-07-12 09:02:11.606973 slice_to_py_dist-0.2.1/slice_to_py_dist/__main__.py
+-rw-r--r--   0        0        0     4547 2023-07-14 03:59:36.872429 slice_to_py_dist-0.2.1/slice_to_py_dist/build_sdist.py
+-rw-r--r--   0        0        0     2735 2023-07-14 03:59:36.872429 slice_to_py_dist-0.2.1/slice_to_py_dist/custom_build_backend/backend.py
+-rw-r--r--   0        0        0      247 2023-07-12 09:02:11.606973 slice_to_py_dist-0.2.1/slice_to_py_dist/types.py
+-rw-r--r--   0        0        0      852 2023-07-12 09:02:11.606973 slice_to_py_dist-0.2.1/slice_to_py_dist/utils.py
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 slice_to_py_dist-0.2.1/PKG-INFO
```

### Comparing `slice_to_py_dist-0.0.3/pyproject.toml` & `slice_to_py_dist-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.poetry]
 name = "slice_to_py_dist"
-version = "0.0.3"
+version = "0.2.1"  # a placeholder; will be set dynamically by poetry-dynamic-versioning
 description = "Put a set of ZeroC/ICE slice files (.ice) into python distribution package."
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 configargparse = "^1.5.5"
 toml = "^0.10.2"
 build = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 black = "^23.3.0"
 pylint = "^2.17.4"
+importlib-resources = "^6.0.0"
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"  # "poetry.core.masonry.api"
+
+[tool.poetry-dynamic-versioning]
+enable = false
 
 [tool.pylint.format]
 max-line-length = 120
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
   "C0114",  # missing-module-docstring
```

### Comparing `slice_to_py_dist-0.0.3/README.md` & `slice_to_py_dist-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.0.3/slice_to_py_dist/__main__.py` & `slice_to_py_dist-0.2.1/slice_to_py_dist/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 """
 Put a set of ZeroC/ICE slice files (.ice) into python distribution package.
 """
 
+from __future__ import annotations
+
 import sys
-from typing import Any, List, Optional, cast
+from typing import Any, Optional, cast
 
 import configargparse  # pyright: ignore[reportMissingTypeStubs]
 
 from slice_to_py_dist.build_sdist import build_sdist
 from slice_to_py_dist.types import DistPackageInfo
 
 
-def parse_args(argv: List[str]) -> configargparse.Namespace:
+def parse_args(argv: list[str]) -> configargparse.Namespace:
     parser = configargparse.ArgumentParser(
         description=__doc__,
         epilog=None,
         formatter_class=configargparse.RawDescriptionHelpFormatter,
         add_help=False,
         config_file_parser_class=configargparse.TomlConfigParser(["main"]),
     )
@@ -89,15 +91,15 @@
         help="""The name of the additional import package which will store input slice files.""",
     )
 
     args: Any = parser.parse_args(argv)  # pyright: ignore[reportUnknownMemberType]
     return cast(configargparse.Namespace, args)
 
 
-def main(argv: Optional[List[str]] = None) -> int:
+def main(argv: Optional[list[str]] = None) -> int:
     "Main function."
 
     if argv is None:
         argv = sys.argv[1:]
 
     args = parse_args(argv)
```

### Comparing `slice_to_py_dist-0.0.3/slice_to_py_dist/build_sdist.py` & `slice_to_py_dist-0.2.1/slice_to_py_dist/build_sdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from __future__ import annotations
+
 import sys
 import os
 import shutil
 import subprocess
 import tempfile
 from pathlib import Path
-from typing import List
 
 import toml
 
 from slice_to_py_dist.types import DistPackageInfo, SliceToPyDistError
 from slice_to_py_dist.utils import parse_author
 
 
 BACKEND_DIR = "custom_build_backend"  # Must exist next to current __file__
 BACKEND_MODULE = "backend.py"
 
 
 SLICE_SUFFIX = ".ice"
 
 
-def find_slice_files(directory: Path) -> List[Path]:
+def find_slice_files(directory: Path) -> list[Path]:
     slice_files = [p.relative_to(directory) for p in directory.glob(f"**/*{SLICE_SUFFIX}")]
     if len(slice_files) == 0:
         raise SliceToPyDistError(f"Can't find {SLICE_SUFFIX} files under {directory.absolute()}")
     return slice_files
 
 
 def expand_path(path: Path) -> Path:
@@ -53,15 +54,15 @@
             "version": dist_info.version,
             "authors": [parse_author(a) for a in dist_info.authors],
             "description": dist_info.summary,
             "requires-python": dist_info.requires_python,
             "dependencies": ["zeroc-ice"],
         },
         "build-system": {
-            "requires": ["setuptools", "zeroc-ice"],
+            "requires": ["setuptools"],
             "build-backend": os.path.splitext(BACKEND_MODULE)[0],
             "backend-path": [BACKEND_DIR],
         },
     }
     with open(build_dir / "pyproject.toml", "xt", encoding="utf-8") as f:
         toml.dump(data, f)
```

### Comparing `slice_to_py_dist-0.0.3/slice_to_py_dist/custom_build_backend/backend.py` & `slice_to_py_dist-0.2.1/slice_to_py_dist/custom_build_backend/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 import os
 import subprocess
 from pathlib import Path
 from typing import List, Mapping, Optional, Union
 
 from setuptools import build_meta as orig_build_meta
@@ -21,14 +23,21 @@
 class BackendError(Exception):
     pass
 
 
 ConfigSettings = Mapping[str, Union[str, List[str]]]
 
 
+def get_requires_for_build_wheel(config_settings: Optional[ConfigSettings] = None) -> List[str]:
+    # pylint: disable=function-redefined
+    result = orig_build_meta.get_requires_for_build_wheel(config_settings=config_settings)
+    result.append("zeroc-ice")
+    return result
+
+
 def build_wheel(
     wheel_directory: str,
     config_settings: Optional[ConfigSettings] = None,
     metadata_directory: Optional[str] = None,
 ) -> str:
     # pylint: disable=function-redefined
 
@@ -44,15 +53,15 @@
     slice_pkg_dir = Path(".") / slice_storage_pkg_name
     slice_files_rel_paths = [p.relative_to(slice_pkg_dir) for p in slice_pkg_dir.glob(f"**/*{SLICE_SUFFIX}")]
     subprocess_cwd = slice_pkg_dir
     subprocess_output_dir = ".."
 
     # Use --underscore option to permit underscores in the Slice:
     # https://forums.zeroc.com/discussion/5923/slice-illegal-underscore-in-identifier
-    args: List[str] = f"{sys.executable} -m slice2py --underscore -I. --output-dir {subprocess_output_dir}".split()
+    args: list[str] = f"{sys.executable} -m slice2py --underscore -I. --output-dir {subprocess_output_dir}".split()
     args += [str(rel_path) for rel_path in slice_files_rel_paths]
     completed = subprocess.run(args, cwd=subprocess_cwd, check=False)
     if completed.returncode != 0:
         raise BackendError(f"Command {args} failed with code {completed.returncode}")
 
     # Call original setuptools function.
     return orig_build_meta.build_wheel(
```

### Comparing `slice_to_py_dist-0.0.3/slice_to_py_dist/utils.py` & `slice_to_py_dist-0.2.1/slice_to_py_dist/utils.py`

 * *Files identical despite different names*

### Comparing `slice_to_py_dist-0.0.3/PKG-INFO` & `slice_to_py_dist-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slice-to-py-dist
-Version: 0.0.3
+Version: 0.2.1
 Summary: Put a set of ZeroC/ICE slice files (.ice) into python distribution package.
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

