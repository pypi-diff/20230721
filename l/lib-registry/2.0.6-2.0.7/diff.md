# Comparing `tmp/lib_registry-2.0.6.tar.gz` & `tmp/lib_registry-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lib_registry-2.0.6.tar", last modified: Fri Oct  9 15:47:26 2020, max compression
+gzip compressed data, was "dist/lib_registry-2.0.7.tar", last modified: Sat Oct 10 20:15:09 2020, max compression
```

## Comparing `lib_registry-2.0.6.tar` & `lib_registry-2.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 15:47:26.000000 lib_registry-2.0.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4217 2020-10-09 15:46:33.000000 lib_registry-2.0.6/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16440 2020-10-09 15:46:33.000000 lib_registry-2.0.6/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 15:47:26.000000 lib_registry-2.0.6/lib_registry.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 15:47:25.000000 lib_registry-2.0.6/lib_registry.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      514 2020-10-09 15:47:25.000000 lib_registry-2.0.6/lib_registry.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-10-09 15:47:25.000000 lib_registry-2.0.6/lib_registry.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-10-09 15:47:25.000000 lib_registry-2.0.6/lib_registry.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 15:47:25.000000 lib_registry-2.0.6/lib_registry.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-10-09 15:47:25.000000 lib_registry-2.0.6/lib_registry.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    21227 2020-10-09 15:47:25.000000 lib_registry-2.0.6/lib_registry.egg-info/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 15:47:26.000000 lib_registry-2.0.6/lib_registry/
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-10-09 15:46:33.000000 lib_registry-2.0.6/lib_registry/types_custom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      537 2020-10-09 15:46:33.000000 lib_registry-2.0.6/lib_registry/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55409 2020-10-09 15:46:33.000000 lib_registry-2.0.6/lib_registry/lib_registry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-09 15:46:33.000000 lib_registry-2.0.6/lib_registry/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2020-10-09 15:46:33.000000 lib_registry-2.0.6/lib_registry/lib_registry_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-10-09 15:46:33.000000 lib_registry-2.0.6/lib_registry/__init__conf__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      270 2020-10-09 15:46:33.000000 lib_registry-2.0.6/lib_registry/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21227 2020-10-09 15:47:26.000000 lib_registry-2.0.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-10-09 15:46:33.000000 lib_registry-2.0.6/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-10-09 15:47:26.000000 lib_registry-2.0.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-10-09 15:46:33.000000 lib_registry-2.0.6/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1762 2020-10-09 15:46:33.000000 lib_registry-2.0.6/CHANGES.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-10 20:15:09.000000 lib_registry-2.0.7/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4217 2020-10-10 20:14:16.000000 lib_registry-2.0.7/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16484 2020-10-10 20:14:16.000000 lib_registry-2.0.7/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-10 20:15:08.000000 lib_registry-2.0.7/lib_registry.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      514 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21303 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry.egg-info/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-10 20:15:09.000000 lib_registry-2.0.7/lib_registry/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-10-10 20:14:16.000000 lib_registry-2.0.7/lib_registry/types_custom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      537 2020-10-10 20:14:16.000000 lib_registry-2.0.7/lib_registry/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55473 2020-10-10 20:14:16.000000 lib_registry-2.0.7/lib_registry/lib_registry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-10 20:14:16.000000 lib_registry-2.0.7/lib_registry/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2020-10-10 20:14:16.000000 lib_registry-2.0.7/lib_registry/lib_registry_cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      530 2020-10-10 20:14:16.000000 lib_registry-2.0.7/lib_registry/__init__conf__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      270 2020-10-10 20:14:16.000000 lib_registry-2.0.7/lib_registry/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21303 2020-10-10 20:15:09.000000 lib_registry-2.0.7/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-10-10 20:14:16.000000 lib_registry-2.0.7/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-10-10 20:15:09.000000 lib_registry-2.0.7/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-10-10 20:14:16.000000 lib_registry-2.0.7/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1806 2020-10-10 20:14:16.000000 lib_registry-2.0.7/CHANGES.rst
```

### Comparing `lib_registry-2.0.6/setup.py` & `lib_registry-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 if is_travis_deploy() and is_tagged_commit():
     setup_requires = strip_links_from_required(setup_requires)
     tests_require = strip_links_from_required(tests_require)
     install_requires = strip_links_from_required(install_requires)
 
 setup_kwargs: Dict[str, Any] = dict()
 setup_kwargs["name"] = "lib_registry"
