# Comparing `tmp/metapensiero.sphinx.patchdb-4.0.dev5.tar.gz` & `tmp/metapensiero.sphinx.patchdb-4.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev5.tar", last modified: Sun Jun  4 15:33:19 2023, max compression
+gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev6.tar", last modified: Fri Jul 21 08:35:07 2023, max compression
```

## Comparing `metapensiero.sphinx.patchdb-4.0.dev5.tar` & `metapensiero.sphinx.patchdb-4.0.dev6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3725 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/CHANGES.rst
--rw-r--r--   0        0        0      609 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/Makefile
--rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/OLDERCHANGES.rst
--rw-r--r--   0        0        0    30372 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/README.rst
--rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/flake.lock
--rw-r--r--   0        0        0     3373 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/flake.nix
--rw-r--r--   0        0        0     1738 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/pyproject.toml
--rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/__init__.py
--rw-r--r--   0        0        0     7496 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/__init__.py
--rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/firebird.py
--rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/mysql.py
--rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/postgres.py
--rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/python.py
--rw-r--r--   0        0        0    17886 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sql.py
--rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
--rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/__init__.py
--rw-r--r--   0        0        0    13004 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
--rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
--rw-r--r--   0        0        0     8858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
--rw-r--r--   0        0        0     4730 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/manager.py
--rw-r--r--   0        0        0    14938 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/patch.py
--rw-r--r--   0        0        0     6155 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/planner.py
--rw-r--r--   0        0        0     9175 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/pup.py
--rw-r--r--   0        0        0    24368 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/script.py
--rw-r--r--   0        0        0     7312 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/states.py
--rw-r--r--   0        0        0     8148 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/fixtures.py
--rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/postgresql
--rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_bad.py
--rw-r--r--   0        0        0     4424 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_drops.py
--rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_external_file.py
--rw-r--r--   0        0        0     3557 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_helpers.py
--rw-r--r--   0        0        0     1862 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_manager.py
--rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_modular.py
--rw-r--r--   0        0        0     3531 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_patch.py
--rw-r--r--   0        0        0     6685 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_planner.py
--rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_python.py
--rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_revisions.py
--rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql.py
--rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_fb.py
--rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_ms.py
--rw-r--r--   0        0        0     7639 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_pg.py
--rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_states.py
--rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_variables.py
--rw-r--r--   0        0        0    31467 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     3809 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/CHANGES.rst
+-rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/Makefile
+-rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/OLDERCHANGES.rst
+-rw-r--r--   0        0        0    30372 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/README.rst
+-rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/flake.lock
+-rw-r--r--   0        0        0     3615 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/flake.nix
+-rw-r--r--   0        0        0     1745 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/__init__.py
+-rw-r--r--   0        0        0     7496 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/__init__.py
+-rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/firebird.py
+-rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/mysql.py
+-rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/postgres.py
+-rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/python.py
+-rw-r--r--   0        0        0    17886 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/sql.py
+-rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
+-rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/locale/__init__.py
+-rw-r--r--   0        0        0    13004 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
+-rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
+-rw-r--r--   0        0        0     8858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
+-rw-r--r--   0        0        0     4730 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/manager.py
+-rw-r--r--   0        0        0    14938 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/patch.py
+-rw-r--r--   0        0        0     6155 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/planner.py
+-rw-r--r--   0        0        0     9175 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/pup.py
+-rw-r--r--   0        0        0    24368 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/script.py
+-rw-r--r--   0        0        0     7312 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/states.py
+-rw-r--r--   0        0        0     8148 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/fixtures.py
+-rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/postgresql
+-rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_bad.py
+-rw-r--r--   0        0        0     4424 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_drops.py
+-rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_external_file.py
+-rw-r--r--   0        0        0     3557 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_helpers.py
+-rw-r--r--   0        0        0     1862 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_manager.py
+-rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_modular.py
+-rw-r--r--   0        0        0     3531 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_patch.py
+-rw-r--r--   0        0        0     6685 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_planner.py
+-rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_python.py
+-rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_revisions.py
+-rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql.py
+-rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql_fb.py
+-rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql_ms.py
+-rw-r--r--   0        0        0     7639 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql_pg.py
+-rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_states.py
+-rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/tests/test_variables.py
+-rw-r--r--   0        0        0    31467 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev6/PKG-INFO
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/CHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev6/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes\ [#]_
 -------------
 
+4.0.dev6 (2023-07-21)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Explicitly require sqlparse 0.4.4+
+
+
 4.0.dev5 (2023-06-04)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Reimplement the logic used to determine the correct application ordering of the patches,
   leveraging more dependencies constraints to avoid the old "postponing" strategy
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/Makefile` & `metapensiero.sphinx.patchdb-4.0.dev6/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2014, 2015, 2016, 2017, 2022, 2023 Lele Gaifax
 #
 
 # List of Python versions to test against, keep it in sync with flake.nix
 SNAKES = 310 311
 
-
 .PHONY: test
-test: $(addprefix test-python,$(SNAKES))
-
 
 define test-snake
+test:: test-python$(1)
+
 .PHONY: test-python$(1)
 test-python$(1):
 	nix develop '.#test-python$(1)' -c just check
 endef
 
-
 $(foreach snake,$(SNAKES),$(eval $(call test-snake,$(snake))))
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/OLDERCHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev6/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/README.rst` & `metapensiero.sphinx.patchdb-4.0.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/flake.lock` & `metapensiero.sphinx.patchdb-4.0.dev6/flake.lock`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/flake.nix` & `metapensiero.sphinx.patchdb-4.0.dev6/flake.nix`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,35 @@
         };
 
         # List of supported Python versions, see also Makefile
         snakes = flip map [ "310" "311"]
           (ver: rec { name = "python${ver}"; value = builtins.getAttr name pkgs;});
 
         mkPatchDBPkg = python: python.pkgs.buildPythonPackage {
-          name = pinfo.name;
+          pname = pinfo.name;
           version = pinfo.version;
 
           src = getSource "patchdb" ./.;
+          format = "pyproject";
+
           propagatedBuildInputs = (with python.pkgs; [
             enlighten
-            sqlparse
+            sqlparse.overridePythonAttrs (old: {
+              version = "0.4.4";
+              src = fetchPypi {
+                inherit pname version;
+                hash = "sha256-1EYYPoS4NJ+jBh8P5/BsqUumW0JpRv/r5uPoKVMyQgw=";
+              };
+            })
           ]);
-          format = "pyproject";
+
           nativeBuildInputs = (with python.pkgs; [
             pdm-pep517
           ]);
+
           doCheck = false;
         };
 
         patchDBPkgs = flip map snakes
           (py: {
             name = "patchdb-${py.name}";
             value = mkPatchDBPkg py.value;
@@ -67,14 +76,15 @@
           in
             pkgs.mkShell {
               name = "Test Python ${python.version}";
               packages = [
                 python
                 patchdb
               ] ++ (with pkgs; [
+                gnumake
                 just
                 postgresql_15
                 yq-go
               ]) ++ (with python.pkgs; [
                 docutils
                 psycopg
                 pytest
@@ -98,15 +108,14 @@
           default = pkgs.mkShell {
             name = "Dev shell";
 
             packages = with pkgs; [
               bump2version
               gnumake
               just
-              postgresql_15
               python3
               twine
               yq-go
             ] ++ (with pkgs.python3Packages; [
               babel
               build
             ]);
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/pyproject.toml` & `metapensiero.sphinx.patchdb-4.0.dev6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "metapensiero.sphinx.patchdb"
 description = "Extract scripts from a reST document and apply them in order."
-version = "4.0.dev5"
+version = "4.0.dev6"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -20,15 +20,15 @@
     "Environment :: Console",
     "Natural Language :: English",
     "Natural Language :: Italian",
 ]
 requires-python = ">=3.10"
 dependencies = [
     "enlighten",
-    "sqlparse",
+    "sqlparse>=0.4.4",
 ]
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Changelog = "https://gitlab.com/metapensiero/metapensiero.sphinx.patchdb/-/blob/master/CHANGES.rst"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/firebird.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/firebird.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/mysql.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/mysql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/postgres.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/postgres.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/python.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sql.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sqlite.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/contexts/sqlite.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2016, 2017, 2019, 2021, 2022, 2023 Lele Gaifax
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # Lele Gaifax <lele@metapensiero.it>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev5\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev6\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
 "POT-Creation-Date: 2023-06-04 17:23+0200\n"
 "PO-Revision-Date: 2023-06-04 17:26+0200\n"
 "Last-Translator: Lele Gaifax <lele@metapensiero.it>\n"
 "Language: it\n"
 "Language-Team: it <lele@metapensiero.it>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev5\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev6\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
 "POT-Creation-Date: 2023-06-04 17:23+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/manager.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/manager.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/patch.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/patch.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/planner.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/planner.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/pup.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/pup.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/script.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/script.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/states.py` & `metapensiero.sphinx.patchdb-4.0.dev6/src/metapensiero/sphinx/patchdb/states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/fixtures.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/postgresql` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/postgresql`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_bad.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_bad.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_drops.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_drops.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_external_file.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_external_file.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_helpers.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_manager.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_modular.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_modular.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_patch.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_planner.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_planner.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_python.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_revisions.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_revisions.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_fb.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql_fb.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_ms.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql_ms.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_pg.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_sql_pg.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_states.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_variables.py` & `metapensiero.sphinx.patchdb-4.0.dev6/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev5/PKG-INFO` & `metapensiero.sphinx.patchdb-4.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metapensiero.sphinx.patchdb
-Version: 4.0.dev5
+Version: 4.0.dev6
 Summary: Extract scripts from a reST document and apply them in order.
 License: GPL-3.0-or-later
 Author-email: Lele Gaifax <lele@metapensiero.it>
 Requires-Python: >=3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Sphinx :: Extension
```

