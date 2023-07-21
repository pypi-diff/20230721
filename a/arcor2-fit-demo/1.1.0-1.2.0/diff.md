# Comparing `tmp/arcor2_fit_demo-1.1.0.tar.gz` & `tmp/arcor2_fit_demo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_fit_demo-1.1.0.tar", last modified: Mon Mar  6 12:57:30 2023, max compression
+gzip compressed data, was "arcor2_fit_demo-1.2.0.tar", last modified: Thu Jul 20 11:09:55 2023, max compression
```

## Comparing `arcor2_fit_demo-1.1.0.tar` & `arcor2_fit_demo-1.2.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.771087 arcor2_fit_demo-1.1.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     3114 2023-03-06 12:57:30.771087 arcor2_fit_demo-1.1.0/PKG-INFO
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.747086 arcor2_fit_demo-1.1.0/arcor2_fit_demo/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/VERSION
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      238 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/__init__.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.751087 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  4711017 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/conveyor_belt.fbx
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.755087 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    10856 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1.urdf
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.743086 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.759086 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/
--r--r--r--   0 zdenal    (1000) zdenal    (1000)   854819 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-2.dae
--r--r--r--   0 zdenal    (1000) zdenal    (1000)   900206 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-3.dae
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    32762 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-4.dae
--r--r--r--   0 zdenal    (1000) zdenal    (1000)   592601 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_base.dae
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  2349673 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_stand.dae
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)   317364 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_z-axis.dae
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.759086 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.743086 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.743086 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.743086 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.767087 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  1977859 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianBase.dae
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  1773998 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianGripper.dae
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  1903113 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink1.dae
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  1423857 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink2.dae
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  2233581 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink3.dae
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)   321500 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink4.dae
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)   248396 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianSuctionCup.dae
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     8700 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot_magician.xml
--r--r--r--   0 zdenal    (1000) zdenal    (1000)  2552395 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/kinect_azure.dae
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.771087 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      106 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5934 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/abstract_dobot.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2509 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/conveyor_belt.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      871 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/dobot_m1.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2239 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/dobot_magician.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      521 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/fit_common_mixin.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2630 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/kinect_azure.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/py.typed
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.771087 arcor2_fit_demo-1.1.0/arcor2_fit_demo/scripts/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/scripts/__init__.py
--rwxr-xr-x   0 zdenal    (1000) zdenal    (1000)     1230 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo/scripts/upload_objects.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-06 12:57:30.747086 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     3114 2023-03-06 12:57:30.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     1977 2023-03-06 12:57:30.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-03-06 12:57:30.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       95 2023-03-06 12:57:30.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/entry_points.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-03-06 12:57:30.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       28 2023-03-06 12:57:30.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       16 2023-03-06 12:57:30.000000 arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/top_level.txt
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      699 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/backend_shim.py
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-03-06 12:57:30.771087 arcor2_fit_demo-1.1.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5068 2023-03-06 12:57:28.000000 arcor2_fit_demo-1.1.0/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.954966 arcor2_fit_demo-1.2.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     3269 2023-07-20 11:09:55.954966 arcor2_fit_demo-1.2.0/PKG-INFO
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.934966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/VERSION
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      238 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/__init__.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.938966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  4711017 2023-07-20 07:23:50.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/conveyor_belt.fbx
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.938966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    10856 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1.urdf
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.930966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.946966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)   854819 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-2.dae
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)   900206 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-3.dae
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    32762 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-4.dae
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)   592601 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_base.dae
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  2349673 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_stand.dae
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)   317364 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_z-axis.dae
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.946966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.930966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.930966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.930966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.954966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  1977859 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianBase.dae
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  1773998 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianGripper.dae
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  1903113 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink1.dae
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  1423857 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink2.dae
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  2233581 2023-07-19 14:08:41.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink3.dae
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)   321500 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink4.dae
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)   248396 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianSuctionCup.dae
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     8700 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot_magician.xml
+-r--r--r--   0 zdenal    (1000) zdenal    (1000)  2552395 2023-07-20 07:23:50.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/kinect_azure.dae
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.954966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      106 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5934 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/abstract_dobot.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2509 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/conveyor_belt.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      871 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/dobot_m1.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2239 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/dobot_magician.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      521 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/fit_common_mixin.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/py.typed
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.954966 arcor2_fit_demo-1.2.0/arcor2_fit_demo/scripts/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/scripts/__init__.py
+-rwxr-xr-x   0 zdenal    (1000) zdenal    (1000)     1239 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo/scripts/upload_objects.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-07-20 11:09:55.934966 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     3269 2023-07-20 11:09:55.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     1932 2023-07-20 11:09:55.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:55.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       95 2023-07-20 11:09:55.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-07-20 11:09:55.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       46 2023-07-20 11:09:55.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       16 2023-07-20 11:09:55.000000 arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/top_level.txt
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      822 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/backend_shim.py
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-07-20 11:09:55.954966 arcor2_fit_demo-1.2.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     5241 2023-07-20 11:09:54.000000 arcor2_fit_demo-1.2.0/setup.py
```

### Comparing `arcor2_fit_demo-1.1.0/PKG-INFO` & `arcor2_fit_demo-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2_fit_demo
-Version: 1.1.0
+Version: 1.2.0
 Summary: ARCOR2 FIT Demo
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,15 +16,21 @@
 Description-Content-Type: text/markdown
 
 # arcor2_fit_demo
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.0.0] - 2023-03-06
+## [1.2.0] - 2023-07-20
+
+### Changed
+
+- `KinectAzure` ObjectType is now imported from `src/python/arcor2_kinect_azure_data/object_types/kinect_azure.py`.
+
+## [1.1.0] - 2023-03-07
 
 ### Changed
 
 - Compatibility with `arcor2_kinect_azure:0.6.0`.
 - Default url for Kinect.
 
 ## [1.0.0] - 2023-02-14
