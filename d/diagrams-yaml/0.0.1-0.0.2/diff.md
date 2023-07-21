# Comparing `tmp/diagrams-yaml-0.0.1.tar.gz` & `tmp/diagrams-yaml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagrams-yaml-0.0.1.tar", last modified: Fri Jul 21 10:49:46 2023, max compression
+gzip compressed data, was "diagrams-yaml-0.0.2.tar", last modified: Fri Jul 21 15:12:25 2023, max compression
```

## Comparing `diagrams-yaml-0.0.1.tar` & `diagrams-yaml-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 10:49:46.496010 diagrams-yaml-0.0.1/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        6 2023-07-21 10:32:27.000000 diagrams-yaml-0.0.1/.project-version
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-21 10:32:46.000000 diagrams-yaml-0.0.1/LICENSE
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       87 2023-07-21 10:33:03.000000 diagrams-yaml-0.0.1/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      801 2023-07-21 10:49:46.496061 diagrams-yaml-0.0.1/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-20 12:02:34.000000 diagrams-yaml-0.0.1/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 10:49:46.495199 diagrams-yaml-0.0.1/diagrams_yaml/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 08:47:14.000000 diagrams-yaml-0.0.1/diagrams_yaml/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4443 2023-07-21 10:30:44.000000 diagrams-yaml-0.0.1/diagrams_yaml/entrypoint.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      224 2023-07-21 10:15:57.000000 diagrams-yaml-0.0.1/diagrams_yaml/enums.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      781 2023-07-21 10:18:15.000000 diagrams-yaml-0.0.1/diagrams_yaml/resources.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      842 2023-07-21 10:15:30.000000 diagrams-yaml-0.0.1/diagrams_yaml/schema.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 10:49:46.495806 diagrams-yaml-0.0.1/diagrams_yaml.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      801 2023-07-21 10:49:46.000000 diagrams-yaml-0.0.1/diagrams_yaml.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      457 2023-07-21 10:49:46.000000 diagrams-yaml-0.0.1/diagrams_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-21 10:49:46.000000 diagrams-yaml-0.0.1/diagrams_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       71 2023-07-21 10:49:46.000000 diagrams-yaml-0.0.1/diagrams_yaml.egg-info/entry_points.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       47 2023-07-21 10:49:46.000000 diagrams-yaml-0.0.1/diagrams_yaml.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       14 2023-07-21 10:49:46.000000 diagrams-yaml-0.0.1/diagrams_yaml.egg-info/top_level.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      374 2023-07-21 10:31:27.000000 diagrams-yaml-0.0.1/pyproject.toml
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 10:49:46.495910 diagrams-yaml-0.0.1/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       47 2023-07-21 10:35:05.000000 diagrams-yaml-0.0.1/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      195 2023-07-21 10:49:46.496226 diagrams-yaml-0.0.1/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1460 2023-07-21 10:43:01.000000 diagrams-yaml-0.0.1/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653851 diagrams-yaml-0.0.2/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        6 2023-07-21 10:51:47.000000 diagrams-yaml-0.0.2/.project-version
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-21 10:32:46.000000 diagrams-yaml-0.0.2/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       87 2023-07-21 10:33:03.000000 diagrams-yaml-0.0.2/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4054 2023-07-21 15:12:25.653898 diagrams-yaml-0.0.2/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3237 2023-07-21 15:11:10.000000 diagrams-yaml-0.0.2/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653027 diagrams-yaml-0.0.2/diagrams_yaml/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 08:47:14.000000 diagrams-yaml-0.0.2/diagrams_yaml/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4528 2023-07-21 14:22:19.000000 diagrams-yaml-0.0.2/diagrams_yaml/entrypoint.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      206 2023-07-21 14:10:41.000000 diagrams-yaml-0.0.2/diagrams_yaml/enums.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      781 2023-07-21 10:18:15.000000 diagrams-yaml-0.0.2/diagrams_yaml/resources.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      842 2023-07-21 10:15:30.000000 diagrams-yaml-0.0.2/diagrams_yaml/schema.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653661 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4054 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      457 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       71 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       47 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       14 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/top_level.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      374 2023-07-21 10:31:27.000000 diagrams-yaml-0.0.2/pyproject.toml
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653762 diagrams-yaml-0.0.2/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       47 2023-07-21 10:35:05.000000 diagrams-yaml-0.0.2/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      195 2023-07-21 15:12:25.654069 diagrams-yaml-0.0.2/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1483 2023-07-21 15:06:40.000000 diagrams-yaml-0.0.2/setup.py
```

### Comparing `diagrams-yaml-0.0.1/LICENSE` & `diagrams-yaml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diagrams-yaml-0.0.1/diagrams_yaml/entrypoint.py` & `diagrams-yaml-0.0.2/diagrams_yaml/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,20 @@
 
     with open(yaml_file_path, 'r') as yaml_file:
         yaml_as_dict = yaml.safe_load(yaml_file)
 
     diagram_as_dict = yaml_as_dict.get('diagram')
     diagram = YamlDiagram(**diagram_as_dict)
 
-    with Diagram(diagram.name, show=diagram.show):
+    graph_attr = {
+        "layout": "osage"  # or ""
+    }
+
+
+    with Diagram(diagram.name, show=diagram.show, graph_attr=graph_attr):
         for resource in diagram.resources:
             process_resource(resource, 'diagram')
 
         for relationship in relationships:
             resource_from_instance = resources.get(relationship.from_)
             resource_to_instance = resources.get(relationship.to)
```

### Comparing `diagrams-yaml-0.0.1/diagrams_yaml/resources.py` & `diagrams-yaml-0.0.2/diagrams_yaml/resources.py`

 * *Files identical despite different names*

### Comparing `diagrams-yaml-0.0.1/diagrams_yaml/schema.py` & `diagrams-yaml-0.0.2/diagrams_yaml/schema.py`

 * *Files identical despite different names*

### Comparing `diagrams-yaml-0.0.1/setup.py` & `diagrams-yaml-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('.project-version', 'r') as project_version_file:
     project_version = project_version_file.read().strip()
 
 setup(
     version=project_version,
     name='diagrams-yaml',
-    description='Diagram as Code using YAML syntax for cloud system architectures',
+    description='Diagram as Code in a declarative way using YAML for drawing cloud system architectures.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/diagrams-yaml',
     project_urls={
         'Issue Tracker': 'https://github.com/dmytrostriletskyi/diagrams-yaml/issues',
         'Source Code': 'https://github.com/dmytrostriletskyi/diagrams-yaml',
         'Download': 'https://github.com/dmytrostriletskyi/diagrams-yaml/tags',
```

