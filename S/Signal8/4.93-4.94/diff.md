# Comparing `tmp/Signal8-4.93.tar.gz` & `tmp/Signal8-4.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.93.tar", last modified: Tue Jul 18 19:58:38 2023, max compression
+gzip compressed data, was "Signal8-4.94.tar", last modified: Fri Jul 21 00:30:32 2023, max compression
```

## Comparing `Signal8-4.93.tar` & `Signal8-4.94.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 19:58:38.973797 Signal8-4.93/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.93/LICENSE
--rw-rw-rw-   0        0        0     4769 2023-07-18 19:58:38.965797 Signal8-4.93/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.93/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 19:58:38.871797 Signal8-4.93/Signal8/
--rw-rw-rw-   0        0        0    11288 2023-07-17 22:25:05.000000 Signal8-4.93/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.93/Signal8/__init__.py
--rw-rw-rw-   0        0        0      240 2023-07-17 21:38:01.000000 Signal8-4.93/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:58:38.946798 Signal8-4.93/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.93/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5285 2023-07-14 01:01:24.000000 Signal8-4.93/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2377 2023-07-18 19:56:04.000000 Signal8-4.93/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.93/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.93/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.93/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:58:38.922796 Signal8-4.93/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4769 2023-07-18 19:58:38.000000 Signal8-4.93/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-18 19:58:38.000000 Signal8-4.93/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 19:58:38.000000 Signal8-4.93/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 19:58:38.000000 Signal8-4.93/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 19:58:38.974800 Signal8-4.93/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-07-18 19:57:06.000000 Signal8-4.93/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:30:32.738595 Signal8-4.94/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.94/LICENSE
+-rw-rw-rw-   0        0        0     6075 2023-07-21 00:30:32.737595 Signal8-4.94/PKG-INFO
+-rw-rw-rw-   0        0        0     5576 2023-07-21 00:28:58.000000 Signal8-4.94/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 00:30:32.626595 Signal8-4.94/Signal8/
+-rw-rw-rw-   0        0        0    11167 2023-07-20 21:05:39.000000 Signal8-4.94/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.94/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      240 2023-07-17 21:38:01.000000 Signal8-4.94/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:30:32.731596 Signal8-4.94/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.94/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5285 2023-07-14 01:01:24.000000 Signal8-4.94/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2328 2023-07-20 21:04:43.000000 Signal8-4.94/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.94/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.94/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.94/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-21 00:30:32.717594 Signal8-4.94/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     6075 2023-07-21 00:30:32.000000 Signal8-4.94/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-21 00:30:32.000000 Signal8-4.94/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 00:30:32.000000 Signal8-4.94/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 00:30:32.000000 Signal8-4.94/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 00:30:32.739596 Signal8-4.94/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-07-20 21:05:58.000000 Signal8-4.94/setup.py
```

### Comparing `Signal8-4.93/LICENSE` & `Signal8-4.94/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.93/PKG-INFO` & `Signal8-4.94/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-Metadata-Version: 2.1
-Name: Signal8
-Version: 4.93
-Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
-Home-page: https://github.com/ethanmclark1/signal8
-Author: Ethan Clark
-Author-email: eclark715@gmail.com.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# An Extension of Multi-Agent Particle Environment
 
-# A Fork of Multi-Agent Particle Environment
-
-Signal8 is an enhanced version of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
+Signal8 is an enhancement on top of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
-Signal8 is an open-source research project devoted to facilitating the evolution of communication strategies in multi-agent systems. The project, drawing inspiration from real-world scenarios such as disaster response and precision farming, features a dynamic environment that elevates the principles of the Lewis signaling game. This unique setting serves as a testing ground for the advancement of robot-to-robot communication protocols.
+Signal8 is an open-source research project aimed advancing the development of communication strategies in multi-agent systems. The project proposes a unique environment that emphasizes the principles of the Lewis signaling game. This distinct setting serves as a testing ground for advancing robot-to-robot communication protocols.
 
-Each problem set within Signal8 encompasses four distinct instances, with each one posing different constraints on the positioning of entities such as starting points, goals, and both static and dynamic obstacles. This dynamic feature fosters examination of communication strategies in diverse settings, enhancing the environment's realism and adaptability.
+Each problem set within Signal8 introduces different constraints on entity positioning such as start points, goals, and obstacles. This dynamic aspect encourages the investigation of communication strategies in diverse settings, enhancing the environment's adaptability and realism.
 
-A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents â€“ an 'eye in the sky' agent with global information and ground agents with only local information â€“ operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
+A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents – an 'eye in the sky' agent with global information and ground agents with only local information – operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
 
