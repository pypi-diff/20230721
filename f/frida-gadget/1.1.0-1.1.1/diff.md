# Comparing `tmp/frida-gadget-1.1.0.tar.gz` & `tmp/frida-gadget-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frida-gadget-1.1.0.tar", last modified: Thu Jul 20 19:00:32 2023, max compression
+gzip compressed data, was "frida-gadget-1.1.1.tar", last modified: Fri Jul 21 17:03:28 2023, max compression
```

## Comparing `frida-gadget-1.1.0.tar` & `frida-gadget-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 19:00:32.889369 frida-gadget-1.1.0/
--rw-rw-rw-   0        0        0     7692 2023-07-20 19:00:32.889369 frida-gadget-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7021 2023-07-20 19:00:09.000000 frida-gadget-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-20 19:00:32.882858 frida-gadget-1.1.0/frida_gadget.egg-info/
--rw-rw-rw-   0        0        0     7692 2023-07-20 19:00:32.000000 frida-gadget-1.1.0/frida_gadget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-20 19:00:32.000000 frida-gadget-1.1.0/frida_gadget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 19:00:32.000000 frida-gadget-1.1.0/frida_gadget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-20 19:00:32.000000 frida-gadget-1.1.0/frida_gadget.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-20 19:00:32.000000 frida-gadget-1.1.0/frida_gadget.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-20 19:00:32.000000 frida-gadget-1.1.0/frida_gadget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 19:00:32.885860 frida-gadget-1.1.0/scripts/
--rw-rw-rw-   0        0        0      673 2023-07-20 18:12:04.000000 frida-gadget-1.1.0/scripts/__init__.py
--rw-rw-rw-   0        0        0     8797 2023-07-20 18:35:23.000000 frida-gadget-1.1.0/scripts/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:00:32.886364 frida-gadget-1.1.0/scripts/files/
--rw-rw-rw-   0        0        0       80 2023-07-20 18:51:06.000000 frida-gadget-1.1.0/scripts/files/README.md
--rw-rw-rw-   0        0        0     3518 2023-07-20 18:43:58.000000 frida-gadget-1.1.0/scripts/frida_github.py
--rw-rw-rw-   0        0        0      648 2023-07-20 18:11:49.000000 frida-gadget-1.1.0/scripts/logger.py
--rw-rw-rw-   0        0        0       42 2023-07-20 19:00:32.889369 frida-gadget-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1471 2023-07-20 18:52:30.000000 frida-gadget-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 19:00:32.888369 frida-gadget-1.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 15:35:47.000000 frida-gadget-1.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      418 2023-07-20 18:46:32.000000 frida-gadget-1.1.0/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.972683 frida-gadget-1.1.1/
+-rw-rw-rw-   0        0        0     7738 2023-07-21 17:03:28.971684 frida-gadget-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7067 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.950153 frida-gadget-1.1.1/frida_gadget.egg-info/
+-rw-rw-rw-   0        0        0     7738 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-21 17:03:28.000000 frida-gadget-1.1.1/frida_gadget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.955147 frida-gadget-1.1.1/scripts/
+-rw-rw-rw-   0        0        0      699 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/__init__.py
+-rw-rw-rw-   0        0        0     9150 2023-07-21 16:59:55.000000 frida-gadget-1.1.1/scripts/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.957154 frida-gadget-1.1.1/scripts/files/
+-rw-rw-rw-   0        0        0       84 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/files/README.md
+-rw-rw-rw-   0        0        0     3531 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/frida_github.py
+-rw-rw-rw-   0        0        0      648 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/scripts/logger.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 17:03:28.972683 frida-gadget-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1471 2023-07-21 16:47:39.000000 frida-gadget-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:03:28.969682 frida-gadget-1.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-07-21 16:46:23.000000 frida-gadget-1.1.1/tests/test_cli.py
```

### Comparing `frida-gadget-1.1.0/PKG-INFO` & `frida-gadget-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-gadget
-Version: 1.1.0
+Version: 1.1.1
 Summary: Frida gadget into an APK
 Home-page: https://github.com/ksg97031/frida-gadget
 Author: ksg97031
 Author-email: ksg97031@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,38 +15,43 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 
 frida-gadget
 ============
 
