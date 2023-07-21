# Comparing `tmp/arcor2_build-1.0.2.tar.gz` & `tmp/arcor2_build-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_build-1.0.2.tar", last modified: Tue Apr  4 13:33:54 2023, max compression
+gzip compressed data, was "arcor2_build-1.1.0.tar", last modified: Thu Jul 20 11:09:54 2023, max compression
```

## Comparing `arcor2_build-1.0.2.tar` & `arcor2_build-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.558016 arcor2_build-1.0.2/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     6290 2023-04-04 13:33:54.558016 arcor2_build-1.0.2/PKG-INFO
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.558016 arcor2_build-1.0.2/arcor2_build/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/VERSION
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       96 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/py.typed
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.558016 arcor2_build-1.0.2/arcor2_build/scripts/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/scripts/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    21125 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/scripts/build.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.558016 arcor2_build-1.0.2/arcor2_build/source/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/source/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    10214 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/source/logic.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      918 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/source/object_types.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    18019 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build/source/utils.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-04 13:33:54.558016 arcor2_build-1.0.2/arcor2_build.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     6290 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      556 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       65 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build.egg-info/entry_points.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      172 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       13 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/arcor2_build.egg-info/top_level.txt
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      822 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/backend_shim.py
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-04-04 13:33:54.558016 arcor2_build-1.0.2/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     7209 2023-04-04 13:33:54.000000 arcor2_build-1.0.2/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.586951 arcor2_build-1.1.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     7020 2023-07-20 11:09:54.582951 arcor2_build-1.1.0/PKG-INFO
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.582951 arcor2_build-1.1.0/arcor2_build/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/VERSION
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       96 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/py.typed
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.582951 arcor2_build-1.1.0/arcor2_build/scripts/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/scripts/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    22122 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/scripts/build.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.582951 arcor2_build-1.1.0/arcor2_build/source/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/source/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    10300 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/source/logic.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      918 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/source/object_types.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    17825 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/source/python_to_json.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    19211 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build/source/utils.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.582951 arcor2_build-1.1.0/arcor2_build.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     7020 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      594 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       65 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      172 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       13 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/arcor2_build.egg-info/top_level.txt
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      822 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/backend_shim.py
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-20 11:09:54.586951 arcor2_build-1.1.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     7939 2023-07-20 11:09:54.000000 arcor2_build-1.1.0/setup.py
```

### Comparing `arcor2_build-1.0.2/PKG-INFO` & `arcor2_build-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2_build
-Version: 1.0.2
+Version: 1.1.0
 Summary: ARCOR2 Build
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -24,14 +24,31 @@
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project service.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 - `ARCOR2_PROJECT_PATH=""` - can be set to an arbitrary value, not actually used.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Decompiler
+  - Possibility to decompile script from imported execution package and then update of project data. 
+  - Decompiler has also detection of unsupported operations, syntax and semantic errors.
+  - Commands that can be decompiled:
+    - Object with method which can have many outputs, parameters in method can be:
+      - constant
+      - variable which is result of method
+      - project parameter
+      - value of ActionPoint
+      - attribute of class
+    - Conditions: alone "if" or "if" continued many "elif",  condition must be in form `if "variable" == "constant":`.
+    - Command "Continue" if is some command after command "continue" on same level it will be not compiled.
+
 ## [1.0.2] - 2023-04-04
 
 ### Fixed
 
 - Fix of the fix (from the previous release).
 - Side effect is that it is now necessary to set `ARCOR2_PROJECT_PATH` (can be set to an arbitrary value).
```

### Comparing `arcor2_build-1.0.2/arcor2_build/scripts/build.py` & `arcor2_build-1.1.0/arcor2_build/scripts/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from arcor2.logging import get_logger
 from arcor2.object_types.abstract import Generic
 from arcor2.object_types.utils import base_from_source, built_in_types_names, prepare_object_types_dir
 from arcor2.parameter_plugins.base import TypesDict
 from arcor2.source import SourceException
 from arcor2.source.utils import parse
 from arcor2_build.source.logic import program_src
+from arcor2_build.source.python_to_json import python_to_json
 from arcor2_build.source.utils import global_action_points_class
 from arcor2_build_data import DEPENDENCIES, SERVICE_NAME, URL, ImportResult
 from arcor2_build_data.exceptions import Conflict, InvalidPackage, InvalidProject, NotFound, WebApiError
 
 OBJECT_TYPE_MODULE = "arcor2_object_types"
 
 original_sys_path = list(sys.path)
