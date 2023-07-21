# Comparing `tmp/iparapheur-utils-0.9.8.tar.gz` & `tmp/iparapheur-utils-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iparapheur-utils-0.9.8.tar", last modified: Thu Apr 25 09:18:00 2019, max compression
+gzip compressed data, was "dist/iparapheur-utils-0.9.9.tar", last modified: Tue May 28 14:15:57 2019, max compression
```

## Comparing `iparapheur-utils-0.9.8.tar` & `iparapheur-utils-0.9.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/
--rw-rw-rw-   0 root         (0) root         (0)    11256 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/iparapheur_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      528 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/iparapheur_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       10 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/iparapheur_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       49 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/iparapheur_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1227 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/iparapheur_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    14455 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/iparapheur_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/iparapheur_utils.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/
--rw-rw-rw-   0 root         (0) root         (0)      394 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/parapheur/
--rw-rw-rw-   0 root         (0) root         (0)    12644 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/parapheur/Client.py
--rwxrwxrwx   0 root         (0) root         (0)     3513 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/parapheur/JSONHelper.py
--rwxrwxrwx   0 root         (0) root         (0)     3624 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/parapheur/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8364 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/parapheur/Webservice.py
--rwxrwxrwx   0 root         (0) root         (0)     3319 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/parapheur/pprint.py
--rwxrwxrwx   0 root         (0) root         (0)       82 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/script.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/configs/
--rw-rw-rw-   0 root         (0) root         (0)      155 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/configs/ldapsearch.cfg
--rw-rw-rw-   0 root         (0) root         (0)      206 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/configs/import.cfg
--rw-rw-rw-   0 root         (0) root         (0)      253 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/configs/recuparchives.cfg
--rwxrwxrwx   0 root         (0) root         (0)       82 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/configs/script.cfg
--rw-rw-rw-   0 root         (0) root         (0)      163 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/configs/pushdoc.cfg
--rw-rw-rw-   0 root         (0) root         (0)      206 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/configs/export.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     6660 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/pushdoc.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/ldapsearch.py
--rw-rw-rw-   0 root         (0) root         (0)    39622 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/checkInstallationIP.py
--rw-rw-rw-   0 root         (0) root         (0)    11112 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/recupArchives.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/scripts/javascript/
--rw-rw-rw-   0 root         (0) root         (0)       98 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/javascript/removeNode.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/scripts/script/
--rw-rw-rw-   0 root         (0) root         (0)     2944 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/script/count_files.sh
--rw-rw-rw-   0 root         (0) root         (0)     4203 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/script/ipclean.sh
--rw-rw-rw-   0 root         (0) root         (0)      946 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/remove_ldap.py
--rw-rw-rw-   0 root         (0) root         (0)    20022 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/import_data.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/ipclean.py
--rw-rw-rw-   0 root         (0) root         (0)     3070 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/change_name.py
--rw-rw-rw-   0 root         (0) root         (0)    11202 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/export_data.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/scripts/count_files.py
--rwxrwxrwx   0 root         (0) root         (0)    10547 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/parapheur/files/
--rw-rw-rw-   0 root         (0) root         (0)     1675 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/files/private.pem
--rw-rw-rw-   0 root         (0) root         (0)     2520 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/parapheur/files/public.pem
--rw-rw-rw-   0 root         (0) root         (0)       68 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1408 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    14455 2019-04-25 09:18:00.000000 iparapheur-utils-0.9.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4272 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.8/CHANGELOG.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)    11395 2019-05-28 14:08:03.000000 iparapheur-utils-0.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/iparapheur_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      528 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/iparapheur_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/iparapheur_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/iparapheur_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1227 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/iparapheur_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    14642 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/iparapheur_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/iparapheur_utils.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/parapheur/
+-rw-rw-rw-   0 root         (0) root         (0)    12644 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/parapheur/Client.py
+-rwxrwxrwx   0 root         (0) root         (0)     3513 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/parapheur/JSONHelper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3624 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/parapheur/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8364 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/parapheur/Webservice.py
+-rwxrwxrwx   0 root         (0) root         (0)     3319 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/parapheur/pprint.py
+-rwxrwxrwx   0 root         (0) root         (0)       82 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/script.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/configs/ldapsearch.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      206 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/configs/import.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      281 2019-05-28 14:08:03.000000 iparapheur-utils-0.9.9/parapheur/configs/recuparchives.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       82 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/configs/script.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      163 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/configs/pushdoc.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      206 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/configs/export.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     6660 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/pushdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2019-05-28 14:15:47.000000 iparapheur-utils-0.9.9/parapheur/scripts/ldapsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)    40906 2019-05-28 14:08:03.000000 iparapheur-utils-0.9.9/parapheur/scripts/checkInstallationIP.py
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2019-05-28 14:08:03.000000 iparapheur-utils-0.9.9/parapheur/scripts/recupArchives.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/scripts/javascript/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/javascript/removeNode.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/scripts/script/
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2019-05-28 14:08:03.000000 iparapheur-utils-0.9.9/parapheur/scripts/script/count_files.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/script/ipclean.sh
+-rw-rw-rw-   0 root         (0) root         (0)      946 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/remove_ldap.py
+-rw-rw-rw-   0 root         (0) root         (0)    20022 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/import_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/ipclean.py
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/change_name.py
+-rw-rw-rw-   0 root         (0) root         (0)    11202 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/export_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/scripts/count_files.py
+-rwxrwxrwx   0 root         (0) root         (0)    10759 2019-05-28 14:08:03.000000 iparapheur-utils-0.9.9/parapheur/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/parapheur/files/
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/files/private.pem
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/parapheur/files/public.pem
+-rw-rw-rw-   0 root         (0) root         (0)       68 2019-04-25 09:17:49.000000 iparapheur-utils-0.9.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    14642 2019-05-28 14:15:57.000000 iparapheur-utils-0.9.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4637 2019-05-28 14:15:47.000000 iparapheur-utils-0.9.9/CHANGELOG.md
```

### Comparing `iparapheur-utils-0.9.8/README.md` & `iparapheur-utils-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,16 @@
   -h, --help  Affiche ce message et quitte
 
 ```
 
 
 ## `ph-count_files`
 
-Cette commande affiche un tableau récapitulatif des dossiers par bureaux.
+Cette commande affiche un tableau récapitulatif des dossiers par bureaux. Si le parapheur est multitenant 2 tableaux 
+sont proposés: les dossiers en fin de parcours par tenant et le nombre d'archives par tenant.
 
 Exemple d'utilisation :
 ```bash
 usage: ph-count_files [-h]
 
 Arguments:
   -h, --help  Affiche ce message et quitte
