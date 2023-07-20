# Comparing `tmp/collective.mosaicpage-1.0.0a1.tar.gz` & `tmp/collective.mosaicpage-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.mosaicpage-1.0.0a1.tar", last modified: Fri Jun 23 21:01:49 2023, max compression
+gzip compressed data, was "collective.mosaicpage-1.0.0a2.tar", last modified: Thu Jul 20 22:14:27 2023, max compression
```

## Comparing `collective.mosaicpage-1.0.0a1.tar` & `collective.mosaicpage-1.0.0a2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.503058 collective.mosaicpage-1.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       67 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      886 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/DEVELOP.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      668 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)       86 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     2496 2023-06-23 21:01:49.503188 collective.mosaicpage-1.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1110 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      322 2023-06-23 21:01:49.503697 collective.mosaicpage-1.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2303 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.488040 collective.mosaicpage-1.0.0a1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.493275 collective.mosaicpage-1.0.0a1/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.498311 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      369 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.498759 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/content/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/content/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      327 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/content/mosaic_page.py
--rw-r--r--   0 maurits    (501) staff       (20)      182 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.499380 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/locales/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/locales/collective.mosaicpage.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.489167 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.499635 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/locales/nl/LC_MESSAGES/collective.mosaicpage.po
--rwxr-xr-x   0 maurits    (501) staff       (20)      500 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/locales/update.sh
--rw-r--r--   0 maurits    (501) staff       (20)      114 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/messagefactory.py
--rw-r--r--   0 maurits    (501) staff       (20)      523 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.490110 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.500746 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      189 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      250 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.501248 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      647 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/registry/icons.xml
--rw-r--r--   0 maurits    (501) staff       (20)      179 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/registry/main.xml
--rw-r--r--   0 maurits    (501) staff       (20)      283 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.501579 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     3742 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/types/MosaicPage.xml
--rw-r--r--   0 maurits    (501) staff       (20)      313 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.502011 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1287 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3815 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1207 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.502764 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3119 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/tests/test_ct_mosaic_page.py
--rw-r--r--   0 maurits    (501) staff       (20)     2233 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/tests/test_setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:01:49.495376 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     2496 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1752 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      126 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       78 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 21:01:49.000000 collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.906206 collective.mosaicpage-1.0.0a2/
+-rw-r--r--   0 maurits    (501) staff       (20)      277 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       67 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      886 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/DEVELOP.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      668 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       86 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     2670 2023-07-20 22:14:27.906327 collective.mosaicpage-1.0.0a2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1110 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      322 2023-07-20 22:14:27.906977 collective.mosaicpage-1.0.0a2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2303 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.890787 collective.mosaicpage-1.0.0a2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.894894 collective.mosaicpage-1.0.0a2/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.899630 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      369 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.900208 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/content/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/content/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      327 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/content/mosaic_page.py
+-rw-r--r--   0 maurits    (501) staff       (20)      182 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.900856 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/locales/collective.mosaicpage.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.891342 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.901819 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)       28 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/locales/nl/LC_MESSAGES/collective.mosaicpage.mo
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/locales/nl/LC_MESSAGES/collective.mosaicpage.po
+-rwxr-xr-x   0 maurits    (501) staff       (20)      500 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/locales/update.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      114 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/messagefactory.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.891892 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.902971 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      189 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      250 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.903834 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      647 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/registry/icons.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      179 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/registry/main.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      283 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.904211 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     3746 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/types/MosaicPage.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      313 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.904768 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1119 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3815 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1207 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.905912 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3119 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/tests/test_ct_mosaic_page.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2233 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/tests/test_setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-20 22:14:27.897322 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     2670 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1826 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      126 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       78 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-20 22:14:27.000000 collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/top_level.txt
```

### Comparing `collective.mosaicpage-1.0.0a1/DEVELOP.rst` & `collective.mosaicpage-1.0.0a2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/LICENSE.GPL` & `collective.mosaicpage-1.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/LICENSE.rst` & `collective.mosaicpage-1.0.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/PKG-INFO` & `collective.mosaicpage-1.0.0a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.mosaicpage
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A page with Mosaic selected as only layout
 Home-page: https://github.com/collective/collective.mosaicpage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.mosaicpage/
 Project-URL: Source, https://github.com/collective/collective.mosaicpage
@@ -84,12 +84,20 @@
 - Maurits van Rees, maurits@vanrees.org
 
 
 Changelog
 =========
 
 