-setup_kwargs["version"] = "v2.0.6"
+setup_kwargs["version"] = "v2.0.7"
 setup_kwargs["url"] = "https://github.com/bitranox/lib_registry"
 setup_kwargs["packages"] = find_packages()
 setup_kwargs["package_data"] = {"lib_registry": ["py.typed", "*.pyi", "__init__.pyi"]}
 setup_kwargs[
     "description"
 ] = "a more pythonic way to access the windows registry as winreg"
 setup_kwargs["long_description"] = long_description
```

### Comparing `lib_registry-2.0.6/README.rst` & `lib_registry-2.0.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_registry
 ============
 
 
-Version v2.0.6 as of 2020-10-09 see `Changelog`_
+Version v2.0.7 as of 2020-10-10 see `Changelog`_
 
 |travis_build| |license| |jupyter| |pypi|
 
 |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 .. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_registry/master.svg
@@ -433,14 +433,18 @@
 
 tasks:
     - test if caching of handles make sense, especially on network
     - documentation update
     - pathlib-like Interface
     - jupyter notebook update
 
+v2.0.7
+--------
+2020-10-10: fix minor bugs
+
 v2.0.6
 --------
 2020-10-09: service release
     - update travis build matrix for linux 3.9-dev
     - update travis build matrix (paths) for windows 3.9 / 3.10
 
 v2.0.5
```

### Comparing `lib_registry-2.0.6/lib_registry.egg-info/SOURCES.txt` & `lib_registry-2.0.7/lib_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_registry-2.0.6/lib_registry.egg-info/PKG-INFO` & `lib_registry-2.0.7/lib_registry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lib-registry
-Version: 2.0.6
+Version: 2.0.7
 Summary: a more pythonic way to access the windows registry as winreg
 Home-page: https://github.com/bitranox/lib_registry
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 License: UNKNOWN
 Description: lib_registry
         ============
         
         
-        Version v2.0.6 as of 2020-10-09 see `Changelog`_
+        Version v2.0.7 as of 2020-10-10 see `Changelog`_
         
         |travis_build| |license| |jupyter| |pypi|
         
         |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
         
         
         .. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_registry/master.svg
@@ -441,14 +441,18 @@
         
         tasks:
             - test if caching of handles make sense, especially on network
             - documentation update
             - pathlib-like Interface
             - jupyter notebook update
         
+        v2.0.7
+        --------
+        2020-10-10: fix minor bugs
+        
         v2.0.6
         --------
         2020-10-09: service release
             - update travis build matrix for linux 3.9-dev
             - update travis build matrix (paths) for windows 3.9 / 3.10
         
         v2.0.5
```

### Comparing `lib_registry-2.0.6/lib_registry/helpers.py` & `lib_registry-2.0.7/lib_registry/helpers.py`

 * *Files identical despite different names*

### Comparing `lib_registry-2.0.6/lib_registry/lib_registry.py` & `lib_registry-2.0.7/lib_registry/lib_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     from types_custom import *      # type: ignore      # pragma: no cover
 
 if is_platform_windows:
     import winreg                           # type: ignore
 else:
     import fake_winreg as winreg            # type: ignore
     # an empty Registry at the Moment