```

### Comparing `iparapheur-utils-0.9.8/iparapheur_utils.egg-info/entry_points.txt` & `iparapheur-utils-0.9.9/iparapheur_utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/iparapheur_utils.egg-info/SOURCES.txt` & `iparapheur-utils-0.9.9/iparapheur_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/iparapheur_utils.egg-info/PKG-INFO` & `iparapheur-utils-0.9.9/iparapheur_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: iparapheur-utils
-Version: 0.9.8
+Version: 0.9.9
 Summary: Client python pour i-Parapheur
 Home-page: https://gitlab.libriciel.fr/i-parapheur/client-python
 Author: Lukas Hameury
 Author-email: lukas.hameury@libriciel.fr
 License: CeCILL v2
 Description: # Introduction
         
@@ -295,15 +295,16 @@
           -h, --help  Affiche ce message et quitte
         
         ```
         
         
         ## `ph-count_files`
         
-        Cette commande affiche un tableau récapitulatif des dossiers par bureaux.
+        Cette commande affiche un tableau récapitulatif des dossiers par bureaux. Si le parapheur est multitenant 2 tableaux 
+        sont proposés: les dossiers en fin de parcours par tenant et le nombre d'archives par tenant.
         
         Exemple d'utilisation :
         ```bash
         usage: ph-count_files [-h]
         
         Arguments:
           -h, --help  Affiche ce message et quitte
