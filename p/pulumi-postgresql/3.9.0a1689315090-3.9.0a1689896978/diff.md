# Comparing `tmp/pulumi_postgresql-3.9.0a1689315090.tar.gz` & `tmp/pulumi_postgresql-3.9.0a1689896978.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_postgresql-3.9.0a1689315090.tar", last modified: Fri Jul 14 06:19:24 2023, max compression
+gzip compressed data, was "pulumi_postgresql-3.9.0a1689896978.tar", last modified: Thu Jul 20 23:53:33 2023, max compression
```

## Comparing `pulumi_postgresql-3.9.0a1689315090.tar` & `pulumi_postgresql-3.9.0a1689896978.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:19:24.843894 pulumi_postgresql-3.9.0a1689315090/
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-14 06:19:24.843894 pulumi_postgresql-3.9.0a1689315090/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:19:24.839894 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:19:24.843894 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    30248 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/default_privileg.py
--rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/get_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/grant_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/physical_replication_slot.py
--rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/publication.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/replication_slot.py
--rw-r--r--   0 runner    (1001) docker     (123)    67908 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/user_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:19:24.843894 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:19:24.843894 pulumi_postgresql-3.9.0a1689315090/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-14 06:19:24.000000 pulumi_postgresql-3.9.0a1689315090/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:53:33.274522 pulumi_postgresql-3.9.0a1689896978/
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-20 23:53:33.274522 pulumi_postgresql-3.9.0a1689896978/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:53:33.274522 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:53:33.274522 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30248 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/default_privileg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/get_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/grant_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/physical_replication_slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26057 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/replication_slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68718 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18896 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/user_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:53:33.274522 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-20 23:53:33.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-20 23:53:33.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:53:33.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:53:33.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 23:53:33.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 23:53:33.000000 pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:53:33.274522 pulumi_postgresql-3.9.0a1689896978/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-20 23:53:32.000000 pulumi_postgresql-3.9.0a1689896978/setup.py
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/PKG-INFO` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi_postgresql
-Version: 3.9.0a1689315090
+Name: pulumi-postgresql
+Version: 3.9.0a1689896978
 Summary: A Pulumi package for creating and managing postgresql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-postgresql
 Keywords: pulumi postgresql
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-postgresql/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-postgresql/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpostgresql.svg)](https://www.npmjs.com/package/@pulumi/postgresql)
 [![Python version](https://badge.fury.io/py/pulumi-postgresql.svg)](https://pypi.org/project/pulumi-postgresql)
 [![NuGet version](https://badge.fury.io/nu/pulumi.postgresql.svg)](https://badge.fury.io/nu/pulumi.postgresql)
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/README.md` & `pulumi_postgresql-3.9.0a1689896978/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/__init__.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/_inputs.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -122,14 +122,16 @@
                  usage_with_grant: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[bool] create: Should the specified ROLE have CREATE privileges to the specified SCHEMA.
         :param pulumi.Input[bool] create_with_grant: Should the specified ROLE have CREATE privileges to the specified SCHEMA and the ability to GRANT the CREATE privilege to other ROLEs.
         :param pulumi.Input[str] role: The ROLE who is receiving the policy.  If this value is empty or not specified it implies the policy is referring to the [`PUBLIC` role](https://www.postgresql.org/docs/current/static/sql-grant.html).
         :param pulumi.Input[bool] usage: Should the specified ROLE have USAGE privileges to the specified SCHEMA.
         :param pulumi.Input[bool] usage_with_grant: Should the specified ROLE have USAGE privileges to the specified SCHEMA and the ability to GRANT the USAGE privilege to other ROLEs.
+               
+               > **NOTE on `policy`:** The permissions of a role specified in multiple policy blocks is cumulative.  For example, if the same role is specified in two different `policy` each with different permissions (e.g. `create` and `usage_with_grant`, respectively), then the specified role with have both `create` and `usage_with_grant` privileges.
         """
         if create is not None:
             pulumi.set(__self__, "create", create)
         if create_with_grant is not None:
             pulumi.set(__self__, "create_with_grant", create_with_grant)
         if role is not None:
             pulumi.set(__self__, "role", role)
@@ -187,14 +189,16 @@
         pulumi.set(self, "usage", value)
 
     @property
     @pulumi.getter(name="usageWithGrant")
     def usage_with_grant(self) -> Optional[pulumi.Input[bool]]:
         """
         Should the specified ROLE have USAGE privileges to the specified SCHEMA and the ability to GRANT the USAGE privilege to other ROLEs.
+
+        > **NOTE on `policy`:** The permissions of a role specified in multiple policy blocks is cumulative.  For example, if the same role is specified in two different `policy` each with different permissions (e.g. `create` and `usage_with_grant`, respectively), then the specified role with have both `create` and `usage_with_grant` privileges.
         """
         return pulumi.get(self, "usage_with_grant")
 
     @usage_with_grant.setter
     def usage_with_grant(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "usage_with_grant", value)
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/_utilities.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/config/outputs.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/config/vars.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/database.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/default_privileg.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/default_privileg.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/default_privileges.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/default_privileges.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/extension.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/function.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/function.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/get_schemas.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/get_schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 include_system_schemas: Optional[bool] = None,
                 like_all_patterns: Optional[Sequence[str]] = None,
                 like_any_patterns: Optional[Sequence[str]] = None,
                 not_like_all_patterns: Optional[Sequence[str]] = None,
                 regex_pattern: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSchemasResult:
     """
-    The `_get_schemas_` data source retrieves a list of schema names from a specified PostgreSQL database.
+    The ``get_schemas`` data source retrieves a list of schema names from a specified PostgreSQL database.
 
     ## Usage
 
     ```python
     import pulumi
     import pulumi_postgresql as postgresql
 
