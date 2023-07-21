# Comparing `tmp/garth-0.1.8.tar.gz` & `tmp/garth-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.1.8.tar", last modified: Tue Jul 18 18:28:02 2023, max compression
+gzip compressed data, was "garth-0.1.9.tar", last modified: Tue Jul 18 19:12:46 2023, max compression
```

## Comparing `garth-0.1.8.tar` & `garth-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.8/README.md
--rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.8/garth/__init__.py
--rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.8/garth/auth_token.py
--rw-r--r--   0        0        0     2930 2023-07-18 14:39:54.464611 garth-0.1.8/garth/http.py
--rw-r--r--   0        0        0     3605 2023-07-18 18:25:44.073499 garth-0.1.8/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.8/garth/version.py
--rw-r--r--   0        0        0      512 2023-07-18 18:28:02.766786 garth-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.9/README.md
+-rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.9/garth/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.9/garth/auth_token.py
+-rw-r--r--   0        0        0      266 2023-07-18 18:38:39.454258 garth-0.1.9/garth/exc.py
+-rw-r--r--   0        0        0     2930 2023-07-18 14:39:54.464611 garth-0.1.9/garth/http.py
+-rw-r--r--   0        0        0     3657 2023-07-18 19:10:05.985264 garth-0.1.9/garth/sso.py
+-rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.9/garth/version.py
+-rw-r--r--   0        0        0      512 2023-07-18 19:12:46.570114 garth-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.9/PKG-INFO
```

### Comparing `garth-0.1.8/garth/auth_token.py` & `garth-0.1.9/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.8/garth/http.py` & `garth-0.1.9/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.8/garth/sso.py` & `garth-0.1.9/garth/sso.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import time
 from typing import Optional
 
 from . import http
+from .exc import GarthException
 
 
 CSRF_RE = re.compile(r'name="_csrf"\s+value="(.+?)"')
 TITLE_RE = re.compile(r"<title>(.+?)</title>")
 
 
 def login(
@@ -72,20 +73,20 @@
                 "embed": "true",
                 "_csrf": csrf_token,
                 "fromPage": "setupEnterMfaCode",
             },
         )
 
     if _get_title(resp.text) != "Success":
-        raise Exception("Login failed")
+        raise GarthException("Login failed")
 
     # Parse ticket
     m = re.search(r'embed\?ticket=([^"]+)"', resp.text)
     if not m:
-        raise Exception("Could not find Service Ticket")
+        raise GarthException("Could not find Service Ticket")
     ticket = m.group(1)
 
     # Exchange SSO Ticket for Connect Token
     client.get(
         "connect",
         "/modern",
         params=dict(ticket=ticket),
@@ -126,16 +127,16 @@
     )
     return token
 
 
 def _get_csrf_token(html: str) -> str:
     m = CSRF_RE.search(html)
     if not m:
-        raise Exception("Couldn't find CSRF token")
+        raise GarthException("Couldn't find CSRF token")
     return m.group(1)
 
 
 def _get_title(html: str) -> str:
     m = TITLE_RE.search(html)
     if not m:
-        raise Exception("Couldn't find title")
+        raise GarthException("Couldn't find title")
     return m.group(1)
```

### Comparing `garth-0.1.8/pyproject.toml` & `garth-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "garth"
-version = "0.1.8"
+version = "0.1.9"
 description = "Garmin SSO auth"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "requests>=2.27.0",
 ]
```

