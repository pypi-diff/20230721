# Comparing `tmp/eea.coremetadata-3.1.zip` & `tmp/eea.coremetadata-3.2.zip`

## zipinfo {}

```diff
@@ -1,257 +1,257 @@
-Zip file size: 85491 bytes, number of entries: 255
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/
--rw-r--r--  2.0 unx       38 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/setup.cfg
--rw-r--r--  2.0 unx     2286 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/CONTRIBUTING.md
--rw-r--r--  2.0 unx     6129 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/PKG-INFO
--rw-r--r--  2.0 unx     2989 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/README.rst
--rw-r--r--  2.0 unx     1661 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/setup.py
--rw-r--r--  2.0 unx      126 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/MANIFEST.in
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     6129 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/not-zip-safe
--rw-r--r--  2.0 unx       57 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/top_level.txt
--rw-r--r--  2.0 unx     7931 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea.coremetadata.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     2257 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/docs/HISTORY.txt
--rw-r--r--  2.0 unx      915 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/docs/LICENSE.GPL
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/
--rw-r--r--  2.0 unx       93 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/behaviors/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/browser/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/version.txt
--rw-r--r--  2.0 unx      566 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/configure.zcml
--rw-r--r--  2.0 unx      668 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/setuphandlers.py
--rw-r--r--  2.0 unx     7270 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/interfaces.py
--rw-r--r--  2.0 unx      482 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/indexer.py
--rw-r--r--  2.0 unx      346 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/README.txt
--rw-r--r--  2.0 unx    23100 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/metadata.py
--rw-r--r--  2.0 unx      991 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles.zcml
--rw-r--r--  2.0 unx      221 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/de/
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/eea.pot
--rwxr-xr-x  2.0 unx      218 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx     1456 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/upgrades/configure.zcml
--rw-r--r--  2.0 unx     5469 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/upgrades/to_24.py
--rw-r--r--  2.0 unx      822 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/upgrades/to_20.py
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/upgrades/__init__.py
--rw-r--r--  2.0 unx     1716 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/tests/base.py
--rw-r--r--  2.0 unx      672 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/tests/__init__.py
--rw-r--r--  2.0 unx     1466 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/behaviors/configure.zcml
--rw-r--r--  2.0 unx     4675 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/behaviors/vocabulary.py
--rw-r--r--  2.0 unx     3285 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/behaviors/metadata.py
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/behaviors/__init__.py
--rw-r--r--  2.0 unx      141 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/browser/configure.zcml
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/browser/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/
--rw-r--r--  2.0 unx      126 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/uninstall/browserlayer.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/
--rw-r--r--  2.0 unx      187 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/metadata.xml
--rw-r--r--  2.0 unx      789 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/catalog.xml
--rw-r--r--  2.0 unx     2434 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/registry.xml
--rw-r--r--  2.0 unx      174 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/browserlayer.xml
--rw-r--r--  2.0 unx      209 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/topics.cfg
--rw-r--r--  2.0 unx      194 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
--rw-r--r--  2.0 unx     6611 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/topics.xml
--rw-r--r--  2.0 unx     3664 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/organisations.xml
--rw-r--r--  2.0 unx     3656 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/publisher.xml
--rw-r--r--  2.0 unx      182 b- defN 23-Apr-26 18:48 eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
-255 files, 122374 bytes uncompressed, 34957 bytes compressed:  71.4%
+Zip file size: 85572 bytes, number of entries: 255
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/setup.cfg
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     6224 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/PKG-INFO
+-rw-r--r--  2.0 unx     2989 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/README.rst
+-rw-r--r--  2.0 unx     1661 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/MANIFEST.in
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6224 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     7931 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea.coremetadata.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     2372 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      915 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/docs/LICENSE.GPL
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/behaviors/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/browser/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/version.txt
+-rw-r--r--  2.0 unx      566 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/configure.zcml
+-rw-r--r--  2.0 unx      668 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/setuphandlers.py
+-rw-r--r--  2.0 unx     7270 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/interfaces.py
+-rw-r--r--  2.0 unx      482 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/indexer.py
+-rw-r--r--  2.0 unx      346 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/README.txt
+-rw-r--r--  2.0 unx    23389 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/metadata.py
+-rw-r--r--  2.0 unx      991 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles.zcml
+-rw-r--r--  2.0 unx      221 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/upgrades/configure.zcml
+-rw-r--r--  2.0 unx     5469 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/upgrades/to_24.py
+-rw-r--r--  2.0 unx      822 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/upgrades/to_20.py
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/upgrades/__init__.py
+-rw-r--r--  2.0 unx     1716 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/tests/base.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/tests/__init__.py
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/behaviors/configure.zcml
+-rw-r--r--  2.0 unx     4675 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/behaviors/vocabulary.py
+-rw-r--r--  2.0 unx     3244 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/behaviors/metadata.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/behaviors/__init__.py
+-rw-r--r--  2.0 unx      141 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/browser/configure.zcml
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/browser/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/
+-rw-r--r--  2.0 unx      126 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/uninstall/browserlayer.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/
+-rw-r--r--  2.0 unx      187 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/metadata.xml
+-rw-r--r--  2.0 unx      789 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/catalog.xml
+-rw-r--r--  2.0 unx     2434 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/registry.xml
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/browserlayer.xml
+-rw-r--r--  2.0 unx      209 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/topics.cfg
+-rw-r--r--  2.0 unx      194 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
+-rw-r--r--  2.0 unx     6611 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/topics.xml
+-rw-r--r--  2.0 unx     3664 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/organisations.xml
+-rw-r--r--  2.0 unx     3656 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/publisher.xml
+-rw-r--r--  2.0 unx      182 b- defN 23-Jul-21 11:50 eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
+255 files, 122914 bytes uncompressed, 35038 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -1,766 +1,766 @@
-Filename: eea.coremetadata-3.1/
+Filename: eea.coremetadata-3.2/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/
 Comment: 
 
-Filename: eea.coremetadata-3.1/docs/
+Filename: eea.coremetadata-3.2/docs/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/
+Filename: eea.coremetadata-3.2/eea/
 Comment: 
 
-Filename: eea.coremetadata-3.1/setup.cfg
+Filename: eea.coremetadata-3.2/setup.cfg
 Comment: 
 
-Filename: eea.coremetadata-3.1/CONTRIBUTING.md
+Filename: eea.coremetadata-3.2/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.coremetadata-3.1/PKG-INFO
+Filename: eea.coremetadata-3.2/PKG-INFO
 Comment: 
 
-Filename: eea.coremetadata-3.1/README.rst
+Filename: eea.coremetadata-3.2/README.rst
 Comment: 
 
-Filename: eea.coremetadata-3.1/setup.py
+Filename: eea.coremetadata-3.2/setup.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/MANIFEST.in
+Filename: eea.coremetadata-3.2/MANIFEST.in
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/entry_points.txt
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/dependency_links.txt
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/PKG-INFO
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/namespace_packages.txt
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/not-zip-safe
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/requires.txt
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/requires.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/top_level.txt
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea.coremetadata.egg-info/SOURCES.txt
+Filename: eea.coremetadata-3.2/eea.coremetadata.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/docs/HISTORY.txt
+Filename: eea.coremetadata-3.2/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/docs/LICENSE.txt
+Filename: eea.coremetadata-3.2/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/docs/LICENSE.GPL
+Filename: eea.coremetadata-3.2/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/
+Filename: eea.coremetadata-3.2/eea/coremetadata/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/__init__.py
+Filename: eea.coremetadata-3.2/eea/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/upgrades/
+Filename: eea.coremetadata-3.2/eea/coremetadata/upgrades/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/tests/
+Filename: eea.coremetadata-3.2/eea/coremetadata/tests/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/behaviors/
+Filename: eea.coremetadata-3.2/eea/coremetadata/behaviors/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/browser/
+Filename: eea.coremetadata-3.2/eea/coremetadata/browser/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/version.txt
+Filename: eea.coremetadata-3.2/eea/coremetadata/version.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/configure.zcml
+Filename: eea.coremetadata-3.2/eea/coremetadata/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/setuphandlers.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/setuphandlers.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/interfaces.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/interfaces.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/indexer.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/indexer.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/README.txt
+Filename: eea.coremetadata-3.2/eea/coremetadata/README.txt
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/metadata.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/metadata.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles.zcml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/__init__.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/en/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/en/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hr/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hr/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/es/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/es/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ro/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ro/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/eu/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/eu/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/el/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/el/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/it/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/it/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ru/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ru/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/is/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/is/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lt/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lt/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hu/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hu/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/nl/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/nl/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fi/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fi/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lv/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lv/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sl/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sl/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/mt/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/mt/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/tr/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/tr/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/no/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/no/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sv/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sv/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/bg/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/bg/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/kl/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/kl/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/et/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/et/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sk/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sk/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pl/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pl/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/cs/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/cs/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/da/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/da/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fr/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fr/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/de/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/de/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/eea.pot
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/eea.pot
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/update.sh
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/update.sh
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/plone-manual.pot
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/__init__.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.2/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/upgrades/configure.zcml
+Filename: eea.coremetadata-3.2/eea/coremetadata/upgrades/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/upgrades/to_24.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/upgrades/to_24.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/upgrades/to_20.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/upgrades/to_20.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/upgrades/__init__.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/upgrades/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/tests/base.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/tests/base.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/tests/test_doctests.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/tests/test_doctests.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/tests/__init__.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/tests/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/behaviors/configure.zcml
+Filename: eea.coremetadata-3.2/eea/coremetadata/behaviors/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/behaviors/vocabulary.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/behaviors/vocabulary.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/behaviors/metadata.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/behaviors/metadata.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/behaviors/__init__.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/behaviors/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/browser/configure.zcml
+Filename: eea.coremetadata-3.2/eea/coremetadata/browser/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/browser/__init__.py
+Filename: eea.coremetadata-3.2/eea/coremetadata/browser/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/uninstall/
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/uninstall/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/uninstall/browserlayer.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/uninstall/browserlayer.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/metadata.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/metadata.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/catalog.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/catalog.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/registry.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/registry.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/browserlayer.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/browserlayer.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/topics.cfg
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/topics.cfg
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/topics.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/topics.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/organisations.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/organisations.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/publisher.xml
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/publisher.xml
 Comment: 
 
-Filename: eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
+Filename: eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.coremetadata-3.1/CONTRIBUTING.md` & `eea.coremetadata-3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/PKG-INFO` & `eea.coremetadata-3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eea.coremetadata
-Version: 3.1
+Version: 3.2
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.coremetadata
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -125,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.2 - (2023-07-19)
+---------------------------
+* Bug fix: Object is of wrong type
+  [nileshgulia1 - refs #254921]
+
 3.1 - (2023-04-26)
 ---------------------------
 * Change: Develop refs #250426
   [alecghica]
 
 3.0 - (2023-03-23)
 ---------------------------
@@ -218,9 +222,7 @@
   [iulianpetchesi refs #142720]
 
 1.0 - (2022-04-05)
 -----------------------
 
 * Initial release.
   [eea]
-
-
```