@@ -132,46 +132,48 @@
 
     :param str database: The PostgreSQL database which will be queried for schema names.
     :param bool include_system_schemas: Determines whether to include system schemas (pg_ prefix and information_schema). 'public' will always be included. Defaults to ``false``.
     :param Sequence[str] like_all_patterns: List of expressions which will be pattern matched in the query using the PostgreSQL ``LIKE ALL`` operators.
     :param Sequence[str] like_any_patterns: List of expressions which will be pattern matched in the query using the PostgreSQL ``LIKE ANY`` operators.
     :param Sequence[str] not_like_all_patterns: List of expressions which will be pattern matched in the query using the PostgreSQL ``NOT LIKE ALL`` operators.
     :param str regex_pattern: Expression which will be pattern matched in the query using the PostgreSQL ``~`` (regular expression match) operator.
+           
+           Note that all optional arguments can be used in conjunction.
     """
     __args__ = dict()
     __args__['database'] = database
     __args__['includeSystemSchemas'] = include_system_schemas
     __args__['likeAllPatterns'] = like_all_patterns
     __args__['likeAnyPatterns'] = like_any_patterns
     __args__['notLikeAllPatterns'] = not_like_all_patterns
     __args__['regexPattern'] = regex_pattern
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('postgresql:index/getSchemas:getSchemas', __args__, opts=opts, typ=GetSchemasResult).value
 
     return AwaitableGetSchemasResult(
-        database=__ret__.database,
-        id=__ret__.id,
-        include_system_schemas=__ret__.include_system_schemas,
-        like_all_patterns=__ret__.like_all_patterns,
-        like_any_patterns=__ret__.like_any_patterns,
-        not_like_all_patterns=__ret__.not_like_all_patterns,
-        regex_pattern=__ret__.regex_pattern,
-        schemas=__ret__.schemas)
+        database=pulumi.get(__ret__, 'database'),
+        id=pulumi.get(__ret__, 'id'),
+        include_system_schemas=pulumi.get(__ret__, 'include_system_schemas'),
+        like_all_patterns=pulumi.get(__ret__, 'like_all_patterns'),
+        like_any_patterns=pulumi.get(__ret__, 'like_any_patterns'),
+        not_like_all_patterns=pulumi.get(__ret__, 'not_like_all_patterns'),
+        regex_pattern=pulumi.get(__ret__, 'regex_pattern'),
+        schemas=pulumi.get(__ret__, 'schemas'))
 
 
 @_utilities.lift_output_func(get_schemas)
 def get_schemas_output(database: Optional[pulumi.Input[str]] = None,
                        include_system_schemas: Optional[pulumi.Input[Optional[bool]]] = None,
                        like_all_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                        like_any_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                        not_like_all_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                        regex_pattern: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSchemasResult]:
     """
