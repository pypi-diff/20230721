# Comparing `tmp/collective.iframe-1.0.0a1.tar.gz` & `tmp/collective.iframe-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.iframe-1.0.0a1.tar", last modified: Fri Jun 23 21:03:21 2023, max compression
+gzip compressed data, was "collective.iframe-1.0.0a2.tar", last modified: Thu Jul 20 22:04:59 2023, max compression
```

## Comparing `collective.iframe-1.0.0a1.tar` & `collective.iframe-1.0.0a2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.095635 collective.iframe-1.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       74 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/DEVELOP.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      664 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      120 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     4047 2023-06-23 21:03:21.095736 collective.iframe-1.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2679 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.082413 collective.iframe-1.0.0a1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     7937 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)       74 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      340 2023-06-23 21:03:21.096205 collective.iframe-1.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2098 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.076809 collective.iframe-1.0.0a1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.082777 collective.iframe-1.0.0a1/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.087297 collective.iframe-1.0.0a1/src/collective/iframe/
--rw-r--r--   0 maurits    (501) staff       (20)      134 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.088246 collective.iframe-1.0.0a1/src/collective/iframe/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      341 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3726 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/browser/iframe.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1361 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.089180 collective.iframe-1.0.0a1/src/collective/iframe/content/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/content/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2868 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/content/iframe.py
--rw-r--r--   0 maurits    (501) staff       (20)      317 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/content/iframe.xml
--rw-r--r--   0 maurits    (501) staff       (20)      266 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.090866 collective.iframe-1.0.0a1/src/collective/iframe/locales/
--rw-r--r--   0 maurits    (501) staff       (20)      611 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/locales/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/locales/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/locales/collective.iframe.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.077710 collective.iframe-1.0.0a1/src/collective/iframe/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.091402 collective.iframe-1.0.0a1/src/collective/iframe/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/locales/en/LC_MESSAGES/collective.iframe.po
--rw-r--r--   0 maurits    (501) staff       (20)     1750 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/locales/update.py
--rwxr-xr-x   0 maurits    (501) staff       (20)      488 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/locales/update.sh
--rw-r--r--   0 maurits    (501) staff       (20)      372 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.078437 collective.iframe-1.0.0a1/src/collective/iframe/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.093177 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      177 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      105 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      260 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.093920 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      623 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/registry/icons.xml
--rw-r--r--   0 maurits    (501) staff       (20)      175 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/registry/main.xml
--rw-r--r--   0 maurits    (501) staff       (20)      336 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.094263 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     3248 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/types/Iframe.xml
--rw-r--r--   0 maurits    (501) staff       (20)      309 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.094509 collective.iframe-1.0.0a1/src/collective/iframe/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      784 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1280 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.095374 collective.iframe-1.0.0a1/src/collective/iframe/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3096 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/tests/test_ct_iframe.py
--rw-r--r--   0 maurits    (501) staff       (20)     2376 2023-06-23 21:03:20.000000 collective.iframe-1.0.0a1/src/collective/iframe/tests/test_setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:03:21.085468 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     4047 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1896 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       81 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 21:03:21.000000 collective.iframe-1.0.0a1/src/collective.iframe.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.649125 collective.iframe-1.0.0a2/
+-rw-r--r--   0 maurits    (501) staff       (20)      273 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       74 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/DEVELOP.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      664 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      120 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     4217 2023-07-20 22:04:59.649222 collective.iframe-1.0.0a2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2679 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.637374 collective.iframe-1.0.0a2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     7937 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)       74 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      340 2023-07-20 22:04:59.649696 collective.iframe-1.0.0a2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2098 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.632712 collective.iframe-1.0.0a2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.637726 collective.iframe-1.0.0a2/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.641387 collective.iframe-1.0.0a2/src/collective/iframe/
+-rw-r--r--   0 maurits    (501) staff       (20)      134 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.642306 collective.iframe-1.0.0a2/src/collective/iframe/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      341 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3726 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/browser/iframe.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1548 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.643259 collective.iframe-1.0.0a2/src/collective/iframe/content/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/content/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2868 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/content/iframe.py
+-rw-r--r--   0 maurits    (501) staff       (20)      317 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/content/iframe.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      266 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.644626 collective.iframe-1.0.0a2/src/collective/iframe/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)      611 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/locales/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/locales/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/locales/collective.iframe.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.633399 collective.iframe-1.0.0a2/src/collective/iframe/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.645327 collective.iframe-1.0.0a2/src/collective/iframe/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)       28 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/locales/en/LC_MESSAGES/collective.iframe.mo
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/locales/en/LC_MESSAGES/collective.iframe.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1750 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/locales/update.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)      488 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/locales/update.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      372 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.633916 collective.iframe-1.0.0a2/src/collective/iframe/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.646829 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      177 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      105 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.647440 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      623 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/registry/icons.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      175 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/registry/main.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      336 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.647690 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     3260 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/types/Iframe.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      309 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.648054 collective.iframe-1.0.0a2/src/collective/iframe/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      784 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1280 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.648902 collective.iframe-1.0.0a2/src/collective/iframe/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3096 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/tests/test_ct_iframe.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2376 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective/iframe/tests/test_setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:04:59.639891 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     4217 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1962 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       81 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-20 22:04:59.000000 collective.iframe-1.0.0a2/src/collective.iframe.egg-info/top_level.txt
```

### Comparing `collective.iframe-1.0.0a1/DEVELOP.rst` & `collective.iframe-1.0.0a2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/LICENSE.GPL` & `collective.iframe-1.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/LICENSE.rst` & `collective.iframe-1.0.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/PKG-INFO` & `collective.iframe-1.0.0a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.iframe
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an iframe
 Home-page: https://github.com/collective/collective.iframe
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.iframe/
 Project-URL: Source, https://github.com/collective/collective.iframe
