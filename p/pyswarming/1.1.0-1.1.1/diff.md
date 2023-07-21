# Comparing `tmp/pyswarming-1.1.0.tar.gz` & `tmp/pyswarming-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/macbookpro/Documents/GitHub/pyswarming/dist/.tmp-ttexk_cz/pyswarming-1.1.0.tar", last modified: Fri May  5 02:11:18 2023, max compression
+gzip compressed data, was "/Users/macbookpro/Documents/GitHub/pyswarming/dist/.tmp-cg596bkg/pyswarming-1.1.1.tar", last modified: Fri Jul 21 18:15:11 2023, max compression
```

## Comparing `pyswarming-1.1.0.tar` & `pyswarming-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)     1529 2023-04-24 23:27:31.000000 pyswarming-1.1.0/LICENSE.md
--rw-r--r--   0 macbookpro   (501) staff       (20)    11816 2023-05-05 02:11:18.000000 pyswarming-1.1.0/PKG-INFO
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    11049 2023-05-04 23:15:51.000000 pyswarming-1.1.0/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)      899 2023-05-04 18:36:20.000000 pyswarming-1.1.0/pyswarming/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)    14252 2023-03-29 00:19:04.000000 pyswarming-1.1.0/pyswarming/auto_differentiation.py
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    25881 2023-05-04 23:32:13.000000 pyswarming-1.1.0/pyswarming/behaviors.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8710 2023-05-05 00:54:30.000000 pyswarming-1.1.0/pyswarming/swarm.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)    11816 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)      352 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      106 2023-05-05 02:11:18.000000 pyswarming-1.1.0/setup.cfg
--rwxr-xr-x   0 macbookpro   (501) staff       (20)     1146 2023-04-24 23:22:58.000000 pyswarming-1.1.0/setup.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/tests/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-29 00:19:04.000000 pyswarming-1.1.0/tests/__init__.py
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    16957 2023-05-05 00:54:12.000000 pyswarming-1.1.0/tests/test_behaviors.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1529 2023-04-24 23:27:31.000000 pyswarming-1.1.1/LICENSE.md
+-rw-r--r--   0 macbookpro   (501) staff       (20)    13591 2023-07-21 18:15:11.000000 pyswarming-1.1.1/PKG-INFO
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    12824 2023-07-21 18:04:39.000000 pyswarming-1.1.1/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)      899 2023-07-21 17:48:11.000000 pyswarming-1.1.1/pyswarming/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)    14252 2023-03-29 00:19:04.000000 pyswarming-1.1.1/pyswarming/auto_differentiation.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    25881 2023-07-20 18:25:06.000000 pyswarming-1.1.1/pyswarming/behaviors.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)    12629 2023-07-21 14:37:10.000000 pyswarming-1.1.1/pyswarming/swarm.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)    13591 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)      372 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-07-21 18:15:11.000000 pyswarming-1.1.1/pyswarming.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      106 2023-07-21 18:15:11.000000 pyswarming-1.1.1/setup.cfg
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1146 2023-07-21 17:48:02.000000 pyswarming-1.1.1/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-21 18:15:11.000000 pyswarming-1.1.1/tests/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-29 00:19:04.000000 pyswarming-1.1.1/tests/__init__.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    28166 2023-07-20 18:54:34.000000 pyswarming-1.1.1/tests/test_behaviors.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1391 2023-07-20 20:23:44.000000 pyswarming-1.1.1/tests/test_swarm.py
```

### Comparing `pyswarming-1.1.0/LICENSE.md` & `pyswarming-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyswarming-1.1.0/PKG-INFO` & `pyswarming-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,13 @@
-Metadata-Version: 2.1
-Name: pyswarming
-Version: 1.1.0
-Summary: A research toolkit for Swarm Robotics
-Home-page: https://github.com/mrsonandrade/pyswarming
-Author: Emerson Martins de Andrade
-Author-email: mrson@oceanica.ufrj.br
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # pyswarming
 [![Tests](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml/badge.svg)](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Documentation Status](https://readthedocs.org/projects/pyswarming/badge/?version=latest)](https://pyswarming.readthedocs.io/en/latest/?badge=latest)
-![version](https://img.shields.io/badge/version-1.1.0-blue)
+![version](https://img.shields.io/badge/version-1.1.1-blue)
+[![Downloads](https://static.pepy.tech/badge/pyswarming)](https://pepy.tech/project/pyswarming)
 
 <img align="left" src="docs/readme_pics/logo.png">
 
 `pyswarming` is a research toolkit for Swarm Robotics.
 
 
 ## Installation
@@ -95,170 +76,180 @@
 [^10]: M. Chamanbaz et al., “Swarm-Enabling Technology for Multi-Robot Systems,” Front. Robot. AI, vol. 4, Apr. 2017. https://doi.org/10.3389/frobt.2017.00012.
 
 [^11]: B. M. Zoss et al., “Distributed system of autonomous buoys for scalable deployment and monitoring of large waterbodies,” Auton. Robots, vol. 42, no. 8, pp. 1669–1689, Dec. 2018. https://doi.org/10.1007/s10514-018-9702-0.
 
 ## Examples using pyswarming.swarm
 ```python
 # importing the swarm creator
-import pyswarming.swarm as sw
+import pyswarming.swarm as ps
 ```
 
 ### Repulsion 
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['repulsion']) # list of behaviors
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['repulsion']) # list of behaviors
 my_swarm.simulate()
 ```
 
 ### Collective navigation 
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['repulsion']) # list of behaviors
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['collective_navigation']) # list of behaviors
 my_swarm.behaviors_dict['r_out']['collective_navigation']['alpha'] = 2.0  # setting the strength of the repulsion
-my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = np.array([-40, -40, 0]) # setting the target
+my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = [-40, -40, 0] # setting the target
 my_swarm.simulate()
 ```
 
-### Target + Aggregation 
+### Target + Aggregation
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['target','aggregation']) # list of behaviors
-my_swarm.behaviors_dict['r_out']['target']['T'] = np.array([-40, -40, 0]) # setting the target
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['target','aggregation']) # list of behaviors
+my_swarm.behaviors_dict['r_out']['target']['T'] = [-40, -40, 0] # setting the target
 my_swarm.simulate()
 ```
 
 ## Other Examples
-Considering a swarm of robots, they can show different behaviors by using ``pyswarming``. The following codes are simplified implementations, for detailed ones, see the [Examples](https://github.com/mrsonandrade/pyswarming/tree/main/Examples) folder.
+Considering a swarm of robots, they can show different behaviors by using ``pyswarming``. The following codes are simplified implementations, for detailed ones, see the [examples](https://github.com/mrsonandrade/pyswarming/tree/main/examples) folder.
 ```python
 # importing the swarming behaviors
 import pyswarming.behaviors as ps
 
 # importing numpy to work with arrays
 import numpy as np
 ```
 
 
-### Target 
+### Target
 To simplify, considering just one robot.
 ```python
 # define the robot (x, y, z) position
-r_i = np.asarray([0., 0., 0.])
+robot_position_i = np.asarray([0., 0., 0.])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed_i = 1.0
 
 # define a target (x, y, z) position
-T = np.asarray([8., 8., 0.])
+target_position = np.asarray([8., 8., 0.])
 
 for t in range(15):
 
     # print the robot (x, y, z) position
-    print(r_i)
+    print(robot_position_i)
 
     # update the robot (x, y, z) position
-    r_i += s_i*ps.target(r_i, T)
+    robot_position_i += robot_speed_i*ps.target(robot_position_i, target_position)
 ```
-![Target](Examples/pics/Target.gif)
+![Target](notebooks/pics/Target.gif)
 
 
 ### Aggregation 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[8., 8., 0.],
-                [-8., 8., 0.],
-                [8., -8., 0.],
-                [-8., -8., 0.]])
+robot_position = np.asarray([[8., 8., 0.],
+                            [-8., 8., 0.],
+                            [8., -8., 0.],
+                            [-8., -8., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_speed)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*ps.aggregation(r_i, r_j)
+    for r_ind in range(len(robot_speed)):
+        r_i = robot_speed[r_ind]
+        r_j = np.delete(robot_speed, np.array([r_ind]), axis=0)
+        robot_speed[r_ind] += robot_speed*ps.aggregation(r_i, r_j)
 ```
-![Aggregation](Examples/pics/Aggregation.gif)
+![Aggregation](notebooks/pics/Aggregation.gif)
 
 
 ### Repulsion 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[1., 1., 0.],
-                [-1., 1., 0.],
-                [1., -1., 0.],
-                [-1., -1., 0.]])
+robot_position = np.asarray([[1., 1., 0.],
+                            [-1., 1., 0.],
+                            [1., -1., 0.],
+                            [-1., -1., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_position)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*ps.repulsion(r_i, r_j, 3.0)
+    for r_ind in range(len(robot_position)):
+        r_i = robot_position[r_ind]
+        r_j = np.delete(robot_position, np.array([r_ind]), axis=0)
+        robot_position[r_ind] += robot_speed*ps.repulsion(r_i, r_j, 3.0)
 ```
-![Repulsion](Examples/pics/Repulsion.gif)
+![Repulsion](notebooks/pics/Repulsion.gif)
 
 ### Aggregation + Repulsion 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[8., 8., 0.],
-                [-8., 8., 0.],
-                [8., -8., 0.],
-                [-8., -8., 0.]])
+robot_position = np.asarray([[8., 8., 0.],
+                            [-8., 8., 0.],
+                            [8., -8., 0.],
+                            [-8., -8., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_position)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*(ps.aggregation(r_i, r_j) + ps.repulsion(r_i, r_j, 5.0))
+    for r_ind in range(len(robot_position)):
+        r_i = robot_position[r_ind]
+        r_j = np.delete(robot_position, np.array([r_ind]), axis=0)
+        robot_position[r_ind] += s_i*(ps.aggregation(r_i, r_j) + ps.repulsion(r_i, r_j, 5.0))
 ```
-![AggregationRepulsion](Examples/pics/AggregationRepulsion.gif)
+![AggregationRepulsion](notebooks/pics/AggregationRepulsion.gif)
 
 ## Contributing to pyswarming
 All kind of contributions are welcome: 
 * Improvement of code with new features, bug fixes, and  bug reports
 * Improvement of documentation
 * Additional tests
 
 Follow the instructions [here](https://pyswarming.readthedocs.io/en/latest/Contribution.html)
-for submitting a PR.
+for submitting a PR (Pull Request).
 
 If you have any ideas or questions, feel free to open an issue.
 
 
 ## Acknowledgements
+The authors would like to thank the Human Resources Program from the National Agency of Oil, Gas and Bio Combustibles – PRH-ANP for the financial support.
 This work was supported by "Coordenação de Aperfeiçoamento de Pessoal de Nível Superior - Brasil (CAPES)", [LOC/COPPE/UFRJ](https://www.loc.ufrj.br/index.php/en/) ([Laboratory of Waves and Current](https://www.loc.ufrj.br/index.php/en/) - [Federal University of Rio de Janeiro](https://ufrj.br/en/)) and the National Council for Scientific and Technological Development (CNPq), which are gratefully acknowledged.
```

### Comparing `pyswarming-1.1.0/README.md` & `pyswarming-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: pyswarming
+Version: 1.1.1
+Summary: A research toolkit for Swarm Robotics
+Home-page: https://github.com/mrsonandrade/pyswarming
+Author: Emerson Martins de Andrade
+Author-email: mrson@oceanica.ufrj.br
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # pyswarming
 [![Tests](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml/badge.svg)](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Documentation Status](https://readthedocs.org/projects/pyswarming/badge/?version=latest)](https://pyswarming.readthedocs.io/en/latest/?badge=latest)
-![version](https://img.shields.io/badge/version-1.1.0-blue)
+![version](https://img.shields.io/badge/version-1.1.1-blue)
+[![Downloads](https://static.pepy.tech/badge/pyswarming)](https://pepy.tech/project/pyswarming)
 
 <img align="left" src="docs/readme_pics/logo.png">
 
 `pyswarming` is a research toolkit for Swarm Robotics.
 
 
 ## Installation
@@ -75,170 +96,180 @@
 [^10]: M. Chamanbaz et al., “Swarm-Enabling Technology for Multi-Robot Systems,” Front. Robot. AI, vol. 4, Apr. 2017. https://doi.org/10.3389/frobt.2017.00012.
 
 [^11]: B. M. Zoss et al., “Distributed system of autonomous buoys for scalable deployment and monitoring of large waterbodies,” Auton. Robots, vol. 42, no. 8, pp. 1669–1689, Dec. 2018. https://doi.org/10.1007/s10514-018-9702-0.
 
 ## Examples using pyswarming.swarm
 ```python
 # importing the swarm creator
-import pyswarming.swarm as sw
+import pyswarming.swarm as ps
 ```
 
 ### Repulsion 
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['repulsion']) # list of behaviors
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['repulsion']) # list of behaviors
 my_swarm.simulate()
 ```
 
 ### Collective navigation 
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['repulsion']) # list of behaviors
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['collective_navigation']) # list of behaviors
 my_swarm.behaviors_dict['r_out']['collective_navigation']['alpha'] = 2.0  # setting the strength of the repulsion
-my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = np.array([-40, -40, 0]) # setting the target
+my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = [-40, -40, 0] # setting the target
 my_swarm.simulate()
 ```
 
-### Target + Aggregation 
+### Target + Aggregation
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['target','aggregation']) # list of behaviors
-my_swarm.behaviors_dict['r_out']['target']['T'] = np.array([-40, -40, 0]) # setting the target
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['target','aggregation']) # list of behaviors
+my_swarm.behaviors_dict['r_out']['target']['T'] = [-40, -40, 0] # setting the target
 my_swarm.simulate()
 ```
 
 ## Other Examples
-Considering a swarm of robots, they can show different behaviors by using ``pyswarming``. The following codes are simplified implementations, for detailed ones, see the [Examples](https://github.com/mrsonandrade/pyswarming/tree/main/Examples) folder.
+Considering a swarm of robots, they can show different behaviors by using ``pyswarming``. The following codes are simplified implementations, for detailed ones, see the [examples](https://github.com/mrsonandrade/pyswarming/tree/main/examples) folder.
 ```python
 # importing the swarming behaviors
 import pyswarming.behaviors as ps
 
 # importing numpy to work with arrays
 import numpy as np
 ```
 
 
-### Target 
+### Target
 To simplify, considering just one robot.
 ```python
 # define the robot (x, y, z) position
-r_i = np.asarray([0., 0., 0.])
+robot_position_i = np.asarray([0., 0., 0.])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed_i = 1.0
 
 # define a target (x, y, z) position
-T = np.asarray([8., 8., 0.])
+target_position = np.asarray([8., 8., 0.])
 
 for t in range(15):
 
     # print the robot (x, y, z) position
-    print(r_i)
+    print(robot_position_i)
 
     # update the robot (x, y, z) position
-    r_i += s_i*ps.target(r_i, T)
+    robot_position_i += robot_speed_i*ps.target(robot_position_i, target_position)
 ```
-![Target](Examples/pics/Target.gif)
+![Target](notebooks/pics/Target.gif)
 
 
 ### Aggregation 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[8., 8., 0.],
-                [-8., 8., 0.],
-                [8., -8., 0.],
-                [-8., -8., 0.]])
+robot_position = np.asarray([[8., 8., 0.],
+                            [-8., 8., 0.],
+                            [8., -8., 0.],
+                            [-8., -8., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_speed)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*ps.aggregation(r_i, r_j)
+    for r_ind in range(len(robot_speed)):
+        r_i = robot_speed[r_ind]
+        r_j = np.delete(robot_speed, np.array([r_ind]), axis=0)
+        robot_speed[r_ind] += robot_speed*ps.aggregation(r_i, r_j)
 ```
-![Aggregation](Examples/pics/Aggregation.gif)
+![Aggregation](notebooks/pics/Aggregation.gif)
 
 
 ### Repulsion 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[1., 1., 0.],
-                [-1., 1., 0.],
-                [1., -1., 0.],
-                [-1., -1., 0.]])
+robot_position = np.asarray([[1., 1., 0.],
+                            [-1., 1., 0.],
+                            [1., -1., 0.],
+                            [-1., -1., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_position)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*ps.repulsion(r_i, r_j, 3.0)
+    for r_ind in range(len(robot_position)):
+        r_i = robot_position[r_ind]
+        r_j = np.delete(robot_position, np.array([r_ind]), axis=0)
+        robot_position[r_ind] += robot_speed*ps.repulsion(r_i, r_j, 3.0)
 ```
-![Repulsion](Examples/pics/Repulsion.gif)
+![Repulsion](notebooks/pics/Repulsion.gif)
 
 ### Aggregation + Repulsion 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[8., 8., 0.],
-                [-8., 8., 0.],
-                [8., -8., 0.],
-                [-8., -8., 0.]])
+robot_position = np.asarray([[8., 8., 0.],
+                            [-8., 8., 0.],
+                            [8., -8., 0.],
+                            [-8., -8., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_position)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*(ps.aggregation(r_i, r_j) + ps.repulsion(r_i, r_j, 5.0))
+    for r_ind in range(len(robot_position)):
+        r_i = robot_position[r_ind]
+        r_j = np.delete(robot_position, np.array([r_ind]), axis=0)
+        robot_position[r_ind] += s_i*(ps.aggregation(r_i, r_j) + ps.repulsion(r_i, r_j, 5.0))
 ```
-![AggregationRepulsion](Examples/pics/AggregationRepulsion.gif)
+![AggregationRepulsion](notebooks/pics/AggregationRepulsion.gif)
 
 ## Contributing to pyswarming
 All kind of contributions are welcome: 
 * Improvement of code with new features, bug fixes, and  bug reports
 * Improvement of documentation
 * Additional tests
 
 Follow the instructions [here](https://pyswarming.readthedocs.io/en/latest/Contribution.html)
-for submitting a PR.
+for submitting a PR (Pull Request).
 
 If you have any ideas or questions, feel free to open an issue.
 
 
 ## Acknowledgements
+The authors would like to thank the Human Resources Program from the National Agency of Oil, Gas and Bio Combustibles – PRH-ANP for the financial support.
 This work was supported by "Coordenação de Aperfeiçoamento de Pessoal de Nível Superior - Brasil (CAPES)", [LOC/COPPE/UFRJ](https://www.loc.ufrj.br/index.php/en/) ([Laboratory of Waves and Current](https://www.loc.ufrj.br/index.php/en/) - [Federal University of Rio de Janeiro](https://ufrj.br/en/)) and the National Council for Scientific and Technological Development (CNPq), which are gratefully acknowledged.
```

### Comparing `pyswarming-1.1.0/pyswarming/__init__.py` & `pyswarming-1.1.1/pyswarming/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,10 +30,10 @@
 from . import behaviors
 from . import swarm
 
 __all__ = behaviors.__all__.copy()
 __all__ = swarm.__all__.copy()
 
 name = "pyswarming"
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __author__ = "Emerson Martins de Andrade, Antonio Carlos Fernandes and Joel Sena Sales Jr"
 __author_email__ = "mrson@oceanica.ufrj.br"
```

### Comparing `pyswarming-1.1.0/pyswarming/auto_differentiation.py` & `pyswarming-1.1.1/pyswarming/auto_differentiation.py`

 * *Files identical despite different names*

### Comparing `pyswarming-1.1.0/pyswarming/behaviors.py` & `pyswarming-1.1.1/pyswarming/behaviors.py`

 * *Files identical despite different names*

### Comparing `pyswarming-1.1.0/pyswarming/swarm.py` & `pyswarming-1.1.1/pyswarming/swarm.py`

 * *Files 26% similar despite different names*

```diff
@@ -38,63 +38,96 @@
         float number giving the linear speed of each robot. This
         speed is used for those behaviors that have an orientation or
         nonsimensional contributions.
 
     dT : float
         float number giving the sampling time.
 
-    deployment_point : list
-        list containing the swarm deployment point.
+    deployment_point_limits : list
+        list containing two lists with the swarm deployment coordinate limits,
+        where the first list is the lower limit [x_min, y_min, z_min] and the
+        second is the upper limit [x_max, y_max, z_max].
+        For the 'none' distribution_type only the lower limit is considered;
+        For the 'uniform' distribution_type both limits are considered;
+        For the 'gaussian' distribution_type the lower limit is considered
+        as the mean of the distribution and the upper limit is considered
+        as the standard deviation of the distribution.
+
+    deployment_orientation_limits : list
+        list containing two lists with the swarm deployment orientation limits,
+        where the first list is the lower limit [roll_min, pitch_min, yaw_min]
+        and the second is the upper limit [roll_max, pitch_max, yaw_max].
+        For the 'none' distribution_type only the lower limit is considered;
+        For the 'uniform' distribution_type both limits are considered;
+        For the 'gaussian' distribution_type the lower limit is considered
+        as the mean of the distribution and the upper limit is considered
+        as the standard deviation of the distribution.
+
+    distribution_type : {'none', 'uniform', 'gaussian'}
+        type of distribution used to create the robots.
+        - 'none' : the creation is not based in any distribution.
+        - 'uniform' : the creation is based in an uniform distribution.
+        - 'gaussian' : the creation is based in an gaussian distribution.
 
     plot_limits : list
         list containing the plot limits (matplotlib).
 
     behaviors : list
         list containing the behaviors to be simulated.
 
     Example 1
     --------
-    >>> my_swarm = Swarm(10, # number of robots
-                 0.5, # linear speed of each robot
-                 1.0, # sampling time
-                 [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                 [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                 ['collective_navigation']) # list of behaviors
+    >>> import pyswarming.swarm as ps
+    >>> my_swarm = ps.Swarm(n = 10, # number of robots
+                            linear_speed = 0.5, # linear speed of each robot
+                            dT = 1.0, # sampling time
+                            deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                            deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                            distribution_type =  'uniform', # type of distribution used to deploy the robots
+                            plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                            behaviors = ['collective_navigation']) # list of behaviors
     >>> my_swarm.behaviors_dict['r_out']['collective_navigation']['alpha'] = 2.0  # setting the strength of the repulsion
-    >>> my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = np.array([-40, -40, 0]) # setting the target
+    >>> my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = [-40, -40, 0] # setting the target position [x, y, z]
     >>> my_swarm.simulate()
 
     Example 2
     --------
-    >>> my_swarm = Swarm(10, # number of robots
-                 0.5, # linear speed of each robot
-                 1.0, # sampling time
-                 [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                 [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                 ['target','aggregation']) # list of behaviors
-    >>> my_swarm.behaviors_dict['r_out']['target']['T'] = np.array([-40, -40, 0]) # setting the target
+    >>> import pyswarming.swarm as ps
+    >>> my_swarm = ps.Swarm(n = 10, # number of robots
+                            linear_speed = 0.5, # linear speed of each robot
+                            dT = 1.0, # sampling time
+                            deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                            deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                            distribution_type =  'uniform', # type of distribution used to deploy the robots
+                            plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                            behaviors = ['target','aggregation']) # list of behaviors
+    >>> my_swarm.behaviors_dict['r_out']['target']['T'] = [-40, -40, 0] # setting the target position [x, y, z]
     >>> my_swarm.simulate()
     """
 
     def __init__(self, n,
                  linear_speed = 0.5,
                  dT = 1.0,
-                 deployment_point = [0.0, 0.0],
+                 deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]],
+                 deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*np.pi]],
+                 distribution_type =  'uniform',
                  plot_limits = [[-50.0, 50.0], [-50.0, 50.0]],
                  behaviors = ['target']):
 
         if n <= 1:
             raise Exception("The number of robots must be greater than 1 (n > 1).")
 
         self.n = n
         self.dimensions = 2 # this version allows the creation of 2D swarms
         self.linear_speed = linear_speed
         self.dT = dT
         self.plot_limits = plot_limits
-        self.deployment_point = deployment_point
+        self.deployment_point_limits = deployment_point_limits
+        self.deployment_orientation_limits = deployment_orientation_limits
+        self.distribution_type = distribution_type
         self.behaviors = behaviors
         self.pose = self._create_robots()
         self.behaviors_dict = {'r_out':{'aggregation': {'function':None},
                                           'repulsion': {'function':None,
                                                         'alpha': 10.0,
                                                         'd': 2},
                                           'target': {'function':None,
@@ -108,16 +141,34 @@
 
     def _create_robots(self):
         """
         Creates an array of n robots with
         user-specified parameters.
         """
 
-        position = np.random.uniform(low=self.deployment_point[0]-5.0, high=self.deployment_point[1]+5.0, size=(self.n, 3, ))
-        orientation = np.random.uniform(low=0, high=2*np.pi, size=(self.n, 3, ))
+        if self.distribution_type=='none':
+            position = np.asarray([self.deployment_point_limits[0] for i in range(self.n)])
+            orientation = np.asarray([self.deployment_orientation_limits[0] for i in range(self.n)])
+
+        elif self.distribution_type=='uniform':
+            position = np.random.uniform(low=self.deployment_point_limits[0],
+                                         high=self.deployment_point_limits[1],
+                                         size=(self.n, 3, ))
+            orientation = np.random.uniform(low=self.deployment_orientation_limits[0],
+                                            high=self.deployment_orientation_limits[1],
+                                            size=(self.n, 3, ))
+            
+        elif self.distribution_type=='gaussian':
+            position = np.random.normal(loc=self.deployment_point_limits[0],
+                                         scale=self.deployment_point_limits[1],
+                                         size=(self.n, 3, ))
+            orientation = np.random.normal(loc=self.deployment_orientation_limits[0],
+                                            scale=self.deployment_orientation_limits[1],
+                                            size=(self.n, 3, ))
+
         pose = np.concatenate((position, orientation), axis=1)
 
         if self.dimensions==2:
             pose[:,2] = 0 # z
             pose[:,3] = 0 # roll
             pose[:,4] = 0 # pitch
 
@@ -152,22 +203,22 @@
             r_j = np.delete(r, np.array([r_ind]), axis=0)
 
             theta_i = theta[r_ind]
             theta_j = np.delete(theta, np.array([r_ind]), axis=0)
 
             self.behaviors_dict['r_out']['aggregation']['function'] = bh.aggregation(r_i, r_j)
             self.behaviors_dict['r_out']['repulsion']['function'] = bh.repulsion(r_i,
-                                                                                   r_j,
-                                                                                   self.behaviors_dict['r_out']['repulsion']['alpha'],
-                                                                                   self.behaviors_dict['r_out']['repulsion']['d'])
+                                                                                 r_j,
+                                                                                 self.behaviors_dict['r_out']['repulsion']['alpha'],
+                                                                                 self.behaviors_dict['r_out']['repulsion']['d'])
             self.behaviors_dict['r_out']['target']['function'] = bh.target(r_i,
-                                                                             self.behaviors_dict['r_out']['target']['T'])
+                                                                           np.asarray(self.behaviors_dict['r_out']['target']['T']))
             self.behaviors_dict['r_out']['collective_navigation']['function'] = bh.collective_navigation(r_i,
                                                                                                            r_j,
-                                                                                                           self.behaviors_dict['r_out']['collective_navigation']['T'],
+                                                                                                           np.asarray(self.behaviors_dict['r_out']['collective_navigation']['T']),
                                                                                                            self.behaviors_dict['r_out']['collective_navigation']['alpha'],
                                                                                                            self.behaviors_dict['r_out']['collective_navigation']['d'])
 
             self.behaviors_dict['theta_out']['leaderless_heading_consensus']['function'] = bh.leaderless_heading_consensus(theta_i, theta_j)
             self.behaviors_dict['theta_out']['heading_consensus']['function'] = bh.heading_consensus(theta_i, theta_j)
 
             behaviors_output = []
@@ -185,16 +236,20 @@
                 r_sum = (np.sum(np.asarray([r_out[0] for r_out in behaviors_output]), axis=0))
                 r_normalized = r_sum/np.linalg.norm(r_sum)
                 r[r_ind] += r_normalized * self.linear_speed * self.dT
                 theta[r_ind][2] = np.arctan2(r[r_ind][1], r[r_ind][0])
 
         self.pose = np.concatenate((r, theta), axis=1)
 
-    def simulate(self):
+    def simulate(self,
+                 frames = 720,
+                 interval = 1,
+                 blit = False,
+                 repeat = False):
 
         # First set up the figure and the axis
         if self.dimensions == 2:
             self.fig, self.ax = plt.subplots()
 
-        anim = animation.FuncAnimation(self.fig, self._animate, frames=720, interval=1, blit=False)
+        anim = animation.FuncAnimation(self.fig, self._animate, frames=frames, interval=interval, blit=blit, repeat=repeat)
 
         plt.show()
```

### Comparing `pyswarming-1.1.0/pyswarming.egg-info/PKG-INFO` & `pyswarming-1.1.1/pyswarming.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswarming
-Version: 1.1.0
+Version: 1.1.1
 Summary: A research toolkit for Swarm Robotics
 Home-page: https://github.com/mrsonandrade/pyswarming
 Author: Emerson Martins de Andrade
 Author-email: mrson@oceanica.ufrj.br
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pyswarming
 [![Tests](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml/badge.svg)](https://github.com/mrsonandrade/pyswarming/actions/workflows/tests_package.yml)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![Documentation Status](https://readthedocs.org/projects/pyswarming/badge/?version=latest)](https://pyswarming.readthedocs.io/en/latest/?badge=latest)
-![version](https://img.shields.io/badge/version-1.1.0-blue)
+![version](https://img.shields.io/badge/version-1.1.1-blue)
+[![Downloads](https://static.pepy.tech/badge/pyswarming)](https://pepy.tech/project/pyswarming)
 
 <img align="left" src="docs/readme_pics/logo.png">
 
 `pyswarming` is a research toolkit for Swarm Robotics.
 
 
 ## Installation
@@ -95,170 +96,180 @@
 [^10]: M. Chamanbaz et al., “Swarm-Enabling Technology for Multi-Robot Systems,” Front. Robot. AI, vol. 4, Apr. 2017. https://doi.org/10.3389/frobt.2017.00012.
 
 [^11]: B. M. Zoss et al., “Distributed system of autonomous buoys for scalable deployment and monitoring of large waterbodies,” Auton. Robots, vol. 42, no. 8, pp. 1669–1689, Dec. 2018. https://doi.org/10.1007/s10514-018-9702-0.
 
 ## Examples using pyswarming.swarm
 ```python
 # importing the swarm creator
-import pyswarming.swarm as sw
+import pyswarming.swarm as ps
 ```
 
 ### Repulsion 
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['repulsion']) # list of behaviors
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['repulsion']) # list of behaviors
 my_swarm.simulate()
 ```
 
 ### Collective navigation 
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['repulsion']) # list of behaviors
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['collective_navigation']) # list of behaviors
 my_swarm.behaviors_dict['r_out']['collective_navigation']['alpha'] = 2.0  # setting the strength of the repulsion
-my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = np.array([-40, -40, 0]) # setting the target
+my_swarm.behaviors_dict['r_out']['collective_navigation']['T'] = [-40, -40, 0] # setting the target
 my_swarm.simulate()
 ```
 
-### Target + Aggregation 
+### Target + Aggregation
 ```python
-my_swarm = sw.Swarm(10, # number of robots
-                    0.5, # linear speed of each robot
-                    1.0, # sampling time
-                    [0.0, 0.0], # robots deployed randomly around x = 0.0, y = 0.0 (+- 5.0 meters)
-                    [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
-                    ['target','aggregation']) # list of behaviors
-my_swarm.behaviors_dict['r_out']['target']['T'] = np.array([-40, -40, 0]) # setting the target
+# creating the swarm
+my_swarm = ps.Swarm(n = 10, # number of robots
+                    linear_speed = 0.5, # linear speed of each robot
+                    dT = 1.0, # sampling time
+                    deployment_point_limits = [[0.0, 0.0, 0.0], [5.0, 5.0, 0.0]], # lower and upper limits for the position deployment
+                    deployment_orientation_limits = [[0.0, 0.0, 0.0], [0.0, 0.0, 2*3.1415]], # lower and upper limits for the orientation deployment
+                    distribution_type =  'uniform', # type of distribution used to deploy the robots
+                    plot_limits = [[-50.0, 50.0], [-50.0, 50.0]], # plot limits x_lim, y_lim
+                    behaviors = ['target','aggregation']) # list of behaviors
+my_swarm.behaviors_dict['r_out']['target']['T'] = [-40, -40, 0] # setting the target
 my_swarm.simulate()
 ```
 
 ## Other Examples
-Considering a swarm of robots, they can show different behaviors by using ``pyswarming``. The following codes are simplified implementations, for detailed ones, see the [Examples](https://github.com/mrsonandrade/pyswarming/tree/main/Examples) folder.
+Considering a swarm of robots, they can show different behaviors by using ``pyswarming``. The following codes are simplified implementations, for detailed ones, see the [examples](https://github.com/mrsonandrade/pyswarming/tree/main/examples) folder.
 ```python
 # importing the swarming behaviors
 import pyswarming.behaviors as ps
 
 # importing numpy to work with arrays
 import numpy as np
 ```
 
 
-### Target 
+### Target
 To simplify, considering just one robot.
 ```python
 # define the robot (x, y, z) position
-r_i = np.asarray([0., 0., 0.])
+robot_position_i = np.asarray([0., 0., 0.])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed_i = 1.0
 
 # define a target (x, y, z) position
-T = np.asarray([8., 8., 0.])
+target_position = np.asarray([8., 8., 0.])
 
 for t in range(15):
 
     # print the robot (x, y, z) position
-    print(r_i)
+    print(robot_position_i)
 
     # update the robot (x, y, z) position
-    r_i += s_i*ps.target(r_i, T)
+    robot_position_i += robot_speed_i*ps.target(robot_position_i, target_position)
 ```
-![Target](Examples/pics/Target.gif)
+![Target](notebooks/pics/Target.gif)
 
 
 ### Aggregation 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[8., 8., 0.],
-                [-8., 8., 0.],
-                [8., -8., 0.],
-                [-8., -8., 0.]])
+robot_position = np.asarray([[8., 8., 0.],
+                            [-8., 8., 0.],
+                            [8., -8., 0.],
+                            [-8., -8., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_speed)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*ps.aggregation(r_i, r_j)
+    for r_ind in range(len(robot_speed)):
+        r_i = robot_speed[r_ind]
+        r_j = np.delete(robot_speed, np.array([r_ind]), axis=0)
+        robot_speed[r_ind] += robot_speed*ps.aggregation(r_i, r_j)
 ```
-![Aggregation](Examples/pics/Aggregation.gif)
+![Aggregation](notebooks/pics/Aggregation.gif)
 
 
 ### Repulsion 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[1., 1., 0.],
-                [-1., 1., 0.],
-                [1., -1., 0.],
-                [-1., -1., 0.]])
+robot_position = np.asarray([[1., 1., 0.],
+                            [-1., 1., 0.],
+                            [1., -1., 0.],
+                            [-1., -1., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_position)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*ps.repulsion(r_i, r_j, 3.0)
+    for r_ind in range(len(robot_position)):
+        r_i = robot_position[r_ind]
+        r_j = np.delete(robot_position, np.array([r_ind]), axis=0)
+        robot_position[r_ind] += robot_speed*ps.repulsion(r_i, r_j, 3.0)
 ```
-![Repulsion](Examples/pics/Repulsion.gif)
+![Repulsion](notebooks/pics/Repulsion.gif)
 
 ### Aggregation + Repulsion 
 Considering four robots.
 ```python
 # define each robot (x, y, z) position
-r = np.asarray([[8., 8., 0.],
-                [-8., 8., 0.],
-                [8., -8., 0.],
-                [-8., -8., 0.]])
+robot_position = np.asarray([[8., 8., 0.],
+                            [-8., 8., 0.],
+                            [8., -8., 0.],
+                            [-8., -8., 0.]])
 
-# set the robot linear velocity
-s_i = 1.0
+# set the robot speed
+robot_speed = 1.0
 
-for t in range(15):
+for time_i in range(15):
 
     # print the robot (x, y, z) positions
-    print(r)
+    print(robot_position)
 
     # update the robot (x, y, z) positions
-    for r_ind in range(len(r)):
-        r_i = r[r_ind]
-        r_j = np.delete(r, np.array([r_ind]), axis=0)
-        r[r_ind] += s_i*(ps.aggregation(r_i, r_j) + ps.repulsion(r_i, r_j, 5.0))
+    for r_ind in range(len(robot_position)):
+        r_i = robot_position[r_ind]
+        r_j = np.delete(robot_position, np.array([r_ind]), axis=0)
+        robot_position[r_ind] += s_i*(ps.aggregation(r_i, r_j) + ps.repulsion(r_i, r_j, 5.0))
 ```
-![AggregationRepulsion](Examples/pics/AggregationRepulsion.gif)
+![AggregationRepulsion](notebooks/pics/AggregationRepulsion.gif)
 
 ## Contributing to pyswarming
 All kind of contributions are welcome: 
 * Improvement of code with new features, bug fixes, and  bug reports
 * Improvement of documentation
 * Additional tests
 
 Follow the instructions [here](https://pyswarming.readthedocs.io/en/latest/Contribution.html)
-for submitting a PR.
+for submitting a PR (Pull Request).
 
 If you have any ideas or questions, feel free to open an issue.
 
 
 ## Acknowledgements
+The authors would like to thank the Human Resources Program from the National Agency of Oil, Gas and Bio Combustibles – PRH-ANP for the financial support.
 This work was supported by "Coordenação de Aperfeiçoamento de Pessoal de Nível Superior - Brasil (CAPES)", [LOC/COPPE/UFRJ](https://www.loc.ufrj.br/index.php/en/) ([Laboratory of Waves and Current](https://www.loc.ufrj.br/index.php/en/) - [Federal University of Rio de Janeiro](https://ufrj.br/en/)) and the National Council for Scientific and Technological Development (CNPq), which are gratefully acknowledged.
```

### Comparing `pyswarming-1.1.0/setup.py` & `pyswarming-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 INSTALL_REQUIRES = [
     "numpy",
     "matplotlib",
 ]
 
 setuptools.setup(
     name="pyswarming",
-    version="1.1.0",
+    version="1.1.1",
     author="Emerson Martins de Andrade",
     author_email="mrson@oceanica.ufrj.br",
     description="A research toolkit for Swarm Robotics",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/mrsonandrade/pyswarming",
     packages=setuptools.find_packages(),
```