@@ -320,14 +321,20 @@
               description: Replace all existing project sources with new ones.
             - in: query
               name: overwriteCollisionModels
               schema:
                 type: boolean
                 default: false
               description: Replace existing collision models with new ones for specified project.
+            - in: query
+              name: updateProjectFromScript
+              schema:
+                type: boolean
+                default: false
+              description: Compile script and apply changes to the project.
       requestBody:
               content:
                 multipart/form-data:
                   schema:
                     type: object
                     required:
                         - executionPackage
@@ -352,16 +359,18 @@
     file = request.files["executionPackage"]
 
     overwrite_scene = request.args.get("overwriteScene", default="false") == "true"
     overwrite_project = request.args.get("overwriteProject", default="false") == "true"
     overwrite_object_types = request.args.get("overwriteObjectTypes", default="false") == "true"
     overwrite_project_sources = request.args.get("overwriteProjectSources", default="false") == "true"
     overwrite_collision_models = request.args.get("overwriteCollisionModels", default="false") == "true"
+    update_project_from_script = request.args.get("updateProjectFromScript", default="false") == "true"
 
     objects: dict[str, ObjectType] = {}
+    object_type: dict[str, type[Generic]] = {}
     models: dict[str, Models] = {}
 
     """
     1) get and validate all data from zip
     2) check what is already on the Project service
     3) do updates
     """
@@ -410,14 +419,15 @@
                     raise InvalidPackage(f"Invalid code of the {obj_type_name} object type.")
 
                 # TODO fill in OT description (is it used somewhere?)
                 objects[obj_type_name] = ObjectType(obj_type_name, obj_type_src)
                 get_base_from_imported_package(objects[obj_type_name], objects, zip_file, tmp_dir, ast)
 
                 type_def = save_and_import_type_def(obj_type_src, obj_type_name, Generic, tmp_dir, OBJECT_TYPE_MODULE)
+                object_type[scene_obj.name] = type_def
 
                 assert obj_type_name == type_def.__name__
 
                 if type_def.abstract():
                     raise InvalidPackage(f"Scene contains abstract object type: {obj_type_name}.")
 
         for obj_type in objects.values():  # handle models
@@ -449,14 +459,21 @@
                 raise NotFound("Could not find script.py.")
 
             try:
                 parse(script)
             except Arcor2Exception:
                 raise InvalidPackage("Invalid code of the main script.")
 
+        # case when preparing data from script to decompilation
+        if update_project_from_script:
+            try:
+                src = zip_file.read("script.py").decode("UTF-8")
+            except KeyError:
+                raise NotFound("Could not find script.py.")
+
     # check that we are not going to overwrite something
     if not overwrite_scene:
         try:
             ps_scene = ps.get_scene(scene.id)
         except ps.ProjectServiceException:
             pass
         else:
@@ -502,14 +519,19 @@
         for model in models.values():
             try:
                 if model != ps.get_model(model.id, model.type()):
                     raise Conflict("Collision model difference detected. Overwrite needed.")
             except ps.ProjectServiceException:
                 pass
 
+    if update_project_from_script:
+        logger.debug("Decompiling source...")
+        project = python_to_json(project, scene, src, object_type)
+        logger.debug("Decompile was successfull and project was overwritten")
+
     for model in models.values():
         ps.put_model(model)
 
     for obj_type in objects.values():
         ps.update_object_type(obj_type)
 
     ps.update_scene(scene)
```

### Comparing `arcor2_build-1.0.2/arcor2_build/source/logic.py` & `arcor2_build-1.1.0/arcor2_build/source/logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,17 @@
                 targets=[Name(id=param.name, ctx=Store())], value=aval, type_comment=None
             ),
         )
 
     if add_logic:
         add_logic_to_loop(type_defs, tree, scene, project)
 
-    return SCRIPT_HEADER + tree_to_str(tree)
+    Warning = '# Warning: making changes is only allowed in "while" \n \n'
+
+    return SCRIPT_HEADER + Warning + tree_to_str(tree)
 
 
 Container = FunctionDef | If | While  # TODO remove While
 
 
 def add_logic_to_loop(type_defs: TypesDict, tree: Module, scene: CScene, project: CProject) -> None:
     added_actions: set[str] = set()
