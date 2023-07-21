# Comparing `tmp/cool_seq_tool-0.1.8.tar.gz` & `tmp/cool_seq_tool-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool_seq_tool-0.1.8.tar", last modified: Wed Mar 22 17:24:34 2023, max compression
+gzip compressed data, was "cool_seq_tool-0.1.9.tar", last modified: Fri Mar 24 18:28:44 2023, max compression
```

## Comparing `cool_seq_tool-0.1.8.tar` & `cool_seq_tool-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:34.424939 cool_seq_tool-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-22 17:24:27.000000 cool_seq_tool-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-22 17:24:34.424939 cool_seq_tool-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-22 17:24:27.000000 cool_seq_tool-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:34.396940 cool_seq_tool-0.1.8/cool_seq_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-22 17:24:27.000000 cool_seq_tool-0.1.8/cool_seq_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-03-22 17:24:27.000000 cool_seq_tool-0.1.8/cool_seq_tool/cool_seq_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:34.400940 cool_seq_tool-0.1.8/cool_seq_tool/data/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-22 17:24:27.000000 cool_seq_tool-0.1.8/cool_seq_tool/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-22 17:24:27.000000 cool_seq_tool-0.1.8/cool_seq_tool/data/data_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123) 24138769 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data/transcript_mapping.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:34.420940 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/alignment_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/gene_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    41855 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/mane_transcript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/mane_transcript_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/residue_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/seqrepo_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/transcript_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/data_sources/uta_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:34.424939 cool_seq_tool-0.1.8/cool_seq_tool/routers/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/routers/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/routers/mane.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/routers/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20922 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/cool_seq_tool/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:34.396940 cool_seq_tool-0.1.8/cool_seq_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-22 17:24:34.000000 cool_seq_tool-0.1.8/cool_seq_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-22 17:24:34.000000 cool_seq_tool-0.1.8/cool_seq_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:24:34.000000 cool_seq_tool-0.1.8/cool_seq_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:24:34.000000 cool_seq_tool-0.1.8/cool_seq_tool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-22 17:24:34.000000 cool_seq_tool-0.1.8/cool_seq_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-22 17:24:34.000000 cool_seq_tool-0.1.8/cool_seq_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-22 17:24:34.424939 cool_seq_tool-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-22 17:24:28.000000 cool_seq_tool-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:44.492162 cool_seq_tool-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-24 18:28:44.492162 cool_seq_tool-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:44.472162 cool_seq_tool-0.1.9/cool_seq_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/cool_seq_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:44.472162 cool_seq_tool-0.1.9/cool_seq_tool/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data/data_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123) 24138769 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data/transcript_mapping.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:44.492162 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/alignment_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/gene_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41855 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/mane_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/mane_transcript_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/residue_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/seqrepo_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/transcript_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46584 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/data_sources/uta_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:44.492162 cool_seq_tool-0.1.9/cool_seq_tool/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/routers/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/routers/mane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/routers/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20922 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/cool_seq_tool/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:28:44.472162 cool_seq_tool-0.1.9/cool_seq_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-24 18:28:44.000000 cool_seq_tool-0.1.9/cool_seq_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-24 18:28:44.000000 cool_seq_tool-0.1.9/cool_seq_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 18:28:44.000000 cool_seq_tool-0.1.9/cool_seq_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 18:28:44.000000 cool_seq_tool-0.1.9/cool_seq_tool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-24 18:28:44.000000 cool_seq_tool-0.1.9/cool_seq_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-24 18:28:44.000000 cool_seq_tool-0.1.9/cool_seq_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-24 18:28:44.496162 cool_seq_tool-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 18:28:38.000000 cool_seq_tool-0.1.9/setup.py
```

### Comparing `cool_seq_tool-0.1.8/LICENSE` & `cool_seq_tool-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/PKG-INFO` & `cool_seq_tool-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool_seq_tool
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common Operations On Lots-of Sequences Tool.
 Home-page: https://github.com/GenomicMedLab/cool-seq-tool
 Author: Wagner Lab, Nationwide Childrens Hospital
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cool_seq_tool-0.1.8/README.md` & `cool_seq_tool-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/__init__.py` & `cool_seq_tool-0.1.9/cool_seq_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/cool_seq_tool.py` & `cool_seq_tool-0.1.9/cool_seq_tool/cool_seq_tool.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data/data_downloads.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data/data_downloads.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data/transcript_mapping.tsv` & `cool_seq_tool-0.1.9/cool_seq_tool/data/transcript_mapping.tsv`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/alignment_mapper.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/alignment_mapper.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/gene_normalizer.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/gene_normalizer.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/mane_transcript.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/mane_transcript.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/mane_transcript_mappings.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/mane_transcript_mappings.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/residue_mode.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/residue_mode.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/seqrepo_access.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/seqrepo_access.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/transcript_mappings.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/transcript_mappings.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/data_sources/uta_database.py` & `cool_seq_tool-0.1.9/cool_seq_tool/data_sources/uta_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,33 +17,61 @@
 from cool_seq_tool import UTA_DB_URL, logger
 from cool_seq_tool.schemas import AnnotationLayer, Assembly
 
 
 # use `bound` to upper-bound UTADatabase or child classes
 UTADatabaseType = TypeVar("UTADatabaseType", bound="UTADatabase")
 
+# Environment variables for paths to chain files for pyliftover
+LIFTOVER_CHAIN_37_TO_38 = environ.get("LIFTOVER_CHAIN_37_TO_38")
+LIFTOVER_CHAIN_38_TO_37 = environ.get("LIFTOVER_CHAIN_38_TO_37")
+
 
 class UTADatabase:
     """Class for connecting and querying UTA database."""
 
-    def __init__(self, db_url: str = UTA_DB_URL, db_pwd: str = "") -> None:
+    def __init__(
+        self,
+        db_url: str = UTA_DB_URL,
+        db_pwd: str = "",
+        chain_file_37_to_38: Optional[str] = None,
+        chain_file_38_to_37: Optional[str] = None
+    ) -> None:
         """Initialize DB class. Downstream libraries should use the create()
         method to construct a new instance: await UTADatabase.create()
 
-        :param str db_url: PostgreSQL connection URL
+        :param db_url: PostgreSQL connection URL
             Format: `driver://user:pass@host/database/schema`
