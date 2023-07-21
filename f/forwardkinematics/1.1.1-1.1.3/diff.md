# Comparing `tmp/forwardkinematics-1.1.1.tar.gz` & `tmp/forwardkinematics-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forwardkinematics-1.1.1.tar", max compression
+gzip compressed data, was "forwardkinematics-1.1.3.tar", max compression
```

## Comparing `forwardkinematics-1.1.1.tar` & `forwardkinematics-1.1.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      582 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/__init__.py
--rw-r--r--   0        0        0      716 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/fksCommon/fk.py
--rw-r--r--   0        0        0      741 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/fksCommon/fk_by_name.py
--rw-r--r--   0        0        0     1760 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/fksCommon/fk_creator.py
--rw-r--r--   0        0        0     1548 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/planarFks/groundRobotFk.py
--rw-r--r--   0        0        0     1949 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/planarFks/mobileRobotFk.py
--rw-r--r--   0        0        0     1140 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/planarFks/planarArmFk.py
--rw-r--r--   0        0        0      718 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/planarFks/planar_fk.py
--rw-r--r--   0        0        0     1054 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/planarFks/pointFk.py
--rw-r--r--   0        0        0      468 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/albertFk.py
--rw-r--r--   0        0        0      343 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/boxerFk.py
--rw-r--r--   0        0        0        0 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/casadiConversion/__init__.py
--rw-r--r--   0        0        0        0 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
--rw-r--r--   0        0        0     3442 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
--rwxr-xr-x   0        0        0     6129 2023-03-01 10:08:23.787064 forwardkinematics-1.1.1/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
--rw-r--r--   0        0        0      380 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/dual_arm_fk.py
--rw-r--r--   0        0        0     3196 2023-03-01 10:08:23.787064 forwardkinematics-1.1.1/forwardkinematics/urdfFks/generic_urdf_fk.py
--rw-r--r--   0        0        0      306 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/jackalFk.py
--rw-r--r--   0        0        0      436 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/mobilePandaFk.py
--rw-r--r--   0        0        0      367 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/pandaFk.py
--rw-r--r--   0        0        0      365 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/pointRobotUrdfFk.py
--rw-r--r--   0        0        0      841 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/tiagoFk.py
--rw-r--r--   0        0        0     7580 2023-03-01 10:08:23.787064 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/albert.urdf
--rw-r--r--   0        0        0     2031 2023-03-01 10:08:23.787064 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/boxer.urdf
--rw-r--r--   0        0        0     8160 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/dual_arm.urdf
--rw-r--r--   0        0        0     1693 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/jackal.urdf
--rw-r--r--   0        0        0    12167 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/mobilePanda.urdf
--rw-r--r--   0        0        0    12455 2023-03-01 10:08:00.850780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/panda.urdf
--rw-r--r--   0        0        0     2628 2023-03-01 10:08:00.854780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/pointRobot.urdf
--rw-r--r--   0        0        0    33577 2023-03-01 10:08:00.854780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/tiago.urdf
--rw-r--r--   0        0        0     3288 2023-03-01 10:08:00.854780 forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdfFk.py
--rw-r--r--   0        0        0      738 2023-03-01 10:08:23.787064 forwardkinematics-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 forwardkinematics-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      582 2022-05-23 06:27:34.000000 forwardkinematics-1.1.3/README.md
+-rw-r--r--   0        0        0        0 2021-12-23 11:38:15.000000 forwardkinematics-1.1.3/forwardkinematics/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk.py
+-rw-r--r--   0        0        0      741 2022-05-10 14:08:20.000000 forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_by_name.py
+-rw-r--r--   0        0        0     1760 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_creator.py
+-rw-r--r--   0        0        0     1548 2022-03-31 08:49:42.000000 forwardkinematics-1.1.3/forwardkinematics/planarFks/groundRobotFk.py
+-rw-r--r--   0        0        0     1949 2022-03-31 08:49:42.000000 forwardkinematics-1.1.3/forwardkinematics/planarFks/mobileRobotFk.py
+-rw-r--r--   0        0        0     1140 2023-03-01 09:04:08.669225 forwardkinematics-1.1.3/forwardkinematics/planarFks/planarArmFk.py
+-rw-r--r--   0        0        0      842 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/planarFks/planar_fk.py
+-rw-r--r--   0        0        0     1054 2022-05-23 06:19:44.000000 forwardkinematics-1.1.3/forwardkinematics/planarFks/pointFk.py
+-rw-r--r--   0        0        0      468 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/albertFk.py
+-rw-r--r--   0        0        0      343 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/boxerFk.py
+-rw-r--r--   0        0        0        0 2021-12-23 10:47:55.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-23 10:47:55.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
+-rw-r--r--   0        0        0     3442 2022-03-16 12:17:29.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
+-rwxr-xr-x   0        0        0     6237 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
+-rw-r--r--   0        0        0      380 2022-05-23 12:16:36.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/dual_arm_fk.py
+-rw-r--r--   0        0        0     3544 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/urdfFks/generic_urdf_fk.py
+-rw-r--r--   0        0        0      306 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/jackalFk.py
+-rw-r--r--   0        0        0      436 2022-05-23 12:16:36.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/mobilePandaFk.py
+-rw-r--r--   0        0        0      367 2022-05-23 12:16:36.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/pandaFk.py
+-rw-r--r--   0        0        0      365 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/pointRobotUrdfFk.py
+-rw-r--r--   0        0        0      841 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/tiagoFk.py
+-rw-r--r--   0        0        0     7580 2023-03-01 09:56:43.501774 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/albert.urdf
+-rw-r--r--   0        0        0     2031 2023-03-01 09:56:43.501774 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/boxer.urdf
+-rw-r--r--   0        0        0     8160 2022-03-16 12:17:29.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/dual_arm.urdf
+-rw-r--r--   0        0        0     1693 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/jackal.urdf
+-rw-r--r--   0        0        0    12167 2021-12-23 11:38:39.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/mobilePanda.urdf
+-rw-r--r--   0        0        0    12455 2022-03-16 12:17:29.000000 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/panda.urdf
+-rw-r--r--   0        0        0     2628 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/pointRobot.urdf
+-rw-r--r--   0        0        0    33577 2023-01-25 09:37:59.882437 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/tiago.urdf
+-rw-r--r--   0        0        0     3304 2023-07-21 14:40:35.656059 forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdfFk.py
+-rw-r--r--   0        0        0      738 2023-07-21 14:40:42.572056 forwardkinematics-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 forwardkinematics-1.1.3/setup.py
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 forwardkinematics-1.1.3/PKG-INFO
```

### Comparing `forwardkinematics-1.1.1/README.md` & `forwardkinematics-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/fksCommon/fk.py` & `forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
     """Abstract class for forward kinematics"""
 
     def __init__(self):
         ABC.__init__(self)
         self._n = None
 
