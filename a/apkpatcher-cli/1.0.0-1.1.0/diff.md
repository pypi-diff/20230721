# Comparing `tmp/apkpatcher-cli-1.0.0.tar.gz` & `tmp/apkpatcher-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-cli-1.0.0.tar", last modified: Fri Jul 21 13:33:28 2023, max compression
+gzip compressed data, was "apkpatcher-cli-1.1.0.tar", last modified: Fri Jul 21 15:58:50 2023, max compression
```

## Comparing `apkpatcher-cli-1.0.0.tar` & `apkpatcher-cli-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-21 13:33:28.282797 apkpatcher-cli-1.0.0/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.0.0/LICENSE
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-21 13:33:28.282797 apkpatcher-cli-1.0.0/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7537 2023-07-21 13:21:11.000000 apkpatcher-cli-1.0.0/README.md
--rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    40599 2023-07-21 13:16:21.000000 apkpatcher-cli-1.0.0/apkpatcher
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-21 13:33:28.282797 apkpatcher-cli-1.0.0/apkpatcher_cli.egg-info/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-21 13:33:28.000000 apkpatcher-cli-1.0.0/apkpatcher_cli.egg-info/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-21 13:33:28.000000 apkpatcher-cli-1.0.0/apkpatcher_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-21 13:33:28.000000 apkpatcher-cli-1.0.0/apkpatcher_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       17 2023-07-21 13:33:28.000000 apkpatcher-cli-1.0.0/apkpatcher_cli.egg-info/requires.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-21 13:33:28.000000 apkpatcher-cli-1.0.0/apkpatcher_cli.egg-info/top_level.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-21 13:33:28.282797 apkpatcher-cli-1.0.0/setup.cfg
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      804 2023-07-21 13:33:10.000000 apkpatcher-cli-1.0.0/setup.py
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.1.0/LICENSE
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7642 2023-07-21 15:48:01.000000 apkpatcher-cli-1.1.0/README.md
+-rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    42638 2023-07-21 15:57:24.000000 apkpatcher-cli-1.1.0/apkpatcher
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       17 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/requires.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/top_level.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/setup.cfg
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      804 2023-07-21 15:57:10.000000 apkpatcher-cli-1.1.0/setup.py
```

### Comparing `apkpatcher-cli-1.0.0/LICENSE` & `apkpatcher-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.0.0/PKG-INFO` & `apkpatcher-cli-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.0.0
+Version: 1.1.0
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.0.0/README.md` & `apkpatcher-cli-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,52 +31,42 @@
 - jarsigner
 
 If you have Android Studio installed, you will find aapt, zipalign and adb inside `~/Android/Sdk/build-tools/` or `~/Android/Sdk/build-tools/platform-tools/`
 
 A lot of tools used by APK Patcher require Java, so I suppose you will have it installed. Both `jarsigner` and `keytool` will probably come with your java installation. In my case I can find both tools in `/usr/lib/jvm/default/bin/` 
 
 ##### APK Patcher Installation
-Clone the repository:
-```
-cd ~/Tools/
-git clone https://github.com/badadaf/apkpatcher
-```
-
-Add the script to your PATH variable in `.bashrc`
-```
-export PATH=$PATH:/home/user/Tools/apkpatcher
-```
-
-Reopen your terminal to load `.bashrc`
+`pip install apkpatcher-cli`
 
 #### How To Use It
 For all usages, the output file will be something like <apkname>_patched.apk.
 
 **Before using apkpatcher, make sure you have the latest version of apktool**
 - ##### Downloading Gadgets
   Before using APK Patcher, download frida gadgets running the following command
   ```
   apkpatcher --update-gadgets
   ```
 
-
+- ##### Bundles
+  apkpatcher supports bundles out of the box by just passing the bundle path.
 
 - ##### Inserting Frida Gadget
   In order to insert Frida library in APK, **enable USB debugging in your device and connect it in your PC**. APK Patcher will **identify your device** architecture and **insert the right gadget**.
   ```
   apkpatcher -a base.apk
   ```
 
   If you can't connect the device in USB or if you want to select a **custom gadget**, see the *gadgets* folder and use the following syntax:
   ```
   apkpatcher -a base.apk -g ~/Tools/apkpatcher/gadgets/12.5.9/frida-gadget-12.5.9-android-arm.so
   ```
 
   When you open the app, the Android screen will stay freezed. The frida gadget has started and is waiting for connection. Connect with the command `frida -U -n Gadget`
