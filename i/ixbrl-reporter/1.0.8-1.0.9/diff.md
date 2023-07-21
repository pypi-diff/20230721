# Comparing `tmp/ixbrl-reporter-1.0.8.tar.gz` & `tmp/ixbrl-reporter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrl-reporter-1.0.8.tar", last modified: Mon Jun 27 18:48:48 2022, max compression
+gzip compressed data, was "ixbrl-reporter-1.0.9.tar", last modified: Fri Jul  1 09:13:36 2022, max compression
```

## Comparing `ixbrl-reporter-1.0.8.tar` & `ixbrl-reporter-1.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-06-27 18:48:48.976106 ixbrl-reporter-1.0.8/
--rw-rw-r--   0 mark      (1000) mark      (1000)    35149 2021-12-29 10:59:33.000000 ixbrl-reporter-1.0.8/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)     8368 2022-06-27 18:48:48.976106 ixbrl-reporter-1.0.8/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     7718 2022-01-11 15:13:05.000000 ixbrl-reporter-1.0.8/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-06-27 18:48:48.975106 ixbrl-reporter-1.0.8/ixbrl_reporter/
--rw-rw-r--   0 mark      (1000) mark      (1000)        2 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      407 2022-01-11 15:13:05.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/accounts.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3951 2022-05-04 09:16:34.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/accounts_csv.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     5187 2022-03-08 12:30:45.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/accounts_gnucash.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6427 2022-06-27 18:39:53.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/accounts_piecash.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     9014 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/basic_element.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      973 2022-02-12 18:02:31.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/composite.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    14156 2022-03-29 09:07:09.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/computation.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6832 2022-02-10 19:28:37.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/config.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3128 2022-02-08 12:04:14.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/context.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     5796 2022-02-10 15:37:25.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/data_source.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1430 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/datum.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1927 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/debug_reporter.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1136 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/element.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1585 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/expand.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4771 2022-02-04 11:24:05.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/fact.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2721 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/fact_table.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3184 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/flex_sheet.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      580 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/format.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      843 2022-01-11 15:13:05.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/html.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    11488 2022-01-10 14:06:20.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/ixbrl_reporter.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8850 2022-02-04 11:24:05.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/layout.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1435 2022-02-10 15:35:17.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/note_heading.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4703 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/note_parse.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1867 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/notes.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1172 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/page.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      992 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/period.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      772 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/result.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3875 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/simple_sheet.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3209 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/table.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    10795 2022-02-10 19:41:24.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/taxonomy.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3036 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/text_reporter.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      837 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/valueset.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       27 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/worksheet.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1723 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.8/ixbrl_reporter/worksheet_element.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-06-27 18:48:48.976106 ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     8368 2022-06-27 18:48:48.000000 ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     1221 2022-06-27 18:48:48.000000 ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2022-06-27 18:48:48.000000 ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       29 2022-06-27 18:48:48.000000 ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       15 2022-06-27 18:48:48.000000 ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-06-27 18:48:48.976106 ixbrl-reporter-1.0.8/scripts/
--rwxrwxr-x   0 mark      (1000) mark      (1000)     1454 2022-02-04 11:24:05.000000 ixbrl-reporter-1.0.8/scripts/ixbrl-reporter
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2022-06-27 18:48:48.976106 ixbrl-reporter-1.0.8/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      968 2022-06-27 18:48:00.000000 ixbrl-reporter-1.0.8/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-07-01 09:13:36.055494 ixbrl-reporter-1.0.9/
+-rw-rw-r--   0 mark      (1000) mark      (1000)    35149 2021-12-29 10:59:33.000000 ixbrl-reporter-1.0.9/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8368 2022-07-01 09:13:36.054494 ixbrl-reporter-1.0.9/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7718 2022-01-11 15:13:05.000000 ixbrl-reporter-1.0.9/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-07-01 09:13:36.054494 ixbrl-reporter-1.0.9/ixbrl_reporter/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        2 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      407 2022-01-11 15:13:05.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/accounts.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3951 2022-05-04 09:16:34.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/accounts_csv.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5344 2022-07-01 09:12:34.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/accounts_gnucash.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6427 2022-06-27 18:39:53.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/accounts_piecash.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     9014 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/basic_element.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      973 2022-02-12 18:02:31.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/composite.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    14156 2022-03-29 09:07:09.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/computation.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6832 2022-02-10 19:28:37.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/config.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3128 2022-02-08 12:04:14.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/context.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5796 2022-02-10 15:37:25.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/data_source.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1430 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/datum.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1927 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/debug_reporter.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1136 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/element.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1585 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/expand.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4771 2022-02-04 11:24:05.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/fact.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2721 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/fact_table.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3184 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/flex_sheet.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      580 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/format.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      843 2022-01-11 15:13:05.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/html.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    11488 2022-01-10 14:06:20.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/ixbrl_reporter.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8850 2022-02-04 11:24:05.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/layout.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1435 2022-02-10 15:35:17.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/note_heading.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4703 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/note_parse.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1867 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/notes.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1172 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/page.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      992 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/period.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      772 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/result.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3875 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/simple_sheet.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3209 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/table.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    10795 2022-02-10 19:41:24.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/taxonomy.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3036 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/text_reporter.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      837 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/valueset.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       27 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/worksheet.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1723 2021-12-29 11:16:41.000000 ixbrl-reporter-1.0.9/ixbrl_reporter/worksheet_element.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-07-01 09:13:36.054494 ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8368 2022-07-01 09:13:35.000000 ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1221 2022-07-01 09:13:35.000000 ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2022-07-01 09:13:35.000000 ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       29 2022-07-01 09:13:35.000000 ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       15 2022-07-01 09:13:35.000000 ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-07-01 09:13:36.054494 ixbrl-reporter-1.0.9/scripts/
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     1454 2022-02-04 11:24:05.000000 ixbrl-reporter-1.0.9/scripts/ixbrl-reporter
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2022-07-01 09:13:36.055494 ixbrl-reporter-1.0.9/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      968 2022-07-01 09:13:06.000000 ixbrl-reporter-1.0.9/setup.py
```

### Comparing `ixbrl-reporter-1.0.8/LICENSE` & `ixbrl-reporter-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/PKG-INFO` & `ixbrl-reporter-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ixbrl-reporter
-Version: 1.0.8
+Version: 1.0.9
 Summary: Production of iXBRL reports from templates and accounts files
 Home-page: https://github.com/cybermaggedon/ixbrl-reporter
 Author: Cybermaggedon
 Author-email: mark@cyberapocalypse.co.uk
 License: UNKNOWN