-    The `_get_schemas_` data source retrieves a list of schema names from a specified PostgreSQL database.
+    The ``get_schemas`` data source retrieves a list of schema names from a specified PostgreSQL database.
 
     ## Usage
 
     ```python
     import pulumi
     import pulumi_postgresql as postgresql
 
@@ -181,9 +183,11 @@
 
     :param str database: The PostgreSQL database which will be queried for schema names.
     :param bool include_system_schemas: Determines whether to include system schemas (pg_ prefix and information_schema). 'public' will always be included. Defaults to ``false``.
     :param Sequence[str] like_all_patterns: List of expressions which will be pattern matched in the query using the PostgreSQL ``LIKE ALL`` operators.
     :param Sequence[str] like_any_patterns: List of expressions which will be pattern matched in the query using the PostgreSQL ``LIKE ANY`` operators.
     :param Sequence[str] not_like_all_patterns: List of expressions which will be pattern matched in the query using the PostgreSQL ``NOT LIKE ALL`` operators.
     :param str regex_pattern: Expression which will be pattern matched in the query using the PostgreSQL ``~`` (regular expression match) operator.
+           
+           Note that all optional arguments can be used in conjunction.
     """
     ...
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/get_sequences.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/get_sequences.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                   like_all_patterns: Optional[Sequence[str]] = None,
                   like_any_patterns: Optional[Sequence[str]] = None,
                   not_like_all_patterns: Optional[Sequence[str]] = None,
                   regex_pattern: Optional[str] = None,
                   schemas: Optional[Sequence[str]] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSequencesResult:
     """
-    The `_get_sequences_` data source retrieves a list of sequence names from a specified PostgreSQL database.
+    The ``get_sequences`` data source retrieves a list of sequence names from a specified PostgreSQL database.
 
     ## Usage
 
     ```python
     import pulumi
     import pulumi_postgresql as postgresql
 
@@ -133,47 +133,49 @@
 
 
     :param str database: The PostgreSQL database which will be queried for sequence names.
     :param Sequence[str] like_all_patterns: List of expressions which will be pattern matched against sequence names in the query using the PostgreSQL ``LIKE ALL`` operators.
     :param Sequence[str] like_any_patterns: List of expressions which will be pattern matched against sequence names in the query using the PostgreSQL ``LIKE ANY`` operators.
     :param Sequence[str] not_like_all_patterns: List of expressions which will be pattern matched against sequence names in the query using the PostgreSQL ``NOT LIKE ALL`` operators.
     :param str regex_pattern: Expression which will be pattern matched against sequence names in the query using the PostgreSQL ``~`` (regular expression match) operator.
