# Comparing `tmp/security_arbihacker-0.0.2.tar.gz` & `tmp/security_arbihacker-0.0.3.tar.gz`

## Comparing `security_arbihacker-0.0.2.tar` & `security_arbihacker-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/.idea/security_arbihacker.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/src/security_arbihacker/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/LICENSE
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/README.MD
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 security_arbihacker-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/.idea/security_arbihacker.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/src/security_arbihacker/__init__.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/src/security_arbihacker/prefixed_security.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/LICENSE
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/README.MD
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 security_arbihacker-0.0.3/PKG-INFO
```

### Comparing `security_arbihacker-0.0.2/.github/workflows/python-publish.yml` & `security_arbihacker-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `security_arbihacker-0.0.2/src/security_arbihacker/__init__.py` & `security_arbihacker-0.0.3/src/security_arbihacker/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,23 +36,28 @@
             detail="Could not validate credentials",
             headers={"WWW-Authenticate": authenticate_value}
         )
 
 
 def check_token_and_scopes(
     security_scopes: SecurityScopes, token: str, key: str | dict, algorithms: str | list
-) -> int:
+) -> dict:
     if security_scopes.scopes:
         authenticate_value = f"bearer scope={security_scopes.scope_str}"
     else:
         authenticate_value = "bearer"
     try:
         payload = jwt.decode(token, key, algorithms=algorithms)
-        user_id: int = int(payload["sub"])
+        if "sub" not in payload:
+            raise KeyError("sub claim is not present")
+        if not security_scopes.scopes:
+            return payload
         token_scopes = set(payload["scope"].split(" "))
         for scope in security_scopes.scopes:
             if scope not in token_scopes:
-                raise CredentialsException(authenticate_value)
-        return user_id
+                raise KeyError(f"Scope not present: {scope}")
+        return payload
     except (JWTError, KeyError, ValueError):
         logging.error("Invalid JWT token during authentication")
         raise CredentialsException(authenticate_value)
+
+
```

### Comparing `security_arbihacker-0.0.2/LICENSE` & `security_arbihacker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `security_arbihacker-0.0.2/pyproject.toml` & `security_arbihacker-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "security-arbihacker"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Sergei Aslamazov", email="mrvisioo@gmail.com" },
 ]
 description = "Utils to make setting up API security with FastAPI faster and easier."
 readme = "README.MD"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `security_arbihacker-0.0.2/PKG-INFO` & `security_arbihacker-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security-arbihacker
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utils to make setting up API security with FastAPI faster and easier.
 Project-URL: Homepage, https://github.com/ArbiHacker/security_arbihacker
 Author-email: Sergei Aslamazov <mrvisioo@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