-|Docker| |Coverage-Status| |Branch-Coverage-Status| |Codacy-Grade| |Libraries-Rank|
+|Codacy-Grade| |Docker| |Libraries-Rank|
 
 
-| ``frida-gadget`` is a APK patcher for  `frida gadget <https://frida.re/docs/gadget/>`__.
-| I hope this will help you to patch APK when you want to utilize the Frida gadget.
+| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
 
 Installation
 ------------
 
 |Py-Versions| |PyPI-Downloads| |Libraries-Dependents|
 
 .. code:: sh
 
     pip install frida-gadget
     
 Prerequirement
 ----------------
 
-| You should install the Apktool and set the PATH environment variable. (`Install apktool <https://ibotpeaches.github.io/Apktool/install/>`_)
+| You should install Apktool and add it to your PATH environment variable.
 |   
 
 .. code:: sh
 
-   brew install apktool   
+   # Install Apktool on macOS
+   brew install apktool
+    
+   # Add Apktool to your PATH environment variable
+   export PATH=$PATH:$HOME/.brew/bin 
+
+| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
 
 Usage
 ------------
 
 .. code:: sh
 
     $ frida-gadget --help
@@ -56,15 +61,15 @@
         --arch TEXT  Support [arm, arm64, x86]
         --help       Show this message and exit.
 
 Example
 ~~~~~~~
 .. code:: sh
 