-Download-URL: https://github.com/cybermaggedon/ixbrl-reporter/archive/refs/tags/v1.0.8.tar.gz
+Download-URL: https://github.com/cybermaggedon/ixbrl-reporter/archive/refs/tags/v1.0.9.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ixbrl-reporter-1.0.8/README.md` & `ixbrl-reporter-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/accounts_csv.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/accounts_csv.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/accounts_gnucash.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/accounts_gnucash.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,22 +84,34 @@
                 )
 
         return splits
 
     # Return an account given an account locator.  Navigates through
     # hierarchy, account parts are colon separated.
     def get_account(self, par, locator):
+
         if par == None:
             acct = self.root
         else:
             acct = par
+
         for v in locator.split(":"):
-            acct = acct.lookup_by_name(v)
-            if acct == None:
+
+            ch_acct = None
+
+            for ch in acct.get_children():
+                if ch.name == v:
+                    ch_acct = ch
+                    break
+
+            if ch_acct == None:
                 raise RuntimeError("Can't locate account '%s'" % locator)
+
+            acct = ch_acct
+
         return acct
 
     def get_accounts(self, acct=None, pfx=""):
 
         if acct == None: acct = self.root
 
         ch = acct.get_children()
```

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/accounts_piecash.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/accounts_piecash.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/basic_element.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/basic_element.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/composite.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/composite.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/computation.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/computation.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/config.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/config.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/context.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/context.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/data_source.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/data_source.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/datum.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/datum.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/debug_reporter.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/debug_reporter.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/element.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/element.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/expand.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/expand.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/fact.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/fact.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/fact_table.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/fact_table.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/flex_sheet.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/flex_sheet.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/format.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/format.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/html.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/html.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/ixbrl_reporter.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/ixbrl_reporter.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/layout.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/layout.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/note_heading.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/note_heading.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/note_parse.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/note_parse.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/notes.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/notes.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/page.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/page.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/period.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/period.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/result.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/result.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/simple_sheet.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/simple_sheet.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/table.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/table.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/taxonomy.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/text_reporter.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/text_reporter.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/valueset.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/valueset.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter/worksheet_element.py` & `ixbrl-reporter-1.0.9/ixbrl_reporter/worksheet_element.py`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/PKG-INFO` & `ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ixbrl-reporter
-Version: 1.0.8
+Version: 1.0.9
 Summary: Production of iXBRL reports from templates and accounts files
 Home-page: https://github.com/cybermaggedon/ixbrl-reporter
 Author: Cybermaggedon
 Author-email: mark@cyberapocalypse.co.uk
 License: UNKNOWN
-Download-URL: https://github.com/cybermaggedon/ixbrl-reporter/archive/refs/tags/v1.0.8.tar.gz
+Download-URL: https://github.com/cybermaggedon/ixbrl-reporter/archive/refs/tags/v1.0.9.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ixbrl-reporter-1.0.8/ixbrl_reporter.egg-info/SOURCES.txt` & `ixbrl-reporter-1.0.9/ixbrl_reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/scripts/ixbrl-reporter` & `ixbrl-reporter-1.0.9/scripts/ixbrl-reporter`

 * *Files identical despite different names*

### Comparing `ixbrl-reporter-1.0.8/setup.py` & `ixbrl-reporter-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ixbrl-reporter",
-    version="1.0.8",
+    version="1.0.9",
     author="Cybermaggedon",
     author_email="mark@cyberapocalypse.co.uk",
     description="Production of iXBRL reports from templates and accounts files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cybermaggedon/ixbrl-reporter",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    download_url = "https://github.com/cybermaggedon/ixbrl-reporter/archive/refs/tags/v1.0.8.tar.gz",
+    download_url = "https://github.com/cybermaggedon/ixbrl-reporter/archive/refs/tags/v1.0.9.tar.gz",
     install_requires=[
         "requests", "lxml", "piecash", "PyYAML"
     ],
     scripts=[
         "scripts/ixbrl-reporter"
     ]
 )
```