@@ -369,7 +370,8 @@
         Par exemple, pour un appel de `ph-echo` vers `secure-iparapheur.dom.local`, la commande sera :
         
         ```bash
         NO_PROXY="secure-iparapheur.dom.local" ph-echo
         ```
         
 Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `iparapheur-utils-0.9.8/parapheur/parapheur/Client.py` & `iparapheur-utils-0.9.9/parapheur/parapheur/Client.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/parapheur/JSONHelper.py` & `iparapheur-utils-0.9.9/parapheur/parapheur/JSONHelper.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/parapheur/__init__.py` & `iparapheur-utils-0.9.9/parapheur/parapheur/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/parapheur/Webservice.py` & `iparapheur-utils-0.9.9/parapheur/parapheur/Webservice.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/parapheur/pprint.py` & `iparapheur-utils-0.9.9/parapheur/parapheur/pprint.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/pushdoc.py` & `iparapheur-utils-0.9.9/parapheur/scripts/pushdoc.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/ldapsearch.py` & `iparapheur-utils-0.9.9/parapheur/scripts/ldapsearch.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             + groupSearchBase + "' '" + personDifferentialQuery + "' | grep displayName "
     pprint.info(query)
     return query
 
 
 def ldapSearchGrepDisplayname():
     pprint.header("----------- Liste des utilisateurs")
-    os.system(query)
+    os.system(query.replace('\\', ''))
 
 
 getConf()
 isSynchoEnable(active)
 accessUrl(url)
 ldapRequest(url, security_principal, credentials, groupSearchBase, personDifferentialQuery)
 ldapSearchGrepDisplayname()
```

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/checkInstallationIP.py` & `iparapheur-utils-0.9.9/parapheur/scripts/checkInstallationIP.py`

 * *Files 2% similar despite different names*

```diff
@@ -622,31 +622,46 @@
 def check_isexists_alfrescoglobal():
     pprint.header("#", False, ' ')
     pprint.log("---- Exists alfresco-global.properties  ? ----  ", True)
 
     # Alfresco-global.properties
     isexistsdirectory(defaut_iparapheur_root)
     isexistssubdir(defaut_iparapheur_root, "tomcat/shared/classes")
-    return isexistsfile("{0}/tomcat/shared/classes".format(defaut_iparapheur_root), "alfresco-global.properties")
+    return isexistsfile("{0}/tomcat/shared/classes"
+                        .format(defaut_iparapheur_root),
+                        "alfresco-global.properties")
 
 
-def check_config_alfrescoglobal(varconf, version_presente):
+def analyse_is_param_in_conf(keyarray, paramconfarray, prefix):
+    for param_key in keyarray:
+        try:
+            param_value = paramconfarray.get("Parapheur", param_key)
+            pprint.header("#", False, ' ')
+            pprint.info("{2} {0} = {1}".format(param_key, param_value, prefix))
+        except ConfigParser.NoOptionError as e:
+            pprint.header("#", False, ' ')
+            pprint.error("{1}  OMG, need this: {0}".format(param_key, prefix))
+
+
+def check_config_alfrescoglobal(varconf, ihmvarconf, version_presente):
     pprint.header("#", False, ' ')
     pprint.log("---- Check alfresco-global.properties ----  TODO", True)
 
     alf_dir_root = varconf.get("Parapheur", "dir.root")
     # pprint.info(varconf.options("Parapheur"))
     # pprint.info(varconf.items("Parapheur"))
 
     pprint.header("#", False, ' ')
     pprint.info("alf_dir_root = {0}".format(alf_dir_root))
     pprint.header("#", False, ' ')
     pprint.info("database URL = {0}".format(varconf.get("Parapheur", "db.url")))
 
-    needed_alfresco_global_params = ['dir.root', 'db.url', 'index.recovery.mode']
+    needed_alfresco_global_params = ['dir.root',
+                                     'db.url',
+                                     'index.recovery.mode']
     for param_key in needed_alfresco_global_params:
         try:
             param_value = varconf.get("Parapheur", param_key)
             pprint.header("#", False, ' ')
             pprint.info("  {0} = {1}".format(param_key, param_value))
         except ConfigParser.NoOptionError as e:
             pprint.header("#", False, ' ')