-        :param str db_pwd: User's password for uta database
+        :param db_pwd: User's password for uta database
+        :param chain_file_37_to_38: Optional path to chain file for 37 to 38 assembly.
+            This is used for pyliftover. If this is not provided, will check to see if
+            LIFTOVER_CHAIN_37_TO_38 env var is set. If neither is provided, will allow
+            pyliftover to download a chain file from UCSC
+        :param chain_file_38_to_37: Optional path to chain file for 38 to 37 assembly.
+            This is used for pyliftover. If this is not provided, will check to see if
+            LIFTOVER_CHAIN_38_TO_37 env var is set. If neither is provided, will allow
+            pyliftover to download a chain file from UCSC
         """
         self.schema = None
         self.db_url = db_url
         self.db_pwd = db_pwd
         self._connection_pool = None
         self.args = self._get_conn_args()
-        self.liftover_37_to_38 = LiftOver("hg19", "hg38")
-        self.liftover_38_to_37 = LiftOver("hg38", "hg19")
+
+        chain_file_37_to_38 = chain_file_37_to_38 or LIFTOVER_CHAIN_37_TO_38
+        if chain_file_37_to_38:
+            self.liftover_37_to_38 = LiftOver(chain_file_37_to_38)
+        else:
+            self.liftover_37_to_38 = LiftOver("hg19", "hg38")
+
+        chain_file_38_to_37 = chain_file_38_to_37 or LIFTOVER_CHAIN_38_TO_37
+        if chain_file_38_to_37:
+            self.liftover_38_to_37 = LiftOver(chain_file_38_to_37)
+        else:
+            self.liftover_38_to_37 = LiftOver("hg38", "hg19")
 
     @staticmethod
     def _update_db_url(db_pwd: str, db_url: str) -> str:
         """Return new db_url containing password.
 
         :param str db_pwd: User's password for uta database
         :param str db_url: PostgreSQL connection URL
```

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/main.py` & `cool_seq_tool-0.1.9/cool_seq_tool/main.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/routers/default.py` & `cool_seq_tool-0.1.9/cool_seq_tool/routers/default.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/routers/mane.py` & `cool_seq_tool-0.1.9/cool_seq_tool/routers/mane.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/routers/mappings.py` & `cool_seq_tool-0.1.9/cool_seq_tool/routers/mappings.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool/schemas.py` & `cool_seq_tool-0.1.9/cool_seq_tool/schemas.py`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool.egg-info/PKG-INFO` & `cool_seq_tool-0.1.9/cool_seq_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-seq-tool
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common Operations On Lots-of Sequences Tool.
 Home-page: https://github.com/GenomicMedLab/cool-seq-tool
 Author: Wagner Lab, Nationwide Childrens Hospital
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cool_seq_tool-0.1.8/cool_seq_tool.egg-info/SOURCES.txt` & `cool_seq_tool-0.1.9/cool_seq_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cool_seq_tool-0.1.8/setup.cfg` & `cool_seq_tool-0.1.9/setup.cfg`

 * *Files identical despite different names*

