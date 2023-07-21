# Comparing `tmp/abin_sim-1.2.0.tar.gz` & `tmp/abin_sim-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-1.2.0.tar", max compression
+gzip compressed data, was "abin_sim-1.2.1.tar", max compression
```

## Comparing `abin_sim-1.2.0.tar` & `abin_sim-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-07-20 21:06:42.333963 abin_sim-1.2.0/LICENSE
--rw-r--r--   0        0        0     8594 2023-07-20 21:06:42.333963 abin_sim-1.2.0/README.md
--rw-r--r--   0        0        0       21 2023-07-20 21:06:42.333963 abin_sim-1.2.0/abin_sim/__init__.py
--rw-r--r--   0        0        0     9288 2023-07-20 21:06:42.333963 abin_sim-1.2.0/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-07-20 21:06:42.337963 abin_sim-1.2.0/abin_sim/config.py
--rw-r--r--   0        0        0     2063 2023-07-20 21:06:42.337963 abin_sim-1.2.0/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     6603 2023-07-20 21:06:42.337963 abin_sim-1.2.0/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-07-20 21:06:42.337963 abin_sim-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-07-21 12:54:25.561003 abin_sim-1.2.1/LICENSE
+-rw-r--r--   0        0        0     8594 2023-07-21 12:54:25.561003 abin_sim-1.2.1/README.md
+-rw-r--r--   0        0        0       21 2023-07-21 12:54:25.561003 abin_sim-1.2.1/abin_sim/__init__.py
+-rw-r--r--   0        0        0     9315 2023-07-21 12:54:25.561003 abin_sim-1.2.1/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-07-21 12:54:25.561003 abin_sim-1.2.1/abin_sim/config.py
+-rw-r--r--   0        0        0     2063 2023-07-21 12:54:25.561003 abin_sim-1.2.1/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     6676 2023-07-21 12:54:25.561003 abin_sim-1.2.1/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-07-21 12:54:25.561003 abin_sim-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.2.1/PKG-INFO
```

### Comparing `abin_sim-1.2.0/README.md` & `abin_sim-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `abin_sim-1.2.0/abin_sim/cli.py` & `abin_sim-1.2.1/abin_sim/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
     vault_token = settings.params.vault_token
     vault_url = settings.params.vault_url
     if secret == 'env':
         payload = convert_to_json(file)
     else:
         payload = file
 
+    console.print(payload)
     confirm = query_yes_no(f'Gostaria de atualizar a secret "{secret}" para o app {app}, no projeto {env.upper()}-{proj.upper()} ?', 'no')
     if confirm:
         ret = update_secret(app, env, proj, secret, vault_token, vault_url, payload)
         console.print(ret)
     else:
         console.print({'Status': 'Canceled'})
```

### Comparing `abin_sim-1.2.0/abin_sim/core/file_manager.py` & `abin_sim-1.2.1/abin_sim/core/file_manager.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.2.0/abin_sim/core/functions.py` & `abin_sim-1.2.1/abin_sim/core/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,19 @@
 
     contentList = [x.strip().split('^#')[0].split('=', 1) for x in content if '=' in x.split('^#')[0]]
     contentDict = dict(contentList)
     for k, v in contentList:
         # for i, x in enumerate(v.split('$')[1:]):
         #     key = re.findall(r'\w+', x)[0]
         #     v = v.replace('$' + key, contentDict[key])
-        if '=' in v or '$' in v and not "'" in v:
-            contentDict[k] = f"'{v.strip()}'"
+        if '=' in v or '$' in v:
+            if "'" in v:
+                contentDict[k] = v.strip()
+            else:
+                contentDict[k] = f"'{v.strip()}'"
         else:
             contentDict[k] = v.strip()
 
     return json.dumps(contentDict)
 
 def replace_string(secret, search, replace):
     with open(secret, 'rt') as file_in:
```

### Comparing `abin_sim-1.2.0/pyproject.toml` & `abin_sim-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "1.2.0"
+version = "1.2.1"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-1.2.0/PKG-INFO` & `abin_sim-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 1.2.0
+Version: 1.2.1
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