@@ -147,12 +147,20 @@
 - Maurits van Rees, m.van.rees@zestsoftware.nl
 
 
 Changelog
 =========
 
 
+1.0.0a2 (2023-07-21)
+--------------------
+
+- In our typeinfo, use ``contenttype/iframe`` as icon.
+  We have defined this in the registry, so we can use it.
+  [maurits]
+
+
 1.0.0a1 (2023-06-23)
 --------------------
 
 - Initial release.
   [mauritsvanrees]
```

### Comparing `collective.iframe-1.0.0a1/README.rst` & `collective.iframe-1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/docs/conf.py` & `collective.iframe-1.0.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/setup.py` & `collective.iframe-1.0.0a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.iframe",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="Content Type to show an iframe",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/browser/iframe.pt` & `collective.iframe-1.0.0a2/src/collective/iframe/browser/iframe.pt`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/configure.zcml` & `collective.iframe-1.0.0a2/src/collective/iframe/configure.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,22 @@
       title="collective.iframe (uninstall)"
       directory="profiles/uninstall"
       description="Uninstalls the collective.iframe add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
       post_handler=".setuphandlers.uninstall"
       />
 
+  <genericsetup:upgradeDepends
+      title="Apply typeinfo"
+      source="1000"
+      destination="1001"
+      profile="collective.iframe:default"
+      import_steps="typeinfo"
+      />
+
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="collective.iframe-hiddenprofiles"
       />
 
   <!-- -*- extra stuff goes here -*- -->
```

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/content/iframe.py` & `collective.iframe-1.0.0a2/src/collective/iframe/content/iframe.py`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/locales/README.rst` & `collective.iframe-1.0.0a2/src/collective/iframe/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/locales/update.py` & `collective.iframe-1.0.0a2/src/collective/iframe/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/registry/icons.xml` & `collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/registry/icons.xml`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/types/Iframe.xml` & `collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/types/Iframe.xml`

 * *Files 0% similar despite different names*

#### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/profiles/default/types/Iframe.xml` & `collective.iframe-1.0.0a2/src/collective/iframe/profiles/default/types/Iframe.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="Iframe" meta_type="Dexterity FTI" i18n:domain="collective.iframe">
   <!-- Basic properties -->
   <property i18n:translate="" name="title">Iframe</property>
   <property i18n:translate="" name="description">A page that shows an iframe</property>
   <property name="allow_discussion">False</property>
   <property name="factory">Iframe</property>
-  <property name="icon_expr">string:window</property>
+  <property name="icon_expr">string:contenttype/iframe</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="global_allow">True</property>
   <!-- Schema, class and security -->
   <property name="add_permission">collective.iframe.AddIframe</property>
   <property name="klass">collective.iframe.content.iframe.Iframe</property>
   <property name="model_file"/>
```

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/setuphandlers.py` & `collective.iframe-1.0.0a2/src/collective/iframe/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/testing.py` & `collective.iframe-1.0.0a2/src/collective/iframe/testing.py`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/tests/test_ct_iframe.py` & `collective.iframe-1.0.0a2/src/collective/iframe/tests/test_ct_iframe.py`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective/iframe/tests/test_setup.py` & `collective.iframe-1.0.0a2/src/collective/iframe/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.iframe-1.0.0a1/src/collective.iframe.egg-info/PKG-INFO` & `collective.iframe-1.0.0a2/src/collective.iframe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.iframe
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an iframe
 Home-page: https://github.com/collective/collective.iframe
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.iframe/
 Project-URL: Source, https://github.com/collective/collective.iframe
@@ -147,12 +147,20 @@
 - Maurits van Rees, m.van.rees@zestsoftware.nl
 
 
 Changelog
 =========
 
 
+1.0.0a2 (2023-07-21)
+--------------------
+
+- In our typeinfo, use ``contenttype/iframe`` as icon.
+  We have defined this in the registry, so we can use it.
+  [maurits]
+
+
 1.0.0a1 (2023-06-23)
 --------------------
 
 - Initial release.
   [mauritsvanrees]
```

### Comparing `collective.iframe-1.0.0a1/src/collective.iframe.egg-info/SOURCES.txt` & `collective.iframe-1.0.0a2/src/collective.iframe.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/collective/iframe/content/iframe.py
 src/collective/iframe/content/iframe.xml
 src/collective/iframe/locales/README.rst
 src/collective/iframe/locales/__init__.py
 src/collective/iframe/locales/collective.iframe.pot
 src/collective/iframe/locales/update.py
 src/collective/iframe/locales/update.sh
+src/collective/iframe/locales/en/LC_MESSAGES/collective.iframe.mo
 src/collective/iframe/locales/en/LC_MESSAGES/collective.iframe.po
 src/collective/iframe/profiles/default/browserlayer.xml
 src/collective/iframe/profiles/default/catalog.xml
 src/collective/iframe/profiles/default/metadata.xml
 src/collective/iframe/profiles/default/rolemap.xml
 src/collective/iframe/profiles/default/types.xml
 src/collective/iframe/profiles/default/registry/icons.xml
```

