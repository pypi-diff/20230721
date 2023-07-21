# Comparing `tmp/nuclia-1.1.2.tar.gz` & `tmp/nuclia-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.1.2.tar", last modified: Mon Jul 10 12:37:22 2023, max compression
+gzip compressed data, was "nuclia-1.1.3.tar", last modified: Fri Jul 21 09:15:34 2023, max compression
```

## Comparing `nuclia-1.1.2.tar` & `nuclia-1.1.3.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.655895 nuclia-1.1.2/
--rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-10 12:37:22.000000 nuclia-1.1.2/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-10 12:37:22.000000 nuclia-1.1.2/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-10 12:37:22.000000 nuclia-1.1.2/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-10 12:37:22.000000 nuclia-1.1.2/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-10 12:37:22.000000 nuclia-1.1.2/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-10 12:37:22.000000 nuclia-1.1.2/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-10 12:37:22.656070 nuclia-1.1.2/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-10 12:37:22.000000 nuclia-1.1.2/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-10 12:37:22.000000 nuclia-1.1.2/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-10 12:37:22.000000 nuclia-1.1.2/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.644220 nuclia-1.1.2/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/AUTH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/CONVERSATION.md
--rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/DEFAULT.md
--rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/EXTRACT.md
--rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/SEARCH.md
--rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/UPLOAD.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.645780 nuclia-1.1.2/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      303 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.648263 nuclia-1.1.2/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     3040 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.649448 nuclia-1.1.2/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)     6040 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/nua_responses.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.653368 nuclia-1.1.2/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     2021 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/nuas.py
--rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     3338 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/resource.py
--rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.655190 nuclia-1.1.2/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.655525 nuclia-1.1.2/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/fixtures.py
--rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      882 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_resource.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.647578 nuclia-1.1.2/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1291 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-10 12:37:22.000000 nuclia-1.1.2/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-10 12:37:22.656573 nuclia-1.1.2/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-10 12:37:22.000000 nuclia-1.1.2/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-10 12:37:22.000000 nuclia-1.1.2/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.528607 nuclia-1.1.3/
+-rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-21 09:15:33.000000 nuclia-1.1.3/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-21 09:15:33.000000 nuclia-1.1.3/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)      838 2023-07-21 09:15:33.000000 nuclia-1.1.3/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-21 09:15:33.000000 nuclia-1.1.3/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-21 09:15:33.000000 nuclia-1.1.3/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-21 09:15:33.000000 nuclia-1.1.3/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:15:34.528757 nuclia-1.1.3/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-21 09:15:33.000000 nuclia-1.1.3/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-21 09:15:33.000000 nuclia-1.1.3/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-21 09:15:33.000000 nuclia-1.1.3/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.515788 nuclia-1.1.3/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/AUTH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/CONVERSATION.md
+-rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/DEFAULT.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/EXTRACT.md
+-rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/SEARCH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-21 09:15:33.000000 nuclia-1.1.3/docs/UPLOAD.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.517823 nuclia-1.1.3/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      339 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.520858 nuclia-1.1.3/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3068 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.522426 nuclia-1.1.3/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)     5507 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/nua_responses.py
+-rw-r--r--   0 ebr        (501) staff       (20)      444 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/lib/utils.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.526516 nuclia-1.1.3/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2091 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/nuas.py
+-rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3555 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.528159 nuclia-1.1.3/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.528394 nuclia-1.1.3/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/fixtures.py
+-rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      894 2023-07-21 09:15:33.000000 nuclia-1.1.3/nuclia/tests/test_resource.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:15:34.520108 nuclia-1.1.3/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1311 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:15:34.000000 nuclia-1.1.3/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-21 09:15:33.000000 nuclia-1.1.3/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-21 09:15:34.529234 nuclia-1.1.3/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-21 09:15:33.000000 nuclia-1.1.3/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-21 09:15:33.000000 nuclia-1.1.3/test-requirements.txt
```

### Comparing `nuclia-1.1.2/CHANGELOG.md` & `nuclia-1.1.3/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Changelog
 
-## 1.1.2 (2023-07-10)
+## 1.1.3 (2023-07-21)
+
+- Use pyyaml==5.3.1 as 5.4 is broken
+- Handle token expiration in a better way
 
+## 1.1.2 (2023-07-10)
 
 - Manage UserTokenExpired in CLI.
 - Support `show` and `extracted` when getting a resource.
 - Refactor all resource related actions in a class.
 - Support `Link` upload
 