## Comparing `eea.coremetadata-3.1/README.rst` & `eea.coremetadata-3.2/README.rst`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/setup.py` & `eea.coremetadata-3.2/setup.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea.coremetadata.egg-info/PKG-INFO` & `eea.coremetadata-3.2/eea.coremetadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eea.coremetadata
-Version: 3.1
+Version: 3.2
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.coremetadata
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -125,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.2 - (2023-07-19)
+---------------------------
+* Bug fix: Object is of wrong type
+  [nileshgulia1 - refs #254921]
+
 3.1 - (2023-04-26)
 ---------------------------
 * Change: Develop refs #250426
   [alecghica]
 
 3.0 - (2023-03-23)
 ---------------------------
@@ -218,9 +222,7 @@
   [iulianpetchesi refs #142720]
 
 1.0 - (2022-04-05)
 -----------------------
 
 * Initial release.
   [eea]
-
-
```

## Comparing `eea.coremetadata-3.1/eea.coremetadata.egg-info/SOURCES.txt` & `eea.coremetadata-3.2/eea.coremetadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/docs/HISTORY.txt` & `eea.coremetadata-3.2/docs/HISTORY.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+3.2 - (2023-07-19)
+---------------------------
+* Bug fix: Object is of wrong type
+  [nileshgulia1 - refs #254921]
+
 3.1 - (2023-04-26)
 ---------------------------
 * Change: Develop refs #250426
   [alecghica]
 
 3.0 - (2023-03-23)
 ---------------------------
```

## Comparing `eea.coremetadata-3.1/docs/LICENSE.txt` & `eea.coremetadata-3.2/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/docs/LICENSE.GPL` & `eea.coremetadata-3.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/configure.zcml` & `eea.coremetadata-3.2/eea/coremetadata/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/setuphandlers.py` & `eea.coremetadata-3.2/eea/coremetadata/setuphandlers.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/interfaces.py` & `eea.coremetadata-3.2/eea/coremetadata/interfaces.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/metadata.py` & `eea.coremetadata-3.2/eea/coremetadata/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,27 +38,25 @@
 
 
 _marker = []
 _zone = DateTime().timezone()
 
 
 def seq_strip(seq, stripper=lambda x: x.strip()):
-    """ Strip a sequence of strings.
-    """
+    """Strip a sequence of strings."""
     if isinstance(seq, list):
         return map(stripper, seq)
 
     if isinstance(seq, tuple):
         return tuple(map(stripper, seq))
 
     raise ValueError("%s of unsupported sequencetype %s" % (seq, type(seq)))
 
 
 def tuplize(valueName, value, splitter=lambda x: x.split()):
-
     if isinstance(value, tuple):
         return seq_strip(value)
 
     if isinstance(value, list):
         return seq_strip(tuple(value))
 
     if isinstance(value, six.string_types):
@@ -73,16 +71,16 @@
     publisher_env = "DEFAULT_PUBLISHER_" + SITE_STRING
     DEFAULT_PUBLISHER = os.environ.get(publisher_env, [])
 
     if len(DEFAULT_PUBLISHER) < 1:
         DEFAULT_PUBLISHER = os.environ.get("DEFAULT_PUBLISHER", [])
 
     if isinstance(DEFAULT_PUBLISHER, str):
-        if ',' in DEFAULT_PUBLISHER:
-            DEFAULT_PUBLISHER = DEFAULT_PUBLISHER.split(',')
+        if "," in DEFAULT_PUBLISHER:
+            DEFAULT_PUBLISHER = DEFAULT_PUBLISHER.split(",")
         else:
             if DEFAULT_PUBLISHER == "":
                 return ()
 
             DEFAULT_PUBLISHER = [DEFAULT_PUBLISHER]
 
     return tuple(DEFAULT_PUBLISHER)
@@ -94,135 +92,145 @@
     organisations_env = "DEFAULT_ORGANISATIONS_" + SITE_STRING
     DEFAULT_ORGANISATIONS = os.environ.get(organisations_env, [])
 
     if len(DEFAULT_ORGANISATIONS) < 1:
         DEFAULT_ORGANISATIONS = os.environ.get("DEFAULT_ORGANISATIONS", [])
 
     if isinstance(DEFAULT_ORGANISATIONS, str):
-        if ',' in DEFAULT_ORGANISATIONS:
-            DEFAULT_ORGANISATIONS = DEFAULT_ORGANISATIONS.split(',')
+        if "," in DEFAULT_ORGANISATIONS:
+            DEFAULT_ORGANISATIONS = DEFAULT_ORGANISATIONS.split(",")
         else:
             if DEFAULT_ORGANISATIONS == "":
                 return ()
 
             DEFAULT_ORGANISATIONS = [DEFAULT_ORGANISATIONS]
 
     return tuple(DEFAULT_ORGANISATIONS)
 
 
 class EffectiveAfterExpires(Invalid):
     __doc__ = _(
-        "error_invalid_publication", default=u"Invalid effective or expires date"  # noqa
+        "error_invalid_publication",
+        default="Invalid effective or expires date",  # noqa
     )
 
 
 @provider(IFormFieldProvider)
 class ICoreMetadata(model.Schema):
-    """ Core Metadata
-    """
+    """Core Metadata"""
+
     # ownership fieldset
     model.fieldset(
-        'eea.coremetadata',
-        label=_(
-            'label_schema_default',
-            default=u'EEA core metadata'
-        ),
-        fields=['topics', 'temporal_coverage',
-                'geo_coverage', 'publisher', 'rights',
-                'other_organisations', 'data_provenance'],
+        "eea.coremetadata",
+        label=_("label_schema_default", default="EEA core metadata"),
+        fields=[
+            "topics",
+            "temporal_coverage",
+            "geo_coverage",
+            "publisher",
+            "rights",
+            "other_organisations",
+            "data_provenance",
+        ],
     )
 
     title = TextLine(
-        title=_(u"label_title", default=u"Title"),
+        title=_("label_title", default="Title"),
         required=False,
     )
 
     description = Text(
-        title=_(u"label_description", default=u"Description"),
+        title=_("label_description", default="Description"),
         description=_(
-            u"help_description",
-            default=u"Used in item listings and search results."
+            "help_description",
+            default="Used in item listings and search results.",
         ),
         required=False,
     )
 
-    directives.widget('effective', DatetimeFieldWidget)
+    directives.widget("effective", DatetimeFieldWidget)
     effective = Datetime(
-        title=_(u'label_effective_date', u'Publishing Date'),
+        title=_("label_effective_date", "Publishing Date"),
         description=_(
-            u'help_effective_date',
-            default=u'If this date is in the future, the content will '
-                    u'not show up in listings and searches until this date.'),
+            "help_effective_date",
+            default="If this date is in the future, the content will "
+            "not show up in listings and searches until this date.",
+        ),
         required=False,
-        default=None
+        default=None,
     )
 
-    directives.widget('expires', DatetimeFieldWidget)
+    directives.widget("expires", DatetimeFieldWidget)
     expires = Datetime(
-        title=_(u'label_expiration_date', u'Expiration Date'),
+        title=_("label_expiration_date", "Expiration Date"),
         description=_(
-            u'help_expiration_date',
-            default=u'When this date is reached, the content will no '
-                    u'longer be visible in listings and searches.'),
+            "help_expiration_date",
+            default="When this date is reached, the content will no "
+            "longer be visible in listings and searches.",
+        ),
         required=False,
-        default=None
+        default=None,
     )
 
     directives.omitted("effective", "expires")
     directives.no_omit(IEditForm, "effective", "expires")
     directives.no_omit(IAddForm, "effective", "expires")
 
     directives.widget("other_organisations", SelectFieldWidget)
     other_organisations = Tuple(
-        title=_(u"Other organisations involved"),
-        description=_(u"Select other organisations involved in the production of this item"),   # noqa
+        title=_("Other organisations involved"),
+        description=_(
+            "Select other organisations involved in the production"
+            "of this item"
+        ),  # noqa
         required=False,
         value_type=Choice(vocabulary="organisations_vocabulary"),
         defaultFactory=defaultOrganisations,
     )
 
     directives.widget("topics", SelectFieldWidget)
     topics = Tuple(
-        title=_(u"Topics"),
-        description=_(u"Select from the official EEA topics"),
+        title=_("Topics"),
+        description=_("Select from the official EEA topics"),
         required=False,
         value_type=Choice(vocabulary="topics_vocabulary"),
         default=(),
     )
 
     temporal_coverage = JSONField(
-        title=_(u"Temporal coverage"),
-        description=_(u"Add years or period, e.g. 2018-2022"),
+        title=_("Temporal coverage"),
+        description=_("Add years or period, e.g. 2018-2022"),
         required=False,
         widget="temporal",
         default={},
     )
 
     geo_coverage = JSONField(
-        title=_(u"Geographical coverage"),
+        title=_("Geographical coverage"),
         description=_(
-            u"Use the search to add more granular geographic coverage tags"),
+            "Use the search to add more granular geographic coverage tags"
+        ),
         required=False,
         widget="geolocation",
         default={},
     )
 
     rights = TextLine(
-        title=_(u'label_copyrights', default=u'Rights'),
+        title=_("label_copyrights", default="Rights"),
         description=_(
-            u'Copyright statement or other rights information on this item.'
-            u'Only use if needed. Default will be EEA copyright policy'
+            "Copyright statement or other rights information on this item."
+            "Only use if needed. Default will be EEA copyright policy"
         ),
         required=False,
     )
 
     directives.widget("publisher", SelectFieldWidget)
     publisher = Tuple(
-        title=_(u"Publisher"),
-        description=_(u"The publisher of this item. Change only if needed"),
+        title=_("Publisher"),
+        description=_("The publisher of this item. Change only if needed"),
         value_type=Choice(vocabulary="publisher_vocabulary"),
         required=False,
         defaultFactory=defaultPublisher,
     )
 
     preview_image = NamedBlobImage(
         title=_("label_previewimage", default="Preview image"),
@@ -234,401 +242,427 @@
     )
 
     preview_caption = TextLine(
         title=_("Preview image caption"), description=_(""), required=False
     )
 
     data_provenance = JSONField(
-        title=_(u"Add sources for the data used"),
+        title=_("Add sources for the data used"),
         required=False,
         widget="data_provenance",
         default={},
     )
 
     @invariant
     def validate_start_end(data):
         if data.effective and data.expires and data.effective > data.expires:
             raise EffectiveAfterExpires(
                 _(
                     "error_expiration_must_be_after_effective_date",
-                    default=u"Expiration date must be after publishing date.",
+                    default="Expiration date must be after publishing date.",
                 )
             )
 
 
 @implementer(ICM, ICatalogCoreMetadata, IMutableCoreMetadata)
 class DefaultCoreMetadataImpl(PropertyManager):
 
