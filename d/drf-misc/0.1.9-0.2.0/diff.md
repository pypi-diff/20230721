# Comparing `tmp/drf_misc-0.1.9.tar.gz` & `tmp/drf_misc-0.2.0.tar.gz`

## Comparing `drf_misc-0.1.9.tar` & `drf_misc-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.1.9/.isort.cfg
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 drf_misc-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.1.9/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.1.9/ignore-spelling-words.txt
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.1.9/mypy.ini
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.1.9/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.1.9/setup.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.1.9/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 drf_misc-0.1.9/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/admin.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/apps.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/settings.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/api_exceptions.py
--rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/api_views.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/audit_service.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/cache.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/fields.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/filter_backend.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/middlewares.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/models.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/paginations.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/parsers.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/permissions.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/serializers.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/services.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/core/throttling.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/utility/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/utility/decorators.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/utility/epoch_util.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/utility/misc.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.1.9/drf_misc/utility/validator.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.1.9/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.1.9/LICENSE
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 drf_misc-0.1.9/README.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 drf_misc-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 drf_misc-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.isort.cfg
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.2.0/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.2.0/mypy.ini
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.2.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.2.0/setup.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/admin.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/apps.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/settings.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/api_exceptions.py
+-rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/api_views.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/audit_service.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/cache.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/fields.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/filter_backend.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/middlewares.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/models.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/paginations.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/parsers.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/permissions.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/serializers.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/services.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/throttling.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/decorators.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/epoch_util.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/misc.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/validator.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 drf_misc-0.2.0/README.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 drf_misc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 drf_misc-0.2.0/PKG-INFO
```

### Comparing `drf_misc-0.1.9/.pre-commit-config.yaml` & `drf_misc-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/.pylintrc` & `drf_misc-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/.github/workflows/publish.yaml` & `drf_misc-0.2.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/admin.py` & `drf_misc-0.2.0/drf_misc/admin.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/settings.py` & `drf_misc-0.2.0/drf_misc/settings.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/api_exceptions.py` & `drf_misc-0.2.0/drf_misc/core/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/api_views.py` & `drf_misc-0.2.0/drf_misc/core/api_views.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/audit_service.py` & `drf_misc-0.2.0/drf_misc/core/audit_service.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/fields.py` & `drf_misc-0.2.0/drf_misc/core/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     except (ValueError, TypeError) as error:
         raise ValidationError(
             f"{value} is not a valid Unix timestamp",
             params={"value": value},
         ) from error
 
 
-class EpochField(models.CharField):  # Store as CharField for simplicity
+class EpochField(models.FloatField):  # Store as CharField for simplicity
     default_validators = [validate_epoch]
 
     def __init__(self, *args, **kwargs):
         self.nullable = kwargs.pop("nullable", True)
         self.default_current_time = kwargs.pop("default_current_time", False)
         self.update_now = kwargs.pop("update_now", False)
         kwargs["max_length"] = kwargs.pop("max_length", 20)
@@ -30,23 +30,23 @@
             kwargs["null"] = True
             kwargs["blank"] = True
         super().__init__(*args, **kwargs)
 
     def pre_save(self, model_instance, add):
         value = super().pre_save(model_instance, add)
         if self.update_now:
-            value = str(time.time())
+            value = float(time.time())
             setattr(model_instance, self.attname, value)
         return value
 
     def from_db_value(self, value, expression, connection):
         if not value:
             return None
-        return str(value)
+        return float(value)
 
     def to_python(self, value):
         if value:
-            str(value)
+            float(value)
         return None
 
     def get_prep_value(self, value):
-        return str(value) if value is not None else value
+        return float(value) if value is not None else value
```

### Comparing `drf_misc-0.1.9/drf_misc/core/filter_backend.py` & `drf_misc-0.2.0/drf_misc/core/filter_backend.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/middlewares.py` & `drf_misc-0.2.0/drf_misc/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/models.py` & `drf_misc-0.2.0/drf_misc/core/models.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/paginations.py` & `drf_misc-0.2.0/drf_misc/core/paginations.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/serializers.py` & `drf_misc-0.2.0/drf_misc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/services.py` & `drf_misc-0.2.0/drf_misc/core/services.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/core/throttling.py` & `drf_misc-0.2.0/drf_misc/core/throttling.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/utility/decorators.py` & `drf_misc-0.2.0/drf_misc/utility/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/utility/epoch_util.py` & `drf_misc-0.2.0/drf_misc/utility/epoch_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
+
 from dateutil.relativedelta import relativedelta
 
 
 def unix_to_dt(unix):
     # uts can be 1686868399 or 1686868399000 (millisecond) or 1686868399.000 or 1686868399000000 (microseconds) [Not supported for now]
     if len(str(unix)) > 11 and "." not in str(unix):
         unix = float(unix) / 1000
@@ -30,15 +31,15 @@
             else:
                 date_time = datetime.strptime(date_time, "%Y-%m-%d %H:%M:%S.%f")
         elif len(date_time) > 10 and "." not in date_time:
             if "T" in date_time:
                 date_time = datetime.strptime(date_time, "%Y-%m-%dT%H:%M:%S")
             else:
                 date_time = datetime.strptime(date_time, "%Y-%m-%d %H:%M:%S")
-    return str(date_time.timestamp())
+    return float(date_time.timestamp())
 
 
 def append_current_time(unix):
     date_part = unix_to_dt(unix)
     time_part = datetime.now()
     complete_part = datetime(
         date_part.year,
```

### Comparing `drf_misc-0.1.9/drf_misc/utility/misc.py` & `drf_misc-0.2.0/drf_misc/utility/misc.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/drf_misc/utility/validator.py` & `drf_misc-0.2.0/drf_misc/utility/validator.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/.gitignore` & `drf_misc-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/LICENSE` & `drf_misc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/README.md` & `drf_misc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drf_misc-0.1.9/pyproject.toml` & `drf_misc-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "drf-misc"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `drf_misc-0.1.9/PKG-INFO` & `drf_misc-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-misc
-Version: 0.1.9
+Version: 0.2.0
 Summary: A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services.
 Project-URL: Homepage, https://github.com/abhishm20/drf-misc
 Project-URL: Bug Tracker, https://github.com/abhishm20/drf-misc/issues
 Author-email: Abhishek Sharma <abhishm20@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

