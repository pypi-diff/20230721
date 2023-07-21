# Comparing `tmp/timedctl-3.5.0.tar.gz` & `tmp/timedctl-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-3.5.0.tar", max compression
+gzip compressed data, was "timedctl-3.5.1.tar", max compression
```

## Comparing `timedctl-3.5.0.tar` & `timedctl-3.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-07-21 07:55:51.374431 timedctl-3.5.0/LICENSE
--rw-r--r--   0        0        0      810 2023-07-21 07:55:51.374431 timedctl-3.5.0/README.md
--rw-r--r--   0        0        0      849 2023-07-21 07:55:52.178449 timedctl-3.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 07:55:51.374431 timedctl-3.5.0/timedctl/__init__.py
--rw-r--r--   0        0        0    36864 2023-07-21 07:55:51.374431 timedctl-3.5.0/timedctl/http_cache.sqlite
--rwxr-xr-x   0        0        0    16931 2023-07-21 07:55:51.374431 timedctl-3.5.0/timedctl/timedctl.py
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-21 11:07:39.703091 timedctl-3.5.1/LICENSE
+-rw-r--r--   0        0        0      810 2023-07-21 11:07:39.703091 timedctl-3.5.1/README.md
+-rw-r--r--   0        0        0      849 2023-07-21 11:07:40.495108 timedctl-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 11:07:39.703091 timedctl-3.5.1/timedctl/__init__.py
+-rw-r--r--   0        0        0    36864 2023-07-21 11:07:39.703091 timedctl-3.5.1/timedctl/http_cache.sqlite
+-rwxr-xr-x   0        0        0    16931 2023-07-21 11:07:39.703091 timedctl-3.5.1/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-3.5.1/PKG-INFO
```

### Comparing `timedctl-3.5.0/LICENSE` & `timedctl-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-3.5.0/README.md` & `timedctl-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-3.5.0/pyproject.toml` & `timedctl-3.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timedctl"
-version = "3.5.0"
+version = "3.5.1"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timedctl-3.5.0/timedctl/http_cache.sqlite` & `timedctl-3.5.1/timedctl/http_cache.sqlite`

 * *Files identical despite different names*

### Comparing `timedctl-3.5.0/timedctl/timedctl.py` & `timedctl-3.5.1/timedctl/timedctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["ac"])
 def activity():
     """Do stuff with activities."""
     pass  # pylint: disable=W0107
 
 
-@activity.command(aliases=["add", "s"])
+@activity.command(aliases=["add", "a"])
 @click.argument("comment")
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
 def start(comment, customer, project, task):
     """Start recording activity."""
     customers = timed.customers.get(cached=True)
```

### Comparing `timedctl-3.5.0/PKG-INFO` & `timedctl-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 3.5.0
+Version: 3.5.1
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