+1.0.0a2 (2023-07-21)
+--------------------
+
+- In our typeinfo, use ``contenttype/mosaicpage`` as icon.
+  We have defined this in the registry, so we can use it.
+  [maurits]
+
+
 1.0.0a1 (2023-06-23)
 --------------------
 
 - Initial release.
   [mauritsvanrees]
```

### Comparing `collective.mosaicpage-1.0.0a1/README.rst` & `collective.mosaicpage-1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/setup.py` & `collective.mosaicpage-1.0.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.mosaicpage",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="A page with Mosaic selected as only layout",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/permissions.zcml` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/registry/icons.xml` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/registry/icons.xml`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/types/MosaicPage.xml` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/types/MosaicPage.xml`

 * *Files 2% similar despite different names*

#### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles/default/types/MosaicPage.xml` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles/default/types/MosaicPage.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="MosaicPage" meta_type="Dexterity FTI" i18n:domain="collective.mosaicpage">
   <!-- Basic properties -->
   <property i18n:translate="" name="title">MosaicPage</property>
   <property i18n:translate="" name="description">Page with Mosaic layout</property>
   <property name="allow_discussion">False</property>
   <property name="factory">MosaicPage</property>
-  <property name="icon_expr">string:layout-text-window</property>
+  <property name="icon_expr">string:contenttype/mosaicpage</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="global_allow">True</property>
   <property name="filter_content_types">True</property>
   <property name="allowed_content_types">
     <element value="Image"/>
   </property>
```

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/profiles.zcml` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/profiles.zcml`

 * *Files 24% similar despite different names*

```diff
@@ -23,22 +23,16 @@
       />
 
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="collective.mosaicpage-hiddenprofiles"
       />
 
-  <!-- <gs:upgradeSteps
-        source="1000"
-        destination="1001"
-        profile="collective.mosaicpage:default">
-      <gs:upgradeStep
-           title=""
-           handler=".upgrades.upgrade"
-           />
-      <gs:upgradeDepends
-           title=""
-           import_steps="plone.app.registry"
-           />
-    </gs:upgradeSteps> -->
+  <gs:upgradeDepends
+      title="Apply typeinfo"
+      source="1000"
+      destination="1001"
+      profile="collective.mosaicpage:default"
+      import_steps="typeinfo"
+      />
 
 </configure>
```

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/setuphandlers.py` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/testing.py` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/testing.py`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/tests/test_ct_mosaic_page.py` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/tests/test_ct_mosaic_page.py`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/src/collective/mosaicpage/tests/test_setup.py` & `collective.mosaicpage-1.0.0a2/src/collective/mosaicpage/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/PKG-INFO` & `collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.mosaicpage
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A page with Mosaic selected as only layout
 Home-page: https://github.com/collective/collective.mosaicpage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.mosaicpage/
 Project-URL: Source, https://github.com/collective/collective.mosaicpage
@@ -84,12 +84,20 @@
 - Maurits van Rees, maurits@vanrees.org
 
 
 Changelog
 =========
 
 
+1.0.0a2 (2023-07-21)
+--------------------
+
+- In our typeinfo, use ``contenttype/mosaicpage`` as icon.
+  We have defined this in the registry, so we can use it.
+  [maurits]
+
+
 1.0.0a1 (2023-06-23)
 --------------------
 
 - Initial release.
   [mauritsvanrees]
```

### Comparing `collective.mosaicpage-1.0.0a1/src/collective.mosaicpage.egg-info/SOURCES.txt` & `collective.mosaicpage-1.0.0a2/src/collective.mosaicpage.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/collective/mosaicpage/profiles.zcml
 src/collective/mosaicpage/setuphandlers.py
 src/collective/mosaicpage/testing.py
 src/collective/mosaicpage/content/__init__.py
 src/collective/mosaicpage/content/mosaic_page.py
 src/collective/mosaicpage/locales/collective.mosaicpage.pot
 src/collective/mosaicpage/locales/update.sh
+src/collective/mosaicpage/locales/nl/LC_MESSAGES/collective.mosaicpage.mo
 src/collective/mosaicpage/locales/nl/LC_MESSAGES/collective.mosaicpage.po
 src/collective/mosaicpage/profiles/default/browserlayer.xml
 src/collective/mosaicpage/profiles/default/metadata.xml
 src/collective/mosaicpage/profiles/default/rolemap.xml
 src/collective/mosaicpage/profiles/default/types.xml
 src/collective/mosaicpage/profiles/default/registry/icons.xml
 src/collective/mosaicpage/profiles/default/registry/main.xml
```