-    """ Mix-in class which provides eea core metadata methods.
-    """
+    """Mix-in class which provides eea core metadata methods."""
 
     security = ClassSecurityInfo()
 
-    def __init__(self, title='', subject=(), description='', contributors=(),
-                 effective_date=None, expiration_date=None, format='text/html',
-                 language='', rights=''):
+    def __init__(
+        self,
+        title="",
+        subject=(),
+        description="",
+        contributors=(),
+        effective_date=None,
+        expiration_date=None,
+        format="text/html",
+        language="",
+        rights="",
+    ):
         now = DateTime()
         self.creation_date = now
         self.modification_date = now
         self.creators = ()
-        self._editMetadata(title, subject, description, contributors,
-                           effective_date, expiration_date, format, language,
-                           rights)
+        self._editMetadata(
+            title,
+            subject,
+            description,
+            contributors,
+            effective_date,
+            expiration_date,
+            format,
+            language,
+            rights,
+        )
 
     #
     #  Set-modification-date-related methods.
     #  In DefaultCoreMetadataImpl for lack of a better place.
     #
 
     # Class variable default for an upgrade.
     modification_date = None
 
-    security.declarePrivate('notifyModified')
+    security.declarePrivate("notifyModified")
 
     def notifyModified(self):
         # Take appropriate action after the resource has been modified.
         # Update creators and modification_date.
         self.addCreator()
         self.setModificationDate()
 
