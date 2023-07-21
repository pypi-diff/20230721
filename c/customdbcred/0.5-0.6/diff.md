# Comparing `tmp/customdbcred-0.5.tar.gz` & `tmp/customdbcred-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customdbcred-0.5.tar", last modified: Fri Jul 21 06:19:55 2023, max compression
+gzip compressed data, was "customdbcred-0.6.tar", last modified: Fri Jul 21 09:43:54 2023, max compression
```

## Comparing `customdbcred-0.5.tar` & `customdbcred-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 06:19:55.281686 customdbcred-0.5/
--rw-rw-rw-   0        0        0       57 2023-07-21 06:19:55.281686 customdbcred-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 06:19:55.250208 customdbcred-0.5/customdbcred/
--rw-rw-rw-   0        0        0     2171 2023-07-20 12:51:50.000000 customdbcred-0.5/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:19:55.265977 customdbcred-0.5/customdbcred.egg-info/
--rw-rw-rw-   0        0        0       57 2023-07-21 06:19:55.000000 customdbcred-0.5/customdbcred.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-21 06:19:55.000000 customdbcred-0.5/customdbcred.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 06:19:55.000000 customdbcred-0.5/customdbcred.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-21 06:19:55.000000 customdbcred-0.5/customdbcred.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 06:19:55.281686 customdbcred-0.5/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-04-13 12:37:42.000000 customdbcred-0.5/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:19:55.281686 customdbcred-0.5/customvalidator/
--rw-rw-rw-   0        0        0     1404 2023-04-17 13:43:49.000000 customdbcred-0.5/customvalidator/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-21 06:19:55.281686 customdbcred-0.5/setup.cfg
--rw-rw-rw-   0        0        0      201 2023-07-21 06:19:47.000000 customdbcred-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:43:54.674422 customdbcred-0.6/
+-rw-rw-rw-   0        0        0       57 2023-07-21 09:43:54.674422 customdbcred-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 09:43:54.668421 customdbcred-0.6/customdbcred/
+-rw-rw-rw-   0        0        0     2171 2023-07-21 09:07:11.000000 customdbcred-0.6/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:43:54.672422 customdbcred-0.6/customdbcred.egg-info/
+-rw-rw-rw-   0        0        0       57 2023-07-21 09:43:54.000000 customdbcred-0.6/customdbcred.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-21 09:43:54.000000 customdbcred-0.6/customdbcred.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:43:54.000000 customdbcred-0.6/customdbcred.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-21 09:43:54.000000 customdbcred-0.6/customdbcred.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 09:43:54.672422 customdbcred-0.6/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-07-21 08:21:54.000000 customdbcred-0.6/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:43:54.673422 customdbcred-0.6/customvalidator/
+-rw-rw-rw-   0        0        0     1404 2023-07-21 08:21:54.000000 customdbcred-0.6/customvalidator/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:43:54.674422 customdbcred-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      201 2023-07-21 09:30:33.000000 customdbcred-0.6/setup.py
```

### Comparing `customdbcred-0.5/customdbcred/__init__.py` & `customdbcred-0.6/customdbcred/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,16 @@
             if type(req) == dict:
                 result = func(req)
                 return result
             keyVaultName = "myappkv"
             KVUri = f"https://{keyVaultName}.vault.azure.net"
             # credential = DefaultAzureCredential()
             credential = ClientSecretCredential(tenant_id='26afc1b1-8393-439d-aa1a-483105d77dc3',
-                                                client_id='9d2fe19f-47e6-498f-b384-6f94b0d55500',
-                                                client_secret='yXK8Q~3IJa1qOKpF5NyoQNdCsz63ugQEUIutpdv-')
+                                                client_id='580042fa-e891-43c2-8be7-63b708582a07',
+                                                client_secret='DhC8Q~ChYEBbdFIjNck.4rb1F1ziyYIem.4cMach')
             client = SecretClient(vault_url=KVUri, credential=credential)
             dbcred = client.get_secret("DATABASECRED").value
             cred = json.loads(dbcred)
             # server = client.get_secret("SERVER").value
             # database = client.get_secret("DATABASE").value
             # username = client.get_secret("USERNAME").value
             # password = client.get_secret("PASSWORD").value
```

### Comparing `customdbcred-0.5/customstatuscodes/__init__.py` & `customdbcred-0.6/customstatuscodes/__init__.py`

 * *Files identical despite different names*

### Comparing `customdbcred-0.5/customvalidator/__init__.py` & `customdbcred-0.6/customvalidator/__init__.py`

 * *Files identical despite different names*

