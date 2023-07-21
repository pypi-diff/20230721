# Comparing `tmp/pysendpulse-0.1.5.tar.gz` & `tmp/pysendpulse-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysendpulse-0.1.5.tar", last modified: Fri Mar 31 10:55:17 2023, max compression
+gzip compressed data, was "pysendpulse-0.1.7.tar", last modified: Fri Jul 21 09:18:09 2023, max compression
```

## Comparing `pysendpulse-0.1.5.tar` & `pysendpulse-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:55:17.870779 pysendpulse-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-03-31 10:55:01.000000 pysendpulse-0.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-31 10:55:17.870779 pysendpulse-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-31 10:55:01.000000 pysendpulse-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:55:17.870779 pysendpulse-0.1.5/pysendpulse/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-31 10:55:01.000000 pysendpulse-0.1.5/pysendpulse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53265 2023-03-31 10:55:01.000000 pysendpulse-0.1.5/pysendpulse/pysendpulse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:55:17.870779 pysendpulse-0.1.5/pysendpulse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-31 10:55:17.000000 pysendpulse-0.1.5/pysendpulse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-31 10:55:17.000000 pysendpulse-0.1.5/pysendpulse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 10:55:17.000000 pysendpulse-0.1.5/pysendpulse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 10:55:17.000000 pysendpulse-0.1.5/pysendpulse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-31 10:55:17.000000 pysendpulse-0.1.5/pysendpulse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 10:55:17.870779 pysendpulse-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-31 10:55:01.000000 pysendpulse-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:18:09.139128 pysendpulse-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-21 09:17:59.000000 pysendpulse-0.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-21 09:18:09.139128 pysendpulse-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-21 09:17:59.000000 pysendpulse-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:18:09.135128 pysendpulse-0.1.7/pysendpulse/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 09:17:59.000000 pysendpulse-0.1.7/pysendpulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53178 2023-07-21 09:17:59.000000 pysendpulse-0.1.7/pysendpulse/pysendpulse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:18:09.139128 pysendpulse-0.1.7/pysendpulse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-21 09:18:09.000000 pysendpulse-0.1.7/pysendpulse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 09:18:09.000000 pysendpulse-0.1.7/pysendpulse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:18:09.000000 pysendpulse-0.1.7/pysendpulse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:18:09.000000 pysendpulse-0.1.7/pysendpulse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 09:18:09.000000 pysendpulse-0.1.7/pysendpulse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:18:09.139128 pysendpulse-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-21 09:17:59.000000 pysendpulse-0.1.7/setup.py
```

### Comparing `pysendpulse-0.1.5/LICENSE.md` & `pysendpulse-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysendpulse-0.1.5/PKG-INFO` & `pysendpulse-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysendpulse
-Version: 0.1.5
+Version: 0.1.7
 Summary: A simple SendPulse REST client library and example for Python
 Home-page: https://github.com/sendpulse/sendpulse-rest-api-python
 Author: Maksym Ustymenko
 Author-email: tech@sendpulse.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pysendpulse-0.1.5/pysendpulse/pysendpulse.py` & `pysendpulse-0.1.7/pysendpulse/pysendpulse.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,17 +139,17 @@
         logger.debug("__send_request method: {} url: '{}' with parameters: {}".format(method, url, params))
         if type(params) not in (dict, list):
             params = {}
         if use_token and self.__token:
             headers = {'Authorization': 'Bearer {}'.format(self.__token)}
         else:
             headers = {}
-        if use_json_content_type and params:
-            headers['Content-Type'] = 'application/json'
-            params = json.dumps(params)
+        # if use_json_content_type and params:
+        headers['Content-Type'] = 'application/json'
+        params = json.dumps(params)
 
         if method == "POST":
             response = requests.post(url, headers=headers, data=params)
         elif method == "PUT":
             response = requests.put(url, headers=headers, data=params)
         elif method == "DELETE":
             response = requests.delete(url, headers=headers, data=params)
@@ -174,42 +174,40 @@
         """ Process request results
 
         @param data: a Response object from the Python Requests package
         @return: dictionary with response message and/or http code
         """
         try:
             result = data.json()
+            errors = {}
         except:
-            result = {
+            result = {}
+            errors = {
                 'is_error': True,
                 'http_code': data.status_code,
                 'message': "Response is empty, invalid or not JSON."
             }
 
         if data.ok:
-            errors = {
-                'is_error': False,
-                'http_code': data.status_code
-            }
             logger.debug("Handle result: {}".format(result, ))
         else:
             errors = {
                 'is_error': True,
                 'http_code': data.status_code
             }
             if data.status_code == 404:
                 errors['message'] = "Sorry, the page you are looking for {} could not be found.".format(data.url, )
             elif data.status_code == 500:
                 errors['message'] = "Whoops, looks like something went wrong on the server. Please contact with out support tech@sendpulse.com."
 
-        logger.debug("Handle result: {}".format(errors, ))
+            logger.debug("Handle result: {}".format(errors, ))
 
         # return object that maintains backward-compatibility
-        result.update(errors)
-        result.update({'data': result.copy()})
+        if not data.ok:
+            result = {'data': errors}
         return result
 
     def __handle_error(self, custom_message=None):
         """ Process request errors
 
         @param custom_message:
         @return: dictionary with response custom error message and/or error code
```

### Comparing `pysendpulse-0.1.5/pysendpulse.egg-info/PKG-INFO` & `pysendpulse-0.1.7/pysendpulse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysendpulse
-Version: 0.1.5
+Version: 0.1.7
 Summary: A simple SendPulse REST client library and example for Python
 Home-page: https://github.com/sendpulse/sendpulse-rest-api-python
 Author: Maksym Ustymenko
 Author-email: tech@sendpulse.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pysendpulse-0.1.5/setup.py` & `pysendpulse-0.1.7/setup.py`

 * *Files identical despite different names*