-    security.declareProtected(ModifyPortalContent, 'addCreator')
+    security.declareProtected(ModifyPortalContent, "addCreator")
 
     def addCreator(self, creator=None):
         # Add creator to core creators.
         if creator is None:
             user = getSecurityManager().getUser()
             creator = user and user.getId()
 
         # call self.listCreators() to make sure self.creators exists
         if creator and creator not in self.listCreators():
-            self.creators = self.creators + (creator, )
+            self.creators = self.creators + (creator,)
 
-    security.declareProtected(ModifyPortalContent, 'setModificationDate')
+    security.declareProtected(ModifyPortalContent, "setModificationDate")
 
     def setModificationDate(self, modification_date=None):
         # Set the date when the resource was last modified.
         # When called without an argument, sets the date to now.
         if modification_date is None:
             self.modification_date = DateTime()
         else:
             self.modification_date = self._datify(modification_date)
 
     #
     #  Core interface query methods
     #
-    security.declareProtected(View, 'Title')
+    security.declareProtected(View, "Title")
 
     def Title(self):
         # Core Title element - resource name.
         return self.title
 
-    security.declareProtected(View, 'listCreators')
+    security.declareProtected(View, "listCreators")
 
     def listCreators(self):
         # List Core Creator elements - resource authors.
-        if not hasattr(aq_base(self), 'creators'):
+        if not hasattr(aq_base(self), "creators"):
             # for content created with CMF versions before 1.5
             owner_tuple = self.getOwnerTuple()
             if owner_tuple:
                 self.creators = (owner_tuple[1],)
             else:
                 self.creators = ()
         return self.creators
 