-In Signal8, both static and dynamic obstacles are present, creating further complexities for agents navigating through the environment. Static obstacles provide persistent barriers, while dynamic obstacles introduce predictable elements that can move or change over time. This complexity enriches the environment, making it an even more challenging and realistic platform for testing multi-agent communication strategies.
+In Signal8, obstacles are split into two categories: large obstacles that are observable exclusively by the aerial agents, and small obstacles which are observable to ground agents only. This distinct division introduces further complexity for agents navigating the environment. Large obstacles serve as barriers that define the structure of the environment, while small obstacles, appearing unpredictably within the vicinity of the ground agents. Both large and small obstacles remain stationary throughout the instance, adding an element of constant challenge to the environment. This multi-layered design richly expands the realism and complexity of the environment, making Signal8 a more demanding and intriguing platform for testing multi-agent communication strategies.
 
-For more information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
+For additional information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
 
 ## Installation
 
 ```
 git clone https://github.com/ethanmclark1/signal8.git
 cd signal8
 pip install -r requirements.txt
@@ -49,23 +37,39 @@
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :---------------: | :--------------------------------------------: |
 |    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
 |    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
-|   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
+|   ``corners``    | ![1686604788813](image/README/1686604788813.png) |
 |     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
 | ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
 |   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
 | ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
 | ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
 
 The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
+## Contributing
+
+We welcome contributions to Signal8! If you're interested in contributing, you can do so in the following ways:
+
+* **Bug Reports** : If you discover a bug when using Signal8, please submit a report via the issues tab. When submitting an issue, please do your best to include a detailed description of the problem and a code sample, if applicable.
+* **Feature Requests** : If you have a great idea that you think would improve Signal8, don't hesitate to post your suggestions in the issues tab. Please be as detailed as possible in your explanation.
+* **Pull Requests** : If you have made enhancements to Signal8, please feel free to submit a pull request. We appreciate all the help we can get to make Signal8 better!
+
+## Support
+
+If you encounter any issues or have questions about Signal8, please feel free to contact us. You can either create an issue in the GitHub repository or reach out to us directly at [eclark715@gmail.com](mailto:eclark715@gmail.com).
+
+## License
+
+Signal8 is open-source software licensed under the [MIT license](https://chat.openai.com/LINK_TO_YOUR_LICENSE).
+
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
 
 <pre>
```

### Comparing `Signal8-4.93/README.md` & `Signal8-4.94/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,34 @@
-# A Fork of Multi-Agent Particle Environment
+Metadata-Version: 2.1
+Name: Signal8
+Version: 4.94
+Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
+Home-page: https://github.com/ethanmclark1/signal8
+Author: Ethan Clark
+Author-email: eclark715@gmail.com.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-Signal8 is an enhanced version of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
+# An Extension of Multi-Agent Particle Environment
+
+Signal8 is an enhancement on top of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
-Signal8 is an open-source research project devoted to facilitating the evolution of communication strategies in multi-agent systems. The project, drawing inspiration from real-world scenarios such as disaster response and precision farming, features a dynamic environment that elevates the principles of the Lewis signaling game. This unique setting serves as a testing ground for the advancement of robot-to-robot communication protocols.
+Signal8 is an open-source research project aimed advancing the development of communication strategies in multi-agent systems. The project proposes a unique environment that emphasizes the principles of the Lewis signaling game. This distinct setting serves as a testing ground for advancing robot-to-robot communication protocols.
 
-Each problem set within Signal8 encompasses four distinct instances, with each one posing different constraints on the positioning of entities such as starting points, goals, and both static and dynamic obstacles. This dynamic feature fosters examination of communication strategies in diverse settings, enhancing the environment's realism and adaptability.
+Each problem set within Signal8 introduces different constraints on entity positioning such as start points, goals, and obstacles. This dynamic aspect encourages the investigation of communication strategies in diverse settings, enhancing the environment's adaptability and realism.
 
-A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents – an 'eye in the sky' agent with global information and ground agents with only local information – operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
+A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents â€“ an 'eye in the sky' agent with global information and ground agents with only local information â€“ operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
 
-In Signal8, both static and dynamic obstacles are present, creating further complexities for agents navigating through the environment. Static obstacles provide persistent barriers, while dynamic obstacles introduce predictable elements that can move or change over time. This complexity enriches the environment, making it an even more challenging and realistic platform for testing multi-agent communication strategies.
+In Signal8, obstacles are split into two categories: large obstacles that are observable exclusively by the aerial agents, and small obstacles which are observable to ground agents only. This distinct division introduces further complexity for agents navigating the environment. Large obstacles serve as barriers that define the structure of the environment, while small obstacles, appearing unpredictably within the vicinity of the ground agents. Both large and small obstacles remain stationary throughout the instance, adding an element of constant challenge to the environment. This multi-layered design richly expands the realism and complexity of the environment, making Signal8 a more demanding and intriguing platform for testing multi-agent communication strategies.
 
