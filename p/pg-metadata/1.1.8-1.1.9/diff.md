# Comparing `tmp/pg_metadata-1.1.8.tar.gz` & `tmp/pg_metadata-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pg_metadata-1.1.8.tar", last modified: Tue May 24 08:43:31 2022, max compression
+gzip compressed data, was "dist\pg_metadata-1.1.9.tar", last modified: Tue May 24 15:19:15 2022, max compression
```

## Comparing `pg_metadata-1.1.8.tar` & `pg_metadata-1.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/
--rw-rw-rw-   0        0        0     3418 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2203 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/pg_metadata/
--rw-rw-rw-   0        0        0     2256 2022-05-24 08:37:42.000000 pg_metadata-1.1.8/pg_metadata/Cast.py
--rw-rw-rw-   0        0        0     1285 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/Comment.py
--rw-rw-rw-   0        0        0     1845 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/DDL.py
--rw-rw-rw-   0        0        0    30722 2022-05-24 08:42:54.000000 pg_metadata-1.1.8/pg_metadata/Database.py
--rw-rw-rw-   0        0        0     6116 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/Diff.py
--rw-rw-rw-   0        0        0     3228 2022-05-16 13:42:48.000000 pg_metadata-1.1.8/pg_metadata/EventTrigger.py
--rw-rw-rw-   0        0        0     2303 2022-05-16 13:42:48.000000 pg_metadata-1.1.8/pg_metadata/Extension.py
--rw-rw-rw-   0        0        0     3404 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/ForeignServer.py
--rw-rw-rw-   0        0        0     4207 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/ForeignTable.py
--rw-rw-rw-   0        0        0     5804 2022-05-24 06:24:33.000000 pg_metadata-1.1.8/pg_metadata/Function.py
--rw-rw-rw-   0        0        0     2337 2022-05-23 06:47:45.000000 pg_metadata-1.1.8/pg_metadata/Grabber.py
--rw-rw-rw-   0        0        0     2459 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/Grant.py
--rw-rw-rw-   0        0        0     2866 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/Namespace.py
--rw-rw-rw-   0        0        0     1264 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/Owner.py
--rw-rw-rw-   0        0        0     3451 2022-05-16 13:42:48.000000 pg_metadata-1.1.8/pg_metadata/Publication.py
--rw-rw-rw-   0        0        0     4714 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/Sequence.py
--rw-rw-rw-   0        0        0     4513 2022-05-16 13:42:48.000000 pg_metadata-1.1.8/pg_metadata/Subscription.py
--rw-rw-rw-   0        0        0     3551 2022-05-16 13:42:48.000000 pg_metadata-1.1.8/pg_metadata/System.py
--rw-rw-rw-   0        0        0     7847 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/Table.py
--rw-rw-rw-   0        0        0     4472 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/TableColumn.py
--rw-rw-rw-   0        0        0     3297 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/TableConstraint.py
--rw-rw-rw-   0        0        0     1809 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/TableIndex.py
--rw-rw-rw-   0        0        0     1772 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/TableSettings.py
--rw-rw-rw-   0        0        0     2452 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/TableTrigger.py
--rw-rw-rw-   0        0        0     4421 2022-04-06 09:27:37.000000 pg_metadata-1.1.8/pg_metadata/View.py
--rw-rw-rw-   0        0        0       22 2020-01-15 06:06:44.000000 pg_metadata-1.1.8/pg_metadata/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/pg_metadata.egg-info/
--rw-rw-rw-   0        0        0     3418 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/pg_metadata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/pg_metadata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/pg_metadata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/pg_metadata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/pg_metadata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-24 08:43:31.000000 pg_metadata-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      752 2022-05-24 08:41:25.000000 pg_metadata-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-24 15:19:15.000000 pg_metadata-1.1.9/
+-rw-rw-rw-   0        0        0     3418 2022-05-24 15:19:15.000000 pg_metadata-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2203 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-24 15:19:15.000000 pg_metadata-1.1.9/pg_metadata/
+-rw-rw-rw-   0        0        0     2256 2022-05-24 08:37:42.000000 pg_metadata-1.1.9/pg_metadata/Cast.py
+-rw-rw-rw-   0        0        0     1285 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/Comment.py
+-rw-rw-rw-   0        0        0     1845 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/DDL.py
+-rw-rw-rw-   0        0        0    30722 2022-05-24 08:42:54.000000 pg_metadata-1.1.9/pg_metadata/Database.py
+-rw-rw-rw-   0        0        0     6116 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/Diff.py
+-rw-rw-rw-   0        0        0     3187 2022-05-24 15:17:11.000000 pg_metadata-1.1.9/pg_metadata/EventTrigger.py
+-rw-rw-rw-   0        0        0     2303 2022-05-16 13:42:48.000000 pg_metadata-1.1.9/pg_metadata/Extension.py
+-rw-rw-rw-   0        0        0     3404 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/ForeignServer.py
+-rw-rw-rw-   0        0        0     4207 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/ForeignTable.py
+-rw-rw-rw-   0        0        0     5804 2022-05-24 06:24:33.000000 pg_metadata-1.1.9/pg_metadata/Function.py
+-rw-rw-rw-   0        0        0     2337 2022-05-23 06:47:45.000000 pg_metadata-1.1.9/pg_metadata/Grabber.py
+-rw-rw-rw-   0        0        0     2459 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/Grant.py
+-rw-rw-rw-   0        0        0     2866 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/Namespace.py
+-rw-rw-rw-   0        0        0     1264 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/Owner.py
+-rw-rw-rw-   0        0        0     3451 2022-05-16 13:42:48.000000 pg_metadata-1.1.9/pg_metadata/Publication.py
+-rw-rw-rw-   0        0        0     4714 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/Sequence.py
+-rw-rw-rw-   0        0        0     4513 2022-05-16 13:42:48.000000 pg_metadata-1.1.9/pg_metadata/Subscription.py
+-rw-rw-rw-   0        0        0     3551 2022-05-16 13:42:48.000000 pg_metadata-1.1.9/pg_metadata/System.py
+-rw-rw-rw-   0        0        0     7847 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/Table.py
+-rw-rw-rw-   0        0        0     4472 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/TableColumn.py
+-rw-rw-rw-   0        0        0     3297 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/TableConstraint.py
+-rw-rw-rw-   0        0        0     1809 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/TableIndex.py
+-rw-rw-rw-   0        0        0     1772 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/TableSettings.py
+-rw-rw-rw-   0        0        0     2452 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/TableTrigger.py
+-rw-rw-rw-   0        0        0     4421 2022-04-06 09:27:37.000000 pg_metadata-1.1.9/pg_metadata/View.py
+-rw-rw-rw-   0        0        0       22 2020-01-15 06:06:44.000000 pg_metadata-1.1.9/pg_metadata/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-24 15:19:15.000000 pg_metadata-1.1.9/pg_metadata.egg-info/
+-rw-rw-rw-   0        0        0     3418 2022-05-24 15:19:14.000000 pg_metadata-1.1.9/pg_metadata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-05-24 15:19:14.000000 pg_metadata-1.1.9/pg_metadata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-24 15:19:14.000000 pg_metadata-1.1.9/pg_metadata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2022-05-24 15:19:14.000000 pg_metadata-1.1.9/pg_metadata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-05-24 15:19:14.000000 pg_metadata-1.1.9/pg_metadata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-24 15:19:15.000000 pg_metadata-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      752 2022-05-24 15:17:20.000000 pg_metadata-1.1.9/setup.py
```

### Comparing `pg_metadata-1.1.8/PKG-INFO` & `pg_metadata-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg_metadata
-Version: 1.1.8
+Version: 1.1.9
 Summary: PostgreSQL metadata grabber and comparer
 Home-page: https://github.com/ish1mura/pg_metadata
 Author: ish1mura
 Author-email: ek.dummy@gmail.com
 License: UNKNOWN
 Description: # Description