-    security.declareProtected(View, 'Creator')
+    security.declareProtected(View, "Creator")
 
     def Creator(self):
         # Core Creator element - resource author.
         creators = self.listCreators()
-        return creators and creators[0] or ''
+        return creators and creators[0] or ""
 
-    security.declareProtected(View, 'Subject')
+    security.declareProtected(View, "Subject")
 
     def Subject(self):
         # Core Subject element - resource keywords.
-        return getattr(self, 'subject', ())  # compensate for *old* content
+        return getattr(self, "subject", ())  # compensate for *old* content
 
-    security.declareProtected(View, 'Description')
+    security.declareProtected(View, "Description")
 
     def Description(self):
         # Core Description element - resource summary.
         return self.description
 
-    security.declareProtected(View, 'Publisher')
+    security.declareProtected(View, "Publisher")
 
     def Publisher(self):
         # Core Publisher element - resource publisher.
-        tool = getToolByName(self, 'portal_metadata', None)
+        tool = getToolByName(self, "portal_metadata", None)
 
         if tool is not None:
             return tool.getPublisher()
 
-        return 'No publisher'
+        return "No publisher"
 
-    security.declareProtected(View, 'listContributors')
+    security.declareProtected(View, "listContributors")
 
     def listContributors(self):
         # Core Contributor elements - resource collaborators.
         return self.contributors
 
-    security.declareProtected(View, 'Contributors')
+    security.declareProtected(View, "Contributors")
 
     def Contributors(self):
         # Deprecated alias of listContributors.
         return self.listContributors()
 
-    security.declareProtected(View, 'Date')
+    security.declareProtected(View, "Date")
 
     def Date(self, zone=None):
         # Core Date element - default date.
         if zone is None:
             zone = _zone
         # Return effective_date if set, modification date otherwise
-        date = getattr(self, 'effective_date', None)
+        date = getattr(self, "effective_date", None)
         if date is None:
             date = self.modified()
         return date.toZone(zone).ISO()
 
-    security.declareProtected(View, 'CreationDate')
+    security.declareProtected(View, "CreationDate")
 
     def CreationDate(self, zone=None):
         # Core Date element - date resource created.
         if zone is None:
             zone = _zone
         # return unknown if never set properly
         if self.creation_date:
             return self.creation_date.toZone(zone).ISO()
-        return 'Unknown'
+        return "Unknown"
 
-    security.declareProtected(View, 'EffectiveDate')
+    security.declareProtected(View, "EffectiveDate")
 
     def EffectiveDate(self, zone=None):
         # Core Date element - date resource becomes effective.
         if zone is None:
             zone = _zone
-        ed = getattr(self, 'effective_date', None)
-        return ed and ed.toZone(zone).ISO() or 'None'
+        ed = getattr(self, "effective_date", None)
+        return ed and ed.toZone(zone).ISO() or "None"
 
-    security.declareProtected(View, 'ExpirationDate')
+    security.declareProtected(View, "ExpirationDate")
 
     def ExpirationDate(self, zone=None):
         # Core Date element - date resource expires.
         if zone is None:
             zone = _zone
-        ed = getattr(self, 'expiration_date', None)
-        return ed and ed.toZone(zone).ISO() or 'None'
+        ed = getattr(self, "expiration_date", None)
+        return ed and ed.toZone(zone).ISO() or "None"
 
-    security.declareProtected(View, 'ModificationDate')
+    security.declareProtected(View, "ModificationDate")
 
     def ModificationDate(self, zone=None):
         # Core Date element - date resource last modified.
         if zone is None:
             zone = _zone
         return self.modified().toZone(zone).ISO()
 
-    security.declareProtected(View, 'Type')
+    security.declareProtected(View, "Type")
 
     def Type(self):
         # Core Type element - resource type.
         ti = self.getTypeInfo()
-        return ti is not None and ti.Title() or 'Unknown'
+        return ti is not None and ti.Title() or "Unknown"
 
-    security.declareProtected(View, 'Format')
+    security.declareProtected(View, "Format")
 
     def Format(self):
         # Core Format element - resource format.
         return self.format
 
-    security.declareProtected(View, 'Identifier')
+    security.declareProtected(View, "Identifier")
 
     def Identifier(self):
         # Core Identifier element - resource ID.
         return self.absolute_url()
 
-    security.declareProtected(View, 'Language')
+    security.declareProtected(View, "Language")
 
     def Language(self):
         # Core Language element - resource language.
         return self.language
 
-    security.declareProtected(View, 'Rights')
+    security.declareProtected(View, "Rights")
 
     def Rights(self):
         # Core Rights element - resource copyright.
         return self.rights
 
-    security.declareProtected(View, 'WordCount')
+    security.declareProtected(View, "WordCount")
 
     #
     #  Core utility methods
     #
     def content_type(self):
-        """ WebDAV needs this to do the Right Thing (TM).
-        """
+        """WebDAV needs this to do the Right Thing (TM)."""
         return self.Format()
 
     __FLOOR_DATE = DateTime(1970, 0)  # always effective
 