-For more information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
+For additional information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
 
 ## Installation
 
 ```
 git clone https://github.com/ethanmclark1/signal8.git
 cd signal8
 pip install -r requirements.txt
@@ -37,23 +49,39 @@
 
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :---------------: | :--------------------------------------------: |
 |    ``bisect``    | ![1688231528499](image/README/1688231528499.png) |
 |    ``circle``    | ![1688231542146](image/README/1688231542146.png) |
-|   ``corners``    | ![1686604788813](image/README/1686604788813.png) |
+|   ``corners``Â    | ![1686604788813](image/README/1686604788813.png) |
 |     ``cross``     | ![1686604808540](image/README/1686604808540.png) |
 | ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
 |   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
 | ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
 | ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
 
 The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
+## Contributing
+
+We welcome contributions to Signal8! If you're interested in contributing, you can do so in the following ways:
+
+* **Bug Reports** : If you discover a bug when using Signal8, please submit a report via the issues tab. When submitting an issue, please do your best to include a detailed description of the problem and a code sample, if applicable.
+* **Feature Requests** : If you have a great idea that you think would improve Signal8, don't hesitate to post your suggestions in the issues tab. Please be as detailed as possible in your explanation.
+* **Pull Requests** : If you have made enhancements to Signal8, please feel free to submit a pull request. We appreciate all the help we can get to make Signal8 better!
+
+## Support
+
+If you encounter any issues or have questions about Signal8, please feel free to contact us. You can either create an issue in the GitHub repository or reach out to us directly at [eclark715@gmail.com](mailto:eclark715@gmail.com).
+
+## License
+
+Signal8 is open-source software licensed under the [MIT license](https://chat.openai.com/LINK_TO_YOUR_LICENSE).
+
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
 
 <pre>
```

### Comparing `Signal8-4.93/Signal8/Signal8.py` & `Signal8-4.94/Signal8/Signal8.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,19 @@
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
         num_agents=1, 
         num_large_obstacles=4, 
         num_small_obstacles=10, 
         render_mode=None,
-        max_cycles=500,
+        max_cycles=100,
         ):
         
-        if num_agents > 1:
-            raise ValueError("Signal8 currently can only support up to 1 agent.")
-        
-        if num_large_obstacles > 16:
-            raise ValueError("Signal8 has a maximum of 16 large obstacles.")
+        if num_large_obstacles > 10:
+            raise ValueError("Signal8 has a maximum of 10 large obstacles.")
         
         scenario = Scenario()
         world = scenario.make_world(num_agents, num_large_obstacles, num_small_obstacles)
         
         super().__init__(
             scenario=scenario, 
             world=world,
```

### Comparing `Signal8-4.93/Signal8/utils/core.py` & `Signal8-4.94/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.93/Signal8/utils/problems.py` & `Signal8-4.94/Signal8/utils/problems.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         ((0.5, 0.5), (0.45)),
         ((-0.15, -0.675), (0.225)),
         ((-0.625, 0.175), (0.175)),
         ((-0.0375, 0), (0.1125)),
         ((-0.125, 0.475), (0.075)),
         ],
     'right_arrows': [
-        ((0.4, 0.2), (0.4, -0.2), (0.7, 0)), # middle right
-        ((0.3, 0.9), (0.3, 0.5), (0.6, 0.7)), # top right
-        ((-0.75, 0.5), (-0.75, 0.1), (-0.45, 0.3)), # top left
-        ((-0.3, -0.45), (-0.3, -0.85), (0, -0.65)), # bottom left
+        ((0.4, 0.2), (0.4, -0.2), (0.7, 0)), 
+        ((0.3, 0.9), (0.3, 0.5), (0.6, 0.7)), 
+        ((-0.75, 0.5), (-0.75, 0.1), (-0.45, 0.3)), 
+        ((-0.3, -0.45), (-0.3, -0.85), (0, -0.65)),
         ]
     }
 
 def get_problem_list():
     return list(problems.keys())
 
 def get_problem_instance(instance_name):
```

### Comparing `Signal8-4.93/Signal8/utils/simple_env.py` & `Signal8-4.94/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.93/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.94/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.93/Signal8.egg-info/PKG-INFO` & `Signal8-4.94/Signal8.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.93
+Version: 4.94
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# A Fork of Multi-Agent Particle Environment
+# An Extension of Multi-Agent Particle Environment
 
