# Comparing `tmp/maglevai-0.1.0.tar.gz` & `tmp/maglevai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maglevai-0.1.0.tar", max compression
+gzip compressed data, was "maglevai-0.1.1.tar", max compression
```

## Comparing `maglevai-0.1.0.tar` & `maglevai-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152228 maglevai-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152104 maglevai-0.1.0/maglevai/__init__.py
--rw-r--r--   0        0        0      861 2023-07-21 17:08:19.108606 maglevai-0.1.0/maglevai/main.py
--rw-r--r--   0        0        0      313 2023-07-21 16:47:26.612856 maglevai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 maglevai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152228 maglevai-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:45:01.152104 maglevai-0.1.1/maglevai/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-21 17:25:06.526000 maglevai-0.1.1/maglevai/main.py
+-rw-r--r--   0        0        0      317 2023-07-21 17:23:42.280686 maglevai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 maglevai-0.1.1/PKG-INFO
```

### Comparing `maglevai-0.1.0/maglevai/main.py` & `maglevai-0.1.1/maglevai/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,31 @@
             response_json = response.json()
             if "NO" in response_json['is_passed_hallucination_check'].upper():
                 return False
             else:
                 return True
         else:
             return "Error Code: " + str(response.status_code)
+        
+    def secrets(self, content):
+        endpoint = "/secrets/"
+        url = f"{self.api_base_url}{endpoint}"
+        headers = {
+                    f"Authorization": "Bearer {self.api_key}"
+                }
+
+        data = {
+            "content": content,
+        }
+
+        response = r.post(url, json=data, headers=headers)
+
+        if str(response.status_code) == '200':
+            response_json = response.json()
+            if "YES" in response_json['is_contain_secrets'].upper():
+                return False
+            else:
+                return True
+        else:
+            return "Error Code: " + str(response.status_code)
+
```