```

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/conveyor_belt.fbx` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/conveyor_belt.fbx`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1.urdf` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1.urdf`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-2.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-2.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-3.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-3.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-4.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_axis-4.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_base.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_base.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_stand.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_stand.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_z-axis.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-m1/dobot_m1_description/meshes/dobot_m1_z-axis.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianBase.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianBase.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianGripper.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianGripper.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink1.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink1.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink2.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink2.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink3.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink3.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink4.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianLink4.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianSuctionCup.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianSuctionCup.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/dobot-magician/dobot_magician.xml` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/dobot-magician/dobot_magician.xml`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/data/kinect_azure.dae` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/data/kinect_azure.dae`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/abstract_dobot.py` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/abstract_dobot.py`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/conveyor_belt.py` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/conveyor_belt.py`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/dobot_m1.py` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/dobot_m1.py`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/dobot_magician.py` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/dobot_magician.py`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/object_types/fit_common_mixin.py` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/object_types/fit_common_mixin.py`

 * *Files identical despite different names*

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo/scripts/upload_objects.py` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo/scripts/upload_objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from arcor2.object_types.upload import Urdf, upload_def, upload_whatever
 from arcor2_fit_demo import get_data
 from arcor2_fit_demo.object_types.abstract_dobot import AbstractDobot
 from arcor2_fit_demo.object_types.conveyor_belt import ConveyorBelt
 from arcor2_fit_demo.object_types.dobot_m1 import DobotM1
 from arcor2_fit_demo.object_types.dobot_magician import DobotMagician
 from arcor2_fit_demo.object_types.fit_common_mixin import FitCommonMixin
-from arcor2_fit_demo.object_types.kinect_azure import KinectAzure
+from arcor2_kinect_azure_data.object_types.kinect_azure import KinectAzure
 
 
 def main() -> None:
     upload_def(AbstractDobot)
     upload_def(DobotMagician, urdf=Urdf(get_data("dobot-magician"), DobotMagician.urdf_package_name))
     upload_def(DobotM1, urdf=Urdf(get_data("dobot-m1"), DobotM1.urdf_package_name))
     upload_def(
```

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/PKG-INFO` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcor2-fit-demo
-Version: 1.1.0
+Version: 1.2.0
 Summary: ARCOR2 FIT Demo
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,15 +16,21 @@
 Description-Content-Type: text/markdown
 
 # arcor2_fit_demo
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.0.0] - 2023-03-06
+## [1.2.0] - 2023-07-20
+
+### Changed
+
+- `KinectAzure` ObjectType is now imported from `src/python/arcor2_kinect_azure_data/object_types/kinect_azure.py`.
+
+## [1.1.0] - 2023-03-07
 
 ### Changed
 
 - Compatibility with `arcor2_kinect_azure:0.6.0`.
 - Default url for Kinect.
 
 ## [1.0.0] - 2023-02-14
```

### Comparing `arcor2_fit_demo-1.1.0/arcor2_fit_demo.egg-info/SOURCES.txt` & `arcor2_fit_demo-1.2.0/arcor2_fit_demo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,10 +30,9 @@
 arcor2_fit_demo/data/dobot-magician/dobot/model/meshes/dae/magicianSuctionCup.dae
 arcor2_fit_demo/object_types/__init__.py
 arcor2_fit_demo/object_types/abstract_dobot.py
 arcor2_fit_demo/object_types/conveyor_belt.py
 arcor2_fit_demo/object_types/dobot_m1.py
 arcor2_fit_demo/object_types/dobot_magician.py
 arcor2_fit_demo/object_types/fit_common_mixin.py
-arcor2_fit_demo/object_types/kinect_azure.py
 arcor2_fit_demo/scripts/__init__.py
 arcor2_fit_demo/scripts/upload_objects.py
```

### Comparing `arcor2_fit_demo-1.1.0/backend_shim.py` & `arcor2_fit_demo-1.2.0/backend_shim.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,21 @@
         '--python-tag',
         'py310',
     ],
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `arcor2_fit_demo-1.1.0/setup.py` & `arcor2_fit_demo-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,30 @@
     'description': 'ARCOR2 FIT Demo',
     'entry_points': {
         'console_scripts': [
             'arcor2_fit_demo_upload_objects = arcor2_fit_demo.scripts.upload_objects:main',
         ],
     },
     'install_requires': (
-        'Pillow~=9.4.0',
-        'arcor2~=1.0.0',
+        'arcor2_kinect_azure_data~=0.1.0',
+        'arcor2~=1.1.0',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2_fit_demo
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.0.0] - 2023-03-06
+## [1.2.0] - 2023-07-20
+
+### Changed
+
+- `KinectAzure` ObjectType is now imported from `src/python/arcor2_kinect_azure_data/object_types/kinect_azure.py`.
+
+## [1.1.0] - 2023-03-07
 
 ### Changed
 
 - Compatibility with `arcor2_kinect_azure:0.6.0`.
 - Default url for Kinect.
 
 ## [1.0.0] - 2023-02-14
@@ -183,9 +189,9 @@
     },
     'packages': (
         'arcor2_fit_demo',
         'arcor2_fit_demo.object_types',
         'arcor2_fit_demo.scripts',
     ),
     'python_requires': '==3.10.*',
-    'version': '1.1.0',
+    'version': '1.2.0',
 })
```