-    fake_registry = winreg.fake_reg_tools.get_minimal_windows_testregistry()
-    winreg.load_fake_registry(fake_registry)
+    fake_registry = winreg.fake_reg_tools.get_minimal_windows_testregistry()    # type: ignore
+    winreg.load_fake_registry(fake_registry)                                    # type: ignore
 
 
 main_key_hashed_by_name: Dict[str, int] = \
     {
         'hkey_classes_root': winreg.HKEY_CLASSES_ROOT,
         'hkcr': winreg.HKEY_CLASSES_ROOT,
         'hkey_current_config': winreg.HKEY_CURRENT_CONFIG,
@@ -307,25 +307,32 @@
             if hive_key in self.reg_hive_connections:
                 hive_handle = self.reg_hive_connections[hive_key]
             else:
                 hive_handle = winreg.ConnectRegistry(computer_name, hive_key)
                 self.reg_hive_connections[hive_key] = hive_handle
                 self._is_computer_name_set = True
             return hive_handle
+
         except FileNotFoundError as e_fnf:
             if hasattr(e_fnf, 'winerror') and e_fnf.winerror == 53:    # type: ignore
-                raise RegistryNetworkConnectionError('The network path to "{}" was not found'.format(computer_name))
+                raise RegistryNetworkConnectionError(f'The network path to "{computer_name}" was not found')
+            else:
+                raise RegistryConnectionError('unknown error connecting to registry')
 
         except OSError as e_os:
             if hasattr(e_os, 'winerror'):
                 if e_os.winerror == 1707:       # type: ignore
                     # OSError: [WinError 1707] The network address is invalid
-                    raise RegistryNetworkConnectionError('The network address "{}" is invalid'.format(computer_name))
+                    raise RegistryNetworkConnectionError(f'The network address "{computer_name}" is invalid')
                 elif e_os.winerror == 6:        # type: ignore
-                    raise RegistryHKeyError('invalid KEY: "{}"'.format(key))
+                    raise RegistryHKeyError(f'invalid KEY: "{key}"')
+            else:
+                raise RegistryConnectionError('unknown error connecting to registry')
+
+        assert False
 
     def _open_key(self, key: Union[str, int], sub_key: str = '', access: int = winreg.KEY_READ) -> winreg.HKEYType:
         """
         Opens a registry key and returns a reg_handle to it.
         Openend Keys with the Access Rights are stored in a Hash Table and Reused if possible.
         The user should not need to use this method - keys are opened , reused and closed automatically
 
@@ -363,15 +370,15 @@
         else:
             reg_handle = self._reg_connect(hive_key)
             try:
                 key_handle = winreg.OpenKey(reg_handle, hive_sub_key, 0, access)
                 self.reg_key_handles[(hive_key, hive_sub_key, access)] = key_handle
             except FileNotFoundError:
                 key_str = get_key_as_string(key, sub_key)
-                raise RegistryKeyNotFoundError('registry key "{}" not found'.format(key_str))
+                raise RegistryKeyNotFoundError(f'registry key "{key_str}" not found')
         return key_handle
 
     # create_key{{{
     def create_key(self, key: Union[str, int], sub_key: str = '', exist_ok: bool = True, parents: bool = False) -> winreg.HKEYType:
         """
         Creates a Key, and returns a Handle to the new key
 
@@ -431,24 +438,24 @@
         """
         # create_key}}}
 
         hive_key, hive_sub_key = resolve_key(key, sub_key)
         _key_exists = self.key_exist(hive_key, hive_sub_key)
         if (not exist_ok) and _key_exists:
             key_string = get_key_as_string(hive_key, hive_sub_key)
-            raise RegistryKeyCreateError('can not create key, it already exists: {key_string}'.format(key_string=key_string))
+            raise RegistryKeyCreateError(f'can not create key, it already exists: {key_string}')
         elif _key_exists:
             key_handle = self._open_key(hive_key, hive_sub_key, winreg.KEY_ALL_ACCESS)
             return key_handle
 
         if not parents:
             hive_sub_key_parent = '\\'.join(hive_sub_key.split('\\')[:-1])
             if not self.key_exist(hive_key, hive_sub_key_parent):
                 key_str = get_key_as_string(hive_key, hive_sub_key)
-                raise RegistryKeyCreateError('can not create key, the parent key to "{key_str}" does not exist'.format(key_str=key_str))
+                raise RegistryKeyCreateError(f'can not create key, the parent key to "{key_str}" does not exist')
 
         new_key_handle = winreg.CreateKey(hive_key, hive_sub_key)
         self.reg_key_handles[(hive_key, hive_sub_key, winreg.KEY_ALL_ACCESS)] = new_key_handle
 
         return new_key_handle
 
     # delete_key{{{
@@ -518,20 +525,20 @@
         _key_exists = self.key_exist(hive_key, hive_sub_key)
 
         if not _key_exists:
             if missing_ok:
                 return
             else:
                 key_str = get_key_as_string(key, sub_key)
-                raise RegistryKeyDeleteError('can not delete key none existing key "{key_str}"'.format(key_str=key_str))
+                raise RegistryKeyDeleteError(f'can not delete key none existing key "{key_str}"')
 
         if self.has_subkeys(hive_key, hive_sub_key):
             if not delete_subkeys:
                 key_str = get_key_as_string(key, sub_key)
-                raise RegistryKeyDeleteError('can not delete none empty key "{key_str}"'.format(key_str=key_str))
+                raise RegistryKeyDeleteError(f'can not delete none empty key "{key_str}"')
             else:
                 for sub_key in self.subkeys(hive_key, hive_sub_key):
                     hive_subkey_child = '\\'.join([hive_sub_key, sub_key])
                     self.delete_key(hive_key, hive_subkey_child, missing_ok=True, delete_subkeys=True)
 
         # we know only two access methods - KEY_READ and KEY_ALL_ACCESS
         # we close the handles before we delete the key
@@ -900,15 +907,15 @@
 
         key_handle = self._open_key(key)
         try:
             reg_value, reg_type = winreg.QueryValueEx(key_handle, value_name)
             return reg_value, reg_type
         except FileNotFoundError:
             key_str = get_key_as_string(key)
-            raise RegistryValueNotFoundError('value "{}" not found in key "{}"'.format(value_name, key_str))
+            raise RegistryValueNotFoundError(f'value "{value_name}" not found in key "{key_str}"')
 
     def username_from_sid(self, sid: str) -> str:
         """
 
         >>> # Setup
         >>> l_users = list()
         >>> registry = Registry()
@@ -929,17 +936,17 @@
                 return username
         except RegistryError:
             pass
 
         try:
             username = self._get_username_from_profile_list(sid)
         except RegistryError:
-            raise RegistryError('can not determine User for SID "{}"'.format(sid))
+            raise RegistryError(f'can not determine User for SID "{sid}"')
         if not username:
-            raise RegistryError('can not determine User for SID "{}"'.format(sid))
+            raise RegistryError(f'can not determine User for SID "{sid}"')
         return username
 
     def _get_username_from_profile_list(self, sid: str) -> str:
         """
         gets the username by SID from the Profile Image Path
 
         >>> # Setup
@@ -955,15 +962,15 @@
         >>> # Test Key not Found
         >>> registry._get_username_from_profile_list('unknown')
         Traceback (most recent call last):
             ...
         lib_registry.RegistryKeyNotFoundError: registry key "...unknown" not found
 
         """
-        value, value_type = self.get_value_ex(r'HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\ProfileList\{}'.format(sid), 'ProfileImagePath')
+        value, value_type = self.get_value_ex(fr'HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\ProfileList\{sid}', 'ProfileImagePath')
         assert isinstance(value, str)
         username = pathlib.PureWindowsPath(value).name
         return username
 
     def _get_username_from_volatile_environment(self, sid: str) -> str:
         """
         gets the username by SID from the Volatile Environment
@@ -979,15 +986,15 @@
         ...         except RegistryKeyNotFoundError:
         ...             pass
         ... else:
         ...   print("'pass'")
         '...'
 
         """
-        value, value_type = self.get_value_ex(r'HKEY_USERS\{}\Volatile Environment'.format(sid), 'USERNAME')
+        value, value_type = self.get_value_ex(fr'HKEY_USERS\{sid}\Volatile Environment', 'USERNAME')
         assert isinstance(value, str)
         return str(value)
 
     def set_value(self, key: Union[str, int], value_name: Optional[str], value: RegData, value_type: Optional[int] = None) -> None:
         """
         Stores data in the value field of an open registry key.
         key is a key by string, or one of the predefined HKEY_* constants.
@@ -1074,22 +1081,22 @@
             elif isinstance(value, str):
                 value_type = winreg.REG_SZ
             else:
                 value_type = winreg.REG_BINARY
 
         key_handle = self._open_key(key, access=winreg.KEY_ALL_ACCESS)
         try:
-            winreg.SetValueEx(key_handle, value_name, 0, value_type, value)
+            winreg.SetValueEx(key_handle, value_name, 0, value_type, value)     # type: ignore
         except Exception:       # ToDo: narrow down
             # different Errors can occur here :
             # TypeError: Objects of type 'str' can not be used as binary registry values (if try to write string to REG_NONE type)
             # others to explore ...
             key_str = get_key_as_string(key)
             value_type_str = get_value_type_as_string(value_type)
-            raise RegistryValueWriteError('can not write data to key "{}", value_name "{}", value_type "{}"'.format(key_str, value_name, value_type_str))
+            raise RegistryValueWriteError(f'can not write data to key "{key_str}", value_name "{value_name}", value_type "{value_type_str}"')
 
     def delete_value(self, key: Union[str, int], value_name: Optional[str]) -> None:
         """
         deletes the value field of an open registry key, if value_name == '' or 'None',
         then delete the default value of the key
 
 
@@ -1131,15 +1138,15 @@
 
         key_handle = self._open_key(key, access=winreg.KEY_ALL_ACCESS)
         try:
             winreg.DeleteValue(key_handle, value_name)
         except FileNotFoundError as e:
             if hasattr(e, 'winerror') and e.winerror == 2:  # type: ignore
                 key_str = get_key_as_string(key)
-                raise RegistryValueDeleteError('can not delete value "{}" from key "{}"'.format(value_name, key_str))
+                raise RegistryValueDeleteError(f'can not delete value "{value_name}" from key "{key_str}"')
             else:
                 raise e
 
 
 def get_value_type_as_string(value_type: int) -> str:
     """
     Return the value type as string
@@ -1203,15 +1210,15 @@
         if sub_key:
             sub_key = '\\'.join([key_without_hive, sub_key])
         else:
             sub_key = key_without_hive
     else:
         hive_key = key
         if hive_key not in hive_names_hashed_by_int:
-            raise RegistryHKeyError('invalid HIVE KEY: "{hive_key}"'.format(hive_key=hive_key))
+            raise RegistryHKeyError(f'invalid HIVE KEY: "{hive_key}"')
     return hive_key, sub_key
 
 
 def get_hkey_int(key_name: str) -> int:
     """
     gets the root hive key from a key_name, containing short or long form, not case sensitive
 
@@ -1228,15 +1235,15 @@
     """
     main_key_name = helpers.get_first_part_of_the_key(key_name)
     main_key_name_lower = main_key_name.lower()
     if main_key_name_lower in main_key_hashed_by_name:
         main_key = int(main_key_hashed_by_name[main_key_name_lower])
         return main_key
     else:
-        raise RegistryHKeyError('invalid KEY: "{main_key_name}"'.format(main_key_name=main_key_name))
+        raise RegistryHKeyError(f'invalid KEY: "{main_key_name}"')
 
 
 def remove_hive_from_key_str_if_present(key_name: str) -> str:
     """
     >>> # DONE #3
     >>> remove_hive_from_key_str_if_present(r'HKEY_LOCAL_MACHINE\\SOFTWARE\\Microsoft')
     'SOFTWARE\\\\Microsoft'
```

### Comparing `lib_registry-2.0.6/lib_registry/lib_registry_cli.py` & `lib_registry-2.0.7/lib_registry/lib_registry_cli.py`

 * *Files identical despite different names*

### Comparing `lib_registry-2.0.6/lib_registry/__init__conf__.py` & `lib_registry-2.0.7/lib_registry/__init__conf__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 name = 'lib_registry'
 title = 'a more pythonic way to access the windows registry as winreg'
-version = 'v2.0.6'
+version = 'v2.0.7'
 url = 'https://github.com/bitranox/lib_registry'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_registry'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_registry:
 
     a more pythonic way to access the windows registry as winreg
 
-    Version : v2.0.6
+    Version : v2.0.7
     Url     : https://github.com/bitranox/lib_registry
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_registry-2.0.6/PKG-INFO` & `lib_registry-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lib_registry
-Version: 2.0.6
+Version: 2.0.7
 Summary: a more pythonic way to access the windows registry as winreg
 Home-page: https://github.com/bitranox/lib_registry
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 License: UNKNOWN
 Description: lib_registry
         ============
         
         
-        Version v2.0.6 as of 2020-10-09 see `Changelog`_
+        Version v2.0.7 as of 2020-10-10 see `Changelog`_
         
         |travis_build| |license| |jupyter| |pypi|
         
         |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
         
         
         .. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_registry/master.svg
@@ -441,14 +441,18 @@
         
         tasks:
             - test if caching of handles make sense, especially on network
             - documentation update
             - pathlib-like Interface
             - jupyter notebook update
         
+        v2.0.7
+        --------
+        2020-10-10: fix minor bugs
+        
         v2.0.6
         --------
         2020-10-09: service release
             - update travis build matrix for linux 3.9-dev
             - update travis build matrix (paths) for windows 3.9 / 3.10
         
         v2.0.5
```

### Comparing `lib_registry-2.0.6/setup.cfg` & `lib_registry-2.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `lib_registry-2.0.6/CHANGES.rst` & `lib_registry-2.0.7/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 tasks:
     - test if caching of handles make sense, especially on network
     - documentation update
     - pathlib-like Interface
     - jupyter notebook update
 
+v2.0.7
+--------
+2020-10-10: fix minor bugs
+
 v2.0.6
 --------
 2020-10-09: service release
     - update travis build matrix for linux 3.9-dev
     - update travis build matrix (paths) for windows 3.9 / 3.10
 
 v2.0.5
```

