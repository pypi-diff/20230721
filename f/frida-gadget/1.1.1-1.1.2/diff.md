# Comparing `tmp/frida-gadget-1.1.1.tar.gz` & `tmp/frida-gadget-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frida-gadget-1.1.1.tar", last modified: Fri Jul 21 17:03:28 2023, max compression
+gzip compressed data, was "frida-gadget-1.1.2.tar", last modified: Fri Jul 21 17:09:38 2023, max compression
```

## Comparing `frida-gadget-1.1.1.tar` & `frida-gadget-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.972683 frida-gadget-1.1.1/
--rw-rw-rw-   0        0        0     7738 2023-07-21 17:03:28.971684 frida-gadget-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7067 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.950153 frida-gadget-1.1.1/frida_gadget.egg-info/
--rw-rw-rw-   0        0        0     7738 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.955147 frida-gadget-1.1.1/scripts/
--rw-rw-rw-   0        0        0      699 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/__init__.py
--rw-rw-rw-   0        0        0     9150 2023-07-21 16:59:55.000000 frida-gadget-1.1.1/scripts/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.957154 frida-gadget-1.1.1/scripts/files/
--rw-rw-rw-   0        0        0       84 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/files/README.md
--rw-rw-rw-   0        0        0     3531 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/frida_github.py
--rw-rw-rw-   0        0        0      648 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/logger.py
--rw-rw-rw-   0        0        0       42 2023-07-21 17:03:28.972683 frida-gadget-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1471 2023-07-21 16:47:39.000000 frida-gadget-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.969682 frida-gadget-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      418 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.412231 frida-gadget-1.1.2/
+-rw-rw-rw-   0        0        0     7738 2023-07-21 17:09:38.412231 frida-gadget-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7067 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.402804 frida-gadget-1.1.2/frida_gadget.egg-info/
+-rw-rw-rw-   0        0        0     7738 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 17:09:38.000000 frida-gadget-1.1.2/frida_gadget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.406797 frida-gadget-1.1.2/scripts/
+-rw-rw-rw-   0        0        0      699 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/__init__.py
+-rw-rw-rw-   0        0        0     8974 2023-07-21 17:09:05.000000 frida-gadget-1.1.2/scripts/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.407797 frida-gadget-1.1.2/scripts/files/
+-rw-rw-rw-   0        0        0       84 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/files/README.md
+-rw-rw-rw-   0        0        0     3531 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/frida_github.py
+-rw-rw-rw-   0        0        0      648 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/scripts/logger.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 17:09:38.412231 frida-gadget-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1471 2023-07-21 17:08:00.000000 frida-gadget-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.408797 frida-gadget-1.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-07-21 16:46:23.000000 frida-gadget-1.1.2/tests/test_cli.py
```

### Comparing `frida-gadget-1.1.1/PKG-INFO` & `frida-gadget-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-gadget
-Version: 1.1.1
+Version: 1.1.2
 Summary: Frida gadget into an APK
 Home-page: https://github.com/ksg97031/frida-gadget
 Author: ksg97031
 Author-email: ksg97031@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `frida-gadget-1.1.1/README.rst` & `frida-gadget-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.1/frida_gadget.egg-info/PKG-INFO` & `frida-gadget-1.1.2/frida_gadget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-gadget
-Version: 1.1.1
+Version: 1.1.2
 Summary: Frida gadget into an APK
 Home-page: https://github.com/ksg97031/frida-gadget
 Author: ksg97031
 Author-email: ksg97031@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `frida-gadget-1.1.1/scripts/__init__.py` & `frida-gadget-1.1.2/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.1/scripts/cli.py` & `frida-gadget-1.1.2/scripts/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -190,34 +190,25 @@
 
     logger.debug('Recompiling the new APK using apktool')
 
 
 
 @click.command()
 @click.option('--arch', default="arm64", help='Support [arm, arm64, x86]')
-@click.argument('apk_path')
+@click.argument('apk_path', type=click.Path(exists=True), required=True)
 def run(apk_path: str, arch: str):
-    """Inject Frida gadget into an APK
+    """Patch an APK with the Frida gadget library
 
     Args:
-        apk_path (str): path of apk file
-        arch (str): type of device architecture
+        apk_path (str): Path of the target APK file
+        arch (str): Target architecture of the device
 
-    Raises:
-        Exception: _description_
-        Exception: _description_
-        Exception: _description_
-
-    Returns:
-        _type_: _description_
+    Outputs:
+        Injected APK file
     """
-    if not os.path.exists(apk_path):
-        logger.error("Can't find the target APK '%s'", apk_path)
-        sys.exit(-1)
-
     assert apk_path.endswith('.apk')
     apk_path = Path(apk_path)
 
     logger.info("APK: '%s'", apk_path)
     logger.info("Gadget Architecture(--arch): %s%s", arch, "(default)" if arch == "arm64" else "")
 
     arch = arch.lower()
```

### Comparing `frida-gadget-1.1.1/scripts/frida_github.py` & `frida-gadget-1.1.2/scripts/frida_github.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.1/scripts/logger.py` & `frida-gadget-1.1.2/scripts/logger.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.1/setup.py` & `frida-gadget-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'coverage',
     'requests',
 ]
 
 setuptools.setup(
     name="frida-gadget",
     python_requires='>=3.6',
-    version="1.1.1",
+    version="1.1.2",
     author="ksg97031",
     author_email="ksg97031@gmail.com",
     description="Frida gadget into an APK",
     install_requires=requires,
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/ksg97031/frida-gadget",
```

