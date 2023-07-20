# Comparing `tmp/talc-0.0.3.tar.gz` & `tmp/talc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talc-0.0.3.tar", last modified: Thu Jul 20 20:30:26 2023, max compression
+gzip compressed data, was "talc-0.0.5.tar", last modified: Thu Jul 20 23:10:55 2023, max compression
```

## Comparing `talc-0.0.3.tar` & `talc-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.310779 talc-0.0.3/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.3/LICENSE
--rw-r--r--   0 mkerr      (501) staff       (20)      648 2023-07-20 20:30:26.310655 talc-0.0.3/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      274 2023-07-10 19:53:13.000000 talc-0.0.3/README.md
--rw-r--r--   0 mkerr      (501) staff       (20)      531 2023-07-20 20:29:04.000000 talc-0.0.3/pyproject.toml
--rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-20 20:30:26.310814 talc-0.0.3/setup.cfg
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.308798 talc-0.0.3/src/
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.309282 talc-0.0.3/src/talc/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.3/src/talc/__init__.py
--rw-r--r--   0 mkerr      (501) staff       (20)     6537 2023-07-20 20:28:21.000000 talc-0.0.3/src/talc/talc.py
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 20:30:26.310480 talc-0.0.3/src/talc.egg-info/
--rw-r--r--   0 mkerr      (501) staff       (20)      648 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/SOURCES.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/dependency_links.txt
--rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/requires.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-20 20:30:26.000000 talc-0.0.3/src/talc.egg-info/top_level.txt
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 23:10:55.398770 talc-0.0.5/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.5/LICENSE
+-rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-20 23:10:55.398645 talc-0.0.5/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)     1642 2023-07-20 23:07:33.000000 talc-0.0.5/README.md
+-rw-r--r--   0 mkerr      (501) staff       (20)      585 2023-07-20 23:10:47.000000 talc-0.0.5/pyproject.toml
+-rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-20 23:10:55.398803 talc-0.0.5/setup.cfg
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 23:10:55.397242 talc-0.0.5/src/
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 23:10:55.397863 talc-0.0.5/src/talc/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.5/src/talc/__init__.py
+-rw-r--r--   0 mkerr      (501) staff       (20)     6671 2023-07-20 20:36:20.000000 talc-0.0.5/src/talc/talc.py
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-20 23:10:55.398481 talc-0.0.5/src/talc.egg-info/
+-rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-20 23:10:55.000000 talc-0.0.5/src/talc.egg-info/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-20 23:10:55.000000 talc-0.0.5/src/talc.egg-info/SOURCES.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-20 23:10:55.000000 talc-0.0.5/src/talc.egg-info/dependency_links.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-20 23:10:55.000000 talc-0.0.5/src/talc.egg-info/requires.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-20 23:10:55.000000 talc-0.0.5/src/talc.egg-info/top_level.txt
```

### Comparing `talc-0.0.3/pyproject.toml` & `talc-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talc"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
   { name="Max Kerr", email="max@talc.ai" },
   { name="Matt Lee", email="matt@talc.ai" },
 ]
-description = "Logging client for Talc."
+description = "Logging client for Talc Debugger."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "supabase>=1.0.3",
     "openai>=0.11.6",
-]
+]
+
+[project.urls]
+homepage = "https://talc.ai"
```

### Comparing `talc-0.0.3/src/talc/talc.py` & `talc-0.0.5/src/talc/talc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,33 @@
         )
         key: str = os.environ.get(
             "INSTANCE_ANON_KEY",
             default="eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InFkZ29keGtmeHp6bXp3ZmxpYWhoIiwicm9sZSI6ImFub24iLCJpYXQiOjE2ODg0OTc0NzcsImV4cCI6MjAwNDA3MzQ3N30.4bgCdg77wwOJ9w1hOtCD-z0gBVGv8X_kIxBCr5KDCuA",
         )
 
         # API key format is organization:api_key
-        talc_api_key: str = os.environ.get("TALC_API_KEY", default="")
+        talc_api_key: str = os.environ.get("TALC_API_KEY", default=":")
 
         if talc_api_key == "":
             logging.warning(
                 "TALC_API_KEY environment variable not set. Logging disabled."
             )
+            self.__initialized = False
             return
+
         organization, api_key = talc_api_key.split(":")
         self.__organization: str = organization
 
         options = ClientOptions(headers={"talckey": api_key})
         self.supabase: Client = create_client(url, key, options=options)
+        self.__initialized = True
 
     def createSession(self):
+        if not self.__initialized:
+            return None
         response = (
             self.supabase.table("sessions")
             .insert(
                 {
                     "organization": self.__organization,
                 }
             )
```

