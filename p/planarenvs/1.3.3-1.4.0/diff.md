# Comparing `tmp/planarenvs-1.3.3.tar.gz` & `tmp/planarenvs-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planarenvs-1.3.3.tar", max compression
+gzip compressed data, was "planarenvs-1.4.0.tar", max compression
```

## Comparing `planarenvs-1.3.3.tar` & `planarenvs-1.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/.gitignore
--rw-r--r--   0        0        0       71 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/__init__.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_base/.gitignore
--rw-r--r--   0        0        0      254 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_base/__init__.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_base/envs/.gitignore
--rw-r--r--   0        0        0      122 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_base/envs/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_base/envs/acc.py
--rw-r--r--   0        0        0     2077 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_base/envs/mobile_base_env.py
--rw-r--r--   0        0        0      180 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_base/envs/vel.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_robot/.gitignore
--rw-r--r--   0        0        0      260 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_robot/__init__.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_robot/envs/.gitignore
--rw-r--r--   0        0        0      126 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_robot/envs/__init__.py
--rw-r--r--   0        0        0      185 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_robot/envs/acc.py
--rw-r--r--   0        0        0     3844 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_robot/envs/mobile_robot_env.py
--rw-r--r--   0        0        0      185 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/mobile_robot/envs/vel.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/.gitignore
--rw-r--r--   0        0        0      268 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/__init__.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/envs/.gitignore
--rw-r--r--   0        0        0      132 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/envs/__init__.py
--rw-r--r--   0        0        0      192 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/envs/acc.py
--rw-r--r--   0        0        0     2399 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/envs/n_link_reacher_env.py
--rw-r--r--   0        0        0      192 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/envs/vel.py
--rw-r--r--   0        0        0        0 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/resources/.gitignore
--rw-r--r--   0        0        0       78 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/resources/__init__.py
--rw-r--r--   0        0        0      516 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/n_link_reacher/resources/accController.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.619420 planarenvs-1.3.3/planarenvs/planar_common/.gitignore
--rw-r--r--   0        0        0      802 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/planar_common/acc_env.py
--rw-r--r--   0        0        0    11246 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/planar_common/planar_env.py
--rw-r--r--   0        0        0      929 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/planar_common/vel_env.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/point_robot/.gitignore
--rw-r--r--   0        0        0      254 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/point_robot/__init__.py
--rw-r--r--   0        0        0       13 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/point_robot/envs/.gitignore
--rw-r--r--   0        0        0      122 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/point_robot/envs/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/point_robot/envs/acc.py
--rw-r--r--   0        0        0     3208 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/point_robot/envs/point_robot_env.py
--rw-r--r--   0        0        0      180 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/point_robot/envs/vel.py
--rw-r--r--   0        0        0     1428 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/scenes/goal.py
--rw-r--r--   0        0        0     1037 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/scenes/obstacles.py
--rw-r--r--   0        0        0     1978 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/sensors/full_sensor.py
--rw-r--r--   0        0        0     1487 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/sensors/goal_sensor.py
--rw-r--r--   0        0        0     2443 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/sensors/obstacle_sensor.py
--rw-r--r--   0        0        0     1260 2023-05-17 09:49:31.623420 planarenvs-1.3.3/planarenvs/sensors/sensor_common.py
--rw-r--r--   0        0        0      606 2023-05-17 09:49:31.623420 planarenvs-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 planarenvs-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/.gitignore
+-rw-r--r--   0        0        0       71 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/__init__.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_base/.gitignore
+-rw-r--r--   0        0        0      254 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_base/__init__.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_base/envs/.gitignore
+-rw-r--r--   0        0        0      122 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_base/envs/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_base/envs/acc.py
+-rw-r--r--   0        0        0     2077 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_base/envs/mobile_base_env.py
+-rw-r--r--   0        0        0      180 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_base/envs/vel.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_robot/.gitignore
+-rw-r--r--   0        0        0      260 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_robot/__init__.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_robot/envs/.gitignore
+-rw-r--r--   0        0        0      126 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_robot/envs/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_robot/envs/acc.py
+-rw-r--r--   0        0        0     3844 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_robot/envs/mobile_robot_env.py
+-rw-r--r--   0        0        0      185 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/mobile_robot/envs/vel.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/.gitignore
+-rw-r--r--   0        0        0      268 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/__init__.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/envs/.gitignore
+-rw-r--r--   0        0        0      132 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/envs/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/envs/acc.py
+-rw-r--r--   0        0        0     2399 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/envs/n_link_reacher_env.py
+-rw-r--r--   0        0        0      192 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/envs/vel.py
+-rw-r--r--   0        0        0        0 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/resources/.gitignore
+-rw-r--r--   0        0        0       78 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/resources/__init__.py
+-rw-r--r--   0        0        0      516 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/n_link_reacher/resources/accController.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/planar_common/.gitignore
+-rw-r--r--   0        0        0      802 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/planar_common/acc_env.py
+-rw-r--r--   0        0        0    11246 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/planar_common/planar_env.py
+-rw-r--r--   0        0        0      929 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/planar_common/vel_env.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/point_robot/.gitignore
+-rw-r--r--   0        0        0      254 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/point_robot/__init__.py
+-rw-r--r--   0        0        0       13 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/point_robot/envs/.gitignore
+-rw-r--r--   0        0        0      122 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/point_robot/envs/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-21 05:50:50.202263 planarenvs-1.4.0/planarenvs/point_robot/envs/acc.py
+-rw-r--r--   0        0        0     3208 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/point_robot/envs/point_robot_env.py
+-rw-r--r--   0        0        0      180 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/point_robot/envs/vel.py
+-rw-r--r--   0        0        0     1428 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/scenes/goal.py
+-rw-r--r--   0        0        0     1037 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/scenes/obstacles.py
+-rw-r--r--   0        0        0     1978 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/sensors/full_sensor.py
+-rw-r--r--   0        0        0     1487 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/sensors/goal_sensor.py
+-rw-r--r--   0        0        0     2443 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/sensors/obstacle_sensor.py
+-rw-r--r--   0        0        0     1260 2023-07-21 05:50:50.206263 planarenvs-1.4.0/planarenvs/sensors/sensor_common.py
+-rw-r--r--   0        0        0      604 2023-07-21 05:50:50.206263 planarenvs-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 planarenvs-1.4.0/PKG-INFO
```

### Comparing `planarenvs-1.3.3/planarenvs/mobile_base/envs/mobile_base_env.py` & `planarenvs-1.4.0/planarenvs/mobile_base/envs/mobile_base_env.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/mobile_robot/envs/mobile_robot_env.py` & `planarenvs-1.4.0/planarenvs/mobile_robot/envs/mobile_robot_env.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/n_link_reacher/envs/n_link_reacher_env.py` & `planarenvs-1.4.0/planarenvs/n_link_reacher/envs/n_link_reacher_env.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/n_link_reacher/resources/accController.py` & `planarenvs-1.4.0/planarenvs/n_link_reacher/resources/accController.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/planar_common/acc_env.py` & `planarenvs-1.4.0/planarenvs/planar_common/acc_env.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/planar_common/planar_env.py` & `planarenvs-1.4.0/planarenvs/planar_common/planar_env.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/planar_common/vel_env.py` & `planarenvs-1.4.0/planarenvs/planar_common/vel_env.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/point_robot/envs/point_robot_env.py` & `planarenvs-1.4.0/planarenvs/point_robot/envs/point_robot_env.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/scenes/goal.py` & `planarenvs-1.4.0/planarenvs/scenes/goal.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/scenes/obstacles.py` & `planarenvs-1.4.0/planarenvs/scenes/obstacles.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/sensors/full_sensor.py` & `planarenvs-1.4.0/planarenvs/sensors/full_sensor.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/sensors/goal_sensor.py` & `planarenvs-1.4.0/planarenvs/sensors/goal_sensor.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/sensors/obstacle_sensor.py` & `planarenvs-1.4.0/planarenvs/sensors/obstacle_sensor.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/planarenvs/sensors/sensor_common.py` & `planarenvs-1.4.0/planarenvs/sensors/sensor_common.py`

 * *Files identical despite different names*

### Comparing `planarenvs-1.3.3/pyproject.toml` & `planarenvs-1.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "planarenvs"
-version = "1.3.3"
+version = "1.4.0"
 description = "Lightweight open-ai gym environments for planar kinematic chains."
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
 gym = "^0.26.0"
 numpy = "^1.19,<1.24"
 pyglet = "^1.5.21"
 scipy = "^1.5"
 forwardkinematics = "^1.0.3"
 pylint = "^2.13.3"
-mpscenes = "^0.3"
+mpscenes = "^0"
 pygame = "^2.1.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 pylint = "^2.13.3"
 black = "^22.3.0"
 pytest-cov = "^3.0.0"
```

### Comparing `planarenvs-1.3.3/PKG-INFO` & `planarenvs-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: planarenvs
-Version: 1.3.3
+Version: 1.4.0
 Summary: Lightweight open-ai gym environments for planar kinematic chains.
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: forwardkinematics (>=1.0.3,<2.0.0)
 Requires-Dist: gym (>=0.26.0,<0.27.0)
-Requires-Dist: mpscenes (>=0.3,<0.4)
+Requires-Dist: mpscenes (>=0,<1)
 Requires-Dist: numpy (>=1.19,<1.24)
 Requires-Dist: pygame (>=2.1.2,<3.0.0)
 Requires-Dist: pyglet (>=1.5.21,<2.0.0)
 Requires-Dist: pylint (>=2.13.3,<3.0.0)
 Requires-Dist: scipy (>=1.5,<2.0)
```

