# Comparing `tmp/tnnt_discordbot_cogs-0.3.1.tar.gz` & `tmp/tnnt_discordbot_cogs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tnnt_discordbot_cogs-0.3.1.tar", last modified: Tue Jun 27 21:17:38 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `tnnt_discordbot_cogs-0.3.1.tar` & `tnnt_discordbot_cogs-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:17:38.038624 tnnt_discordbot_cogs-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 21:17:38.038624 tnnt_discordbot_cogs-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-27 21:17:38.038624 tnnt_discordbot_cogs-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:17:38.034624 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:17:38.038624 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/price_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-27 21:17:19.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/timers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:17:38.034624 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 21:17:38.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-27 21:17:38.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:17:38.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:17:37.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 21:17:38.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 21:17:38.000000 tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs.egg-info/top_level.txt
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/__init__.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/apps.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/auth_hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/__init__.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/about.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/auth.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/members.py
+-rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/price_check.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/timers.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/LICENSE
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/README.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/PKG-INFO
```

### Comparing `tnnt_discordbot_cogs-0.3.1/LICENSE` & `tnnt_discordbot_cogs-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/about.py` & `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/about.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/auth.py` & `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/members.py` & `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/members.py`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.3.1/tnnt_discordbot_cogs/cogs/timers.py` & `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/timers.py`

 * *Files identical despite different names*

