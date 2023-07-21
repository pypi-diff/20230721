# Comparing `tmp/bcpandas-2.4.1.tar.gz` & `tmp/bcpandas-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcpandas-2.4.1.tar", max compression
+gzip compressed data, was "bcpandas-2.4.2.tar", max compression
```

## Comparing `bcpandas-2.4.1.tar` & `bcpandas-2.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-07-12 06:14:03.708241 bcpandas-2.4.1/LICENSE
--rw-r--r--   0        0        0    16614 2023-07-12 06:14:03.708241 bcpandas-2.4.1/README.md
--rw-r--r--   0        0        0      563 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/__init__.py
--rw-r--r--   0        0        0     2339 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/constants.py
--rw-r--r--   0        0        0    17016 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/main.py
--rw-r--r--   0        0        0     8288 2023-07-12 06:14:03.708241 bcpandas-2.4.1/bcpandas/utils.py
--rw-r--r--   0        0        0     2510 2023-07-12 06:14:20.780206 bcpandas-2.4.1/pyproject.toml
--rw-r--r--   0        0        0    17676 1970-01-01 00:00:00.000000 bcpandas-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-21 02:45:58.262030 bcpandas-2.4.2/LICENSE
+-rw-r--r--   0        0        0    16614 2023-07-21 02:45:58.262030 bcpandas-2.4.2/README.md
+-rw-r--r--   0        0        0      563 2023-07-21 02:45:58.262030 bcpandas-2.4.2/bcpandas/__init__.py
+-rw-r--r--   0        0        0     2339 2023-07-21 02:45:58.262030 bcpandas-2.4.2/bcpandas/constants.py
+-rw-r--r--   0        0        0    17196 2023-07-21 02:45:58.262030 bcpandas-2.4.2/bcpandas/main.py
+-rw-r--r--   0        0        0     8347 2023-07-21 02:45:58.262030 bcpandas-2.4.2/bcpandas/utils.py
+-rw-r--r--   0        0        0     2510 2023-07-21 02:46:19.162306 bcpandas-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0    17676 1970-01-01 00:00:00.000000 bcpandas-2.4.2/PKG-INFO
```

### Comparing `bcpandas-2.4.1/LICENSE` & `bcpandas-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.1/README.md` & `bcpandas-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.1/bcpandas/__init__.py` & `bcpandas-2.4.2/bcpandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.1/bcpandas/constants.py` & `bcpandas-2.4.2/bcpandas/constants.py`

 * *Files identical despite different names*

### Comparing `bcpandas-2.4.1/bcpandas/main.py` & `bcpandas-2.4.2/bcpandas/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import csv
 import logging
 import os
 from pathlib import Path
 from textwrap import dedent
 from typing import Dict, List, Optional, Union
 from urllib.parse import quote_plus
+from re import sub
 
 import pandas as pd
 from pandas.io.sql import SQLDatabase, SQLTable
 import pyodbc
 import sqlalchemy as sa
 
 from bcpandas.constants import (
@@ -101,23 +102,25 @@
             db_url += f"UID={username};PWD={password};"
         else:
             self.username = ""
             self.password = ""
             self.with_krb_auth = True
             db_url += "Trusted_Connection=yes;"
 
-        logger.info(f"Created creds:\t{self}")
+        self_msg = sub(r"password=\'.*\'", "password=[REDACTED]", str(self))
+        logger.info(f"Created creds:\t{self_msg}")
 
         # construct the engine for sqlalchemy
         if odbc_kwargs:
             db_url += ";".join(f"{k}={v}" for k, v in odbc_kwargs.items())
         conn_string = f"mssql+pyodbc:///?odbc_connect={quote_plus(db_url)}"
         self.engine = sa.engine.create_engine(conn_string)
+        engine_msg = sub("PWD%3D.*%3B", "PWD%3D[REDACTED]%3B", str(self.engine))
 
-        logger.info(f"Created engine for sqlalchemy:\t{self.engine}")
+        logger.info(f"Created engine for sqlalchemy:\t{engine_msg}")
 
     @classmethod
     def from_engine(cls, engine: sa.engine.base.Engine) -> "SqlCreds":
         """
         Alternate constructor, from a `sqlalchemy.engine.base.Engine` that uses `pyodbc` as the DBAPI
         (which is the SQLAlchemy default for MS SQL) and using an exact PyODBC connection string (not DSN or hostname).
         See https://docs.sqlalchemy.org/en/13/dialects/mssql.html#connecting-to-pyodbc for more.
```

### Comparing `bcpandas-2.4.1/bcpandas/utils.py` & `bcpandas-2.4.2/bcpandas/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pathlib import Path
 import random
 import shlex
 import string
 from subprocess import PIPE, STDOUT, Popen
 import tempfile
 from typing import Dict, List, Optional, Tuple, Union
+from re import sub
 
 import pandas as pd
 
 from bcpandas.constants import (
     DIRECTIONS,
     IN,
     IS_WIN32,
@@ -120,16 +121,17 @@
             ),
             quote_this(
                 f"-r{read_data_settings['newline'] if row_terminator is None else row_terminator}"
             ),
         ]
 
     # execute
-    bcp_command_log = [c if c != creds.password else "[REDACTED]" for c in bcp_command]
-    logger.info(f"Executing BCP command now... \nBCP command is: {bcp_command_log}")
+    bcp_command_log = ", ".join(bcp_command)
+    bcp_command_log_msg = sub(r"-P,\s.*,", "-P, [REDACTED],", bcp_command_log)
+    logger.info(f"Executing BCP command now... \nBCP command is: {bcp_command_log_msg}")
     ret_code, output = run_cmd(bcp_command, print_output=print_output)
     if ret_code != 0:
         raise BCPandasException(
             f"Bcp command failed with exit code {ret_code}",
             details=[line for line in output if line.startswith("Error =")],
         )
```

### Comparing `bcpandas-2.4.1/pyproject.toml` & `bcpandas-2.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 description = "High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!"
 keywords = ["bcp", "mssql", "pandas"]
 license = "MIT"
 maintainers = ["Oliver Borchert <me@borchero.com>"]
 name = "bcpandas"
 readme = "README.md"
 repository = "https://github.com/yehoshuadimarsky/bcpandas"
-version = "v2.4.1"
+version = "v2.4.2"
 
 [tool.poetry.plugins."pandas.sql.engine"]
 bcpandas = "bcpandas.main:to_sql"
 
 [tool.poetry.dependencies]
 pandas = ">=1.5"
 pyodbc = "*"
```

### Comparing `bcpandas-2.4.1/PKG-INFO` & `bcpandas-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcpandas
-Version: 2.4.1
+Version: 2.4.2
 Summary: High-level wrapper around BCP for high performance data transfers between pandas and SQL Server. No knowledge of BCP required!!
 Home-page: https://github.com/yehoshuadimarsky/bcpandas
 License: MIT
 Keywords: bcp,mssql,pandas
 Author: yehoshuadimarsky
 Maintainer: Oliver Borchert
 Maintainer-email: me@borchero.com
```

