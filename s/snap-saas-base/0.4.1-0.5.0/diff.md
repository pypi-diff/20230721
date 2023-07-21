# Comparing `tmp/snap_saas_base-0.4.1.tar.gz` & `tmp/snap_saas_base-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snap_saas_base-0.4.1.tar", max compression
+gzip compressed data, was "snap_saas_base-0.5.0.tar", max compression
```

## Comparing `snap_saas_base-0.4.1.tar` & `snap_saas_base-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4822 2023-07-15 17:52:18.542059 snap_saas_base-0.4.1/README.md
--rw-r--r--   0        0        0     4202 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/__init__.py
--rw-r--r--   0        0        0       30 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/__init__.py
--rw-r--r--   0        0        0     2153 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/base_model.py
--rw-r--r--   0        0        0     5740 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/organization.py
--rw-r--r--   0        0        0     3300 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/user.py
--rw-r--r--   0        0        0     6632 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/workspace.py
--rw-r--r--   0        0        0        0 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/py.typed
--rw-r--r--   0        0        0       38 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/schemas/__init__.py
--rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 snap_saas_base-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4822 2023-07-21 15:42:20.738427 snap_saas_base-0.5.0/README.md
+-rw-r--r--   0        0        0     4202 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/__init__.py
+-rw-r--r--   0        0        0     2153 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/base_model.py
+-rw-r--r--   0        0        0     5740 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/organization.py
+-rw-r--r--   0        0        0     3361 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/user.py
+-rw-r--r--   0        0        0     6632 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/workspace.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/py.typed
+-rw-r--r--   0        0        0       38 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/schemas/__init__.py
+-rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 snap_saas_base-0.5.0/PKG-INFO
```

### Comparing `snap_saas_base-0.4.1/README.md` & `snap_saas_base-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.1/pyproject.toml` & `snap_saas_base-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "snap-saas-base"
-version = "0.4.1"
+version = "0.5.0"
 description = "Snap Env (https://snapenv.com) Python base module."
 authors = ["Abner G Jacobsen <abner@apoana.com.br>"]
 readme = "README.md"
 repository = "https://github.com/orgs/snapenv/snap-saas-base"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "0.4.1"
+version = "0.5.0"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.11,<4.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.18"}
 cuid = "^0.4"
 pydantic = ">=1.0.0,<2.0.0"
```

### Comparing `snap_saas_base-0.4.1/src/snap_saas_base/models/base_model.py` & `snap_saas_base-0.5.0/src/snap_saas_base/models/base_model.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.1/src/snap_saas_base/models/organization.py` & `snap_saas_base-0.5.0/src/snap_saas_base/models/organization.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.1/src/snap_saas_base/models/user.py` & `snap_saas_base-0.5.0/src/snap_saas_base/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     __tablename__ = "users"
     username: so.Mapped[str] = so.mapped_column(nullable=False)
     provider: so.Mapped[str] = so.mapped_column(default="local", nullable=True)
     email: so.Mapped[str] = so.mapped_column(nullable=True)
     cell_phone: so.Mapped[str] = so.mapped_column(nullable=True, index=True)
     full_name: so.Mapped[str] = so.mapped_column(nullable=False)
+    avatar: so.Mapped[str] = so.mapped_column(nullable=True)
     hashed_password: so.Mapped[str] = so.mapped_column(nullable=True)
     is_verified: so.Mapped[bool] = so.mapped_column(
         nullable=False, default=False, server_default=sa.text("false")
     )
     is_premium: so.Mapped[bool] = so.mapped_column(
         nullable=False, default=False, server_default=sa.text("false")
     )
```

### Comparing `snap_saas_base-0.4.1/src/snap_saas_base/models/workspace.py` & `snap_saas_base-0.5.0/src/snap_saas_base/models/workspace.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.1/PKG-INFO` & `snap_saas_base-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snap-saas-base
-Version: 0.4.1
+Version: 0.5.0
 Summary: Snap Env (https://snapenv.com) Python base module.
 Home-page: https://github.com/orgs/snapenv/snap-saas-base
 Author: Abner G Jacobsen
 Author-email: abner@apoana.com.br
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