```

### Comparing `pg_metadata-1.1.8/README.md` & `pg_metadata-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Cast.py` & `pg_metadata-1.1.9/pg_metadata/Cast.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Comment.py` & `pg_metadata-1.1.9/pg_metadata/Comment.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/DDL.py` & `pg_metadata-1.1.9/pg_metadata/DDL.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Database.py` & `pg_metadata-1.1.9/pg_metadata/Database.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Diff.py` & `pg_metadata-1.1.9/pg_metadata/Diff.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/EventTrigger.py` & `pg_metadata-1.1.9/pg_metadata/EventTrigger.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,14 @@
             "Event trigger event is null"
 
         self.Function = (data.get("fnc") or "").strip()
         assert len(self.Function) > 0, \
             "Event trigger function is null"
 
         self.Tags = (data.get("tags") or [])
-        assert len(self.Tags) > 0, \
-            "Event trigger tags is null"
 
         self.Owner = Owner(
             self.GetObjectName(),
             {
                 "instance_type" : self.GetTag(),
                 "instance_name" : self.GetFullName(),
                 "owner_name"    : data.get("owner")
@@ -64,15 +62,18 @@
         r = ""
         r += "-- Event trigger: {0}".format(self.GetFullName()) + SEP
         r += SEP
         r += "-- {0}".format(self.DDL_Drop()) + SEP
         r += SEP
         r += "CREATE {0} {1}".format(self.GetTag(), self.GetFullName()) + SEP
         r += "  ON {0}".format(self.Event) + SEP
-        r += "  WHERE TAG IN ({0})".format(", ".join(["'{0}'".format(i) for i in sorted(self.Tags)])) + SEP
+
+        if len(self.Tags) > 0:
+            r += "  WHEN TAG IN ({0})".format(", ".join(["'{0}'".format(i) for i in sorted(self.Tags)])) + SEP
+
         r += "  EXECUTE PROCEDURE {0};".format(self.Function) + SEP
         r += SEP
         r += self.Owner.DDL_Create() + SEP
         r += SEP
         r += self.DDL_Status() + SEP
         return r.strip() + SEP
```

### Comparing `pg_metadata-1.1.8/pg_metadata/Extension.py` & `pg_metadata-1.1.9/pg_metadata/Extension.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/ForeignServer.py` & `pg_metadata-1.1.9/pg_metadata/ForeignServer.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/ForeignTable.py` & `pg_metadata-1.1.9/pg_metadata/ForeignTable.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Function.py` & `pg_metadata-1.1.9/pg_metadata/Function.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Grabber.py` & `pg_metadata-1.1.9/pg_metadata/Grabber.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Grant.py` & `pg_metadata-1.1.9/pg_metadata/Grant.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Namespace.py` & `pg_metadata-1.1.9/pg_metadata/Namespace.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Owner.py` & `pg_metadata-1.1.9/pg_metadata/Owner.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Publication.py` & `pg_metadata-1.1.9/pg_metadata/Publication.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Sequence.py` & `pg_metadata-1.1.9/pg_metadata/Sequence.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Subscription.py` & `pg_metadata-1.1.9/pg_metadata/Subscription.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/System.py` & `pg_metadata-1.1.9/pg_metadata/System.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/Table.py` & `pg_metadata-1.1.9/pg_metadata/Table.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/TableColumn.py` & `pg_metadata-1.1.9/pg_metadata/TableColumn.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/TableConstraint.py` & `pg_metadata-1.1.9/pg_metadata/TableConstraint.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/TableIndex.py` & `pg_metadata-1.1.9/pg_metadata/TableIndex.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/TableSettings.py` & `pg_metadata-1.1.9/pg_metadata/TableSettings.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/TableTrigger.py` & `pg_metadata-1.1.9/pg_metadata/TableTrigger.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata/View.py` & `pg_metadata-1.1.9/pg_metadata/View.py`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/pg_metadata.egg-info/PKG-INFO` & `pg_metadata-1.1.9/pg_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-metadata
-Version: 1.1.8
+Version: 1.1.9
 Summary: PostgreSQL metadata grabber and comparer
 Home-page: https://github.com/ish1mura/pg_metadata
 Author: ish1mura
 Author-email: ek.dummy@gmail.com
 License: UNKNOWN
 Description: # Description
```

### Comparing `pg_metadata-1.1.8/pg_metadata.egg-info/SOURCES.txt` & `pg_metadata-1.1.9/pg_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pg_metadata-1.1.8/setup.py` & `pg_metadata-1.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pg_metadata",
-    version="1.1.8",
+    version="1.1.9",
     author="ish1mura",
     author_email="ek.dummy@gmail.com",
     description="PostgreSQL metadata grabber and comparer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ish1mura/pg_metadata",
     packages=setuptools.find_packages(),
```

