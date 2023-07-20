# Comparing `tmp/nginx-ldap-auth-service-2.0.4.tar.gz` & `tmp/nginx-ldap-auth-service-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-ldap-auth-service-2.0.4.tar", last modified: Fri Jul 14 17:39:23 2023, max compression
+gzip compressed data, was "nginx-ldap-auth-service-2.0.5.tar", last modified: Thu Jul 20 23:24:57 2023, max compression
```

## Comparing `nginx-ldap-auth-service-2.0.4.tar` & `nginx-ldap-auth-service-2.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.255685 nginx-ldap-auth-service-2.0.4/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.4/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.4/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     1706 2023-07-14 17:39:18.000000 nginx-ldap-auth-service-2.0.4/Makefile
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-14 17:39:23.256192 nginx-ldap-auth-service-2.0.4/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.4/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.226056 nginx-ldap-auth-service-2.0.4/etc/
--rw-r--r--   0 cmalek     (501) admin       (80)      716 2023-07-14 17:10:58.000000 nginx-ldap-auth-service-2.0.4/etc/environment.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.227427 nginx-ldap-auth-service-2.0.4/etc/nginx/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.229831 nginx-ldap-auth-service-2.0.4/etc/nginx/certs/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.crt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.key
--rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.4/etc/nginx/nginx.conf
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.237480 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/
--rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-14 17:39:18.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.243909 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3635 2023-07-12 00:14:38.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     7601 2023-07-14 17:31:00.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/main.py
--rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/middleware.py
--rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-12 00:21:31.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/models.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.248676 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/
--rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-12 00:06:35.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/server.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/ldap.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/logging.py
--rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/main.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5746 2023-07-14 17:23:15.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/types.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.254953 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      270 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      634 2023-07-12 16:14:11.000000 nginx-ldap-auth-service-2.0.4/requirements.dev.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-14 17:39:23.259392 nginx-ldap-auth-service-2.0.4/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1927 2023-07-14 17:39:18.000000 nginx-ldap-auth-service-2.0.4/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.462020 nginx-ldap-auth-service-2.0.5/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.5/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.5/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2049 2023-07-20 23:24:53.000000 nginx-ldap-auth-service-2.0.5/Makefile
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-20 23:24:57.462160 nginx-ldap-auth-service-2.0.5/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.5/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.447403 nginx-ldap-auth-service-2.0.5/etc/
+-rw-r--r--   0 cmalek     (501) admin       (80)      930 2023-07-20 17:52:19.000000 nginx-ldap-auth-service-2.0.5/etc/environment.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.447779 nginx-ldap-auth-service-2.0.5/etc/nginx/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.449311 nginx-ldap-auth-service-2.0.5/etc/nginx/certs/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.5/etc/nginx/certs/localhost.crt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.5/etc/nginx/certs/localhost.key
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.5/etc/nginx/nginx.conf
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.453658 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-20 23:24:53.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.457374 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3635 2023-07-12 00:14:38.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     7601 2023-07-14 17:31:00.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/main.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/middleware.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-12 00:21:31.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/models.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.459347 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/cli/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/cli/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/cli/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-12 00:06:35.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/cli/server.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/ldap.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/logging.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/main.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5746 2023-07-14 17:23:15.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/types.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-20 23:24:57.461730 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-20 23:24:57.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-20 23:24:57.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-20 23:24:57.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-20 23:24:57.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      270 2023-07-20 23:24:57.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-20 23:24:57.000000 nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      634 2023-07-12 16:14:11.000000 nginx-ldap-auth-service-2.0.5/requirements.dev.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-20 23:24:57.463641 nginx-ldap-auth-service-2.0.5/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1927 2023-07-20 23:24:53.000000 nginx-ldap-auth-service-2.0.5/setup.py
```

### Comparing `nginx-ldap-auth-service-2.0.4/LICENSE.txt` & `nginx-ldap-auth-service-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/Makefile` & `nginx-ldap-auth-service-2.0.5/Makefile`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,28 @@
-VERSION = 2.0.4
+VERSION = 2.0.5
 
 PACKAGE = nginx-ldap-auth-service
 
 DOCKER_REGISTRY = caltechads
 #======================================================================
 
+image_name:
+	@echo ${PACKAGE}
+
+version:
+	@echo ${VERSION}
+
+docs:
+	@echo "Installing docs dependencies ..."
+	@pip install -r doc/requirements.txt
+	@echo "Generating docs..."
+	@cd doc && rm -rf build && make json
+	@cd doc/build && tar zcf docs.tar.gz json
+	@mv doc/build/docs.tar.gz .
+	@echo "New doc package is in docs.tar.gz"
 
 clean:
 	rm -rf *.tar.gz dist *.egg-info *.rpm
 	find . -name "*.pyc" -exec rm '{}' ';'
 
 dist: clean
 	@python setup.py sdist
@@ -46,14 +60,15 @@
 restart:
 	docker-compose restart nginx-ldap-auth-service
 
 exec:
 	docker exec -it nginx-ldap-auth-service /bin/sh
 
 release: dist
+	@bin/release.sh
 	@twine upload dist/*
 
 log:
 	docker-compose logs -f nginx-ldap-auth-service
 
 logall:
 	docker-compose logs -f
```