+           
+           Note that all optional arguments can be used in conjunction.
     :param Sequence[str] schemas: List of PostgreSQL schema(s) which will be queried for sequence names. Queries all schemas in the database by default.
     """
     __args__ = dict()
     __args__['database'] = database
     __args__['likeAllPatterns'] = like_all_patterns
     __args__['likeAnyPatterns'] = like_any_patterns
     __args__['notLikeAllPatterns'] = not_like_all_patterns
     __args__['regexPattern'] = regex_pattern
     __args__['schemas'] = schemas
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('postgresql:index/getSequences:getSequences', __args__, opts=opts, typ=GetSequencesResult).value
 
     return AwaitableGetSequencesResult(
-        database=__ret__.database,
-        id=__ret__.id,
-        like_all_patterns=__ret__.like_all_patterns,
-        like_any_patterns=__ret__.like_any_patterns,
-        not_like_all_patterns=__ret__.not_like_all_patterns,
-        regex_pattern=__ret__.regex_pattern,
-        schemas=__ret__.schemas,
-        sequences=__ret__.sequences)
+        database=pulumi.get(__ret__, 'database'),
+        id=pulumi.get(__ret__, 'id'),
+        like_all_patterns=pulumi.get(__ret__, 'like_all_patterns'),
+        like_any_patterns=pulumi.get(__ret__, 'like_any_patterns'),
+        not_like_all_patterns=pulumi.get(__ret__, 'not_like_all_patterns'),
+        regex_pattern=pulumi.get(__ret__, 'regex_pattern'),
+        schemas=pulumi.get(__ret__, 'schemas'),
+        sequences=pulumi.get(__ret__, 'sequences'))
 
 
 @_utilities.lift_output_func(get_sequences)
 def get_sequences_output(database: Optional[pulumi.Input[str]] = None,
                          like_all_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                          like_any_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                          not_like_all_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                          regex_pattern: Optional[pulumi.Input[Optional[str]]] = None,
                          schemas: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSequencesResult]:
     """
-    The `_get_sequences_` data source retrieves a list of sequence names from a specified PostgreSQL database.
+    The ``get_sequences`` data source retrieves a list of sequence names from a specified PostgreSQL database.
 
     ## Usage
 
     ```python
     import pulumi
     import pulumi_postgresql as postgresql
 
@@ -182,10 +184,12 @@
 
 
     :param str database: The PostgreSQL database which will be queried for sequence names.
     :param Sequence[str] like_all_patterns: List of expressions which will be pattern matched against sequence names in the query using the PostgreSQL ``LIKE ALL`` operators.
     :param Sequence[str] like_any_patterns: List of expressions which will be pattern matched against sequence names in the query using the PostgreSQL ``LIKE ANY`` operators.
     :param Sequence[str] not_like_all_patterns: List of expressions which will be pattern matched against sequence names in the query using the PostgreSQL ``NOT LIKE ALL`` operators.
     :param str regex_pattern: Expression which will be pattern matched against sequence names in the query using the PostgreSQL ``~`` (regular expression match) operator.
+           
+           Note that all optional arguments can be used in conjunction.
     :param Sequence[str] schemas: List of PostgreSQL schema(s) which will be queried for sequence names. Queries all schemas in the database by default.
     """
     ...
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/get_tables.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/get_tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                like_any_patterns: Optional[Sequence[str]] = None,
                not_like_all_patterns: Optional[Sequence[str]] = None,
                regex_pattern: Optional[str] = None,
                schemas: Optional[Sequence[str]] = None,
                table_types: Optional[Sequence[str]] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTablesResult:
     """
-    The `_get_tables_` data source retrieves a list of table names from a specified PostgreSQL database.
+    The ``get_tables`` data source retrieves a list of table names from a specified PostgreSQL database.
 
     ## Usage
 
     ```python
     import pulumi
     import pulumi_postgresql as postgresql
 
@@ -143,14 +143,16 @@
 
 
     :param str database: The PostgreSQL database which will be queried for table names.
     :param Sequence[str] like_all_patterns: List of expressions which will be pattern matched against table names in the query using the PostgreSQL ``LIKE ALL`` operators.
     :param Sequence[str] like_any_patterns: List of expressions which will be pattern matched against table names in the query using the PostgreSQL ``LIKE ANY`` operators.
     :param Sequence[str] not_like_all_patterns: List of expressions which will be pattern matched against table names in the query using the PostgreSQL ``NOT LIKE ALL`` operators.
     :param str regex_pattern: Expression which will be pattern matched against table names in the query using the PostgreSQL ``~`` (regular expression match) operator.