@@ -659,14 +674,15 @@
         for param_key in needed_alfresco_global_params_4_3_2:
             try:
                 param_value = varconf.get("Parapheur", param_key)
                 pprint.header("#", False, ' ')
                 pprint.info("  {0} = {1}".format(param_key, param_value))
             except ConfigParser.NoOptionError as e:
                 pprint.error("  OMG, need this: {0}".format(param_key))
+        analyse_is_param_in_conf(needed_iparapheur_global_params_4_3_2, ihmvarconf, "I")
     if parse_version("4.4.0") <= parse_version(version_presente):
         needed_alfresco_global_params_4_4_0 = ['openOffice.test.cronExpression',
                                                'parapheur.exploit.xemelios.command']
         needed_iparapheur_global_params_4_4_0 = ['parapheur.ihm.password.strength',
                                                  'parapheur.ihm.aide.libersign.url',
                                                  'parapheur.extension.libersign.firefox.url',
                                                  'parapheur.extension.libersign.chrome.url',
@@ -674,25 +690,27 @@
         for param_key in needed_alfresco_global_params_4_4_0:
             try:
                 param_value = varconf.get("Parapheur", param_key)
                 pprint.header("#", False, ' ')
                 pprint.info("  {0} = {1}".format(param_key, param_value))
             except ConfigParser.NoOptionError as e:
                 pprint.error("  OMG, need this: {0}".format(param_key))
+        analyse_is_param_in_conf(needed_iparapheur_global_params_4_4_0, ihmvarconf, "I")
     if parse_version("4.4.1") <= parse_version(version_presente):
         needed_alfresco_global_params_4_4_1 = ['parapheur.document.lockedPDF.accept',
                                                'parapheur.hostname']
         needed_iparapheur_global_params_4_4_1 = ['parapheur.ihm.admin.users.connected.threshold']
         for param_key in needed_alfresco_global_params_4_4_1:
             try:
                 param_value = varconf.get("Parapheur", param_key)
                 pprint.header("#", False, ' ')
                 pprint.info("  {0} = {1}".format(param_key, param_value))
             except ConfigParser.NoOptionError as e:
                 pprint.error("  OMG, need this: {0}".format(param_key))
+        analyse_is_param_in_conf(needed_iparapheur_global_params_4_4_1, ihmvarconf, "I")
     if parse_version("4.5.0") <= parse_version(version_presente):
         needed_alfresco_global_params_4_5 = ['parapheur.cachetserver.security.key',
                                              'parapheur.libersign.tag.cachet.name',
                                              'parapheur.libersign.tag.cachet.name.tenants',
                                              'parapheur.notification.retards.cron',
                                              'parapheur.cachetserver.warnexpiration.cronexpression',
                                              'parapheur.cachetserver.warnexpiration.daysuntilexpiration']
@@ -700,14 +718,15 @@
         for param_key in needed_alfresco_global_params_4_5:
             try:
                 param_value = varconf.get("Parapheur", param_key)
                 pprint.header("#", False, ' ')
                 pprint.info("  {0} = {1}".format(param_key, param_value))
             except ConfigParser.NoOptionError as e:
                 pprint.error("  OMG, need this: {0}".format(param_key))
+        analyse_is_param_in_conf(needed_iparapheur_global_params_4_5, ihmvarconf, "I")
 
     # has_db_url = False
     # if not has_db_url:
     #    pprint.header("#    ", False, ' ')
     #    pprint.warning("     Il manque '{1}' dans le {0}".format(alf_dir_root, "ulimit -Sn 16384"))
 
 
@@ -901,14 +920,15 @@
 check_smtp_needed("localhost")
 
 if not check_isexists_alfrescoglobal():
     pprint.error("BAD")
     sys.exit()
 
 ALF_CONFIG_PATH = "{0}/tomcat/shared/classes/alfresco-global.properties".format(defaut_iparapheur_root)
+IHM_CONFIG_PATH = "{0}/tomcat/shared/classes/iparapheur-global.properties".format(defaut_iparapheur_root)
 '''
 def get_config_app(varfichier):
  ### lire https://stackoverflow.com/questions/2819696/parsing-properties-file-in-python/25493615#25493615
  ####   https://stackoverflow.com/questions/2885190/using-pythons-configparser-to-read-a-file-without-section-name
  with open(varfichier, 'r') as f:
      config_string = '[Parapheur]\n' + f.read()
  # config_fp = StringIO.StringIO(config_string)
@@ -920,14 +940,19 @@
     config_string = '[Parapheur]\n' + f.read()
 config_fp = io.BytesIO(config_string)
 config = ConfigParser.RawConfigParser()
 config.readfp(config_fp)
 # alfrescoconfig = get_config_app(CONFIG_PATH)
 # print(config.items("Parapheur"))
 # print(config.get("Parapheur", "dir.root"))
+with open(IHM_CONFIG_PATH, 'r') as f:
+    ihmconfig_string = '[Parapheur]\n' + f.read()
+ihmconfig_fp = io.BytesIO(ihmconfig_string)
+ihmconfig = ConfigParser.RawConfigParser()
+ihmconfig.readfp(ihmconfig_fp)
 
 check_https_service_config(config)
 
 # check health of MySQL configuration
 check_mysql_service_config(config)
 
 # tests nettoyage libs obsoletes dans common/lib
@@ -948,13 +973,13 @@
 
 check_pastellconnector_service_config()
 
 # Controles anti-fraude
 version_ip = check_iParapheur_version_is_valid(defaut_iparapheur_root)
 
 # ne manque-t-il pas quelques paramètres?
-check_config_alfrescoglobal(config, version_ip)
+check_config_alfrescoglobal(config, ihmconfig, version_ip)
 
 # check CRONTAB
 check_crontab_jobs()
 
 pprint.info(".end.")
```

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/recupArchives.py` & `iparapheur-utils-0.9.9/parapheur/scripts/recupArchives.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
 # Params
 recup_folder = config.get(__config_section__, "folder")
 # recup_folder = "/tmp/getdoc/"
 page_size = config.get(__config_section__, "page_size")
 # page_size = "500"
 
+use_only_print_pdfs = config.get(__config_section__, "use_only_print_pdfs") == "true"
+# use_only_print_pdfs = False
 use_reduced_download_path = config.get(__config_section__, "use_reduced_download_path") == "true"
 # use_reduced_download_path = False
 purge = config.get(__config_section__, "purge") == "true"
 # purge = False
 download = config.get(__config_section__, "download") == "true"
 # download = True
 
 type_filter = config.get(__config_section__, "type_filter")
 # type_filter = "*"
 subtype_filter = config.get(__config_section__, "subtype_filter")
 # subtype_filter = "*"
 waiting_days = int(config.get(__config_section__, "waiting_days"))
-
-
 # waiting_days = 0
 
 
 # region Private methods
 
 
 def move_incomplete_download_to_temp(path):
@@ -209,40 +209,43 @@
         type_clean = cleanup_special_chars(dossier['type'])
         subtype_clean = cleanup_special_chars(dossier['sousType'])
 
         if download:
 
             # Create folders
 
-            if use_reduced_download_path:
-                download_folder_path = get_reduced_folder_path(type_clean, subtype_clean, title_clean, dossier['id'])
+            if use_only_print_pdfs:
+                download_folder_path = recup_folder
             else:
-                download_folder_path = get_full_folder_path(type_clean, subtype_clean, title_clean, dossier['id'])
+                if use_reduced_download_path:
+                    download_folder_path = get_reduced_folder_path(type_clean, subtype_clean, title_clean, dossier['id'])
+                else:
+                    download_folder_path = get_full_folder_path(type_clean, subtype_clean, title_clean, dossier['id'])
 
             # Cleanup
 
             is_already_downloaded = os.path.exists("{0}/.done".format(download_folder_path))
 
             if use_reduced_download_path:
                 folder_already_contains_data = len(os.listdir(download_folder_path)) > 2
             else:
                 folder_already_contains_data = len(os.listdir(download_folder_path)) > 0
 
-            if folder_already_contains_data and not is_already_downloaded:
+            if folder_already_contains_data and not is_already_downloaded and not use_only_print_pdfs:
                 move_incomplete_download_to_temp(download_folder_path)
 
                 if use_reduced_download_path:
                     download_folder_path = get_reduced_folder_path(type_clean, subtype_clean, title_clean,
                                                                    dossier['id'])
                 else:
                     download_folder_path = get_full_folder_path(type_clean, subtype_clean, title_clean, dossier['id'])
 
             # Download content
 
-            if not is_already_downloaded:
+            if not is_already_downloaded and not use_only_print_pdfs:
 
                 content_url = "/api/node/content/workspace/SpacesStore/{0}/{1}".format(dossier['id'], title_clean)
                 content_url = content_url.replace(" ", "%20")
                 client.dodownload(content_url, "{0}/{1}".format(download_folder_path, title_clean))
 
                 if dossier['original'] == "true":
 
@@ -266,20 +269,29 @@
                         dossier['id'], title_clean)
                     sign_url = sign_url.replace(" ", "%20")
                     client.dodownload(sign_url, "{0}/{1}_sig.zip".format(download_folder_path, title_clean))
 
                 os.mknod("{0}/.done".format(download_folder_path))
                 # pprint.success("Downloaded : {0} ({1}/{2})".format(dossier['id'], dossier_index + 1, len(dossiers_archive)))
             else:
-                pprint.warning("Already downloaded : {0} ({1}/{2})".format(dossier['id'], dossier_index + 1,
-                                                                           len(dossiers_archive)))
+                if not use_only_print_pdfs:
+                    pprint.warning("Already downloaded : {0} ({1}/{2})".format(dossier['id'], dossier_index + 1,
+                                                                               len(dossiers_archive)))
+
+            # very special thing (only print-PDF files, flat-stored. sogecap-style)
+
+            if use_only_print_pdfs:
+                content_url = "/api/node/content/workspace/SpacesStore/{0}/{1}".format(dossier['id'], title_clean)
+                content_url = content_url.replace(" ", "%20")
+                client.dodownload(content_url, "{0}/{1}".format(download_folder_path, title_clean))
+
 
         if purge:
             if download:
-                if os.path.exists("{0}/.done".format(download_folder_path)):
+                if os.path.exists("{0}/.done".format(download_folder_path)) or use_only_print_pdfs:
                     client.executescript("removeNode.js", format=(dossier['id'],))
             else:
                 client.executescript("removeNode.js", format=(dossier['id'],))
                 #  pprint.success("Deleted : {0} ({1}/{2})".format(dossier['id'], dossier_index + 1, len(dossiers_archive)))
 
         bar.next()
```

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/__init__.py` & `iparapheur-utils-0.9.9/parapheur/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/script/ipclean.sh` & `iparapheur-utils-0.9.9/parapheur/scripts/script/ipclean.sh`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/remove_ldap.py` & `iparapheur-utils-0.9.9/parapheur/scripts/remove_ldap.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/import_data.py` & `iparapheur-utils-0.9.9/parapheur/scripts/import_data.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/change_name.py` & `iparapheur-utils-0.9.9/parapheur/scripts/change_name.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/scripts/export_data.py` & `iparapheur-utils-0.9.9/parapheur/scripts/export_data.py`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/core.py` & `iparapheur-utils-0.9.9/parapheur/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     parser.add_argument('-p', help='Mot de passe')
 
     parser.add_argument('-f', help='Répertoire de destination')
     parser.add_argument('-ps', help='Taille des pages à récupérer')
     parser.add_argument('-r', help='Chemins réduis des téléchargements', choices=["true", "false"])
     parser.add_argument('-pu', help='Active la purge les données', choices=["true", "false"])
     parser.add_argument('-d', help='Télécharge les données', choices=["true", "false"])
+    parser.add_argument('-pdf', help='Télécharge seulement les bordereaux PDF', choices=["true", "false"])
     parser.add_argument('-t', help='Filtre sur type')
     parser.add_argument('-st', help='Filtre sur sous-type')
     parser.add_argument('-w', help='Délai de conservation des données')
 
     args = parser.parse_args()
 
     if args.c:
@@ -112,14 +113,16 @@
 
     if args.f:
         parapheur.setconfigproperty("RecupArchives", "folder", args.f)
     if args.ps:
         parapheur.setconfigproperty("RecupArchives", "page_size", args.ps)
     if args.r:
         parapheur.setconfigproperty("RecupArchives", "use_reduced_download_path", args.r)
+    if args.pdf:
+        parapheur.setconfigproperty("RecupArchives", "use_only_print_pdfs", args.pdf)
     if args.pu:
         parapheur.setconfigproperty("RecupArchives", "purge", args.pu)
     if args.d:
         parapheur.setconfigproperty("RecupArchives", "download", args.d)
     if args.t:
         parapheur.setconfigproperty("RecupArchives", "type_filter", args.t)
     if args.st:
```

### Comparing `iparapheur-utils-0.9.8/parapheur/files/private.pem` & `iparapheur-utils-0.9.9/parapheur/files/private.pem`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/parapheur/files/public.pem` & `iparapheur-utils-0.9.9/parapheur/files/public.pem`

 * *Files identical despite different names*

### Comparing `iparapheur-utils-0.9.8/setup.py` & `iparapheur-utils-0.9.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     name='iparapheur-utils',
     version=parapheur.__version__,
     packages=find_packages(),
     author="Lukas Hameury",
     author_email="lukas.hameury@libriciel.fr",
     description="Client python pour i-Parapheur",
     long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     install_requires=[
         'suds',
         'requests>=2.16.0',
         'importlib',
         'PyMySql',
         'progress'
     ],
```

### Comparing `iparapheur-utils-0.9.8/PKG-INFO` & `iparapheur-utils-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: iparapheur-utils
-Version: 0.9.8
+Version: 0.9.9
 Summary: Client python pour i-Parapheur
 Home-page: https://gitlab.libriciel.fr/i-parapheur/client-python
 Author: Lukas Hameury
 Author-email: lukas.hameury@libriciel.fr
 License: CeCILL v2
 Description: # Introduction
         
@@ -295,15 +295,16 @@
           -h, --help  Affiche ce message et quitte
         
         ```
         
         
         ## `ph-count_files`
         
-        Cette commande affiche un tableau récapitulatif des dossiers par bureaux.
+        Cette commande affiche un tableau récapitulatif des dossiers par bureaux. Si le parapheur est multitenant 2 tableaux 
+        sont proposés: les dossiers en fin de parcours par tenant et le nombre d'archives par tenant.
         
         Exemple d'utilisation :
         ```bash
         usage: ph-count_files [-h]
         
         Arguments:
           -h, --help  Affiche ce message et quitte
@@ -369,7 +370,8 @@
         Par exemple, pour un appel de `ph-echo` vers `secure-iparapheur.dom.local`, la commande sera :
         
         ```bash
         NO_PROXY="secure-iparapheur.dom.local" ph-echo
         ```
         
 Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `iparapheur-utils-0.9.8/CHANGELOG.md` & `iparapheur-utils-0.9.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Change Log
 Tous les changements notables sur ce projet seront documentés dans ce fichier.
 
 Ce format est basé sur [Keep a Changelog](http://keepachangelog.com/)
 et ce projet adhère au [Semantic Versioning](http://semver.org/).
 
-## [0.9.8] - 2019-04-17
+## [0.9.9] - 2019-05-28
+
+### Ajouts
+- Nouveau paramètre pour la fonction `ph-recupArchives` : `use_only_print_pdfs` permettant de récupérer uniquement les PDF d'impression
+
+### Modifications
+- La fonction `count-files` prend en compte les parapheur multitenant.
+- `ldapsearch`: la requête qui liste les utilisateurs est lancée sans caractère d'échappement.
+
+## [0.9.8] - 2019-04-24
 
 ### Corrections
 - Coquille dans le core.py pour count_files
 - import_data.py: modifiction des conditions d'importation de groupe
 
 ## [0.9.7] - 2019-04-17
 
 ### Ajouts
-- Ajout de la fonction 'count_files' qui permet d'afficher un tableau de tous les dossiers par bureaux.
+- Ajout de la fonction `count_files` qui permet d'afficher un tableau de tous les dossiers par bureaux.
 
 ## [0.9.6] - 2019-03-12
 
 ### Ajouts
 - Ajout de la fonction `ldapsearch` qui génère vérifie la présence du fichier conf, les propriétés, la requêtes LDAP et 
 la liste des utilisateurs retournés.
```

