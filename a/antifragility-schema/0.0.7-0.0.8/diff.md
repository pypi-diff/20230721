# Comparing `tmp/antifragility-schema-0.0.7.tar.gz` & `tmp/antifragility-schema-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antifragility-schema-0.0.7.tar", last modified: Thu Jul 20 20:10:16 2023, max compression
+gzip compressed data, was "antifragility-schema-0.0.8.tar", last modified: Thu Jul 20 20:20:30 2023, max compression
```

## Comparing `antifragility-schema-0.0.7.tar` & `antifragility-schema-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:10:16.507386 antifragility-schema-0.0.7/
--rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 20:10:16.507078 antifragility-schema-0.0.7/PKG-INFO
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:10:16.504586 antifragility-schema-0.0.7/antifragility_schema/
--rw-r--r--   0 sol        (501) staff       (20)        0 2023-07-20 20:07:41.000000 antifragility-schema-0.0.7/antifragility_schema/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)    11977 2023-07-20 20:05:17.000000 antifragility-schema-0.0.7/antifragility_schema/models.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:10:16.506802 antifragility-schema-0.0.7/antifragility_schema.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      297 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 20:10:16.000000 antifragility-schema-0.0.7/antifragility_schema.egg-info/top_level.txt
--rw-r--r--   0 sol        (501) staff       (20)      410 2023-07-20 20:08:57.000000 antifragility-schema-0.0.7/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 20:10:16.507511 antifragility-schema-0.0.7/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:20:30.280701 antifragility-schema-0.0.8/
+-rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 20:20:30.280470 antifragility-schema-0.0.8/PKG-INFO
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:20:30.279056 antifragility-schema-0.0.8/antifragility_schema/
+-rw-r--r--   0 sol        (501) staff       (20)        0 2023-07-20 20:07:41.000000 antifragility-schema-0.0.8/antifragility_schema/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)    12044 2023-07-20 20:18:56.000000 antifragility-schema-0.0.8/antifragility_schema/models.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 20:20:30.280213 antifragility-schema-0.0.8/antifragility_schema.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      266 2023-07-20 20:20:30.000000 antifragility-schema-0.0.8/antifragility_schema.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      297 2023-07-20 20:20:30.000000 antifragility-schema-0.0.8/antifragility_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 20:20:30.000000 antifragility-schema-0.0.8/antifragility_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-20 20:20:30.000000 antifragility-schema-0.0.8/antifragility_schema.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 20:20:30.000000 antifragility-schema-0.0.8/antifragility_schema.egg-info/top_level.txt
+-rw-r--r--   0 sol        (501) staff       (20)      410 2023-07-20 20:20:10.000000 antifragility-schema-0.0.8/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 20:20:30.280762 antifragility-schema-0.0.8/setup.cfg
```

### Comparing `antifragility-schema-0.0.7/antifragility_schema/models.py` & `antifragility-schema-0.0.8/antifragility_schema/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     status: AdvStatus = fields.IntEnumField(AdvStatus)
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True, index=True)
 
     orders: fields.ReverseRelation["Order"]
 
     def repr(self):
-        return f"{self.pair.repr()} {self.price}"
+        return f"{self.pair_id}: {self.price:.3g}"
 
     class Meta:
         table_description = "P2P Advertisements"
 
 
 class Pt(Model):
     name: str = fields.CharField(63)
@@ -221,14 +221,17 @@
 
 class Ptc(Model):
     pt: fields.ForeignKeyRelation[Pt] = fields.ForeignKeyField("models.Pt")
     cur: fields.ForeignKeyRelation[Cur] = fields.ForeignKeyField("models.Cur")
     blocked: fields.BooleanField = fields.BooleanField(default=False)
     fiats: fields.ReverseRelation["Fiat"]
 
+    def repr(self):
+        return f"{self.pt_id}-{self.cur_id}"
+
     class Meta:
         table_description = "Payment methods - Currencies"
         unique_together = (("pt", "cur"),)
 
 
 class Fiat(Model):
     id: int = fields.IntField(pk=True)
```

