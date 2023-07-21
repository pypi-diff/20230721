# Comparing `tmp/detecttoxicity-0.1.0.tar.gz` & `tmp/detecttoxicity-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detecttoxicity-0.1.0.tar", last modified: Fri Jul 21 12:56:17 2023, max compression
+gzip compressed data, was "detecttoxicity-0.1.1.tar", last modified: Fri Jul 21 13:19:33 2023, max compression
```

## Comparing `detecttoxicity-0.1.0.tar` & `detecttoxicity-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:56:17.203122 detecttoxicity-0.1.0/
--rw-rw-rw-   0        0        0        0 2023-07-21 12:15:50.000000 detecttoxicity-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      225 2023-07-21 12:56:17.200111 detecttoxicity-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 12:56:17.179129 detecttoxicity-0.1.0/detecttoxicity.egg-info/
--rw-rw-rw-   0        0        0      225 2023-07-21 12:56:16.000000 detecttoxicity-0.1.0/detecttoxicity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-21 12:56:17.000000 detecttoxicity-0.1.0/detecttoxicity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:56:16.000000 detecttoxicity-0.1.0/detecttoxicity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 12:56:16.000000 detecttoxicity-0.1.0/detecttoxicity.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-21 12:56:16.000000 detecttoxicity-0.1.0/detecttoxicity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 12:56:17.204109 detecttoxicity-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      355 2023-07-21 12:55:42.000000 detecttoxicity-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:56:17.192108 detecttoxicity-0.1.0/toxic/
--rw-rw-rw-   0        0        0        0 2023-07-21 10:38:11.000000 detecttoxicity-0.1.0/toxic/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-07-21 12:43:20.000000 detecttoxicity-0.1.0/toxic/toxic.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:19:33.340429 detecttoxicity-0.1.1/
+-rw-rw-rw-   0        0        0        0 2023-07-21 12:15:50.000000 detecttoxicity-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-07-21 13:19:33.338427 detecttoxicity-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 13:19:33.328426 detecttoxicity-0.1.1/detecttoxicity.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-07-21 13:19:33.000000 detecttoxicity-0.1.1/detecttoxicity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-07-21 13:19:33.000000 detecttoxicity-0.1.1/detecttoxicity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:19:33.000000 detecttoxicity-0.1.1/detecttoxicity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 13:19:33.000000 detecttoxicity-0.1.1/detecttoxicity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-21 13:19:33.000000 detecttoxicity-0.1.1/detecttoxicity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:19:33.341428 detecttoxicity-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      355 2023-07-21 13:19:10.000000 detecttoxicity-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:19:33.335428 detecttoxicity-0.1.1/toxic/
+-rw-rw-rw-   0        0        0        0 2023-07-21 10:38:11.000000 detecttoxicity-0.1.1/toxic/__init__.py
+-rw-rw-rw-   0        0        0     1301 2023-07-21 13:18:10.000000 detecttoxicity-0.1.1/toxic/toxic.py
```

### Comparing `detecttoxicity-0.1.0/toxic/toxic.py` & `detecttoxicity-0.1.1/toxic/toxic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 import requests
 
-
 class Toxic(object):
-    """
-      Toxic Object containing functions to retrieve various toxic details
-    """
     DOMAIN = "https://api-inference.huggingface.co"
-    API_ENDPOINT = DOMAIN+"/models/unitary/unbiased-toxic-roberta"  
-    
-    def __init__(self,query,token):
-        super(Toxic,self).__init__()
+    API_ENDPOINT = DOMAIN + "/models/unitary/unbiased-toxic-roberta"
+
+    def __init__(self, query, token):
+        super(Toxic, self).__init__()
         self.query = query
         self.response = ""
         self.token = token
-        self.HEADERS = {"Authorization": "Bearer"+self.token}
+        self.HEADERS = {"Authorization": "Bearer " + self.token}
         try:
             self.response = self.getScoreFromAPI()
         except Exception:
             self.response = "error in moderation layer"
-    
-    def check_toxicity(response_data):
+
+    def check_toxicity(self, response_data):
         for label_info in response_data[0]:
             if label_info['score'] >= 0.8:
                 return True
         return False
-            
+
     def getScoreFromAPI(self):
-        """
-        Get current  response score
-        """
-        payload = str({"inputs": self.query})
+        payload = {"inputs": self.query}
         response = requests.post(self.API_ENDPOINT, headers=self.HEADERS, json=payload)
-        if response.status_code==200:
+        if response.status_code == 200:
             response_json = response.json()
+            self.check_toxicity(response_json)
             if self.check_toxicity(response_json):
                 return "Sorry, we can't show this content as it is flagged as toxic."
             else:
-                self.query
-        else :
+                return self.query
+        else:
             raise Exception("Hugging Face Space is down...")
-
```