-Signal8 is an enhanced version of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
+Signal8 is an enhancement on top of the Simple environment, originally developed by the [Farama Foundation](https://farama.org/) as part of their [Multi-Agent Particle Environment (MPE)](https://pettingzoo.farama.org/environments/mpe/).
 
 # Signal8
 
-Signal8 is an open-source research project devoted to facilitating the evolution of communication strategies in multi-agent systems. The project, drawing inspiration from real-world scenarios such as disaster response and precision farming, features a dynamic environment that elevates the principles of the Lewis signaling game. This unique setting serves as a testing ground for the advancement of robot-to-robot communication protocols.
+Signal8 is an open-source research project aimed advancing the development of communication strategies in multi-agent systems. The project proposes a unique environment that emphasizes the principles of the Lewis signaling game. This distinct setting serves as a testing ground for advancing robot-to-robot communication protocols.
 
-Each problem set within Signal8 encompasses four distinct instances, with each one posing different constraints on the positioning of entities such as starting points, goals, and both static and dynamic obstacles. This dynamic feature fosters examination of communication strategies in diverse settings, enhancing the environment's realism and adaptability.
+Each problem set within Signal8 introduces different constraints on entity positioning such as start points, goals, and obstacles. This dynamic aspect encourages the investigation of communication strategies in diverse settings, enhancing the environment's adaptability and realism.
 
 A notable characteristic of Signal8 is its incorporation of asymmetric information, whereby two types of agents â€“ an 'eye in the sky' agent with global information and ground agents with only local information â€“ operate simultaneously. This asymmetry replicates real-world situations, presenting challenges for the development of efficient communication strategies. It also provides intriguing prospects for the generation of context-dependent language and high-level directives.
 
-In Signal8, both static and dynamic obstacles are present, creating further complexities for agents navigating through the environment. Static obstacles provide persistent barriers, while dynamic obstacles introduce predictable elements that can move or change over time. This complexity enriches the environment, making it an even more challenging and realistic platform for testing multi-agent communication strategies.
+In Signal8, obstacles are split into two categories: large obstacles that are observable exclusively by the aerial agents, and small obstacles which are observable to ground agents only. This distinct division introduces further complexity for agents navigating the environment. Large obstacles serve as barriers that define the structure of the environment, while small obstacles, appearing unpredictably within the vicinity of the ground agents. Both large and small obstacles remain stationary throughout the instance, adding an element of constant challenge to the environment. This multi-layered design richly expands the realism and complexity of the environment, making Signal8 a more demanding and intriguing platform for testing multi-agent communication strategies.
 
-For more information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
+For additional information on utilizing the environment API, please refer to the [PettingZoo API documentation](https://pettingzoo.farama.org/content/basic_usage/).
 
 ## Installation
 
 ```
 git clone https://github.com/ethanmclark1/signal8.git
 cd signal8
 pip install -r requirements.txt
@@ -58,14 +58,30 @@
 | ``einstein_tile`` | ![1688231581499](image/README/1688231581499.png) |
 |   ``quarters``   | ![1688231597856](image/README/1688231597856.png) |
 | ``solar_system`` | ![1688231626872](image/README/1688231626872.png) |
 | ``right_arrows`` | ![1688231657789](image/README/1688231657789.png) |
 
 The red zones denote regions where large obstacles can be spawned, while the remaining space (indicated in white) designates areas eligible for agent deployment, goal placement, and generation of small obstacles.
 
+## Contributing
+
+We welcome contributions to Signal8! If you're interested in contributing, you can do so in the following ways:
+
+* **Bug Reports** : If you discover a bug when using Signal8, please submit a report via the issues tab. When submitting an issue, please do your best to include a detailed description of the problem and a code sample, if applicable.
+* **Feature Requests** : If you have a great idea that you think would improve Signal8, don't hesitate to post your suggestions in the issues tab. Please be as detailed as possible in your explanation.
+* **Pull Requests** : If you have made enhancements to Signal8, please feel free to submit a pull request. We appreciate all the help we can get to make Signal8 better!
+
+## Support
+
+If you encounter any issues or have questions about Signal8, please feel free to contact us. You can either create an issue in the GitHub repository or reach out to us directly at [eclark715@gmail.com](mailto:eclark715@gmail.com).
+
+## License
+
+Signal8 is open-source software licensed under the [MIT license](https://chat.openai.com/LINK_TO_YOUR_LICENSE).
+
 ## Paper Citation
 
 If you used this environment for your experiments or found it helpful, consider citing the following papers:
 
 Environments in this repo:
 
 <pre>
```

### Comparing `Signal8-4.93/setup.py` & `Signal8-4.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.93",
+    version="4.94",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

