# Comparing `tmp/discohooker-1.0.2.tar.gz` & `tmp/discohooker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-1.0.2.tar", last modified: Fri Jul 21 07:29:01 2023, max compression
+gzip compressed data, was "discohooker-1.0.3.tar", last modified: Fri Jul 21 07:49:23 2023, max compression
```

## Comparing `discohooker-1.0.2.tar` & `discohooker-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:29:01.651622 discohooker-1.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:29:01.651622 discohooker-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1008 2023-07-21 04:47:01.000000 discohooker-1.0.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:29:01.643622 discohooker-1.0.2/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.2/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.2/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:07:46.000000 discohooker-1.0.2/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3315 2023-07-21 07:28:36.000000 discohooker-1.0.2/discohooker/message.py
--rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:24:20.000000 discohooker-1.0.2/discohooker/tasks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3539 2023-07-21 07:27:18.000000 discohooker-1.0.2/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:29:01.647622 discohooker-1.0.2/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:29:01.000000 discohooker-1.0.2/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-21 07:29:01.000000 discohooker-1.0.2/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-21 07:29:01.000000 discohooker-1.0.2/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-21 07:29:01.000000 discohooker-1.0.2/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-21 07:29:01.000000 discohooker-1.0.2/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-21 07:29:01.655622 discohooker-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-21 07:28:49.000000 discohooker-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:49:23.977807 discohooker-1.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:49:23.977807 discohooker-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1008 2023-07-21 04:47:01.000000 discohooker-1.0.3/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:49:23.973807 discohooker-1.0.3/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2023-07-20 07:47:04.000000 discohooker-1.0.3/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-20 07:40:11.000000 discohooker-1.0.3/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:07:46.000000 discohooker-1.0.3/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3176 2023-07-21 07:49:02.000000 discohooker-1.0.3/discohooker/message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      474 2023-07-21 04:24:20.000000 discohooker-1.0.3/discohooker/tasks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3387 2023-07-21 07:48:33.000000 discohooker-1.0.3/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-21 07:49:23.973807 discohooker-1.0.3/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1472 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-21 07:49:23.000000 discohooker-1.0.3/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-20 07:25:45.000000 discohooker-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-21 07:49:23.977807 discohooker-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      712 2023-07-21 07:49:13.000000 discohooker-1.0.3/setup.py
```

### Comparing `discohooker-1.0.2/LICENSE` & `discohooker-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.2/PKG-INFO` & `discohooker-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.2
+Version: 1.0.3
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-1.0.2/README.md` & `discohooker-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.2/discohooker/embed.py` & `discohooker-1.0.3/discohooker/embed.py`

 * *Files identical despite different names*

### Comparing `discohooker-1.0.2/discohooker/message.py` & `discohooker-1.0.3/discohooker/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,15 @@
             _embeds.append(embed._to_dict)
         if content == None:
             _content=""
         else:
             _content=content
         _jdata={"content": _content, "embeds": _embeds}
         response=requests.patch(f"{self.weburl}/messages/{message_id}", data=_jdata)
-        if response.status_code == 204:
-            raise Errors.APIError("The request completed successfully but returned no content.")
-        elif response.status_code == 304:
+        if response.status_code == 304:
             raise Errors.APIError("The entity was not modified (no action was taken).")
         elif response.status_code == 429:
             raise Errors.APIError("You are being rate limited, see https://discord.com/developers/docs/topics/rate-limits.")
         elif response.status_code == 400:
             raise Errors.APIError("The request was improperly formatted, or the server couldn't understand it.(Bad Request)")
         elif response.status_code == 401:
             raise Errors.APIError("The Authorization header was missing or invalid.")
```

### Comparing `discohooker-1.0.2/discohooker/webhook.py` & `discohooker-1.0.3/discohooker/webhook.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,22 +54,20 @@
             _embeds.append(embed._to_dict)
         if content == None:
             _content=""
         else:
             _content=content
         _jdata={"content": _content, "embeds": _embeds, "username": self.name, "avatar_url": self.avatar_url}
         response=requests.post(self.weburl, data=_jdata)
-        if response.status_code == 204:
-            raise Errors.APIError("The request completed successfully but returned no content.")
-        elif response.status_code == 304:
+        if response.status_code == 304:
             raise Errors.APIError("The entity was not modified (no action was taken).")
         elif response.status_code == 429:
             raise Errors.APIError("You are being rate limited, see https://discord.com/developers/docs/topics/rate-limits.")
         elif response.status_code == 400:
-            raise Errors.APIError("The request was improperly formatted, or the server couldn't understand it.(Bad Request)")
+            raise Errors.APIError("The request was improperly formatted, or the server couldn't understand it.")
         elif response.status_code == 401:
             raise Errors.APIError("The Authorization header was missing or invalid.")
         elif response.status_code == 403:
             raise Errors.APIError("The Authorization token you passed did not have permission to the resource")
         elif response.status_code == 404:
             raise Errors.APIError("The resource at the location specified doesn't exist.")
         elif response.status_code == 405:
```

### Comparing `discohooker-1.0.2/discohooker.egg-info/PKG-INFO` & `discohooker-1.0.3/discohooker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 1.0.2
+Version: 1.0.3
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-1.0.2/setup.py` & `discohooker-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="1.0.2",
+    version="1.0.3",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

