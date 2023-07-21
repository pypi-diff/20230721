# Comparing `tmp/gridworks_cert-0.1.0.tar.gz` & `tmp/gridworks_cert-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_cert-0.1.0.tar", max compression
+gzip compressed data, was "gridworks_cert-0.2.0.tar", max compression
```

## Comparing `gridworks_cert-0.1.0.tar` & `gridworks_cert-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-19 15:19:38.126045 gridworks_cert-0.1.0/LICENSE
--rw-r--r--   0        0        0     3822 2023-07-19 15:20:01.978072 gridworks_cert-0.1.0/README.md
--rw-r--r--   0        0        0     2043 2023-07-19 15:20:01.982071 gridworks_cert-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-19 15:19:38.126045 gridworks_cert-0.1.0/src/gwcert/__init__.py
--rw-r--r--   0        0        0      381 2023-07-19 15:20:01.982071 gridworks_cert-0.1.0/src/gwcert/__main__.py
--rw-r--r--   0        0        0       99 2023-07-19 15:19:38.126045 gridworks_cert-0.1.0/src/gwcert/ca/__init__.py
--rw-r--r--   0        0        0     7354 2023-07-19 15:20:01.982071 gridworks_cert-0.1.0/src/gwcert/ca/__main__.py
--rw-r--r--   0        0        0        0 2023-07-19 15:19:38.126045 gridworks_cert-0.1.0/src/gwcert/py.typed
--rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 gridworks_cert-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-21 15:12:20.887634 gridworks_cert-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3822 2023-07-21 15:12:20.887634 gridworks_cert-0.2.0/README.md
+-rw-r--r--   0        0        0     2081 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-21 15:12:20.891634 gridworks_cert-0.2.0/src/gwcert/ca/__init__.py
+-rw-r--r--   0        0        0     7319 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/ca/__main__.py
+-rw-r--r--   0        0        0      101 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/key/__init__.py
+-rw-r--r--   0        0        0    19855 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/key/__main__.py
+-rw-r--r--   0        0        0      196 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/paths.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:12:20.891634 gridworks_cert-0.2.0/src/gwcert/py.typed
+-rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 gridworks_cert-0.2.0/PKG-INFO
```

### Comparing `gridworks_cert-0.1.0/LICENSE` & `gridworks_cert-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.1.0/README.md` & `gridworks_cert-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.1.0/pyproject.toml` & `gridworks_cert-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-cert"
-version = "0.1.0"
+version = "0.2.0"
 description = "gwcert"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/anschweitzer/gridworks-cert"
 repository = "https://github.com/anschweitzer/gridworks-cert"
 documentation = "https://gridworks-cert.readthedocs.io"
@@ -50,15 +50,15 @@
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 
 [tool.poetry.scripts]
 gwcert = "gwcert.__main__:app"
 gwcert-ca = "gwcert.ca.__main__:app"
-
+gwcert-key = "gwcert.key.__main__:app"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `gridworks_cert-0.1.0/src/gwcert/ca/__main__.py` & `gridworks_cert-0.2.0/src/gwcert/ca/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,36 @@
 import shutil
 from pathlib import Path
 from typing import Annotated
 from typing import List
 from typing import Optional
 
 import typer
-import xdg
 from ownca import CertificateAuthority
 from ownca._constants import CA_CERT  # noqa
 from ownca._constants import CA_CERTS_DIR  # noqa
 from ownca._constants import CA_CRL  # noqa
 from ownca._constants import CA_CSR  # noqa
 from ownca._constants import CA_KEY  # noqa
 from ownca._constants import CA_PUBLIC_KEY  # noqa
 from ownca.utils import ownca_directory
 from rich import print
 
+from gwcert.paths import DEFAULT_CA_DIR
+
 
 app = typer.Typer(
     no_args_is_help=True,
     pretty_exceptions_enable=False,
     rich_markup_mode="rich",
     help="""
     Commands for creating and using a local Certificate Authority.
     """,
 )
 
-DEFAULT_CA_DIR = Path(xdg.xdg_data_home()) / "gridworks" / "ca"
-
 
 @app.command()
 def clean(
     ca_dir: Annotated[
         Path, typer.Option(help="CA storage directory.")
     ] = DEFAULT_CA_DIR,
     yes_really_forever: Annotated[
```

### Comparing `gridworks_cert-0.1.0/PKG-INFO` & `gridworks_cert-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-cert
-Version: 0.1.0
+Version: 0.2.0
 Summary: gwcert
 Home-page: https://github.com/anschweitzer/gridworks-cert
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