+    def set_mount_transformation(self, mount_transformation: np.ndarray):
+        self._mount_transformation = mount_transformation
+
     def fk(self, q, link, positionOnly=False):
         if isinstance(q, ca.SX):
             return self.casadi(q, link, positionOnly=positionOnly)
         elif isinstance(q, np.ndarray):
             return self.numpy(q, link, positionOnly=positionOnly)
 
     def n(self):
```

### Comparing `forwardkinematics-1.1.1/forwardkinematics/fksCommon/fk_by_name.py` & `forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_by_name.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/fksCommon/fk_creator.py` & `forwardkinematics-1.1.3/forwardkinematics/fksCommon/fk_creator.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/planarFks/groundRobotFk.py` & `forwardkinematics-1.1.3/forwardkinematics/planarFks/groundRobotFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/planarFks/mobileRobotFk.py` & `forwardkinematics-1.1.3/forwardkinematics/planarFks/mobileRobotFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/planarFks/planarArmFk.py` & `forwardkinematics-1.1.3/forwardkinematics/planarFks/planarArmFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/planarFks/planar_fk.py` & `forwardkinematics-1.1.3/forwardkinematics/planarFks/planar_fk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import re
+import numpy as np
 
 from forwardkinematics.fksCommon.fk import ForwardKinematics
 
 class NoLinkIndexFoundInLinkNameError(Exception):
     pass
 
 class ForwardKinematicsPlanar(ForwardKinematics):
 
+    def __init__(self):
+        super().__init__()
+        self._mount_transformation = np.identity(3)
+
+
     def fk(self, q, link: str, positionOnly: bool=False):
         if isinstance(link, str):
             return super().fk(q, self.get_link_index(link), positionOnly=positionOnly)
         else:
             return super().fk(q, link, positionOnly=positionOnly)
 
     def get_link_index(self, link: str):
