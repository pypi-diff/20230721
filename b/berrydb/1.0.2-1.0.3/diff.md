# Comparing `tmp/berrydb-1.0.2.tar.gz` & `tmp/berrydb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berrydb-1.0.2.tar", last modified: Tue Jul 18 15:33:24 2023, max compression
+gzip compressed data, was "berrydb-1.0.3.tar", last modified: Fri Jul 21 06:09:58 2023, max compression
```

## Comparing `berrydb-1.0.2.tar` & `berrydb-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-18 15:33:24.409824 berrydb-1.0.2/
--rw-rw-r--   0 akash     (1000) akash     (1000)    11157 2023-07-18 15:32:32.000000 berrydb-1.0.2/BerryDB.py
--rw-rw-r--   0 akash     (1000) akash     (1000)      405 2023-07-18 15:33:24.409824 berrydb-1.0.2/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      151 2023-07-05 10:36:56.000000 berrydb-1.0.2/README.md
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-18 15:33:24.409824 berrydb-1.0.2/berrydb.egg-info/
--rw-rw-r--   0 akash     (1000) akash     (1000)      405 2023-07-18 15:33:24.000000 berrydb-1.0.2/berrydb.egg-info/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      183 2023-07-18 15:33:24.000000 berrydb-1.0.2/berrydb.egg-info/SOURCES.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-07-18 15:33:24.000000 berrydb-1.0.2/berrydb.egg-info/dependency_links.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        9 2023-07-18 15:33:24.000000 berrydb-1.0.2/berrydb.egg-info/requires.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        8 2023-07-18 15:33:24.000000 berrydb-1.0.2/berrydb.egg-info/top_level.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)       38 2023-07-18 15:33:24.409824 berrydb-1.0.2/setup.cfg
--rw-rw-r--   0 akash     (1000) akash     (1000)      508 2023-07-18 15:23:43.000000 berrydb-1.0.2/setup.py
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-21 06:09:58.648478 berrydb-1.0.3/
+-rw-rw-r--   0 akash     (1000) akash     (1000)    11470 2023-07-21 06:05:47.000000 berrydb-1.0.3/BerryDB.py
+-rw-rw-r--   0 akash     (1000) akash     (1000)      405 2023-07-21 06:09:58.648478 berrydb-1.0.3/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)      151 2023-07-05 10:36:56.000000 berrydb-1.0.3/README.md
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-21 06:09:58.648478 berrydb-1.0.3/berrydb.egg-info/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      405 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)      183 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/SOURCES.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/dependency_links.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        9 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/requires.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        8 2023-07-21 06:09:58.000000 berrydb-1.0.3/berrydb.egg-info/top_level.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)       38 2023-07-21 06:09:58.648478 berrydb-1.0.3/setup.cfg
+-rw-rw-r--   0 akash     (1000) akash     (1000)      508 2023-07-21 06:09:20.000000 berrydb-1.0.3/setup.py
```

### Comparing `berrydb-1.0.2/BerryDB.py` & `berrydb-1.0.3/BerryDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,26 +68,31 @@
             jsonResponse = response.json()
             if debug_mode:
                 print("databases result ", jsonResponse)
             if (
                 "database" in jsonResponse
                 and "responseList" in jsonResponse["database"]
             ):
-                databaseNames = []
+                databaseNames = {}
                 # print("\nDatabases:")
                 for db in jsonResponse["database"]["responseList"]:
-                    if "name" in db:
-                        databaseNames.append(db["name"])
-                        # print("\t" + db["name"])
-                print("\n")
+                    name = db["name"] if db["name"] else ""
+                    schemaName = db["schemaName"] if db["schemaName"] else ""
+                    description = db["description"] if db["description"] else ""
+                    databaseNames[name] = {
+                        "schemaName": schemaName,
+                        "description": description,
+                    }
+                    # print(name + " : " + str(databaseNames[name]))
+                # print("\n")
                 return databaseNames
-            return []
+            return {}
         except Exception as e:
             print("Failed to fetch databases: {}".format(str(e)))
-            return []
+            return {}
 
     def __getDataBaseId(self, api_key: str, database_name: str) -> int:
         """Function summary
 
         Args:
             arg1 (str): API Key
             arg2 (str): Database Name
```