-
 ## 1.1.1 (2023-07-07)
 
-
 - Set region parameter according KB url
 
-
 ## 1.1.0 (2023-07-05)
 
 - Support `--json` and `--yaml` options
 - Rename `ask` in `chat` as `ask` will be another new feature
 - Support all regular Nuclia resource metadata
 - Update the resource if it exists
```

### Comparing `nuclia-1.1.2/LICENSE` & `nuclia-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/PKG-INFO` & `nuclia-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.2
+Version: 1.1.3
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.2/README.md` & `nuclia-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/docs/AUTH.md` & `nuclia-1.1.3/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/docs/CONVERSATION.md` & `nuclia-1.1.3/docs/CONVERSATION.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/docs/DEFAULT.md` & `nuclia-1.1.3/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/docs/EXTRACT.md` & `nuclia-1.1.3/docs/EXTRACT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/docs/README.md` & `nuclia-1.1.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/docs/SEARCH.md` & `nuclia-1.1.3/docs/SEARCH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/docs/UPLOAD.md` & `nuclia-1.1.3/docs/UPLOAD.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/cli/run.py` & `nuclia-1.1.3/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/cli/utils.py` & `nuclia-1.1.3/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/config.py` & `nuclia-1.1.3/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/data.py` & `nuclia-1.1.3/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/decorators.py` & `nuclia-1.1.3/nuclia/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import wraps
 
 import yaml
 
+from nuclia import BASE_DOMAIN
 from nuclia.data import get_auth
 from nuclia.exceptions import NotDefinedDefault
 from nuclia.lib.kb import Environment, NucliaDBClient
 from nuclia.lib.nua import NuaClient
 
 
 def accounts(func):
@@ -59,15 +60,15 @@
                     ndb = NucliaDBClient(
                         environment=Environment.CLOUD,
                         url=kb_obj.url,
                         api_key=kb_obj.token,
                         region=kb_obj.region,
                     )
 
-        elif url.find("nuclia.cloud") >= 0:
+        elif url.find(BASE_DOMAIN) >= 0:
             region = url.split(".")[0].split("/")[-1]
             ndb = NucliaDBClient(
                 environment=Environment.CLOUD, url=url, api_key=api_key, region=region
             )
         else:
             ndb = NucliaDBClient(environment=Environment.OSS, url=url)
         kwargs["ndb"] = ndb
```

### Comparing `nuclia-1.1.2/nuclia/lib/kb.py` & `nuclia-1.1.3/nuclia/lib/kb.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import httpx
 import requests
 from nucliadb_models.search import ChatRequest
 from nucliadb_sdk import NucliaDB, Region
 
 from nuclia.exceptions import NeedUserToken
+from nuclia.lib.utils import handle_http_errors
 
 RESOURCE_PATH = "/resource/{rid}"
 RESOURCE_PATH_BY_SLUG = "/slug/{slug}"
 SEARCH_PATH = "/search"
 CREATE_RESOURCE_PATH = "/resources"
 CREATE_VECTORSET = "/vectorset/{vectorset}"
 VECTORSETS = "/vectorsets"
@@ -109,40 +110,31 @@
         )
 
     def chat(self, request: ChatRequest):
         url = f"{self.url}{CHAT_URL}"
         response: requests.Response = self.stream_session.post(
             url, data=request.json(), stream=True
         )
-        response
-        if response.status_code == 200:
-            return response
-        else:
-            raise httpx.HTTPError(
-                f"Status code {response.status_code}: {response.text}"
-            )
+        handle_http_errors(response)
+        return response
 
     def download(self, uri: str) -> bytes:
         # uri has format
         # /kb/2a00d5b4-cfcc-48eb-85ac-d70bfd38b26d/resource/41d02aac4ade48098b23e38141807738/file/file/download/field
         # we need to remove the kb url
 
         uri_parts = uri.split("/")
         if len(uri_parts) < 9:
             raise AttributeError("Not a valid download uri")
 
         new_uri = "/".join(uri_parts[3:])
         url = DOWNLOAD_URL.format(uri=new_uri)
         response: httpx.Response = self.reader_session.get(url)
