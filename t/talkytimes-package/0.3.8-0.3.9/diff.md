# Comparing `tmp/talkytimes_package-0.3.8.tar.gz` & `tmp/talkytimes_package-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.3.8.tar", last modified: Tue Jul 18 02:01:16 2023, max compression
+gzip compressed data, was "talkytimes_package-0.3.9.tar", last modified: Tue Jul 18 02:19:45 2023, max compression
```

## Comparing `talkytimes_package-0.3.8.tar` & `talkytimes_package-0.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.729896 talkytimes_package-0.3.8/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.8/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-18 02:01:16.729896 talkytimes_package-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.8/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-18 02:01:16.731898 talkytimes_package-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.693898 talkytimes_package-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.702899 talkytimes_package-0.3.8/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.8/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      525 2023-07-18 01:47:45.000000 talkytimes_package-0.3.8/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     1676 2023-07-18 01:59:23.000000 talkytimes_package-0.3.8/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.706900 talkytimes_package-0.3.8/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-18 02:00:22.000000 talkytimes_package-0.3.8/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.8/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3955 2023-07-18 01:48:52.000000 talkytimes_package-0.3.8/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.728898 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 02:19:45.361848 talkytimes_package-0.3.9/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-18 02:19:45.361848 talkytimes_package-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.9/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-18 02:19:45.362843 talkytimes_package-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:19:45.335841 talkytimes_package-0.3.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 02:19:45.343840 talkytimes_package-0.3.9/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.9/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-07-18 01:47:45.000000 talkytimes_package-0.3.9/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     1676 2023-07-18 01:59:23.000000 talkytimes_package-0.3.9/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:19:45.345838 talkytimes_package-0.3.9/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-18 02:19:38.000000 talkytimes_package-0.3.9/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-07-18 02:19:30.000000 talkytimes_package-0.3.9/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3955 2023-07-18 01:48:52.000000 talkytimes_package-0.3.9/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:19:45.360838 talkytimes_package-0.3.9/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-18 02:19:45.000000 talkytimes_package-0.3.9/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-18 02:19:45.000000 talkytimes_package-0.3.9/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:19:45.000000 talkytimes_package-0.3.9/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-18 02:19:45.000000 talkytimes_package-0.3.9/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 02:19:45.000000 talkytimes_package-0.3.9/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.3.8/LICENSE` & `talkytimes_package-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.8/src/dynamodb/base.py` & `talkytimes_package-0.3.9/src/dynamodb/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.8/src/dynamodb/dynamodb.py` & `talkytimes_package-0.3.9/src/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.8/src/talkytimes/base.py` & `talkytimes_package-0.3.9/src/talkytimes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         options.binary_location = '/opt/chrome/chrome'
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
         options.add_argument("--disable-gpu")
         options.add_argument("--window-size=1280x1696")
         options.add_argument("--single-process")
         options.add_argument("--disable-dev-shm-usage")
+        options.add_argument("--disable-dev-tools")
         options.add_argument("--no-zygote")
         options.add_argument(f"--user-data-dir={mkdtemp()}")
         options.add_argument(f"--data-path={mkdtemp()}")
         options.add_argument(f"--disk-cache-dir={mkdtemp()}")
         options.add_argument("--remote-debugging-port=9222")
         chrome = webdriver.Chrome(service=service, options=options)
         return chrome
```

### Comparing `talkytimes_package-0.3.8/src/talkytimes/talkytimes.py` & `talkytimes_package-0.3.9/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

