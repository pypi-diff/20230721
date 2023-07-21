# Comparing `tmp/nuclia-1.1.3.tar.gz` & `tmp/nuclia-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.1.3.tar", last modified: Fri Jul 21 09:15:34 2023, max compression
+gzip compressed data, was "nuclia-1.1.4.tar", last modified: Fri Jul 21 09:26:28 2023, max compression
```

## Comparing `nuclia-1.1.3.tar` & `nuclia-1.1.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.528607 nuclia-1.1.3/
--rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-21 09:15:33.000000 nuclia-1.1.3/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-21 09:15:33.000000 nuclia-1.1.3/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)      838 2023-07-21 09:15:33.000000 nuclia-1.1.3/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-21 09:15:33.000000 nuclia-1.1.3/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-21 09:15:33.000000 nuclia-1.1.3/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-21 09:15:33.000000 nuclia-1.1.3/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:15:34.528757 nuclia-1.1.3/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-21 09:15:33.000000 nuclia-1.1.3/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-21 09:15:33.000000 nuclia-1.1.3/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-21 09:15:33.000000 nuclia-1.1.3/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.515788 nuclia-1.1.3/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/AUTH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/CONVERSATION.md
--rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/DEFAULT.md
--rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/EXTRACT.md
--rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/SEARCH.md
--rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/UPLOAD.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.517823 nuclia-1.1.3/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      339 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.520858 nuclia-1.1.3/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     3068 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.522426 nuclia-1.1.3/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)     5507 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/nua_responses.py
--rw-r--r--   0 ebr        (501) staff       (20)      444 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/utils.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.526516 nuclia-1.1.3/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     2091 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/nuas.py
--rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     3555 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/resource.py
--rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.528159 nuclia-1.1.3/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.528394 nuclia-1.1.3/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/fixtures.py
--rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      894 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_resource.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.520108 nuclia-1.1.3/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1311 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-21 09:15:33.000000 nuclia-1.1.3/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-21 09:15:34.529234 nuclia-1.1.3/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-21 09:15:33.000000 nuclia-1.1.3/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-21 09:15:33.000000 nuclia-1.1.3/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.444298 nuclia-1.1.4/
+-rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-21 09:26:27.000000 nuclia-1.1.4/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-21 09:26:27.000000 nuclia-1.1.4/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)      886 2023-07-21 09:26:27.000000 nuclia-1.1.4/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-21 09:26:27.000000 nuclia-1.1.4/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-21 09:26:27.000000 nuclia-1.1.4/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-21 09:26:27.000000 nuclia-1.1.4/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:26:28.444494 nuclia-1.1.4/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-21 09:26:27.000000 nuclia-1.1.4/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-21 09:26:27.000000 nuclia-1.1.4/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-21 09:26:27.000000 nuclia-1.1.4/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.431593 nuclia-1.1.4/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/AUTH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/CONVERSATION.md
+-rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/DEFAULT.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/EXTRACT.md
+-rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/SEARCH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/UPLOAD.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.432830 nuclia-1.1.4/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      339 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.435443 nuclia-1.1.4/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3068 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.437064 nuclia-1.1.4/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)     5507 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/nua_responses.py
+-rw-r--r--   0 ebr        (501) staff       (20)      472 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/utils.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.441634 nuclia-1.1.4/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2091 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/nuas.py
+-rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3555 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.443505 nuclia-1.1.4/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.443899 nuclia-1.1.4/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/fixtures.py
+-rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      894 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_resource.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.434619 nuclia-1.1.4/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1311 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-21 09:26:27.000000 nuclia-1.1.4/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-21 09:26:28.445120 nuclia-1.1.4/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-21 09:26:27.000000 nuclia-1.1.4/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-21 09:26:27.000000 nuclia-1.1.4/test-requirements.txt
```

### Comparing `nuclia-1.1.3/CHANGELOG.md` & `nuclia-1.1.4/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 1.1.4 (2023-07-21)
+
+- Fix http status check
+
 ## 1.1.3 (2023-07-21)
 
 - Use pyyaml==5.3.1 as 5.4 is broken
 - Handle token expiration in a better way
 
 ## 1.1.2 (2023-07-10)
```

### Comparing `nuclia-1.1.3/LICENSE` & `nuclia-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/PKG-INFO` & `nuclia-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.3
+Version: 1.1.4
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.3/README.md` & `nuclia-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/docs/AUTH.md` & `nuclia-1.1.4/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/docs/CONVERSATION.md` & `nuclia-1.1.4/docs/CONVERSATION.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/docs/DEFAULT.md` & `nuclia-1.1.4/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/docs/EXTRACT.md` & `nuclia-1.1.4/docs/EXTRACT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/docs/README.md` & `nuclia-1.1.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/docs/SEARCH.md` & `nuclia-1.1.4/docs/SEARCH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/docs/UPLOAD.md` & `nuclia-1.1.4/docs/UPLOAD.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/cli/run.py` & `nuclia-1.1.4/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/cli/utils.py` & `nuclia-1.1.4/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/config.py` & `nuclia-1.1.4/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/data.py` & `nuclia-1.1.4/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/decorators.py` & `nuclia-1.1.4/nuclia/decorators.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/lib/kb.py` & `nuclia-1.1.4/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/lib/nua.py` & `nuclia-1.1.4/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/sdk/auth.py` & `nuclia-1.1.4/nuclia/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/sdk/kb.py` & `nuclia-1.1.4/nuclia/sdk/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/sdk/kbs.py` & `nuclia-1.1.4/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/sdk/nuas.py` & `nuclia-1.1.4/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/sdk/resource.py` & `nuclia-1.1.4/nuclia/sdk/resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/sdk/search.py` & `nuclia-1.1.4/nuclia/sdk/search.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/sdk/upload.py` & `nuclia-1.1.4/nuclia/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/tests/fixtures.py` & `nuclia-1.1.4/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/tests/test_conversation.py` & `nuclia-1.1.4/nuclia/tests/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia/tests/test_resource.py` & `nuclia-1.1.4/nuclia/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/nuclia.egg-info/PKG-INFO` & `nuclia-1.1.4/nuclia.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.3
+Version: 1.1.4
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.3/nuclia.egg-info/SOURCES.txt` & `nuclia-1.1.4/nuclia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.3/setup.py` & `nuclia-1.1.4/setup.py`

 * *Files identical despite different names*