-        if response.status_code == 200:
-            return response.content
-        else:
-            raise httpx.HTTPError(
-                f"Status code {response.status_code}: {response.text}"
-            )
+        handle_http_errors(response)
+        return response.content
 
     def start_tus_upload(
         self,
         size: int,
         filename: str,
         field: Optional[str] = None,
         rid: Optional[str] = None,
@@ -159,29 +151,21 @@
             "upload-length": str(size),
             "tus-resumable": "1.0.0",
             "upload-metadata": f"filename {encoded_filename}",
             "content-type": content_type,
         }
 
         response: httpx.Response = self.writer_session.post(url, headers=headers)
-        if response.status_code == 201:
-            return response.headers.get("Location")
-        else:
-            raise httpx.HTTPError(
-                f"Status code {response.status_code}: {response.text}"
-            )
+        handle_http_errors(response)
+        return response.headers.get("Location")
 
     def patch_tus_upload(self, upload_url: str, data: bytes, offset: int) -> int:
         headers = {
             "upload-offset": str(offset),
         }
         # upload url has all path, we should remove /kb/kbid/
         upload_url = "/" + "/".join(upload_url.split("/")[3:])
         response: httpx.Response = self.writer_session.patch(
             upload_url, headers=headers, content=data
         )
-        if response.status_code == 200:
-            return int(response.headers.get("Upload-Offset"))
-        else:
-            raise httpx.HTTPError(
-                f"Status code {response.status_code}: {response.text}"
-            )
+        handle_http_errors(response)
+        return int(response.headers.get("Upload-Offset"))
```

### Comparing `nuclia-1.1.2/nuclia/lib/nua.py` & `nuclia-1.1.3/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/sdk/auth.py` & `nuclia-1.1.3/nuclia/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/sdk/kb.py` & `nuclia-1.1.3/nuclia/sdk/kb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from nuclia.sdk.logger import logger
-from nuclia.sdk.resource import NucliaResource
+from warnings import warn
+
 from nucliadb_models.resource import Resource, ResourceList
 
 from nuclia.data import get_auth
 from nuclia.decorators import kb, pretty
 from nuclia.sdk.auth import NucliaAuth
+from nuclia.sdk.logger import logger
+from nuclia.sdk.resource import NucliaResource
 from nuclia.sdk.search import NucliaSearch
 from nuclia.sdk.upload import NucliaUpload
-from warnings import warn
+
 
 class NucliaKB:
     @property
     def _auth(self) -> NucliaAuth:
         auth = get_auth()
         return auth
 
@@ -26,30 +28,36 @@
         data: ResourceList = ndb.ndb.list_resources(kbid=ndb.kbid)
         for resource in data.resources:
             print(f"{resource.id} {resource.icon:30} {resource.title}")
 
     @kb
     @pretty
     def get_resource_by_id(self, *, rid: str, **kwargs) -> Resource:
-        warn('get_resource_by_slug is deprecated, use resource.get instead', DeprecationWarning)
-        logger.warning('get_resource_by_slug is deprecated, use resource.get instead')
+        warn(
+            "get_resource_by_id is deprecated, use resource.get instead",
+            DeprecationWarning,
+        )
+        logger.warning("get_resource_by_slug is deprecated, use resource.get instead")
         ndb = kwargs["ndb"]
         return ndb.ndb.get_resource_by_id(
             kbid=ndb.kbid, rid=rid, query_params={"show": "values"}
         )
 
     @kb
     @pretty
     def get_resource_by_slug(self, *, slug: str, **kwargs) -> Resource:
-        warn('get_resource_by_slug is deprecated, use resource.get instead', DeprecationWarning)
-        logger.warning('get_resource_by_slug is deprecated, use resource.get instead')
+        warn(
+            "get_resource_by_slug is deprecated, use resource.get instead",
+            DeprecationWarning,
+        )
+        logger.warning("get_resource_by_slug is deprecated, use resource.get instead")
         ndb = kwargs["ndb"]
         return ndb.ndb.get_resource_by_slug(
             kbid=ndb.kbid, slug=slug, query_params={"show": "values"}
         )
 
     @kb
     def delete(self, *, rid: str, **kwargs):
-        warn('delete is deprecated, use resource.delete instead', DeprecationWarning)
-        logger.warning('delete is deprecated, use resource.delete instead')
+        warn("delete is deprecated, use resource.delete instead", DeprecationWarning)
+        logger.warning("delete is deprecated, use resource.delete instead")
         ndb = kwargs["ndb"]
         ndb.ndb.delete_resource(kbid=ndb.kbid, rid=rid)