### Comparing `nginx-ldap-auth-service-2.0.4/PKG-INFO` & `nginx-ldap-auth-service-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.4
+Version: 2.0.5
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.4/README.md` & `nginx-ldap-auth-service-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/etc/environment.txt` & `nginx-ldap-auth-service-2.0.5/etc/environment.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 SECRET_KEY=__SECRET_KEY__
 LDAP_URI=ldap://host.docker.internal:1389
 LDAP_BINDDN=__LDAP_BINDDN__
 LDAP_PASSWORD=__LDAP_PASSWORD__
 LDAP_BASEDN=ou=users,dc=example,dc=com
 # SENTRY_URL=None
 
+# Uncomment the below if you want to use the
+# Redis backend for session storage in dev
+# ------------------------------------------
+# SESSION_BACKEND=redis
+# REDIS_URL=redis://localhost
+
+# Set any of the below as necessary
+# ------------------------------------------
 # COOKIE_NAME=nginxauth
 # SESSION_MAX_AGE=0
 # USE_ROLLING_SESSIONS=False
-# SESSION_BACKEND=memory
-# REDIS_URL=redis://localhost
 # REDIS_PREFIX=nginx_ldap_auth.
 # LDAP_STARTTLS=True
 # LDAP_DISABLE_REFERRALS=False
 # LDAP_USERNAME_ATTRIBUTE=uid
 # LDAP_FULL_NAME_ATTRIBUTE=cn
 # LDAP_GET_USER_FILTER={username_attribute}={username}
 # LDAP_AUTHORIZATION_FILTER=None
```

### Comparing `nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.crt` & `nginx-ldap-auth-service-2.0.5/etc/nginx/certs/localhost.crt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.key` & `nginx-ldap-auth-service-2.0.5/etc/nginx/certs/localhost.key`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/etc/nginx/nginx.conf` & `nginx-ldap-auth-service-2.0.5/etc/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/forms.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/forms.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/main.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/main.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/middleware.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/middleware.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/models.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/app/models.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/server.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/cli/server.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/ldap.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/ldap.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/logging.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/logging.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/settings.py` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth/settings.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/PKG-INFO` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.4
+Version: 2.0.5
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/SOURCES.txt` & `nginx-ldap-auth-service-2.0.5/nginx_ldap_auth_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/requirements.dev.txt` & `nginx-ldap-auth-service-2.0.5/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/setup.cfg` & `nginx-ldap-auth-service-2.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.4/setup.py` & `nginx-ldap-auth-service-2.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setup(
     name="nginx-ldap-auth-service",
-    version="2.0.4",
+    version="2.0.5",
     description="A FastAPI app that authenticates users via LDAP and sets a cookie for nginx",
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     url="https://github.com/caltechads/nginx-ldap-auth-service",
     packages=find_packages(exclude=["bin"]),
     install_requires=[
         "aiodogstatsd==0.16.0.post0",
```