+           
+           Note that all optional arguments can be used in conjunction.
     :param Sequence[str] schemas: List of PostgreSQL schema(s) which will be queried for table names. Queries all schemas in the database by default.
     :param Sequence[str] table_types: List of PostgreSQL table types which will be queried for table names. Includes all table types by default (including views and temp tables). Use 'BASE TABLE' for normal tables only.
     """
     __args__ = dict()
     __args__['database'] = database
     __args__['likeAllPatterns'] = like_all_patterns
     __args__['likeAnyPatterns'] = like_any_patterns
@@ -158,36 +160,36 @@
     __args__['regexPattern'] = regex_pattern
     __args__['schemas'] = schemas
     __args__['tableTypes'] = table_types
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('postgresql:index/getTables:getTables', __args__, opts=opts, typ=GetTablesResult).value
 
     return AwaitableGetTablesResult(
-        database=__ret__.database,
-        id=__ret__.id,
-        like_all_patterns=__ret__.like_all_patterns,
-        like_any_patterns=__ret__.like_any_patterns,
-        not_like_all_patterns=__ret__.not_like_all_patterns,
-        regex_pattern=__ret__.regex_pattern,
-        schemas=__ret__.schemas,
-        table_types=__ret__.table_types,
-        tables=__ret__.tables)
+        database=pulumi.get(__ret__, 'database'),
+        id=pulumi.get(__ret__, 'id'),
+        like_all_patterns=pulumi.get(__ret__, 'like_all_patterns'),
+        like_any_patterns=pulumi.get(__ret__, 'like_any_patterns'),
+        not_like_all_patterns=pulumi.get(__ret__, 'not_like_all_patterns'),
+        regex_pattern=pulumi.get(__ret__, 'regex_pattern'),
+        schemas=pulumi.get(__ret__, 'schemas'),
+        table_types=pulumi.get(__ret__, 'table_types'),
+        tables=pulumi.get(__ret__, 'tables'))
 
 
 @_utilities.lift_output_func(get_tables)
 def get_tables_output(database: Optional[pulumi.Input[str]] = None,
                       like_all_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                       like_any_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                       not_like_all_patterns: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                       regex_pattern: Optional[pulumi.Input[Optional[str]]] = None,
                       schemas: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                       table_types: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTablesResult]:
     """