-  
+
 - ##### Autoload Script
   You can insert the hook script inside the apk and make it load automatically, without requiring to use frida client.
   
   Create the hook script:
   ```
   Java.perform(function(){
       var Log = Java.use('android.util.Log');
@@ -88,19 +78,23 @@
   ```
   apkpatcher -a base.apk --autoload-script hook.js
   ```
 
   When you open the app, it will automatically load the hook script.
 
 - ##### Autoload script from frida codeshare
-Same as the above, but this time automatically download the script from [codeshare.frida.re](https://codeshare.frida.re).
+  Same as the above, but this time automatically download the script from [codeshare.frida.re](https://codeshare.frida.re).
+
+  ```
+  apkpatcher -a base.apk --codeshare user/hook
+  ```
 
-```
-apkpatcher -a base.apk --codeshare user/hook
-```
+- ##### Load a shared library instead of the frida gadget
+  You may also load a custom shared library (e.g compiled with frida-deepfreeze-rs) instead of a frida gadget
+  `apkpatcher -a base.apk --lib my_lib.so`
 
 - ##### Enable User Certificate Authorities
   When analyzing android apps, you may want to intercept it's HTTPS traffic with some proxy like Burp Suite. Since Android 7 - Nougat, apps that the target API Level is 24 and above no longer trust in user-added CAs. In order to bypass this restriction, you can patch the APK to insert a network configuration. APK Patcher can do this automatically for you. Use the following command
 
   ```
   apkpatcher --enable-user-certificates --prevent-frida-gadget -a base.apk
   ```
```

### Comparing `apkpatcher-cli-1.0.0/apkpatcher` & `apkpatcher-cli-1.1.0/apkpatcher`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import argparse
 import requests
 import zipfile
 from appdirs import user_data_dir, user_cache_dir
 import tempfile
 import subprocess
 
+__version__ = '1.1.0'
+
 
 # noinspection SpellCheckingInspection
 class BColors:
     COLOR_BLUE = '\033[94m'
     COLOR_RED_BG = '\033[101m'
     COLOR_RED = '\033[91m'
     COLOR_GREEN = '\033[92m'
@@ -587,14 +589,25 @@
 
         if delete_custom_files & self.AUTOLOAD_BIT:
             hookfile_path = os.path.join(arch_folder, self.DEFAULT_HOOKFILE_NAME)
 
             if os.path.isfile(hookfile_path):
                 os.remove(hookfile_path)
 
+    def insert_shared_lib(self, base_path, lib_path, lib_name, arch):
+        arch_folders = self.create_lib_arch_folders(base_path, arch)
+        if not arch_folders:
+            self.print_warn('Some error occurred while creating the libs folders')
+            return False
+        for folder in arch_folders:
+            target_path = os.path.join(folder, lib_name)
+            self.print_info('Copying shared library to {}'.format(target_path))
+            shutil.copyfile(lib_path, target_path)
+        return True
+
     def insert_frida_lib(self, base_path, gadget_path, config_file_path=None, auto_load_script_path=None):
         arch = self.get_arch_by_gadget(gadget_path)
         arch_folders = self.create_lib_arch_folders(base_path, arch)
 
         if not arch_folders:
             self.print_warn('Some error occurred while creating the libs folders')
             return False
@@ -843,15 +856,19 @@
                 'jarsigner -sigalg SHA1withRSA -digestalg SHA1 -keystore {0} '
                 '-storepass password {1} apkpatcheralias1'.format(keystorepath, apk),
                 shell=True)
 
             self.print_info('The apk was signed!')
             self.print_info('Optimizing with zipalign...')
             tmp_target_file = apk.replace('.apk', '_tmp.apk')
-            shutil.move(tmp_target_file, apk)
+            shutil.move(apk, tmp_target_file)
+            subprocess.call('zipalign 4 {0} {1}'.format(tmp_target_file, apk), stderr=subprocess.STDOUT, shell=True)
+
+            os.remove(tmp_target_file)
+            self.print_info('The file was optimized!')
             
         if not keep_keystore:
             os.remove(keystorepath)
 
         self.print_info('The APK files were signed and optimized!')
 
     @staticmethod
@@ -917,33 +934,44 @@
     parser.add_argument('--use-aapt2', help='Use aapt2 with apktool',
                         action='store_true')
 
     parser.add_argument('-e', '--enable-user-certificates', help='Add some configs in apk to accept user certificates',
                         action='store_true')
 
     parser.add_argument('--prevent-frida-gadget', help='Does not insert frida gadget', action='store_true')