```

### Comparing `nuclia-1.1.2/nuclia/sdk/kbs.py` & `nuclia-1.1.3/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/sdk/nuas.py` & `nuclia-1.1.3/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/sdk/resource.py` & `nuclia-1.1.3/nuclia/sdk/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List, Optional
 from uuid import uuid4
+
+from nucliadb_models.metadata import ResourceProcessingStatus
+from nucliadb_models.resource import Resource
+
 from nuclia.decorators import kb, pretty
 from nuclia.sdk.logger import logger
-from nucliadb_models.resource import Resource
-from nucliadb_models.metadata import ResourceProcessingStatus
 
 RESOURCE_ATTRIBUTES = [
     "icon",
     "origin",
     "extra",
     "conversations",
     "links",
@@ -17,15 +19,15 @@
     "title",
 ]
 
 
 class NucliaResource:
     """
     Manage existing resource
-    
+
     All commands accept either `rid` or `slug` to identify the targeted resource.
     """
 
     @kb
     def create(*args, **kwargs) -> str:
         ndb = kwargs["ndb"]
         slug = kwargs.get("slug") or uuid4().hex
@@ -38,49 +40,70 @@
                 kw[param] = kwargs.get(param)
         resource = ndb.ndb.create_resource(**kw)
         rid = resource.uuid
         return rid
 
     @kb
     @pretty
-    def get(self, *, rid: Optional[str] = None, slug: Optional[str] = None, show: Optional[List[str]] = ['basic'], extracted: Optional[List[str]] = [], **kwargs) -> Resource:
+    def get(
+        self,
+        *,
+        rid: Optional[str] = None,
+        slug: Optional[str] = None,
+        show: Optional[List[str]] = ["basic"],
+        extracted: Optional[List[str]] = [],
+        **kwargs
+    ) -> Resource:
         ndb = kwargs["ndb"]
         show = list(show or [])
         if "basic" not in show:
             show.append("basic")
         if rid:
             res = ndb.ndb.get_resource_by_id(
-                kbid=ndb.kbid, rid=rid, query_params={"show": show, "extracted": extracted}
+                kbid=ndb.kbid,
+                rid=rid,
+                query_params={"show": show, "extracted": extracted},
             )
         elif slug:
             res = ndb.ndb.get_resource_by_slug(
-                kbid=ndb.kbid, slug=slug, query_params={"show": show, "extracted": extracted}
+                kbid=ndb.kbid,
+                slug=slug,
+                query_params={"show": show, "extracted": extracted},
             )
         else:
             raise ValueError("Either rid or slug must be provided")
-        
-        if 'extracted' in show and res.metadata.status != ResourceProcessingStatus.PROCESSED:
-            logger.warning("Resource is not processed yet, extracted content may be empty or incomplete.")
+
+        if (
+            "extracted" in show
+            and res.metadata.status != ResourceProcessingStatus.PROCESSED
+        ):
+            logger.warning(
+                "Resource is not processed yet, extracted content may be empty or incomplete."
+            )
 
         return res
 
     @kb
-    def update(self, *, rid: Optional[str]=None, slug: Optional[str]=None, **kwargs):
+    def update(
+        self, *, rid: Optional[str] = None, slug: Optional[str] = None, **kwargs
+    ):
         ndb = kwargs["ndb"]
         if rid:
             self._update_resource(kbid=ndb.kbid, rid=rid, **kwargs)
         elif slug:
             # TODO: delete directly when nucliadb sdk will support update by slug
             res = ndb.ndb.get_resource_by_slug(kbid=ndb.kbid, slug=slug)
             self._update_resource(kbid=ndb.kbid, rid=res.id, **kwargs)
         else:
             raise ValueError("Either rid or slug must be provided")
-    
+
     @kb
-    def delete(self, *, rid: Optional[str]=None, slug: Optional[str]=None, **kwargs):
+    def delete(
+        self, *, rid: Optional[str] = None, slug: Optional[str] = None, **kwargs
+    ):
         ndb = kwargs["ndb"]
         if rid:
             ndb.ndb.delete_resource(kbid=ndb.kbid, rid=rid)
         elif slug:
             # TODO: delete directly when nucliadb sdk will support delete by slug
             res = ndb.ndb.get_resource_by_slug(kbid=ndb.kbid, slug=slug)
             ndb.ndb.delete_resource(kbid=ndb.kbid, rid=res.id)