-    security.declareProtected(View, 'isEffective')
+    security.declareProtected(View, "isEffective")
 
     def isEffective(self, date):
         # Is the date within the resource's effective range?
-        pastEffective = (self.effective_date is None or
-                         self.effective_date <= date)
-        beforeExpiration = (self.expiration_date is None or
-                            self.expiration_date >= date)
+        pastEffective = (
+            self.effective_date is None or self.effective_date <= date
+        )
+        beforeExpiration = (
+            self.expiration_date is None or self.expiration_date >= date
+        )
         return pastEffective and beforeExpiration
 
     #
     #  CatalogableCore methods
     #
-    security.declareProtected(View, 'created')
+    security.declareProtected(View, "created")
 
     def created(self):
         # Core Date element - date resource created.
         # allow for non-existent creation_date, existed always
-        date = getattr(self, 'creation_date', None)
+        date = getattr(self, "creation_date", None)
         return date is None and self.__FLOOR_DATE or date
 
-    security.declareProtected(View, 'effective')
+    security.declareProtected(View, "effective")
 
     def effective(self):
         # Core Date element - date resource becomes effective.
         marker = []
-        date = getattr(self, 'effective_date', marker)
+        date = getattr(self, "effective_date", marker)
         if date is marker:
-            date = getattr(self, 'creation_date', None)
+            date = getattr(self, "creation_date", None)
         return date is None and self.__FLOOR_DATE or date
 
     __CEILING_DATE = DateTime(2500, 0)  # never expires
 
-    security.declareProtected(View, 'expires')
+    security.declareProtected(View, "expires")
 
     def expires(self):
         # Core Date element - date resource expires.
-        date = getattr(self, 'expiration_date', None)
+        date = getattr(self, "expiration_date", None)
         return date is None and self.__CEILING_DATE or date
 
-    security.declareProtected(View, 'modified')
+    security.declareProtected(View, "modified")
 
     def modified(self):
         # Core Date element - date resource last modified.
         date = self.modification_date
         if date is None:
             # Upgrade.
             date = DateTime(self._p_mtime)
             self.modification_date = date
         return date
 
-    security.declareProtected(View, 'getMetadataHeaders')
+    security.declareProtected(View, "getMetadataHeaders")
 
     def getMetadataHeaders(self):
         # Return RFC-822-style headers.
         hdrlist = []
-        hdrlist.append(('Title', self.Title()))
-        hdrlist.append(('Subject', ', '.join(self.Subject())))
-        hdrlist.append(('Publisher', self.Publisher()))
-        hdrlist.append(('Description', self.Description()))
-        hdrlist.append(('Contributors', '; '.join(self.Contributors())))
-        hdrlist.append(('Effective_date', self.EffectiveDate()))
-        hdrlist.append(('Expiration_date', self.ExpirationDate()))
-        hdrlist.append(('Type', self.Type()))
-        hdrlist.append(('Format', self.Format()))
-        hdrlist.append(('Language', self.Language()))
-        hdrlist.append(('Rights', self.Rights()))
-        hdrlist.append(('WordCount', self.WordCount()))
+        hdrlist.append(("Title", self.Title()))
+        hdrlist.append(("Subject", ", ".join(self.Subject())))
+        hdrlist.append(("Publisher", self.Publisher()))
+        hdrlist.append(("Description", self.Description()))
+        hdrlist.append(("Contributors", "; ".join(self.Contributors())))
+        hdrlist.append(("Effective_date", self.EffectiveDate()))
+        hdrlist.append(("Expiration_date", self.ExpirationDate()))
+        hdrlist.append(("Type", self.Type()))
+        hdrlist.append(("Format", self.Format()))
+        hdrlist.append(("Language", self.Language()))
+        hdrlist.append(("Rights", self.Rights()))
+        hdrlist.append(("WordCount", self.WordCount()))
         return hdrlist
 
     #
     #  MutableCore methods
     #
-    security.declarePrivate('_datify')
+    security.declarePrivate("_datify")
 
     def _datify(self, attrib):
-        if attrib == 'None':
+        if attrib == "None":
             attrib = None
         elif not isinstance(attrib, DateTime):
             if attrib is not None:
                 attrib = DateTime(attrib)
         return attrib
 
-    security.declareProtected(ModifyPortalContent, 'setTitle')
+    security.declareProtected(ModifyPortalContent, "setTitle")
 
     def setTitle(self, title):
         # Set Core Title element - resource name.
         self.title = title
 
-    security.declareProtected(ModifyPortalContent, 'setCreators')
+    security.declareProtected(ModifyPortalContent, "setCreators")
 
     def setCreators(self, creators):
         # Set Core Creator elements - resource authors.
-        self.creators = tuplize('creators', creators)
+        self.creators = tuplize("creators", creators)
 
-    security.declareProtected(ModifyPortalContent, 'setSubject')
+    security.declareProtected(ModifyPortalContent, "setSubject")
 
     def setSubject(self, subject):
         # Set Core Subject element - resource keywords.
-        self.subject = tuplize('subject', subject)
+        self.subject = tuplize("subject", subject)
 
-    security.declareProtected(ModifyPortalContent, 'setDescription')
+    security.declareProtected(ModifyPortalContent, "setDescription")
 
     def setDescription(self, description):
         # Set Core Description element - resource summary.
         self.description = description
 
-    security.declareProtected(ModifyPortalContent, 'setContributors')
+    security.declareProtected(ModifyPortalContent, "setContributors")
 
     def setContributors(self, contributors):
         # Set Core Contributor elements - resource collaborators.
-        def semi_split(s): return map(lambda x: x.strip(), s.split(';'))
-        self.contributors = tuplize('contributors', contributors, semi_split)
+        def semi_split(s):
+            return map(lambda x: x.strip(), s.split(";"))
 
-    security.declareProtected(ModifyPortalContent, 'setEffectiveDate')
+        self.contributors = tuplize("contributors", contributors, semi_split)
+
+    security.declareProtected(ModifyPortalContent, "setEffectiveDate")
 
     def setEffectiveDate(self, effective_date):
         # Set Core Date element - date resource becomes effective.
         self.effective_date = self._datify(effective_date)
 