```

### Comparing `arcor2_build-1.0.2/arcor2_build/source/object_types.py` & `arcor2_build-1.1.0/arcor2_build/source/object_types.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.0.2/arcor2_build/source/utils.py` & `arcor2_build-1.1.0/arcor2_build/source/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 from ast import (
+    AST,
     AnnAssign,
     Assign,
     Attribute,
     Call,
     ClassDef,
     Compare,
     Eq,
@@ -12,14 +13,15 @@
     FunctionDef,
     If,
     ImportFrom,
     Load,
     Module,
     Name,
     NameConstant,
+    NodeVisitor,
     Pass,
     Return,
     Store,
     Str,
     Try,
     While,
     With,
@@ -35,14 +37,20 @@
 import arcor2.data.common
 from arcor2.cached import CachedProject
 from arcor2.data.common import ActionPoint, Pose, Position, ProjectRobotJoints
 from arcor2.exceptions import Arcor2Exception
 from arcor2.source import SourceException
 from arcor2.source.utils import add_import, find_function, tree_to_str
 
+
+class SpecialValues:
+    poses = "poses"
+    joints = "joints"
+
+
 RES_MODULE = "arcor2_runtime.resources"
 RES_CLS = "Resources"
 
 
 def main_loop(tree: Module) -> While:
     main = find_function("main", tree)
 
@@ -219,15 +227,15 @@
         for joints in project.ap_joints(ap.id):
             ap_joints_init_body.append(
                 Assign(
                     targets=[Attribute(value=Name(id="self", ctx=Load()), attr=f"_{joints.name}", ctx=Store())],
                     value=Call(
                         func=Attribute(
                             value=Attribute(value=Name(id="res", ctx=Load()), attr="project", ctx=Load()),
-                            attr="joints",
+                            attr=SpecialValues.joints,
                             ctx=Load(),
                         ),
                         args=[Str(s=joints.id, kind="")],
                         keywords=[],
                     ),
                     type_comment=None,
                 )
@@ -292,15 +300,15 @@
                     )
                 )
 
             tree.body.append(ap_joints_cls_def)
 
             ap_cls_body.append(
                 Assign(
-                    targets=[Attribute(value=Name(id="self", ctx=Load()), attr="joints", ctx=Store())],
+                    targets=[Attribute(value=Name(id="self", ctx=Load()), attr=SpecialValues.joints, ctx=Store())],
                     value=Call(
                         func=Name(id=f"{ap_type_name}Joints", ctx=Load()),
                         args=[Name(id="res", ctx=Load())],
                         keywords=[],
                     ),
                     type_comment=None,
                 )
@@ -384,15 +392,15 @@
                     )
                 )
 
             tree.body.append(ap_orientations_cls_def)
 
             ap_cls_body.append(
                 Assign(
-                    targets=[Attribute(value=Name(id="self", ctx=Load()), attr="poses", ctx=Store())],
+                    targets=[Attribute(value=Name(id="self", ctx=Load()), attr=SpecialValues.poses, ctx=Store())],
                     value=Call(
                         func=Name(id=f"{ap_type_name}Poses", ctx=Load()),
                         args=[Name(id="res", ctx=Load())],
                         keywords=[],
                     ),
                     type_comment=None,
                 )
@@ -508,7 +516,56 @@
     """
 
     for body_idx, body_item in reversed(list(enumerate(tree.body))):
         if isinstance(body_item, (Assign, AnnAssign)):
             return body_idx
 
     raise Arcor2Exception("Assign not found.")
+
+
+def find_While(tree: Module):
+    if tree.body == []:
+        return tree
+
+    class FindWhile(NodeVisitor):
+        def __init__(self) -> None:
+            self.While_node: While
+
+        def visit_While(self, node: While) -> None:
+            self.While_node = node
+            self.generic_visit(node)
+            return
+
+    ff = FindWhile()
+    ff.visit(tree)
+
+    return ff.While_node
+
+
+def find_Call(tree: Module | AST) -> Call:
+    class FindCall(NodeVisitor):
+        def __init__(self) -> None:
+            self.Call_node: Call
+
+        def visit_Call(self, node: Call) -> None:
+            self.Call_node = node
+            return
+
+    ff = FindCall()
+    ff.visit(tree)
+
+    return ff.Call_node
+
+
+def find_Compare(tree: Module | AST):
+    class FindCompare(NodeVisitor):
+        def __init__(self) -> None:
+            self.Compare_node: list[Compare] = []
+
+        def visit_Compare(self, node: Compare) -> None:
+            self.Compare_node.append(node)
+            return
+
+    ff = FindCompare()
+    ff.visit(tree)
+
+    return ff.Compare_node[0]
```

### Comparing `arcor2_build-1.0.2/arcor2_build.egg-info/PKG-INFO` & `arcor2_build-1.1.0/arcor2_build.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2-build
-Version: 1.0.2
+Version: 1.1.0
 Summary: ARCOR2 Build
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -24,14 +24,31 @@
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project service.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 - `ARCOR2_PROJECT_PATH=""` - can be set to an arbitrary value, not actually used.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Decompiler
+  - Possibility to decompile script from imported execution package and then update of project data. 
+  - Decompiler has also detection of unsupported operations, syntax and semantic errors.
+  - Commands that can be decompiled:
+    - Object with method which can have many outputs, parameters in method can be:
+      - constant
+      - variable which is result of method
+      - project parameter
+      - value of ActionPoint
+      - attribute of class
+    - Conditions: alone "if" or "if" continued many "elif",  condition must be in form `if "variable" == "constant":`.
+    - Command "Continue" if is some command after command "continue" on same level it will be not compiled.
+
 ## [1.0.2] - 2023-04-04
 
 ### Fixed
 
 - Fix of the fix (from the previous release).
 - Side effect is that it is now necessary to set `ARCOR2_PROJECT_PATH` (can be set to an arbitrary value).
```

### Comparing `arcor2_build-1.0.2/arcor2_build.egg-info/SOURCES.txt` & `arcor2_build-1.1.0/arcor2_build.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 arcor2_build.egg-info/requires.txt
 arcor2_build.egg-info/top_level.txt
 arcor2_build/scripts/__init__.py
 arcor2_build/scripts/build.py
 arcor2_build/source/__init__.py
 arcor2_build/source/logic.py
 arcor2_build/source/object_types.py
+arcor2_build/source/python_to_json.py
 arcor2_build/source/utils.py
```

### Comparing `arcor2_build-1.0.2/backend_shim.py` & `arcor2_build-1.1.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `arcor2_build-1.0.2/setup.py` & `arcor2_build-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             'arcor2_build = arcor2_build.scripts.build:main',
         ],
     },
     'install_requires': (
         'Flask~=2.2.3',
         'arcor2_build_data~=1.0.0',
         'arcor2_runtime~=1.0.0',
-        'arcor2~=1.0.0',
+        'arcor2~=1.1.0',
         'dataclasses-jsonschema[apispec,fast-dateparsing,fast-uuid,fast-validation]~=2.16.0',
         'pyhumps==3.8.0',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2_build
 
 ## Environment variables
@@ -40,14 +40,31 @@
 - `ARCOR2_REST_DEBUG=1` - may be used to debug problems related to communication with the Project service.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 - `ARCOR2_PROJECT_PATH=""` - can be set to an arbitrary value, not actually used.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2023-07-20
+
+### Added
+
+- Decompiler
+  - Possibility to decompile script from imported execution package and then update of project data. 
+  - Decompiler has also detection of unsupported operations, syntax and semantic errors.
+  - Commands that can be decompiled:
+    - Object with method which can have many outputs, parameters in method can be:
+      - constant
+      - variable which is result of method
+      - project parameter
+      - value of ActionPoint
+      - attribute of class
+    - Conditions: alone "if" or "if" continued many "elif",  condition must be in form `if "variable" == "constant":`.
+    - Command "Continue" if is some command after command "continue" on same level it will be not compiled.
+
 ## [1.0.2] - 2023-04-04
 
 ### Fixed
 
 - Fix of the fix (from the previous release).
 - Side effect is that it is now necessary to set `ARCOR2_PROJECT_PATH` (can be set to an arbitrary value).
 
@@ -246,9 +263,9 @@
     },
     'packages': (
         'arcor2_build',
         'arcor2_build.scripts',
         'arcor2_build.source',
     ),
     'python_requires': '==3.10.*',
-    'version': '1.0.2',
+    'version': '1.1.0',
 })
```

