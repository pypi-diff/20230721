# Comparing `tmp/install_jdk-1.0.4.tar.gz` & `tmp/install_jdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install_jdk-1.0.4.tar", max compression
+gzip compressed data, was "install_jdk-1.1.0.tar", max compression
```

## Comparing `install_jdk-1.0.4.tar` & `install_jdk-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-04-05 13:13:27.734637 install_jdk-1.0.4/LICENSE.md
--rw-r--r--   0        0        0    11473 2023-04-05 13:13:27.734637 install_jdk-1.0.4/README.md
--rw-r--r--   0        0        0     4690 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/__init__.py
--rw-r--r--   0        0        0      254 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/client/__init__.py
--rw-r--r--   0        0        0     3363 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/client/adoptium.py
--rw-r--r--   0        0        0     2888 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/client/client.py
--rw-r--r--   0        0        0     5229 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/client/corretto.py
--rw-r--r--   0        0        0     5685 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/client/zulu.py
--rw-r--r--   0        0        0     2518 2023-04-05 13:13:44.894972 install_jdk-1.0.4/jdk/enums.py
--rw-r--r--   0        0        0     3450 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/extension.py
--rw-r--r--   0        0        0     2454 2023-04-05 13:13:27.734637 install_jdk-1.0.4/jdk/extractor.py
--rw-r--r--   0        0        0     2135 2023-04-05 13:13:44.894972 install_jdk-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    12879 1970-01-01 00:00:00.000000 install_jdk-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-21 01:18:10.021514 install_jdk-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0    11473 2023-07-21 01:18:10.021514 install_jdk-1.1.0/README.md
+-rw-r--r--   0        0        0     4690 2023-07-21 01:18:10.021514 install_jdk-1.1.0/jdk/__init__.py
+-rw-r--r--   0        0        0      254 2023-07-21 01:18:10.021514 install_jdk-1.1.0/jdk/client/__init__.py
+-rw-r--r--   0        0        0     3607 2023-07-21 01:18:29.593671 install_jdk-1.1.0/jdk/client/adoptium.py
+-rw-r--r--   0        0        0     2766 2023-07-21 01:18:29.593671 install_jdk-1.1.0/jdk/client/client.py
+-rw-r--r--   0        0        0     5229 2023-07-21 01:18:10.021514 install_jdk-1.1.0/jdk/client/corretto.py
+-rw-r--r--   0        0        0     5685 2023-07-21 01:18:10.021514 install_jdk-1.1.0/jdk/client/zulu.py
+-rw-r--r--   0        0        0     2518 2023-07-21 01:18:10.021514 install_jdk-1.1.0/jdk/enums.py
+-rw-r--r--   0        0        0     3450 2023-07-21 01:18:10.021514 install_jdk-1.1.0/jdk/extension.py
+-rw-r--r--   0        0        0     2454 2023-07-21 01:18:10.021514 install_jdk-1.1.0/jdk/extractor.py
+-rw-r--r--   0        0        0     2135 2023-07-21 01:18:29.593671 install_jdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12831 1970-01-01 00:00:00.000000 install_jdk-1.1.0/PKG-INFO
```

### Comparing `install_jdk-1.0.4/LICENSE.md` & `install_jdk-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/README.md` & `install_jdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/jdk/__init__.py` & `install_jdk-1.1.0/jdk/__init__.py`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/jdk/client/adoptium.py` & `install_jdk-1.1.0/jdk/client/adoptium.py`

 * *Files 16% similar despite different names*

```diff
@@ -106,14 +106,19 @@
         version = Client.normalize_version(version)
 
         if operating_system is None:
             operating_system = OperatingSystem.detect()
 
         if arch is None:
             arch = Architecture.detect()
+        arch = AdoptiumArchitecture.transform(arch)
+
+        # Handle edge case for MacOS w/Apple M1 or M2
+        if operating_system is OperatingSystem.MAC and arch == AdoptiumArchitecture.ARM:
+            arch = AdoptiumArchitecture.AARCH64
 
         if jre:
             image_type = ImageType.JRE
 
         if c_lib:
             image_type = AdoptiumImageType.STATIC_LIBS
```

### Comparing `install_jdk-1.0.4/jdk/client/client.py` & `install_jdk-1.1.0/jdk/client/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import cgi
 import shutil
 import tempfile
 from collections.abc import Iterable
 from os import path
 from typing import Callable
 from typing import List
 from typing import Optional
@@ -48,20 +47,18 @@
         if download_url.lower().startswith("http"):
             req = request.Request(download_url, headers={"User-Agent": "Mozilla/5.0"})
         else:
             raise ClientError("Invalid Download URL")
 
         jdk_file = None
         with request.urlopen(req) as open_request:  # noqa: S310
-            info = open_request.info()
-            if "Content-Disposition" in info:
-                content_disposition = info["Content-Disposition"]
-                _, params = cgi.parse_header(content_disposition)
-                if "filename" in params:
-                    jdk_file = params["filename"]
+            headers = open_request.headers
+            content_disposition = headers.get_content_disposition()
+            if content_disposition:
+                jdk_file = headers.get_filename()
             else:
                 url_path = urlsplit(download_url).path
                 jdk_file = path.basename(url_path)
 
             if jdk_file:
                 jdk_file = path.join(tempfile.gettempdir(), jdk_file)
                 with open(jdk_file, "wb") as out_file:
```

### Comparing `install_jdk-1.0.4/jdk/client/corretto.py` & `install_jdk-1.1.0/jdk/client/corretto.py`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/jdk/client/zulu.py` & `install_jdk-1.1.0/jdk/client/zulu.py`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/jdk/enums.py` & `install_jdk-1.1.0/jdk/enums.py`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/jdk/extension.py` & `install_jdk-1.1.0/jdk/extension.py`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/jdk/extractor.py` & `install_jdk-1.1.0/jdk/extractor.py`

 * *Files identical despite different names*

### Comparing `install_jdk-1.0.4/pyproject.toml` & `install_jdk-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 description = "install-jdk allows you to easily install latest Java OpenJDK version. Supports OpenJDK builds from Adoptium (previously AdoptOpenJDK), Corretto, and Zulu. Simplify your Java development with the latest OpenJDK builds."
 name = "install-jdk"
-version = "1.0.4"
+version = "1.1.0"
 keywords = [
     "Java",
     "OpenJDK",
     "AdoptOpenJDK",
     "Adoptium",
     "Corretto",
     "Zulu",
```

### Comparing `install_jdk-1.0.4/PKG-INFO` & `install_jdk-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-jdk
-Version: 1.0.4
+Version: 1.1.0
 Summary: install-jdk allows you to easily install latest Java OpenJDK version. Supports OpenJDK builds from Adoptium (previously AdoptOpenJDK), Corretto, and Zulu. Simplify your Java development with the latest OpenJDK builds.
 Home-page: https://github.com/jyksnw/install-jdk
 License: MIT
 Keywords: Java,OpenJDK,AdoptOpenJDK,Adoptium,Corretto,Zulu,JDK,JRE
 Author: Jason Snow
 Author-email: jason.snow@outlook.com
 Requires-Python: >=3.6,<4.0
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Project-URL: Changelog, https://github.com/jyksnw/install-jdk/releases
 Project-URL: Documentation, https://github.com/jyksnw/install-jdk
 Project-URL: Repository, https://github.com/jyksnw/install-jdk
 Description-Content-Type: text/markdown
```