-    security.declareProtected(ModifyPortalContent, 'setExpirationDate')
+    security.declareProtected(ModifyPortalContent, "setExpirationDate")
 
     def setExpirationDate(self, expiration_date):
         # Set Core Date element - date resource expires.
         self.expiration_date = self._datify(expiration_date)
 
-    security.declareProtected(ModifyPortalContent, 'setFormat')
+    security.declareProtected(ModifyPortalContent, "setFormat")
 
     def setFormat(self, format):
         # Set Core Format element - resource format.
         self.format = format
 
-    security.declareProtected(ModifyPortalContent, 'setLanguage')
+    security.declareProtected(ModifyPortalContent, "setLanguage")
 
     def setLanguage(self, language):
         # Set Core Language element - resource language.
         self.language = language
 
-    security.declareProtected(ModifyPortalContent, 'setRights')
+    security.declareProtected(ModifyPortalContent, "setRights")
 
     def setRights(self, rights):
         # Set Core Rights element - resource copyright.
         self.rights = rights
 
-    security.declareProtected(ModifyPortalContent, 'setWordCount')
+    security.declareProtected(ModifyPortalContent, "setWordCount")
 
     #
     #  Management tab methods
     #
 
-    security.declarePrivate('_editMetadata')
-
-    def _editMetadata(self, title=_marker, subject=_marker, description=_marker,  # noqa
-                      contributors=_marker, effective_date=_marker,
-                      expiration_date=_marker, format=_marker, language=_marker,  # noqa
-                      rights=_marker):
+    security.declarePrivate("_editMetadata")
 
+    def _editMetadata(
+        self,
+        title=_marker,
+        subject=_marker,
+        description=_marker,  # noqa
+        contributors=_marker,
+        effective_date=_marker,
+        expiration_date=_marker,
+        format=_marker,
+        language=_marker,  # noqa
+        rights=_marker,
+    ):
         # Update the editable metadata for this resource.
         if title is not _marker:
             self.setTitle(title)
         if subject is not _marker:
             self.setSubject(subject)
         if description is not _marker:
             self.setDescription(description)
@@ -641,44 +675,78 @@
         if format is not _marker:
             self.setFormat(format)
         if language is not _marker:
             self.setLanguage(language)
         if rights is not _marker:
             self.setRights(rights)
 
-    security.declareProtected(ModifyPortalContent, 'manage_metadata')
-    manage_metadata = DTMLFile('zmi_metadata', WWW_DIR)
+    security.declareProtected(ModifyPortalContent, "manage_metadata")
+    manage_metadata = DTMLFile("zmi_metadata", WWW_DIR)
 
-    security.declareProtected(ModifyPortalContent, 'manage_editMetadata')
+    security.declareProtected(ModifyPortalContent, "manage_editMetadata")
 
-    def manage_editMetadata(self, title, subject, description, contributors,
-                            effective_date, expiration_date, format, language,
-                            rights, REQUEST):
-        """ Update metadata from the ZMI.
-        """
-        self._editMetadata(title, subject, description, contributors,
-                           effective_date, expiration_date, format, language,
-                           rights)
-        REQUEST['RESPONSE'].redirect(self.absolute_url() +
-                                     '/manage_metadata' +
-                                     '?manage_tabs_message=Metadata+updated.')
-
-    security.declareProtected(ModifyPortalContent, 'editMetadata')
-
-    def editMetadata(self, title='', subject=(), description='',
-                     contributors=(), effective_date=None, expiration_date=None,   # noqa
-                     format='text/html', language='en-US', rights=''):
+    def manage_editMetadata(
+        self,
+        title,
+        subject,
+        description,
+        contributors,
+        effective_date,
+        expiration_date,
+        format,
+        language,
+        rights,
+        REQUEST,
+    ):
+        """Update metadata from the ZMI."""
+        self._editMetadata(
+            title,
+            subject,
+            description,
+            contributors,
+            effective_date,
+            expiration_date,
+            format,
+            language,
+            rights,
+        )
+        REQUEST["RESPONSE"].redirect(
+            self.absolute_url() +
+            "/manage_metadata" +
+            "?manage_tabs_message=Metadata+updated."
+        )
+
+    security.declareProtected(ModifyPortalContent, "editMetadata")
+
+    def editMetadata(
+        self,
+        title="",
+        subject=(),
+        description="",
+        contributors=(),
+        effective_date=None,
+        expiration_date=None,  # noqa
+        format="text/html",
+        language="en-US",
+        rights="",
+    ):
         # Need to add check for webDAV locked resource for TTW methods.
         # As per bug #69, we can't assume they use the webdav
         # locking interface, and fail gracefully if they don't.
-        if hasattr(self, 'failIfLocked'):
+        if hasattr(self, "failIfLocked"):
             self.failIfLocked()
 
-        self._editMetadata(title=title, subject=subject,
-                           description=description, contributors=contributors,
-                           effective_date=effective_date,
-                           expiration_date=expiration_date, format=format,
-                           language=language, rights=rights)
+        self._editMetadata(
+            title=title,
+            subject=subject,
+            description=description,
+            contributors=contributors,
+            effective_date=effective_date,
+            expiration_date=expiration_date,
+            format=format,
+            language=language,
+            rights=rights,
+        )
         self.reindexObject()
 
 
 InitializeClass(DefaultCoreMetadataImpl)
```

## Comparing `eea.coremetadata-3.1/eea/coremetadata/profiles.zcml` & `eea.coremetadata-3.2/eea/coremetadata/profiles.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/upgrades/configure.zcml` & `eea.coremetadata-3.2/eea/coremetadata/upgrades/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/upgrades/to_24.py` & `eea.coremetadata-3.2/eea/coremetadata/upgrades/to_24.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/upgrades/to_20.py` & `eea.coremetadata-3.2/eea/coremetadata/upgrades/to_20.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/tests/base.py` & `eea.coremetadata-3.2/eea/coremetadata/tests/base.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/tests/test_doctests.py` & `eea.coremetadata-3.2/eea/coremetadata/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/behaviors/configure.zcml` & `eea.coremetadata-3.2/eea/coremetadata/behaviors/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/behaviors/vocabulary.py` & `eea.coremetadata-3.2/eea/coremetadata/behaviors/vocabulary.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/behaviors/metadata.py` & `eea.coremetadata-3.2/eea/coremetadata/behaviors/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 """ Custom behavior that adds core metadata fields
 """
 # pylint: disable=line-too-long, E0102, C0111
 import os
