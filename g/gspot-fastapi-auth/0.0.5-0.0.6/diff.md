# Comparing `tmp/gspot_fastapi_auth-0.0.5.tar.gz` & `tmp/gspot_fastapi_auth-0.0.6.tar.gz`

## Comparing `gspot_fastapi_auth-0.0.5.tar` & `gspot_fastapi_auth-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/requirements.in
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/requirements.txt
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/example/main.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/example/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/auth.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/base.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/models.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/permissions.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/providers.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/services.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/settings.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/test_factory.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/tests/tests.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/LICENSE
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/requirements.in
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/example/main.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/example/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/auth.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/base.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/models.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/permissions.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/providers.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/services.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/settings.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/test_factory.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/tests/tests.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 gspot_fastapi_auth-0.0.6/PKG-INFO
```

### Comparing `gspot_fastapi_auth-0.0.5/.pre-commit-config.yaml` & `gspot_fastapi_auth-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/requirements.txt` & `gspot_fastapi_auth-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/example/main.py` & `gspot_fastapi_auth-0.0.6/example/main.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/example/tests.py` & `gspot_fastapi_auth-0.0.6/example/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/auth.py` & `gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/auth.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/models.py` & `gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 from typing import List
 from uuid import UUID
 
 
 @dataclass(frozen=True)
 class BaseUser:
     user_id: UUID
+    username: str
+    first_name: str
+    last_name: str
     email: str
     phone: str
     avatar: str
-    country: str
+    country: dict
+    is_banned: bool
+    is_active: bool
+    permissions: List[str]
     created_at: datetime
-    updated_at: datetime
+    update_at: datetime
 
     to_dict = asdict
 
 
 @dataclass(frozen=True)
 class AdminUser(BaseUser):
     is_superuser: bool
@@ -33,14 +39,15 @@
     groups: List[str] = field(default_factory=list)
     user_permissions: List[str] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
 class CustomerUser(BaseUser):
     birthday: datetime
+    friends: List[str] = field(default_factory=list)
 
 
 class UserFactory:
     users = {'administrator': AdminUser, 'developer': DeveloperUser, 'customer': CustomerUser}
 
     def get_user(self, role: str):
         return self.users.get(role)
```

### Comparing `gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/permissions.py` & `gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/providers.py` & `gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/providers.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/src/gspot_fastapi_auth/test_factory.py` & `gspot_fastapi_auth-0.0.6/src/gspot_fastapi_auth/test_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,20 +9,26 @@
 
 
 class BaseUserFactory(factory.Factory):
     class Meta:
         model = BaseUser
 
     user_id = factory.Faker('uuid4')
+    username = factory.Faker('word')
+    first_name = factory.Faker('word')
+    last_name = factory.Faker('word')
     email = factory.Faker('email')
     phone = factory.Faker('phone_number')
     avatar = ''
     country = factory.Faker('country')
+    is_active = True
+    is_banned = False
+    permissions = []
     created_at = str(datetime.now())
-    updated_at = str(datetime.now())
+    update_at = str(datetime.now())
 
 
 class AdminUserFactory(BaseUserFactory):
     class Meta:
         model = AdminUser
 
     is_superuser = True
```

### Comparing `gspot_fastapi_auth-0.0.5/tests/tests.py` & `gspot_fastapi_auth-0.0.6/tests/tests.py`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/.gitignore` & `gspot_fastapi_auth-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/LICENSE` & `gspot_fastapi_auth-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_fastapi_auth-0.0.5/README.md` & `gspot_fastapi_auth-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 ## Install package
 ```shell
 pip install gspot-fastapi-auth
 ```
 
 ## Define env variables
 
-- `REDIS_AUTH_ACCESS_PREFIX`
-- `REDIS_AUTH_DB`
-- `REDIS_AUTH_HOST`
-- `REDIS_AUTH_PORT`
-- `REDIS_AUTH_PASSWORD`
-- `REDIS_AUTH_TOKEN_STORAGE` - 'headers' or 'cookies'
+- `REDIS_AUTH_ACCESS_PREFIX` default ''
+- `REDIS_AUTH_DB` default 0
+- `REDIS_AUTH_HOST` default 127.0.0.1
+- `REDIS_AUTH_PORT` default 6379
+- `REDIS_AUTH_PASSWORD` default None
+- `REDIS_AUTH_TOKEN_STORAGE` default 'headers' should be 'cookies'
 
 ## Define startapp and shutdown logic
 
 ```python
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
```

### Comparing `gspot_fastapi_auth-0.0.5/pyproject.toml` & `gspot_fastapi_auth-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_fastapi_auth"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "gravity48", email = "gravity4849@gmail.com" },
 ]
 description = "GSpot authentication package for FastApi"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_fastapi_auth-0.0.5/PKG-INFO` & `gspot_fastapi_auth-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_fastapi_auth
-Version: 0.0.5
+Version: 0.0.6
 Summary: GSpot authentication package for FastApi
 Project-URL: Homepage, https://github.com/gravity48/gspot_fastapi_auth
 Project-URL: Bug Tracker, https://github.com/gravity48/gspot_fastapi_auth/issues
 Author-email: gravity48 <gravity4849@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,20 +24,20 @@
 ## Install package
 ```shell
 pip install gspot-fastapi-auth
 ```
 
 ## Define env variables
 
-- `REDIS_AUTH_ACCESS_PREFIX`
-- `REDIS_AUTH_DB`
-- `REDIS_AUTH_HOST`
-- `REDIS_AUTH_PORT`
-- `REDIS_AUTH_PASSWORD`
-- `REDIS_AUTH_TOKEN_STORAGE` - 'headers' or 'cookies'
+- `REDIS_AUTH_ACCESS_PREFIX` default ''
+- `REDIS_AUTH_DB` default 0
+- `REDIS_AUTH_HOST` default 127.0.0.1
+- `REDIS_AUTH_PORT` default 6379
+- `REDIS_AUTH_PASSWORD` default None
+- `REDIS_AUTH_TOKEN_STORAGE` default 'headers' should be 'cookies'
 
 ## Define startapp and shutdown logic
 
 ```python
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
```

