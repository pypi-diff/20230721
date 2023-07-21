# Comparing `tmp/kuki-0.9.0.tar.gz` & `tmp/kuki-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.9.0.tar", last modified: Thu Jul 20 14:45:57 2023, max compression
+gzip compressed data, was "kuki-0.9.1.tar", last modified: Fri Jul 21 15:48:40 2023, max compression
```

## Comparing `kuki-0.9.0.tar` & `kuki-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-20 14:45:57.166676 kuki-0.9.0/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.0/LICENSE
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-20 14:45:57.166676 kuki-0.9.0/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      459 2023-07-14 14:43:34.000000 kuki-0.9.0/README.md
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-20 14:45:57.164676 kuki-0.9.0/kuki/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.0/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.0/kuki/config_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1579 2023-07-19 15:39:03.000000 kuki-0.9.0/kuki/kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.0/kuki/ktrl.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4281 2023-07-19 16:30:54.000000 kuki-0.9.0/kuki/ktrl_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4393 2023-07-20 14:44:00.000000 kuki-0.9.0/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3388 2023-07-15 14:00:40.000000 kuki-0.9.0/kuki/package_util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-20 14:45:57.165676 kuki-0.9.0/kuki/q/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.0/kuki/q/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.9.0/kuki/q/cli.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-15 09:03:13.000000 kuki-0.9.0/kuki/q/kest.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.0/kuki/q/ktrl.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1884 2023-07-15 13:50:35.000000 kuki-0.9.0/kuki/q/kuki.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2177 2023-07-03 12:47:22.000000 kuki-0.9.0/kuki/q/log.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.0/kuki/q/path.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    14046 2023-07-20 11:55:48.000000 kuki-0.9.0/kuki/registry_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.0/kuki/util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       22 2023-07-20 14:44:53.000000 kuki-0.9.0/kuki/version.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-20 14:45:57.165676 kuki-0.9.0/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-20 14:45:57.000000 kuki-0.9.0/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      570 2023-07-20 14:45:57.000000 kuki-0.9.0/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-20 14:45:57.000000 kuki-0.9.0/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-20 14:45:57.000000 kuki-0.9.0/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-20 14:45:57.000000 kuki-0.9.0/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-07-20 14:45:57.000000 kuki-0.9.0/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-20 14:45:57.000000 kuki-0.9.0/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      490 2023-07-20 14:45:57.166676 kuki-0.9.0/setup.cfg
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.0/setup.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-20 14:45:57.166676 kuki-0.9.0/test/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.0/test/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.0/test/conftest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.0/test/test_kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15620 2023-07-15 13:06:10.000000 kuki-0.9.0/test/test_kuki.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.747237 kuki-0.9.1/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.1/LICENSE
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-21 15:48:40.747237 kuki-0.9.1/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      459 2023-07-20 14:47:33.000000 kuki-0.9.1/README.md
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.745237 kuki-0.9.1/kuki/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.1/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.1/kuki/config_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1579 2023-07-19 15:39:03.000000 kuki-0.9.1/kuki/kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.1/kuki/ktrl.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4281 2023-07-19 16:30:54.000000 kuki-0.9.1/kuki/ktrl_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4403 2023-07-21 09:51:39.000000 kuki-0.9.1/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3774 2023-07-21 15:41:07.000000 kuki-0.9.1/kuki/package_util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.747237 kuki-0.9.1/kuki/q/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.1/kuki/q/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.9.1/kuki/q/cli.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-15 09:03:13.000000 kuki-0.9.1/kuki/q/kest.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.1/kuki/q/ktrl.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1898 2023-07-21 09:56:43.000000 kuki-0.9.1/kuki/q/kuki.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.1/kuki/q/log.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.1/kuki/q/path.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    14401 2023-07-21 15:19:15.000000 kuki-0.9.1/kuki/registry_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.1/kuki/util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.746237 kuki-0.9.1/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      470 2023-07-21 15:48:40.748237 kuki-0.9.1/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.1/setup.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.747237 kuki-0.9.1/test/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.1/test/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.1/test/conftest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.1/test/test_kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15810 2023-07-21 15:26:05.000000 kuki-0.9.1/test/test_kuki.py
```

### Comparing `kuki-0.9.0/LICENSE` & `kuki-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/PKG-INFO` & `kuki-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.0
+Version: 0.9.1
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## K Ultimate pacKage Installer
 
+Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
+
 ### Commands
 
 `kuki` includes a set of 3 commands
 
 - kuki: _K Ultimate pacKage Installer_, manage q/k packages
 - kest: _K tEST cli_, test q/k codes
 - ktrl: _K conTRoL cli_,control
 
 ### Registry Site
 
 `kuki` can publish and install packages from central registry site [kuki.ninja](https://kuki.ninja/), thanks to [verdaccio](https://verdaccio.org/)
 
-Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `kuki-0.9.0/kuki/config_util.py` & `kuki-0.9.1/kuki/config_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki/kest.py` & `kuki-0.9.1/kuki/kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki/ktrl.py` & `kuki-0.9.1/kuki/ktrl.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki/ktrl_util.py` & `kuki-0.9.1/kuki/ktrl_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki/kuki.py` & `kuki-0.9.1/kuki/kuki.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         proceed = input("Is this OK? (yes/no) ").strip()
         if proceed.lower() == "yes":
             registry_util.add_user(user, password, email)
         else:
             logger.info("Abort registering '{}'".format(user))
     elif args.login:
         user = input("Username: ")
-        password = input("Password: ")
+        password = getpass.getpass("Password: ")
         registry_util.login(user, password)
     elif args.search:
         registry_util.search_package(args.search)
     elif args.download:
         registry_util.download_entry(args.download)
     else:
         if args.globalMode:
```

### Comparing `kuki-0.9.0/kuki/package_util.py` & `kuki-0.9.1/kuki/package_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,47 +22,55 @@
     version: str
     description: str
     author: str
     git: str
     dependencies: Dict[str, str]
 
 
-def generate_json(name: str, description="", author="", git=""):
+def generate_json(name: str, description="", author="", git="", package_type="q"):
     if package_config_path.exists():
         overwrite = input("kuki.json already exists, overwrite: (yes/No) ").strip()
         if not overwrite or not overwrite.lower() in ["yes"]:
             return
     kuki: Kuki = {
         "name": name,
         "version": "0.0.1",
         "description": description,
         "author": author,
         "git": git,
+        "type": package_type,
         "dependencies": {},
     }
     kuki_json = json.dumps(kuki, indent=2)
     logger.info("About to write to {}".format(package_config_path))
     logger.info("\n" + kuki_json)
     proceed = input("Is this OK? (YES/no) ").strip()
     if not proceed or proceed.lower() == "yes":
         dump_kuki(kuki)
         readme_path.touch()
+        readme_path.write_text("# {name}\n\n- author: {author}\n- git: {git}\n".format(**kuki))
         src_path.mkdir(parents=True, exist_ok=True)
 
 
 def init():
     dir = os.path.basename(os.getcwd())
     package = input("package name: ({}) ".format(dir)).strip()
     if not package:
         package = dir
     description = input("description: ").strip()
     author = input("author: ").strip()
     git = input("git repository: ").strip()
+    package_type = input("package type: (q)").strip()
+    if not package_type:
+        package_type = "q"
+    if package_type not in ["q", "k", "k9"]:
+        logger.error("only support q, k, or k9 package type")
+        return
 
-    generate_json(package, description, author, git)
+    generate_json(package, description, author, git, package_type)
 
 
 def dump_kuki(kuki: Kuki):
     with open(package_config_path, "w") as file:
         file.write(json.dumps(kuki, indent=2))
```

### Comparing `kuki-0.9.0/kuki/q/cli.q` & `kuki-0.9.1/kuki/q/cli.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki/q/kest.q` & `kuki-0.9.1/kuki/q/kest.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki/q/kuki.q` & `kuki-0.9.1/kuki/q/kuki.q`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 .kuki.rootDir:{kukiRoot:getenv`KUKIPATH;$[count kukiRoot;kukiRoot;.kuki.joinPath[getenv`HOME;("kuki")]]}[];
 
 .kuki.getRealPath:{[path]
   first @[system;"realpath ", path;{'y, " - No such file or directory"}[;path]]
  };
 
-.kuki.appendDotQ:{ x,$[x like "*.q";"";".q"] };
+.kuki.appendDotQ:{ x,$[any x like/: ("*.q";"*.k");"";".q"] };
 
 .kuki.importModule:{[modulePath]
   realPath: .kuki.getRealPath modulePath;
   if[realPath in .kuki.importedModules;:(::)]
   system"l ", realPath;
   .kuki.importedModules,:realPath;
  };
```

### Comparing `kuki-0.9.0/kuki/q/log.q` & `kuki-0.9.1/kuki/q/log.q`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,22 @@
   .log.Info:.log.log["INFO "];
   .log.Warning:.log.log["WARN "];
   .log.Error:.log.log["ERROR"];
   .log.SetLogLevel .log.level;
  };
 
 .log.SetStdLogFile:{[filepath]
-  h:hopen filepath;
+  h:hopen hsym filepath;
   .log.stdHandle:h;
   .log.errHandle:h;
   .log.refreshLogMethod[];
  };
 
 .log.SetErrLogFile:{[filepath]
-  h:hopen filepath;
+  h:hopen hsym filepath;
   .log.errHandle:h;
   .log.refreshLogMethod[];
  };
 
 .log.SetConsoleSize:{[consoleSize]
   system"c ", " " sv string $[-6 -6h~type each consoleSize;consoleSize;0 0i] | system"c";
  };
```

### Comparing `kuki-0.9.0/kuki/q/path.q` & `kuki-0.9.1/kuki/q/path.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki/registry_util.py` & `kuki-0.9.1/kuki/registry_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 
 class Metadata(TypedDict):
     name: str
     version: str
     dist: any
     dependencies: any
+    type: str
 
 
 def load_global_index() -> Dict[str, package_util.Kuki]:
     if global_index_path.exists():
         with open(global_index_path, "r") as file:
             return json.load(file)
     else:
@@ -301,20 +302,33 @@
         package_util.dump_pkg_index(package_index)
         dump_global_index()
     except Exception as e:
         logger.error("failed to install packages with error: {}".format(e))
 
 
 def install_packages(pkgs: List[str], skip_updating_pkg_index=True, globalMode=False):
+    package_type = kuki_json.get("type", "q")
+
+    if package_type == "k":
+        allow_package_types = ["k"]
+    elif package_type == "k9":
+        allow_package_types = ["k9"]
+    else:
+        allow_package_types = ["q", "k"]
+
     for pkg in pkgs:
         if skip_updating_pkg_index:
             logger.info("install dependency package '{}'".format(pkg))
         else:
             logger.info("install package '{}'".format(pkg))
         metadata = get_metadata(pkg)
+
+        if not metadata.get("type") in allow_package_types and not globalMode:
+            logger.error("")
+
         name = metadata["name"]
         if not globalMode and name == kuki_json["name"]:
             logger.warning("shouldn't install itself, skip...")
             return
 
         version = metadata["version"]
         pkg_id = get_pkg_id(metadata)
```

### Comparing `kuki-0.9.0/kuki/util.py` & `kuki-0.9.1/kuki/util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/kuki.egg-info/PKG-INFO` & `kuki-0.9.1/kuki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.0
+Version: 0.9.1
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## K Ultimate pacKage Installer
 
+Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
+
 ### Commands
 
 `kuki` includes a set of 3 commands
 
 - kuki: _K Ultimate pacKage Installer_, manage q/k packages
 - kest: _K tEST cli_, test q/k codes
 - ktrl: _K conTRoL cli_,control
 
 ### Registry Site
 
 `kuki` can publish and install packages from central registry site [kuki.ninja](https://kuki.ninja/), thanks to [verdaccio](https://verdaccio.org/)
 
-Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `kuki-0.9.0/kuki.egg-info/SOURCES.txt` & `kuki-0.9.1/kuki.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 kuki/kest.py
 kuki/ktrl.py
 kuki/ktrl_util.py
 kuki/kuki.py
 kuki/package_util.py
 kuki/registry_util.py
 kuki/util.py
-kuki/version.py
 kuki.egg-info/PKG-INFO
 kuki.egg-info/SOURCES.txt
 kuki.egg-info/dependency_links.txt
 kuki.egg-info/entry_points.txt
 kuki.egg-info/not-zip-safe
 kuki.egg-info/requires.txt
 kuki.egg-info/top_level.txt
```

### Comparing `kuki-0.9.0/test/test_kest.py` & `kuki-0.9.1/test/test_kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.0/test/test_kuki.py` & `kuki-0.9.1/test/test_kuki.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,18 @@
 def test_adduser(monkeypatch: pytest.MonkeyPatch):
     responses.add(
         responses.PUT,
         registry_util.user_url + "test",
         json={"token": "7IForS1HdYwD7wgFxXGMTA=="},
         status=201,
     )
-    inputs = iter(["test", "password", "test@test.com", "yes"])
+    inputs = iter(["test", "test@test.com", "yes"])
+    password_inputs = iter(["password", "password"])
     monkeypatch.setattr("builtins.input", lambda _: next(inputs))
+    monkeypatch.setattr("getpass.getpass", lambda _: next(password_inputs))
     run_kuki("--adduser")
     assert config_util.load_config()["token"] == "7IForS1HdYwD7wgFxXGMTA=="
 
 
 @pytest.mark.parametrize(
     "command_params, expected_token, expected_registry",
     [
@@ -117,14 +119,15 @@
 def test_init(monkeypatch: pytest.MonkeyPatch):
     inputs = iter(
         [
             "dummy",
             "a dummy package",
             "Saitama",
             "https://github.com/saitama/dummy",
+            "q",
             "yes",
         ]
     )
     monkeypatch.setattr("builtins.input", lambda _: next(inputs))
     run_kuki("--init")
     kuki_json = package_util.load_kuki()
 
@@ -159,21 +162,18 @@
 def test_login(monkeypatch: pytest.MonkeyPatch):
     responses.add(
         responses.PUT,
         registry_util.user_url + "test",
         json={"token": "7IForS1HdYwD7wgFxXGMTA=="},
         status=201,
     )
-    inputs = iter(
-        [
-            "test",
-            "password",
-        ]
-    )
+    inputs = iter(["test"])
+    password_inputs = iter(["password"])
     monkeypatch.setattr("builtins.input", lambda _: next(inputs))
+    monkeypatch.setattr("getpass.getpass", lambda _: next(password_inputs))
     run_kuki("--login")
     assert config_util.load_config()["token"] == "7IForS1HdYwD7wgFxXGMTA=="
 
 
 @responses.activate
 def test_search():
     search_result = {
```