-    The `_get_tables_` data source retrieves a list of table names from a specified PostgreSQL database.
+    The ``get_tables`` data source retrieves a list of table names from a specified PostgreSQL database.
 
     ## Usage
 
     ```python
     import pulumi
     import pulumi_postgresql as postgresql
 
@@ -196,11 +198,13 @@
 
 
     :param str database: The PostgreSQL database which will be queried for table names.
     :param Sequence[str] like_all_patterns: List of expressions which will be pattern matched against table names in the query using the PostgreSQL ``LIKE ALL`` operators.
     :param Sequence[str] like_any_patterns: List of expressions which will be pattern matched against table names in the query using the PostgreSQL ``LIKE ANY`` operators.
     :param Sequence[str] not_like_all_patterns: List of expressions which will be pattern matched against table names in the query using the PostgreSQL ``NOT LIKE ALL`` operators.
     :param str regex_pattern: Expression which will be pattern matched against table names in the query using the PostgreSQL ``~`` (regular expression match) operator.
+           
+           Note that all optional arguments can be used in conjunction.
     :param Sequence[str] schemas: List of PostgreSQL schema(s) which will be queried for table names. Queries all schemas in the database by default.
     :param Sequence[str] table_types: List of PostgreSQL table types which will be queried for table names. Includes all table types by default (including views and temp tables). Use 'BASE TABLE' for normal tables only.
     """
     ...
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/grant.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/grant_role.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/grant_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/outputs.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,16 @@
                  usage_with_grant: Optional[bool] = None):
         """
         :param bool create: Should the specified ROLE have CREATE privileges to the specified SCHEMA.
         :param bool create_with_grant: Should the specified ROLE have CREATE privileges to the specified SCHEMA and the ability to GRANT the CREATE privilege to other ROLEs.
         :param str role: The ROLE who is receiving the policy.  If this value is empty or not specified it implies the policy is referring to the [`PUBLIC` role](https://www.postgresql.org/docs/current/static/sql-grant.html).
         :param bool usage: Should the specified ROLE have USAGE privileges to the specified SCHEMA.
         :param bool usage_with_grant: Should the specified ROLE have USAGE privileges to the specified SCHEMA and the ability to GRANT the USAGE privilege to other ROLEs.
+               
+               > **NOTE on `policy`:** The permissions of a role specified in multiple policy blocks is cumulative.  For example, if the same role is specified in two different `policy` each with different permissions (e.g. `create` and `usage_with_grant`, respectively), then the specified role with have both `create` and `usage_with_grant` privileges.
         """
         if create is not None:
             pulumi.set(__self__, "create", create)
         if create_with_grant is not None:
             pulumi.set(__self__, "create_with_grant", create_with_grant)
         if role is not None:
             pulumi.set(__self__, "role", role)
@@ -148,14 +150,16 @@
         return pulumi.get(self, "usage")
 
     @property
     @pulumi.getter(name="usageWithGrant")
     def usage_with_grant(self) -> Optional[bool]:
         """
         Should the specified ROLE have USAGE privileges to the specified SCHEMA and the ability to GRANT the USAGE privilege to other ROLEs.
+
+        > **NOTE on `policy`:** The permissions of a role specified in multiple policy blocks is cumulative.  For example, if the same role is specified in two different `policy` each with different permissions (e.g. `create` and `usage_with_grant`, respectively), then the specified role with have both `create` and `usage_with_grant` privileges.
         """
         return pulumi.get(self, "usage_with_grant")
 
 
 @pulumi.output_type
 class GetSequencesSequenceResult(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/physical_replication_slot.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/physical_replication_slot.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/provider.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -252,14 +252,17 @@
     @scheme.setter
     def scheme(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scheme", value)
 
     @property
     @pulumi.getter(name="sslMode")
     def ssl_mode(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""Rename PostgreSQL provider `ssl_mode` attribute to `sslmode`""", DeprecationWarning)
+        pulumi.log.warn("""ssl_mode is deprecated: Rename PostgreSQL provider `ssl_mode` attribute to `sslmode`""")
+
         return pulumi.get(self, "ssl_mode")
 
     @ssl_mode.setter
     def ssl_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssl_mode", value)
 
     @property
@@ -512,14 +515,17 @@
     @pulumi.getter
     def scheme(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "scheme")
 
     @property
     @pulumi.getter(name="sslMode")
     def ssl_mode(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""Rename PostgreSQL provider `ssl_mode` attribute to `sslmode`""", DeprecationWarning)
+        pulumi.log.warn("""ssl_mode is deprecated: Rename PostgreSQL provider `ssl_mode` attribute to `sslmode`""")
+
         return pulumi.get(self, "ssl_mode")
 
     @property
     @pulumi.getter
     def sslmode(self) -> pulumi.Output[Optional[str]]:
         """
         This option determines whether or with what priority a secure SSL TCP/IP connection will be negotiated with the
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/publication.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/publication.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/replication_slot.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/replication_slot.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/role.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,17 @@
     @create_role.setter
     def create_role(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_role", value)
 
     @property
     @pulumi.getter
     def encrypted(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""Rename PostgreSQL role resource attribute \"encrypted\" to \"encrypted_password\"""", DeprecationWarning)
+        pulumi.log.warn("""encrypted is deprecated: Rename PostgreSQL role resource attribute \"encrypted\" to \"encrypted_password\"""")
+
         return pulumi.get(self, "encrypted")
 
     @encrypted.setter
     def encrypted(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "encrypted", value)
 
     @property
@@ -606,14 +609,17 @@
     @create_role.setter
     def create_role(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_role", value)
 
     @property
     @pulumi.getter
     def encrypted(self) -> Optional[pulumi.Input[str]]:
+        warnings.warn("""Rename PostgreSQL role resource attribute \"encrypted\" to \"encrypted_password\"""", DeprecationWarning)
+        pulumi.log.warn("""encrypted is deprecated: Rename PostgreSQL role resource attribute \"encrypted\" to \"encrypted_password\"""")
+
         return pulumi.get(self, "encrypted")
 
     @encrypted.setter
     def encrypted(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "encrypted", value)
 
     @property
@@ -1148,14 +1154,17 @@
         is `false`.
         """
         return pulumi.get(self, "create_role")
 
     @property
     @pulumi.getter
     def encrypted(self) -> pulumi.Output[Optional[str]]:
+        warnings.warn("""Rename PostgreSQL role resource attribute \"encrypted\" to \"encrypted_password\"""", DeprecationWarning)
+        pulumi.log.warn("""encrypted is deprecated: Rename PostgreSQL role resource attribute \"encrypted\" to \"encrypted_password\"""")
+
         return pulumi.get(self, "encrypted")
 
     @property
     @pulumi.getter(name="encryptedPassword")
     def encrypted_password(self) -> pulumi.Output[Optional[bool]]:
         """
         Defines whether the password is stored
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/schema.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,17 @@
     @property
     @pulumi.getter
     def policies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SchemaPolicyArgs']]]]:
         """
         Can be specified multiple times for each policy.  Each
         policy block supports fields documented below.
         """
+        warnings.warn("""Use postgresql_grant resource instead (with object_type=\"schema\")""", DeprecationWarning)
+        pulumi.log.warn("""policies is deprecated: Use postgresql_grant resource instead (with object_type=\"schema\")""")
+
         return pulumi.get(self, "policies")
 
     @policies.setter
     def policies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SchemaPolicyArgs']]]]):
         pulumi.set(self, "policies", value)
 
 
@@ -224,14 +227,17 @@
     @property
     @pulumi.getter
     def policies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SchemaPolicyArgs']]]]:
         """
         Can be specified multiple times for each policy.  Each
         policy block supports fields documented below.
         """
+        warnings.warn("""Use postgresql_grant resource instead (with object_type=\"schema\")""", DeprecationWarning)
+        pulumi.log.warn("""policies is deprecated: Use postgresql_grant resource instead (with object_type=\"schema\")""")
+
         return pulumi.get(self, "policies")
 
     @policies.setter
     def policies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SchemaPolicyArgs']]]]):
         pulumi.set(self, "policies", value)
 
 
@@ -395,9 +401,12 @@
     @property
     @pulumi.getter
     def policies(self) -> pulumi.Output[Sequence['outputs.SchemaPolicy']]:
         """
         Can be specified multiple times for each policy.  Each
         policy block supports fields documented below.
         """
+        warnings.warn("""Use postgresql_grant resource instead (with object_type=\"schema\")""", DeprecationWarning)
+        pulumi.log.warn("""policies is deprecated: Use postgresql_grant resource instead (with object_type=\"schema\")""")
+
         return pulumi.get(self, "policies")
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/server.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/subscription.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql/user_mapping.py` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql/user_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/PKG-INFO` & `pulumi_postgresql-3.9.0a1689896978/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi-postgresql
-Version: 3.9.0a1689315090
+Name: pulumi_postgresql
+Version: 3.9.0a1689896978
 Summary: A Pulumi package for creating and managing postgresql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-postgresql
 Keywords: pulumi postgresql
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-postgresql/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-postgresql/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpostgresql.svg)](https://www.npmjs.com/package/@pulumi/postgresql)
 [![Python version](https://badge.fury.io/py/pulumi-postgresql.svg)](https://pypi.org/project/pulumi-postgresql)
 [![NuGet version](https://badge.fury.io/nu/pulumi.postgresql.svg)](https://badge.fury.io/nu/pulumi.postgresql)
```

### Comparing `pulumi_postgresql-3.9.0a1689315090/pulumi_postgresql.egg-info/SOURCES.txt` & `pulumi_postgresql-3.9.0a1689896978/pulumi_postgresql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1689315090/setup.py` & `pulumi_postgresql-3.9.0a1689896978/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.0a1689315090"
-PLUGIN_VERSION = "3.9.0-alpha.1689315090+345e1894"
+VERSION = "3.9.0a1689896978"
+PLUGIN_VERSION = "3.9.0-alpha.1689896978+859ee321"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'postgresql', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "postgresql Pulumi Package - Development Version"
 
 
 setup(name='pulumi_postgresql',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing postgresql cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