```

### Comparing `forwardkinematics-1.1.1/forwardkinematics/planarFks/pointFk.py` & `forwardkinematics-1.1.3/forwardkinematics/planarFks/pointFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/casadiConversion/urdfparser.py` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/casadiConversion/urdfparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module is in most parts copied from https://github.com/mahaarbo/urdf2casadi.
 
 Changes are in get_forward_kinematics as it allows to pass the variable as an argument.
 """
 import casadi as ca
+import numpy as np
 from urdf_parser_py.urdf import URDF
 import forwardkinematics.urdfFks.casadiConversion.geometry.transformation_matrix as T
 
 
 class URDFparser(object):
     """Class that turns a chain from URDF to casadi functions."""
     actuated_types = ["prismatic", "revolute", "continuous"]
@@ -118,15 +119,15 @@
         for link in self.robot_desc.links:
             if link.name in self.robot_desc.parent_map:
                 self._link_names.append(link.name)
             else:
                 print(f"Link with name {link.name} does not has a parent. Link name is skipped.")
         return self._link_names
 
-    def get_forward_kinematics(self, root, tip, q):
+    def get_forward_kinematics(self, root, tip, q, link_transformation=np.eye(4)):
         """Returns the forward kinematics as a casadi function."""
         if self.robot_desc is None:
             raise ValueError('Robot description not loaded from urdf')
         joint_list = self.get_joint_info(self._absolute_root_link, tip)
         T_fk = ca.SX.eye(4)
         for joint in joint_list:
             if joint.type == "fixed":
@@ -152,10 +153,13 @@
                     axis = ca.np.array(joint.axis)
                 axis = (1./ca.np.linalg.norm(axis))*axis
                 joint_frame = T.revolute(
                     joint.origin.xyz,
                     joint.origin.rpy,
                     joint.axis, q[self._joint_map[joint.name]])
                 T_fk = ca.mtimes(T_fk, joint_frame)
+
+            T_fk = ca.mtimes(T_fk, link_transformation)
+
         return {
             "T_fk": T_fk
         }
```

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/generic_urdf_fk.py` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/generic_urdf_fk.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self._rootLink = rootLink
         self.readURDF(rootLink, end_link)
         self._n = self.robot.degrees_of_freedom()
         if base_type in ['diffdrive']:
             self._q_base = ca.SX.sym("q_base", 3)
         self._base_type = base_type
         self._q_ca = ca.SX.sym("q", self._n)
-        self.generateFunctions()
+        self._mount_transformation = np.identity(4)
 
     def readURDF(self, rootLink: str, end_link: str):
         self.robot = u2c.URDFparser(rootLink, end_link)
         self.robot.from_string(self._urdf_file)
         self.robot.detect_link_names()
         self.robot.set_joint_variable_map()
 
@@ -32,49 +32,51 @@
                 q = self._q_ca
             ca_fun = ca.Function(
                 "fk" + link, [q], [self.casadi(q, self._rootLink, link)]
             )
             self._fks[link] = ca_fun
 
 
-    def casadi(self, q: ca.SX, parent_link: str, child_link: str, positionOnly=False):
+    def casadi(self, q: ca.SX, parent_link: str, child_link: str, link_transformation=np.eye(4), positionOnly=False):
         if child_link not in self.robot.link_names():
             raise LinkNotInURDFError(
                 f"""The link you have requested, {child_link}, is not in the urdf.
                     Possible links are  {self.robot.link_names()}"""
             )
         if self._base_type in ['diffdrive']:
-            fk = self.robot.get_forward_kinematics(parent_link, child_link, q[2:])["T_fk"]
+            fk = self.robot.get_forward_kinematics(parent_link, child_link, q[2:], link_transformation)["T_fk"]
             c = ca.cos(q[2])
             s = ca.sin(q[2])
             T_base = ca.vcat([
                 ca.hcat([c, -s, 0, q[0]]),
                 ca.hcat([s, c, 0, q[1]]),
                 ca.hcat([0, 0, 1, 0]),
                 ca.hcat([0, 0, 0, 1]),
             ])
             fk = ca.mtimes(T_base, fk)
         else:
-            fk = self.robot.get_forward_kinematics(parent_link, child_link, q)["T_fk"]
+            fk = self.robot.get_forward_kinematics(parent_link, child_link, q, link_transformation)["T_fk"]
+            fk = ca.mtimes(self._mount_transformation, fk)
 
         if positionOnly:
             fk = fk[0:3, 3]
         return fk
 
-    def fk(self, q: ca.SX, parent_link: str, child_link: str, positionOnly=False):
+    def fk(self, q: ca.SX, parent_link: str, child_link: str,link_transformation=np.eye(4), positionOnly=False):
         if isinstance(q, ca.SX):
-            return self.casadi(q, parent_link, child_link, positionOnly=positionOnly)
+            return self.casadi(q, parent_link, child_link, link_transformation, positionOnly=positionOnly)
         elif isinstance(q, np.ndarray):
-            return self.numpy(q, parent_link, child_link, positionOnly=positionOnly)
+            return self.numpy(q, parent_link, child_link, link_transformation, positionOnly=positionOnly)
 
-    def numpy(self, q: ca.SX, parent_link: str, child_link: str, positionOnly=False):
+    def numpy(self, q: ca.SX, parent_link: str, child_link: str, link_transformation=np.eye(4), positionOnly=False):
         if parent_link == self._rootLink:
             fk_parent = np.identity(4)
         else:
             fk_parent = super().numpy_by_name(q, parent_link)
         fk_child = super().numpy_by_name(q, child_link)
         tf_parent_child = np.dot(np.linalg.inv(fk_parent), fk_child)
+        tf_parent_child = np.dot(link_transformation, tf_parent_child) #ToDo check if correct
         if positionOnly:
             return tf_parent_child[0:3, 3]
         else:
             return tf_parent_child
```

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/tiagoFk.py` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/tiagoFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/albert.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/albert.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/boxer.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/boxer.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/dual_arm.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/dual_arm.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/jackal.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/jackal.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/mobilePanda.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/mobilePanda.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/panda.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/panda.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/pointRobot.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/pointRobot.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdf/tiago.urdf` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdf/tiago.urdf`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.1.1/forwardkinematics/urdfFks/urdfFk.py` & `forwardkinematics-1.1.3/forwardkinematics/urdfFks/urdfFk.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         self._urdf_file = (
             os.path.dirname(os.path.abspath(__file__)) + "/urdf/" + fileName
         )
         self._links = links
         self._rootLink = rootLink
         self._end_links = end_links
         self._q_ca = ca.SX.sym("q", n)
+        self._mount_transformation = np.identity(4)
         self.readURDF()
         self._n = n
-        self.generateFunctions()
 
     def readURDF(self):
         self.robot = u2c.URDFparser(rootLink=self._rootLink, end_links=self._end_links)
         self.robot.from_file(self._urdf_file)
         self.robot.detect_link_names()
         self.robot.set_joint_variable_map()
 
@@ -59,25 +59,26 @@
             LinkNotInURDFError: An error occured accessing the urdf link.
         """
         if link not in self.robot.link_names():
             raise LinkNotInURDFError(
                 f"""The link you have requested, {link}, is not in the urdf.
                     Possible links are  {self.robot.link_names()}"""
             )
+        fk = self.robot.get_forward_kinematics(self._rootLink, link, q)["T_fk"]
         if positionOnly:
-            return self.robot.get_forward_kinematics(self._rootLink, link, q)["T_fk"][
-                0:3, 3
-            ]
+            return fk[0:3, 3]
         else:
-            return self.robot.get_forward_kinematics(self._rootLink, link, q)["T_fk"]
+            return fk
 
     def numpy(self, q: ca.SX, i: int, positionOnly=False):
         return self.numpy_by_name(q, self._links[i], positionOnly=positionOnly)
 
     def numpy_by_name(self, q: np.ndarray, link: str, positionOnly=False):
+        if not hasattr(self, '_fks'):
+            self.generateFunctions()
         """
         Raises:
             LinkNotInURDFError: An error occured accessing the urdf link.
         """
         if link not in self.robot.link_names():
             raise LinkNotInURDFError(
                 f"""The link you have requested, {link}, is not in the urdf.
```

### Comparing `forwardkinematics-1.1.1/pyproject.toml` & `forwardkinematics-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forwardkinematics"
-version = "1.1.1"
+version = "1.1.3"
 description = "\"Light-weight implementation of forward kinematics using casadi.\""
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maxspahn/forwardKinematics.git"
 repository = "https://github.com/maxspahn/forwardKinematics.git"
```

### Comparing `forwardkinematics-1.1.1/PKG-INFO` & `forwardkinematics-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forwardkinematics
-Version: 1.1.1
+Version: 1.1.3
 Summary: "Light-weight implementation of forward kinematics using casadi."
 Home-page: https://github.com/maxspahn/forwardKinematics.git
 License: MIT
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

