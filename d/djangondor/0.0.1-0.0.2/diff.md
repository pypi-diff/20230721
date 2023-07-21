# Comparing `tmp/djangondor-0.0.1.tar.gz` & `tmp/djangondor-0.0.2.tar.gz`

## Comparing `djangondor-0.0.1.tar` & `djangondor-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 djangondor-0.0.1/src/djangondor/__about__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 djangondor-0.0.1/src/djangondor/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 djangondor-0.0.1/src/djangondor/collections.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 djangondor-0.0.1/src/djangondor/requests.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 djangondor-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 djangondor-0.0.1/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 djangondor-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangondor-0.0.1/README.md
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 djangondor-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 djangondor-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 djangondor-0.0.2/src/djangondor/__about__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 djangondor-0.0.2/src/djangondor/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 djangondor-0.0.2/src/djangondor/collections.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 djangondor-0.0.2/src/djangondor/requests.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 djangondor-0.0.2/src/djangondor/time.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 djangondor-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 djangondor-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 djangondor-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 djangondor-0.0.2/README.md
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 djangondor-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 djangondor-0.0.2/PKG-INFO
```

### Comparing `djangondor-0.0.1/src/djangondor/collections.py` & `djangondor-0.0.2/src/djangondor/collections.py`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.1/src/djangondor/requests.py` & `djangondor-0.0.2/src/djangondor/requests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,45 @@
 from django import forms
 from typing import Dict
 from django.http import JsonResponse
 from django.db import models
 
 
+def save_many_and_respond(*models:models.Model,success_status=200,error_status=400):
+    try:
+        for model in models:
+            model.save()
+
+    except Exception as e:
+        return JsonResponse({"message": e.args[0]}, status=error_status)
+    return JsonResponse({"message": 'saved'}, status=success_status)
+
+
+
+def delete_and_respond(model: models.Model):
+    '''
+    Deletes a model and returns a 204 `JsonResponse` response
+    '''
+    try:
+        model.delete()
+        status = 204
+        body = {}
+    except:
+        status = 400
+        body = {"message": "Something is keeping you from deleting this object"}
+
+    return JsonResponse(body, status=status)
+
 
 def save_and_respond(
     model: models.Model,/, serialize_with=None, success_status=200, error_status=400,**kwargs
 ):
+    '''
+    Saves a model and return a a json response.
+    '''
     try:
         for key,val in kwargs.items():
             setattr(model,key,val)
         model.save()
         return JsonResponse(
             {"message": "saved"} if not serialize_with else serialize_with(model).data,
             status=success_status,
@@ -29,14 +57,16 @@
 
 
 def form_error_response(form: forms.ModelForm, status=400):
     return JsonResponse(
         {"message": "%s %s" % format_form_errors(form)[0]}, status=status
     )
 
+
+
 def process_form(
     form: forms.ModelForm, /, set_fields: Dict = None, error_status=400, respond=False
 ):
     """
     Return model that has been saved with `commit=False` when the form has no errors otherwise `None`
     and a `JsonResponse` object with the given `error_status` if the form had errors otherwise None
     The entries in `set_fields` are set on the model just after calling `save(commit=False)` on the form
@@ -52,8 +82,9 @@
                 form.save_m2m()
                 return JsonResponse({"message": "saved"})
             except Exception as e:
                 return JsonResponse({"message": e.args[0]}, status=500)
         return model, None
     elif respond:
         return form_error_response(form)
-    return None, form_error_response(form, error_status)
+    return None, form_error_response(form, error_status)
+
```

### Comparing `djangondor-0.0.1/.gitignore` & `djangondor-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.1/LICENSE.txt` & `djangondor-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.1/pyproject.toml` & `djangondor-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangondor-0.0.1/PKG-INFO` & `djangondor-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangondor
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/unknown/djangondor#readme
 Project-URL: Issues, https://github.com/dalitsosakala/djangondor/issues
 Project-URL: Source, https://github.com/dalitsosakala/djangondor
 Author-email: Dalitso Sakala <dalitso.1sc@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