@@ -92,8 +115,8 @@
         kw = {
             "kbid": ndb.kbid,
             "rid": rid,
         }
         for param in RESOURCE_ATTRIBUTES:
             if param in kwargs:
                 kw[param] = kwargs.get(param)
-        ndb.ndb.update_resource(**kw)
+        ndb.ndb.update_resource(**kw)
```

### Comparing `nuclia-1.1.2/nuclia/sdk/search.py` & `nuclia-1.1.3/nuclia/sdk/search.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/sdk/upload.py` & `nuclia-1.1.3/nuclia/sdk/upload.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Optional, Tuple
 from uuid import uuid4
 
 import requests
-from nuclia.sdk.resource import RESOURCE_ATTRIBUTES, NucliaResource
 from nucliadb_models.text import TextFormat
 from nucliadb_sdk import exceptions
 from tqdm import tqdm
 
 from nuclia.data import get_auth
 from nuclia.decorators import kb
 from nuclia.lib.conversations import Conversation
 from nuclia.sdk.auth import NucliaAuth
 from nuclia.sdk.logger import logger
+from nuclia.sdk.resource import RESOURCE_ATTRIBUTES, NucliaResource
 
 
 class NucliaUpload:
     """
     Create or update resource content in a Nuclia KnowledgeBox.
 
     All commands accept the following parameters:
```

### Comparing `nuclia-1.1.2/nuclia/tests/fixtures.py` & `nuclia-1.1.3/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.2/nuclia/tests/test_conversation.py` & `nuclia-1.1.3/nuclia/tests/test_conversation.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
-from nuclia.sdk.resource import NucliaResource
 
 from nucliadb_sdk.v2.exceptions import NotFoundError
 
 from nuclia.sdk.kb import NucliaKB
+from nuclia.sdk.resource import NucliaResource
 from nuclia.sdk.upload import NucliaUpload
 
 path = f"{os.path.dirname(__file__)}/assets/conversation.json"
 
 
 def test_conversation(testing_config):
     nkb = NucliaKB()
```

### Comparing `nuclia-1.1.2/nuclia/tests/test_resource.py` & `nuclia-1.1.3/nuclia/tests/test_resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from nuclia.sdk.resource import NucliaResource
 from nucliadb_sdk.v2.exceptions import NotFoundError
 
+from nuclia.sdk.resource import NucliaResource
+
 
 def test_resource(testing_config):
     nresource = NucliaResource()
     try:
         res = nresource.get(slug="res1")
         nresource.delete(rid=res.id)
     except NotFoundError:
         pass
-    
+
     res_id = nresource.create(slug="res1")
 
     res = nresource.get(rid=res_id)
     assert res
 
     res = nresource.get(slug="res1")
     assert res
     assert res.id == res_id
 
-    nresource.update(rid=res_id, title="My great resource", texts={"text1": {"body": "Hello here"}})
-    res = nresource.get(slug="res1", show=["basic","values"])
+    nresource.update(
+        rid=res_id, title="My great resource", texts={"text1": {"body": "Hello here"}}
+    )
+    res = nresource.get(slug="res1", show=["basic", "values"])
 
     assert res
     assert res.title == "My great resource"
     assert res.data.texts["text1"]
 
     nresource.delete(rid=res_id)
```

### Comparing `nuclia-1.1.2/nuclia.egg-info/PKG-INFO` & `nuclia-1.1.3/nuclia.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.2
+Version: 1.1.3
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.2/nuclia.egg-info/SOURCES.txt` & `nuclia-1.1.3/nuclia.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 nuclia/cli/run.py
 nuclia/cli/utils.py
 nuclia/lib/__init__.py
 nuclia/lib/conversations.py
 nuclia/lib/kb.py
 nuclia/lib/nua.py
 nuclia/lib/nua_responses.py
+nuclia/lib/utils.py
 nuclia/sdk/__init__.py
 nuclia/sdk/accounts.py
 nuclia/sdk/auth.py
 nuclia/sdk/kb.py
 nuclia/sdk/kbs.py
 nuclia/sdk/logger.py
 nuclia/sdk/nua.py
```

### Comparing `nuclia-1.1.2/setup.py` & `nuclia-1.1.3/setup.py`

 * *Files identical despite different names*

