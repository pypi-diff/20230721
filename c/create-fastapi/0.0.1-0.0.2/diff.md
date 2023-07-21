# Comparing `tmp/create_fastapi-0.0.1.tar.gz` & `tmp/create_fastapi-0.0.2.tar.gz`

## Comparing `create_fastapi-0.0.1.tar` & `create_fastapi-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/main.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/commands/ICommand.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/commands/__init__.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/commands/command_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/commands/impl/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/commands/impl/clone_git.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/commands/impl/dependency_installer.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/commands/impl/dir_creator.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/helpers/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/create-fastapi-app/helpers/logger.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/LICENSE
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 create_fastapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/main.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/commands/ICommand.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/commands/__init__.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/commands/command_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/commands/impl/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/commands/impl/clone_git.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/commands/impl/dependency_installer.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/commands/impl/dir_creator.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/helpers/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/create-fastapi-app/helpers/logger.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/LICENSE
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 create_fastapi-0.0.2/PKG-INFO
```

### Comparing `create_fastapi-0.0.1/create-fastapi-app/commands/command_builder.py` & `create_fastapi-0.0.2/create-fastapi-app/commands/command_builder.py`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.1/create-fastapi-app/commands/impl/clone_git.py` & `create_fastapi-0.0.2/create-fastapi-app/commands/impl/clone_git.py`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.1/create-fastapi-app/commands/impl/dependency_installer.py` & `create_fastapi-0.0.2/create-fastapi-app/commands/impl/dependency_installer.py`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.1/.gitignore` & `create_fastapi-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.1/LICENSE` & `create_fastapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `create_fastapi-0.0.1/pyproject.toml` & `create_fastapi-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 [project]
 name = "create-fastapi"
 description = "create-fastapi-app"
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.2"
 
 authors = [{ name = "Shahar Luftig", email = "shaharluftig@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 
 keywords = ["backend", "fastapi", "create-app", "create-fastapi-app","create-fatapi"]
 classifiers = [
@@ -28,7 +28,10 @@
     "Topic :: Scientific/Engineering",
 ]
 
 dependencies = ["typer~=0.9.0", "virtualenv~=20.24.1", "GitPython~=3.1.32"]
 
 [project.urls]
 "Homepage" = "https://github.com/shaharluftig/create-fastapi-app"
+
+[project.scripts]
+app = "main.py"
```

### Comparing `create_fastapi-0.0.1/PKG-INFO` & `create_fastapi-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-fastapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: create-fastapi-app
 Project-URL: Homepage, https://github.com/shaharluftig/create-fastapi-app
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