-from plone.app.dexterity.behaviors.metadata import (DCFieldProperty,
-                                                    MetadataBase)
+from plone.app.dexterity.behaviors.metadata import (
+    DCFieldProperty,
+    MetadataBase,
+)
 from eea.coremetadata.metadata import ICoreMetadata
 from zope.component.hooks import getSite
 
 
 class CoreMetadata(MetadataBase):
-    """ Core Metadata"""
+    """Core Metadata"""
 
     title = DCFieldProperty(ICoreMetadata["title"])
 
     description = DCFieldProperty(ICoreMetadata["description"])
 
     other_organisations = DCFieldProperty(ICoreMetadata["other_organisations"])
 
     topics = DCFieldProperty(ICoreMetadata["topics"])
 
-    effective = DCFieldProperty(ICoreMetadata["effective"],
-                                get_name="effective_date")
-    expires = DCFieldProperty(ICoreMetadata["expires"],
-                              get_name="expiration_date")
+    effective = DCFieldProperty(
+        ICoreMetadata["effective"], get_name="effective_date"
+    )
+    expires = DCFieldProperty(
+        ICoreMetadata["expires"], get_name="expiration_date"
+    )
 
-    temporal_coverage = DCFieldProperty(
-        ICoreMetadata["temporal_coverage"])
+    temporal_coverage = DCFieldProperty(ICoreMetadata["temporal_coverage"])
 
     geo_coverage = DCFieldProperty(ICoreMetadata["geo_coverage"])
 
     rights = DCFieldProperty(ICoreMetadata["rights"])
 
     publisher = DCFieldProperty(ICoreMetadata["publisher"])
 
     preview_image = DCFieldProperty(ICoreMetadata["preview_image"])
     preview_caption = DCFieldProperty(ICoreMetadata["preview_caption"])
 
     data_provenance = DCFieldProperty(ICoreMetadata["data_provenance"])
 
     @property
     def publisher(self):
-        """ publisher getter """
-        if not getattr(self.context, 'publisher', None):
+        """publisher getter"""
+        if not getattr(self.context, "publisher", None):
             SITE_STRING = getSite().getId()
             publisher_env = "DEFAULT_PUBLISHER_" + SITE_STRING
 
             DEFAULT_PUBLISHER = os.environ.get(publisher_env, [])
             if len(DEFAULT_PUBLISHER) < 1:
                 DEFAULT_PUBLISHER = os.environ.get("DEFAULT_PUBLISHER", [])
 
             if isinstance(DEFAULT_PUBLISHER, str):
-                if ',' in DEFAULT_PUBLISHER:
-                    DEFAULT_PUBLISHER = DEFAULT_PUBLISHER.split(',')
+                if "," in DEFAULT_PUBLISHER:
+                    DEFAULT_PUBLISHER = DEFAULT_PUBLISHER.split(",")
                 else:
                     DEFAULT_PUBLISHER = [DEFAULT_PUBLISHER]
 
-            return DEFAULT_PUBLISHER
+            return tuple(DEFAULT_PUBLISHER)
         return self.context.publisher
 
     @publisher.setter
     def publisher(self, value):
-        """ publisher setter """
-        setattr(self.context, 'publisher', value)
+        """publisher setter"""
+        setattr(self.context, "publisher", value)
 
     @property
     def other_organisations(self):
-        """ other_organisations getter """
-        if not getattr(self.context, 'other_organisations', None):
+        """other_organisations getter"""
+        if not getattr(self.context, "other_organisations", None):
             SITE_STRING = getSite().getId()
             organisations_env = "DEFAULT_ORGANISATIONS_" + SITE_STRING
             DEFAULT_ORGANISATIONS = os.environ.get(organisations_env, [])
 
             if len(DEFAULT_ORGANISATIONS) < 1:
-                DEFAULT_ORGANISATIONS = os.environ.get("DEFAULT_ORGANISATIONS", [])  # noqa
+                DEFAULT_ORGANISATIONS = os.environ.get(
+                    "DEFAULT_ORGANISATIONS", []
+                )  # noqa
 
             if isinstance(DEFAULT_ORGANISATIONS, str):
-                if ',' in DEFAULT_ORGANISATIONS:
-                    DEFAULT_ORGANISATIONS = DEFAULT_ORGANISATIONS.split(',')
+                if "," in DEFAULT_ORGANISATIONS:
+                    DEFAULT_ORGANISATIONS = DEFAULT_ORGANISATIONS.split(",")
                 else:
                     DEFAULT_ORGANISATIONS = [DEFAULT_ORGANISATIONS]
 
-            return DEFAULT_ORGANISATIONS
+            return tuple(DEFAULT_ORGANISATIONS)
         return self.context.other_organisations
 
     @other_organisations.setter
     def other_organisations(self, value):
-        """ other_organisations setter """
-        setattr(self.context, 'other_organisations', value)
+        """other_organisations setter"""
+        setattr(self.context, "other_organisations", value)
```

## Comparing `eea.coremetadata-3.1/eea/coremetadata/profiles/default/catalog.xml` & `eea.coremetadata-3.2/eea/coremetadata/profiles/default/catalog.xml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/profiles/default/registry.xml` & `eea.coremetadata-3.2/eea/coremetadata/profiles/default/registry.xml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/topics.xml` & `eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/topics.xml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/organisations.xml` & `eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/organisations.xml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.1/eea/coremetadata/profiles/default/taxonomies/publisher.xml` & `eea.coremetadata-3.2/eea/coremetadata/profiles/default/taxonomies/publisher.xml`

 * *Files identical despite different names*