-    $ frida-gadget /Users/ksg/demo.apk  --arch arm64
+    $ frida-gadget handtrackinggpu.apk --arch arm64
       [INFO] Auto-detected frida version: 16.1.3
       [INFO] APK: '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu.apk'
       [INFO] Gadget Architecture(--arch): arm64(default)
       [DEBUG] Decompiling the target APK using apktool
       [DEBUG] Downloading the frida gadget library for arm64
       [DEBUG] Checking internet permission and extractNativeLibs settings
       [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
@@ -78,15 +83,15 @@
       
     $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
       21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
        
 loadLibrary code will be injected
 ********************************************
 
-.. image:: https://github.com/ksg97031/frida-gadget/blob/patch-frida-15.1.1/images/decompile.png
+.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
    :width: 600
 
 Easy to re-sign your app by ``apk-signer``
 ********************************************
 
 .. code:: sh
```

### Comparing `frida-gadget-1.1.0/README.rst` & `frida-gadget-1.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 frida-gadget
 ============
 
-|Docker| |Coverage-Status| |Branch-Coverage-Status| |Codacy-Grade| |Libraries-Rank|
+|Codacy-Grade| |Docker| |Libraries-Rank|
 
 
-| ``frida-gadget`` is a APK patcher for  `frida gadget <https://frida.re/docs/gadget/>`__.
-| I hope this will help you to patch APK when you want to utilize the Frida gadget.
+| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
 
 Installation
 ------------
 
 |Py-Versions| |PyPI-Downloads| |Libraries-Dependents|
 
 .. code:: sh
 
     pip install frida-gadget
     
 Prerequirement
 ----------------
 
-| You should install the Apktool and set the PATH environment variable. (`Install apktool <https://ibotpeaches.github.io/Apktool/install/>`_)
+| You should install Apktool and add it to your PATH environment variable.
 |   
 
 .. code:: sh
 
-   brew install apktool   
+   # Install Apktool on macOS
+   brew install apktool
+    
+   # Add Apktool to your PATH environment variable
+   export PATH=$PATH:$HOME/.brew/bin 
+
+| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
 
 Usage
 ------------
 
 .. code:: sh
 
     $ frida-gadget --help
@@ -38,15 +43,15 @@
         --arch TEXT  Support [arm, arm64, x86]
         --help       Show this message and exit.
 
 Example
 ~~~~~~~
 .. code:: sh
 
-    $ frida-gadget /Users/ksg/demo.apk  --arch arm64
+    $ frida-gadget handtrackinggpu.apk --arch arm64
       [INFO] Auto-detected frida version: 16.1.3
       [INFO] APK: '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu.apk'
       [INFO] Gadget Architecture(--arch): arm64(default)
       [DEBUG] Decompiling the target APK using apktool
       [DEBUG] Downloading the frida gadget library for arm64
       [DEBUG] Checking internet permission and extractNativeLibs settings
       [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
@@ -60,15 +65,15 @@
       
     $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
       21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
        
 loadLibrary code will be injected
 ********************************************
 
-.. image:: https://github.com/ksg97031/frida-gadget/blob/patch-frida-15.1.1/images/decompile.png
+.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
    :width: 600
 
 Easy to re-sign your app by ``apk-signer``
 ********************************************
 
 .. code:: sh
```

### Comparing `frida-gadget-1.1.0/frida_gadget.egg-info/PKG-INFO` & `frida-gadget-1.1.1/frida_gadget.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frida-gadget
-Version: 1.1.0
+Version: 1.1.1
 Summary: Frida gadget into an APK
 Home-page: https://github.com/ksg97031/frida-gadget
 Author: ksg97031
 Author-email: ksg97031@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,38 +15,43 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 
 frida-gadget
 ============
 
-|Docker| |Coverage-Status| |Branch-Coverage-Status| |Codacy-Grade| |Libraries-Rank|
+|Codacy-Grade| |Docker| |Libraries-Rank|
 
 
-| ``frida-gadget`` is a APK patcher for  `frida gadget <https://frida.re/docs/gadget/>`__.
-| I hope this will help you to patch APK when you want to utilize the Frida gadget.
+| ``frida-gadget`` is a tool that can be used to patch APKs in order to utilize the `Frida gadget <https://frida.re/docs/gadget/>`_.
 
 Installation
 ------------
 
 |Py-Versions| |PyPI-Downloads| |Libraries-Dependents|
 
 .. code:: sh
 
     pip install frida-gadget
     
 Prerequirement
 ----------------
 
-| You should install the Apktool and set the PATH environment variable. (`Install apktool <https://ibotpeaches.github.io/Apktool/install/>`_)
+| You should install Apktool and add it to your PATH environment variable.
 |   
 
 .. code:: sh
 
-   brew install apktool   
+   # Install Apktool on macOS
+   brew install apktool
+    
+   # Add Apktool to your PATH environment variable
+   export PATH=$PATH:$HOME/.brew/bin 
+
+| Other Platforms: `Install Guide <https://ibotpeaches.github.io/Apktool/install/>`_
 
 Usage
 ------------
 
 .. code:: sh
 
     $ frida-gadget --help
@@ -56,15 +61,15 @@
         --arch TEXT  Support [arm, arm64, x86]
         --help       Show this message and exit.
 
 Example
 ~~~~~~~
 .. code:: sh
 
-    $ frida-gadget /Users/ksg/demo.apk  --arch arm64
+    $ frida-gadget handtrackinggpu.apk --arch arm64
       [INFO] Auto-detected frida version: 16.1.3
       [INFO] APK: '[REDACTED]\frida-gadget\tests\demo-apk\handtrackinggpu.apk'
       [INFO] Gadget Architecture(--arch): arm64(default)
       [DEBUG] Decompiling the target APK using apktool
       [DEBUG] Downloading the frida gadget library for arm64
       [DEBUG] Checking internet permission and extractNativeLibs settings
       [DEBUG] Adding 'android.permission.INTERNET' permission to AndroidManifest.xml
@@ -78,15 +83,15 @@
       
     $ unzip -l handtrackinggpu.apk | grep libfrida-gadget
       21133848  09-15-2021 02:28   lib/arm64-v8a/libfrida-gadget-16.1.3-android-arm64.so 
        
 loadLibrary code will be injected
 ********************************************
 
-.. image:: https://github.com/ksg97031/frida-gadget/blob/patch-frida-15.1.1/images/decompile.png
+.. image:: https://github.com/ksg97031/frida-gadget/blob/trunk/images/decompile.png
    :width: 600
 
 Easy to re-sign your app by ``apk-signer``
 ********************************************
 
 .. code:: sh
```

### Comparing `frida-gadget-1.1.0/scripts/__init__.py` & `frida-gadget-1.1.1/scripts/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """init file for scripts folder."""
-from shutil import which
-from pathlib import Path
+import sys
+import subprocess
 from .logger import logger
-import pip
-from colorlog import ColoredFormatter
 
 
 def import_or_install(package):
     """Function to install missing packages.
 
     Args:
         package (string): Name of the package to install.
     """
     try:
         __import__(package)
     except ImportError:
-        pip.main(['install', '--user', package])
+        subprocess.check_call([sys.executable, '-m', 'pip', 'install', 'frida', '--user'])
+        logger.info('Try Again')
+        sys.exit(0)
 
 
 import_or_install('frida')  # Install missing packages
 INSTALLED_FRIDA_VERSION: str = __import__('frida').__version__  # Get installed frida version
-logger.info("Auto-detected frida version: " + INSTALLED_FRIDA_VERSION)
+logger.info("Auto-detected frida version: %s", INSTALLED_FRIDA_VERSION)
```

### Comparing `frida-gadget-1.1.0/scripts/cli.py` & `frida-gadget-1.1.1/scripts/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Frida gadget injector for Android APK"""
 import os
 import sys
 import shutil
 import subprocess
 from shutil import which
 from pathlib import Path
-from subprocess import check_output, CalledProcessError
+import click
+from androguard.core.bytecodes.apk import APK
 from .logger import logger
 from .frida_github import FridaGithub
 from . import INSTALLED_FRIDA_VERSION
-import click
-from androguard.core.bytecodes.apk import APK
 
 
 p = Path(__file__)
 ROOT_DIR = p.parent.resolve()
 TEMP_DIR = ROOT_DIR.joinpath('temp')
 FILE_DIR = ROOT_DIR.joinpath('files')
 
@@ -33,110 +32,72 @@
     """
     if isinstance(option, list):
         cmd = [APKTOOL] + option + [apk_path]
     else:
         cmd = [APKTOOL, option, apk_path]
 
     pipe = subprocess.PIPE
-    with subprocess.Popen(cmd, stdin=pipe, stdout=pipe, stderr=pipe) as p:
-        _, stderr = p.communicate(b"\n")
-        if p.returncode != 0:
-            raise CalledProcessError(p.returncode, cmd, stderr)
+    with subprocess.Popen(cmd, stdin=pipe, stdout=pipe, stderr=pipe) as process:
+        _, stderr = process.communicate(b"\n")
+        if process.returncode != 0:
+            raise subprocess.CalledProcessError(process.returncode, cmd, stderr)
         return True
 
 def download_gadget(arch: str):
     """Download the frida gadget library
 
     Args:
         arch (str): architecture of the device
     """
-    g = FridaGithub(INSTALLED_FRIDA_VERSION)
-    assets = g.get_assets()
+    frida_github = FridaGithub(INSTALLED_FRIDA_VERSION)
+    assets = frida_github.get_assets()
     file = f'frida-gadget-{INSTALLED_FRIDA_VERSION}-android-{arch}.so.xz'
     for asset in assets:
         if asset['name'] == file:
             logger.debug("Downloading the frida gadget library for %s", arch)
             so_gadget_path = str(FILE_DIR.joinpath(file[:-3]))
-            return g.download_gadget_so(asset['browser_download_url'], so_gadget_path)            
+            return frida_github.download_gadget_so(asset['browser_download_url'], so_gadget_path)
 
     raise FileNotFoundError(f"'{file}' not found in the github releases")
 
-def process(apk_path:str, arch:str, decompiled_path:str):
-    """Inject frida gadget into an APK
+def insert_loadlibary(decompiled_path, main_activity, load_library_name):
+    """Inject loadlibary code to main activity
 
     Args:
-        apk (APK): path of apk file
-        arch (str): architecture of the device
-        decompiled_path (str): decomplied path of apk file
-
-    Raises:
-        FileNotFoundError: file not found
-        NotImplementedError: not implemented
+        text (str): smali code of the main activity
     """
-    apk = APK(apk_path)
-    gadget_path = download_gadget(arch) # Download gadget library
-    gadget_name = Path(gadget_path).name
-    
-    main_activity = apk.get_main_activity()
-    main_activity = main_activity.split('.')
-    main_activity[-1] += '.smali'
-
-    # Add internet permission
-    logger.debug("Checking internet permission and extractNativeLibs settings")
-    android_manifest = decompiled_path.joinpath("AndroidManifest.xml")
-    txt = android_manifest.read_text(encoding="utf-8")
-    pos = txt.index('</manifest>')
-    permission = 'android.permission.INTERNET'
-
-    if permission not in txt:
-        logger.debug(
-            "Adding 'android.permission.INTERNET' permission to AndroidManifest.xml")
-        permissions_txt = f"<uses-permission android:name='{permission}'/>"
-        txt = txt[:pos] + permissions_txt + txt[pos:]
-
-    # Set extractNativeLibs to true
-    if ':extractNativeLibs="false"' in txt:
-        logger.debug('Editing the extractNativeLibs="true"')
-        txt = txt.replace(':extractNativeLibs="false"',
-                            ':extractNativeLibs="true"')
-    android_manifest.write_text(txt, encoding="utf-8")
-
-    # Search the main activity from smali files
     logger.debug('Searching for the main activity in the smali files')
     target_smali = None
-    for smali_dir in decompiled_path.glob("smali*/"):
-        target_smali = smali_dir.joinpath(*main_activity)
-        if target_smali.exists():
-            break
-
+    
+    target_relative_path = main_activity.replace(".", os.sep)
+    target_smali = decompiled_path.joinpath("smali", target_relative_path + ".smali")
     if not target_smali or not target_smali.exists():
-        raise FileNotFoundError(
-            "Not Found, target class file: " + ".".join(main_activity))
+        raise FileNotFoundError(f"The target class file {target_smali} was not found.")
 
     logger.debug("Found the main activity at '%s'", str(target_smali))
     text = target_smali.read_text()
+
     text = text.replace(
         "invoke-virtual {v0, v1}, Ljava/lang/Runtime;->exit(I)V", "")
     text = text.split("\n")
 
     # Find onCreate method and inject loadLibary code for frida gadget
     logger.debug(
         'Locating the onCreate method and injecting the loadLibrary code')
     idx = 0
     status = False
     while idx != len(text):
         line = text[idx].strip()
         if line.startswith('.method') and "onCreate(" in line:
             locals_line_bit = text[idx + 1].split(".locals ")
             locals_variable_count = int(locals_line_bit[1])
-            locals_line_bit[1] = str(locals_variable_count + 1)        
-            load_library_name = gadget_name[:-3] # without extension
+            locals_line_bit[1] = str(locals_variable_count + 1)
             if load_library_name.startswith('lib'):
                 load_library_name = load_library_name[3:]
-                
+
             new_locals_line = ".locals ".join(locals_line_bit)
             text[idx + 1] = new_locals_line
 
             load_str = f'    const-string v{locals_variable_count}, "{load_library_name}"'
             load_library = f'    invoke-static {{v{locals_variable_count}}}, \
                 Ljava/lang/System;->loadLibrary(Ljava/lang/String;)V'
             text.insert(idx + 2, load_library)
@@ -156,14 +117,63 @@
         logger.error("Device/Emulator OS: <Your Device/Emulator OS>")
         logger.error("Frida Version: <Your Frida Version>")
         sys.exit(-1)
 
     # Replace the smali file with the new one
     target_smali.write_text("\n".join(text))
 
+def modify_manifest(decompiled_path):
+    """Modify manifest permssions
+
+    Args:
+        decompiled_path (str): decomplied path of apk file
+    """
+    # Add internet permission
+    logger.debug("Checking internet permission and extractNativeLibs settings")
+    android_manifest = decompiled_path.joinpath("AndroidManifest.xml")
+    txt = android_manifest.read_text(encoding="utf-8")
+    pos = txt.index('</manifest>')
+    permission = 'android.permission.INTERNET'
+
+    if permission not in txt:
+        logger.debug(
+            "Adding 'android.permission.INTERNET' permission to AndroidManifest.xml")
+        permissions_txt = f"<uses-permission android:name='{permission}'/>"
+        txt = txt[:pos] + permissions_txt + txt[pos:]
+
+    # Set extractNativeLibs to true
+    if ':extractNativeLibs="false"' in txt:
+        logger.debug('Editing the extractNativeLibs="true"')
+        txt = txt.replace(':extractNativeLibs="false"',
+                            ':extractNativeLibs="true"')
+    android_manifest.write_text(txt, encoding="utf-8")
+
+def inject_gadget_into_apk(apk_path:str, arch:str, decompiled_path:str):
+    """Inject frida gadget into an APK
+
+    Args:
+        apk (APK): path of apk file
+        arch (str): architecture of the device
+        decompiled_path (str): decomplied path of apk file
+
+    Raises:
+        FileNotFoundError: file not found
+        NotImplementedError: not implemented
+    """
+    apk = APK(apk_path)
+    gadget_path = download_gadget(arch) # Download gadget library
+    gadget_name = Path(gadget_path).name
+    main_activity = apk.get_main_activity()
+    # Apply permission to android manifest
+    modify_manifest(decompiled_path)
+
+    # Search the main activity from smali files
+    load_library_name = gadget_name[:-3]
+    insert_loadlibary(decompiled_path, main_activity, load_library_name)
+
     # Copy the frida gadget library to the lib directory
     lib = decompiled_path.joinpath('lib')
     if not lib.exists():
         lib.mkdir()
     arch_dirnames = {'arm': 'armeabi-v7a', 'arm64': 'arm64-v8a'}
     if arch not in arch_dirnames:
         raise NotImplementedError(f"The architecture '{arch}' is not supported.")
@@ -195,28 +205,28 @@
     Raises:
         Exception: _description_
         Exception: _description_
         Exception: _description_
 
     Returns:
         _type_: _description_
-    """    
+    """
     if not os.path.exists(apk_path):
         logger.error("Can't find the target APK '%s'", apk_path)
         sys.exit(-1)
 
     assert apk_path.endswith('.apk')
     apk_path = Path(apk_path)
 
     logger.info("APK: '%s'", apk_path)
     logger.info("Gadget Architecture(--arch): %s%s", arch, "(default)" if arch == "arm64" else "")
 
     arch = arch.lower()
     supported_archs = ['arm', 'arm64', 'x86']
-    if arch not in supported_archs: 
+    if arch not in supported_archs:
         logger.error(
             "The --arch option only supports the following architectures: %s",
             ", ".join(supported_archs)
         )
         sys.exit(-1)
 
     # Make temp directory for decompile
@@ -226,18 +236,19 @@
         shutil.rmtree(decompiled_path)
     decompiled_path.mkdir()
 
     # APK decompile with apktool
     run_apktool(['d', '-o', str(decompiled_path.resolve()), '-f'], str(apk_path.resolve()))
 
     # Process if decompile is success
-    process(apk_path, arch, decompiled_path)
+    inject_gadget_into_apk(apk_path, arch, decompiled_path)
 
-    # Rebuild with apktool, print apk_path if process is success    
-    run_apktool('b', str(decompiled_path.resolve()))        
+    # Rebuild with apktool, print apk_path if process is success
+    run_apktool('b', str(decompiled_path.resolve()))
     apk_path = decompiled_path.joinpath('dist', apk_path.name)
     logger.info('Success!\n')
-    logger.info('Output: %s', str(apk_path.resolve()))    
+    logger.info('Output: %s', str(apk_path.resolve()))
+
 
 if __name__ == '__main__':
     # pylint: disable=no-value-for-parameter
     run()
```

### Comparing `frida-gadget-1.1.0/scripts/frida_github.py` & `frida-gadget-1.1.1/scripts/frida_github.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Github module for download frida gadget library"""
 # Base code is sourced from the GitHub repository of Objection.
 # Source: https://github.com/sensepost/objection/blob/master/objection/utils/patchers/github.py
 import lzma
-import requests
 from pathlib import Path
+import requests
 
-class FridaGithub(object):
+class FridaGithub:
     """ Interact with Github """
 
     GITHUB_LATEST_RELEASE = 'https://api.github.com/repos/frida/frida/releases/latest'
     GITHUB_TAGGED_RELEASE = 'https://api.github.com/repos/frida/frida/releases/tags/{tag}'
 
     # the 'context' of this Github instance
     gadget_version = None
@@ -33,15 +33,15 @@
         """
 
         # return a cached response if possible
         if endpoint in self.request_cache:
             return self.request_cache[endpoint]
 
         # get a new response
-        results = requests.get(endpoint).json()
+        results = requests.get(endpoint, timeout=30).json()
 
         # cache it
         self.request_cache[endpoint] = results
 
         # and return it
         return results
 
@@ -82,20 +82,20 @@
             :return:
         """
 
         assert output_file.endswith('.xz')
         filepath = Path(output_file)
         if filepath.exists() and filepath.stat().st_size > 0:
             return
-        
-        response = requests.get(url, stream=True)
-        with open(output_file, 'wb') as f:
+
+        response = requests.get(url, timeout=600, stream=True)
+        with open(output_file, 'wb') as asset:
             for chunk in response.iter_content(chunk_size=1024):
                 if chunk:
-                    f.write(chunk)
+                    asset.write(chunk)
 
     def download_gadget_so(self, url, gadget_fullpath: str) -> str:
         """
             Download the gadget library from Github.
 
             :param gadget_path:
             :return:
@@ -110,8 +110,7 @@
 
         with lzma.open(xz_gadget_fullpath, "rb") as lzma_file:
             decompressed_data = lzma_file.read()
         with open(gadget_fullpath, "wb") as gadget_file:
             gadget_file.write(decompressed_data)
 
         return gadget_fullpath
-
```

### Comparing `frida-gadget-1.1.0/scripts/logger.py` & `frida-gadget-1.1.1/scripts/logger.py`

 * *Files identical despite different names*

### Comparing `frida-gadget-1.1.0/setup.py` & `frida-gadget-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'coverage',
     'requests',
 ]
 
 setuptools.setup(
     name="frida-gadget",
     python_requires='>=3.6',
-    version="1.1.0",
+    version="1.1.1",
     author="ksg97031",
     author_email="ksg97031@gmail.com",
     description="Frida gadget into an APK",
     install_requires=requires,
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/ksg97031/frida-gadget",
```