+    parser.add_argument('-l', '--lib', help="Inject a shared library in place of frida gadget")
     parser.add_argument('-w', '--wait-before-repackage', help='Waits for your OK before repackage the apk',
                         action='store_true')
     parser.add_argument('-k', '--keep-keystore', help='Keeps generated keystore for future use',
                         action='store_true')
 
     parser.add_argument('-o', '--output-file', help='Specify the output file (patched)')
 
+    parser.add_argument('--version', help='Display information about the version', action='store_true')
+
     group = parser.add_argument_group('Execute command before repackage')
     group.add_argument('-x', '--exec-before-repackage', help='Specify a command to execute before repackage')
 
     group.add_argument('--pass-temp-path', help='Should I pass the apk folder as parameter to your command?',
                        action='store_true')
 
     args = parser.parse_args()
 
     if len(sys.argv) == 1:
         parser.print_help()
 
         return 1
+    
+    if args.version:
+        patcher.set_verbosity(patcher.VERBOSITY_HIGH)
+
+        frida_version = subprocess.check_output(['frida', '--version']).strip().decode('utf-8')
+        patcher.print_info('frida {0}'.format(frida_version))
+        patcher.print_done('apkpatcher {0}'.format(__version__))
+        return 1
 
     if args.verbosity:
         patcher.set_verbosity(int(args.verbosity))
     else:
         patcher.set_verbosity(patcher.VERBOSITY_HIGH)
 
     if args.update_gadgets:
@@ -1004,15 +1032,15 @@
 
     if not args.prevent_frida_gadget and not has_internet_permission:
         patcher.inject_permission_manifest(temporary_path, patcher.INTERNET_PERMISSION)
 
     if args.enable_user_certificates:
         patcher.enable_user_certificates(temporary_path)
 
-    if not args.prevent_frida_gadget:
+    if not args.prevent_frida_gadget and not args.lib:
         # START --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
         entrypoint_class = patcher.get_entrypoint_class_name(apk_file_path)
         entrypoint_smali_path = patcher.get_entrypoint_smali_path(temporary_path, entrypoint_class)
 
         patcher.insert_frida_loader(entrypoint_smali_path)
 
         if args.autoload_script or args.codeshare:
@@ -1032,14 +1060,28 @@
             patcher.insert_frida_lib(temporary_path, gadget_to_use,
                                      config_file_path=default_config_file, auto_load_script_path=script_file)
 
         else:
             patcher.insert_frida_lib(temporary_path, gadget_to_use)
         # END --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
 
+    elif args.lib:
+        lib_file = args.lib
+        if not os.path.isfile(lib_file):
+            patcher.print_warn('Library {0} was not found.'.format(lib_file))
+        lib_name, lib_ext = os.path.basename(lib_file).rsplit('.', 1)
+        lib_path = os.path.abspath(args.lib)
+        entrypoint_class = patcher.get_entrypoint_class_name(apk_file_path)
+
+        entrypoint_smali_path = patcher.get_entrypoint_smali_path(temporary_path, entrypoint_class)
+        recommended_gadget = patcher.get_recommended_gadget()
+        arch = patcher.get_arch_by_gadget(recommended_gadget)
+        patcher.insert_shared_lib(temporary_path, lib_path, lib_name + '.' + lib_ext, arch)
+        patcher.insert_frida_loader(entrypoint_smali_path, lib_name)
+
     if args.wait_before_repackage:
         patcher.print_info('Apkpatcher is waiting for your OK to repackage the apk...')
 
         answer = input(BColors.COLOR_BLUE + '[*] Are you ready? (y/N): ' + BColors.ENDC)
 
         while answer.lower() != 'y':
             answer = input(BColors.COLOR_BLUE + '[*] Are you ready? (y/N): ' + BColors.ENDC)
```

### Comparing `apkpatcher-cli-1.0.0/apkpatcher_cli.egg-info/PKG-INFO` & `apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.0.0
+Version: 1.1.0
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.0.0/setup.py` & `apkpatcher-cli-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
    name='apkpatcher-cli',
-   version='1.0.0',
+   version='1.1.0',
    description='Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher',
    author='Marcel Alexandru Nitan',
    author_email='nitan.marcel@gmail.com',
    url='https://github.com/nitanmarcel/apkpatcher',
    keywords=['FRIDA', 'APK'],
    scripts=['apkpatcher'],
    install_requires=[
```

